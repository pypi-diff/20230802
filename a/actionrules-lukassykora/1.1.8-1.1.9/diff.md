# Comparing `tmp/actionrules-lukassykora-1.1.8.tar.gz` & `tmp/actionrules-lukassykora-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\actionrules-lukassykora-1.1.8.tar", last modified: Sun Mar 15 07:49:13 2020, max compression
+gzip compressed data, was "dist/actionrules-lukassykora-1.1.9.tar", last modified: Sat May  9 21:29:21 2020, max compression
```

## Comparing `actionrules-lukassykora-1.1.8.tar` & `actionrules-lukassykora-1.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2020-03-15 07:49:13.000000 actionrules-lukassykora-1.1.8/
--rw-rw-rw-   0        0        0     5042 2020-03-15 07:49:13.000000 actionrules-lukassykora-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3826 2020-03-15 07:31:42.000000 actionrules-lukassykora-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2020-03-15 07:49:13.000000 actionrules-lukassykora-1.1.8/actionrules/
--rw-rw-rw-   0        0        0        0 2020-03-15 07:14:21.000000 actionrules-lukassykora-1.1.8/actionrules/__init__.py
-drwxrwxrwx   0        0        0        0 2020-03-15 07:49:13.000000 actionrules-lukassykora-1.1.8/actionrules/actionRules/
--rw-rw-rw-   0        0        0       28 2020-03-12 21:36:40.000000 actionrules-lukassykora-1.1.8/actionrules/actionRules/__init__.py
--rw-rw-rw-   0        0        0    15391 2020-03-15 07:22:23.000000 actionrules-lukassykora-1.1.8/actionrules/actionRules/actionRules.py
-drwxrwxrwx   0        0        0        0 2020-03-15 07:49:13.000000 actionrules-lukassykora-1.1.8/actionrules/actionRulesDiscovery/
--rw-rw-rw-   0        0        0       37 2019-11-25 19:43:08.000000 actionrules-lukassykora-1.1.8/actionrules/actionRulesDiscovery/__init__.py
--rw-rw-rw-   0        0        0    22334 2020-03-15 07:22:23.000000 actionrules-lukassykora-1.1.8/actionrules/actionRulesDiscovery/actionRulesDiscovery.py
-drwxrwxrwx   0        0        0        0 2020-03-15 07:49:13.000000 actionrules-lukassykora-1.1.8/actionrules/decisions/
--rw-rw-rw-   0        0        0       26 2019-10-06 20:03:34.000000 actionrules-lukassykora-1.1.8/actionrules/decisions/__init__.py
--rw-rw-rw-   0        0        0     5123 2020-03-14 11:04:26.000000 actionrules-lukassykora-1.1.8/actionrules/decisions/decisions.py
-drwxrwxrwx   0        0        0        0 2020-03-15 07:49:13.000000 actionrules-lukassykora-1.1.8/actionrules/desiredState/
--rw-rw-rw-   0        0        0       29 2020-03-12 21:36:40.000000 actionrules-lukassykora-1.1.8/actionrules/desiredState/__init__.py
--rw-rw-rw-   0        0        0     6168 2020-03-14 11:04:26.000000 actionrules-lukassykora-1.1.8/actionrules/desiredState/desiredState.py
-drwxrwxrwx   0        0        0        0 2020-03-15 07:49:13.000000 actionrules-lukassykora-1.1.8/actionrules/reduction/
--rw-rw-rw-   0        0        0       26 2019-07-03 07:16:28.000000 actionrules-lukassykora-1.1.8/actionrules/reduction/__init__.py
--rw-rw-rw-   0        0        0     6141 2020-03-15 07:22:23.000000 actionrules-lukassykora-1.1.8/actionrules/reduction/reduction.py
-drwxrwxrwx   0        0        0        0 2020-03-15 07:49:13.000000 actionrules-lukassykora-1.1.8/actionrules_lukassykora.egg-info/
--rw-rw-rw-   0        0        0     5042 2020-03-15 07:49:12.000000 actionrules-lukassykora-1.1.8/actionrules_lukassykora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      669 2020-03-15 07:49:13.000000 actionrules-lukassykora-1.1.8/actionrules_lukassykora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-03-15 07:49:12.000000 actionrules-lukassykora-1.1.8/actionrules_lukassykora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2020-03-15 07:49:12.000000 actionrules-lukassykora-1.1.8/actionrules_lukassykora.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2020-03-15 07:49:12.000000 actionrules-lukassykora-1.1.8/actionrules_lukassykora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-03-15 07:49:13.000000 actionrules-lukassykora-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      752 2020-03-15 07:48:07.000000 actionrules-lukassykora-1.1.8/setup.py
+drwxr-xr-x   0 lukas.sykora   (502) staff       (20)        0 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)     4936 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/PKG-INFO
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)     3735 2020-05-09 18:36:32.000000 actionrules-lukassykora-1.1.9/README.md
+drwxr-xr-x   0 lukas.sykora   (502) staff       (20)        0 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/actionrules/
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)        0 2020-05-09 18:36:32.000000 actionrules-lukassykora-1.1.9/actionrules/__init__.py
+drwxr-xr-x   0 lukas.sykora   (502) staff       (20)        0 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/actionrules/actionRules/
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)       27 2020-05-09 18:36:32.000000 actionrules-lukassykora-1.1.9/actionrules/actionRules/__init__.py
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)    19718 2020-05-09 20:58:22.000000 actionrules-lukassykora-1.1.9/actionrules/actionRules/actionRules.py
+drwxr-xr-x   0 lukas.sykora   (502) staff       (20)        0 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/actionrules/actionRulesDiscovery/
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)       36 2020-05-09 18:36:32.000000 actionrules-lukassykora-1.1.9/actionrules/actionRulesDiscovery/__init__.py
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)    22133 2020-05-09 20:58:22.000000 actionrules-lukassykora-1.1.9/actionrules/actionRulesDiscovery/actionRulesDiscovery.py
+drwxr-xr-x   0 lukas.sykora   (502) staff       (20)        0 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/actionrules/decisions/
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)       25 2020-05-09 18:36:32.000000 actionrules-lukassykora-1.1.9/actionrules/decisions/__init__.py
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)     5059 2020-05-09 20:58:22.000000 actionrules-lukassykora-1.1.9/actionrules/decisions/decisions.py
+drwxr-xr-x   0 lukas.sykora   (502) staff       (20)        0 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/actionrules/desiredState/
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)       28 2020-05-09 18:36:32.000000 actionrules-lukassykora-1.1.9/actionrules/desiredState/__init__.py
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)     6614 2020-05-09 18:36:32.000000 actionrules-lukassykora-1.1.9/actionrules/desiredState/desiredState.py
+drwxr-xr-x   0 lukas.sykora   (502) staff       (20)        0 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/actionrules/reduction/
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)       25 2020-05-09 18:36:32.000000 actionrules-lukassykora-1.1.9/actionrules/reduction/__init__.py
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)     5977 2020-05-09 18:36:32.000000 actionrules-lukassykora-1.1.9/actionrules/reduction/reduction.py
+drwxr-xr-x   0 lukas.sykora   (502) staff       (20)        0 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/actionrules_lukassykora.egg-info/
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)     4936 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/actionrules_lukassykora.egg-info/PKG-INFO
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)      669 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/actionrules_lukassykora.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)        1 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/actionrules_lukassykora.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)       19 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/actionrules_lukassykora.egg-info/requires.txt
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)       12 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/actionrules_lukassykora.egg-info/top_level.txt
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)       38 2020-05-09 21:29:21.000000 actionrules-lukassykora-1.1.9/setup.cfg
+-rw-r--r--   0 lukas.sykora   (502) staff       (20)      743 2020-05-09 21:23:50.000000 actionrules-lukassykora-1.1.9/setup.py
```

### Comparing `actionrules-lukassykora-1.1.8/README.md` & `actionrules-lukassykora-1.1.9/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-# Action Rules
- [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-
-Action Rules (actionrules) is an implementation of Action Rules from Classification Rules algorithm described in
-
-```Dardzinska, A. (2013). Action rules mining. Berlin: Springer.```
-
-## GIT repository
-
-https://github.com/lukassykora/actionrules
-
-## Installation
-
-pip install actionrules-lukassykora
-
-## Jupyter Notebooks
-
-- [Titanic](https://github.com/lukassykora/actionrules/blob/master/notebooks/Titanic%20-%20Action%20Rules.ipynb) It is the best explanation of all possibilities.
-- [Telco](https://github.com/lukassykora/actionrules/blob/master/notebooks/Telco%20-%20Action%20Rules.ipynb) A brief demonstration.
-- [Ras](https://github.com/lukassykora/actionrules/blob/master/notebooks/Ras%20-%20Acton%20Rules.ipynb) Based on the example in (Ras, Zbigniew W and Wyrzykowska, ARAS: Action rules discovery based on agglomerative strategy, 2007). 
-
-
-## Example 1
-Get data from csv.
-Get action rules from classification rules. Classification rules have confidence 55% and support 3%.
-Stable part of action rule is "Age".
-Flexible attributes are "Embarked", "Fare", "Pclass".
-Target is a Survived value 1.0.
-No nan values.
-Use reduction tables for speeding up.
-Minimal 1 stable antecedent
-Minimal 1 flexible antecedent
-
-
-```python
-from actionrules.actionRulesDiscovery import ActionRulesDiscovery
-
-actionRulesDiscovery = ActionRulesDiscovery()
-actionRulesDiscovery.read_csv("data/titanic.csv", sep="\t")
-actionRulesDiscovery.fit(stable_attributes = ["Age"],
-                         flexible_attributes = ["Embarked", "Fare", "Pclass"],
-                         consequent = "Survived",
-                         conf=55,
-                         supp=3,
-                         desired_classes = ["1.0"],
-                         is_nan=False,
-                         is_reduction=True,
-                         min_stable_attributes=1,
-                         min_flexible_attributes=1,
-                         max_stable_attributes=5,
-                         max_flexible_attributes=5)
-actionRulesDiscovery.get_action_rules()
-```
-
-The output is a list where the first part is an action rule and the second part is a tuple of (support before, support after, action rule support) and (confidence before, confidence after, action rule confidence).
-
-## Example 2
-Get data from pandas dataframe.
-Get action rules from classification rules. Classification rules have confidence 50% and support 3%.
-Stable attributes are "Age" and "Sex".
-Flexible attributes are "Embarked", "Fare", "Pclass".
-Target is a Survived that changes from 0.0 to 1.0.
-No nan values.
-Use reduction tables for speeding up.
-Minimal 1 stable antecedent
-Minimal 1 flexible antecedent
-
-
-```python
-from actionrules.actionRulesDiscovery import ActionRulesDiscovery
-import pandas as pd
-
-dataFrame = pd.read_csv("data/titanic.csv", sep="\t")
-actionRulesDiscovery = ActionRulesDiscovery()
-actionRulesDiscovery.load_pandas(dataFrame)
-actionRulesDiscovery.fit(stable_attributes = ["Age", "Sex"],
-                         flexible_attributes = ["Embarked", "Fare", "Pclass"],
-                         consequent = "Survived",
-                         conf=50,
-                         supp=3,
-                         desired_changes = [["0.0", "1.0"]],
-                         is_nan=False,
-                         is_reduction=True,
-                         min_stable_attributes=1,
-                         min_flexible_attributes=1,
-                         max_stable_attributes=5,
-                         max_flexible_attributes=5)
-actionRulesDiscovery.get_pretty_action_rules()
-```
-
-The output is a list of action rules in pretty text form.
+# Action Rules
+ [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+Action Rules (actionrules) is an implementation of Action Rules from Classification Rules algorithm described in
+
+```Dardzinska, A. (2013). Action rules mining. Berlin: Springer.```
+
+## GIT repository
+
+https://github.com/lukassykora/actionrules
+
+## Installation
+
+pip install actionrules-lukassykora
+
+## Jupyter Notebooks
+
+- [Titanic](https://github.com/lukassykora/actionrules/blob/master/notebooks/Titanic%20-%20Action%20Rules.ipynb) It is the best explanation of all possibilities.
+- [Telco](https://github.com/lukassykora/actionrules/blob/master/notebooks/Telco%20-%20Action%20Rules.ipynb) A brief demonstration.
+- [Ras](https://github.com/lukassykora/actionrules/blob/master/notebooks/Ras%20-%20Acton%20Rules.ipynb) Based on the example in (Ras, Zbigniew W and Wyrzykowska, ARAS: Action rules discovery based on agglomerative strategy, 2007). 
+
+
+## Example 1
+Get data from csv.
+Get action rules from classification rules. Classification rules have confidence 55% and support 3%.
+Stable part of action rule is "Age".
+Flexible attributes are "Embarked", "Fare", "Pclass".
+Target is a Survived value 1.0.
+No nan values.
+Use reduction tables for speeding up.
+Minimal 1 stable antecedent
+Minimal 1 flexible antecedent
+
+
+```python
+from actionrules.actionRulesDiscovery import ActionRulesDiscovery
+
+actionRulesDiscovery = ActionRulesDiscovery()
+actionRulesDiscovery.read_csv("data/titanic.csv", sep="\t")
+actionRulesDiscovery.fit(stable_attributes = ["Age"],
+                         flexible_attributes = ["Embarked", "Fare", "Pclass"],
+                         consequent = "Survived",
+                         conf=55,
+                         supp=3,
+                         desired_classes = ["1.0"],
+                         is_nan=False,
+                         is_reduction=True,
+                         min_stable_attributes=1,
+                         min_flexible_attributes=1,
+                         max_stable_attributes=5,
+                         max_flexible_attributes=5)
+actionRulesDiscovery.get_action_rules()
+```
+
+The output is a list where the first part is an action rule and the second part is a tuple of (support before, support after, action rule support) and (confidence before, confidence after, action rule confidence).
+
+## Example 2
+Get data from pandas dataframe.
+Get action rules from classification rules. Classification rules have confidence 50% and support 3%.
+Stable attributes are "Age" and "Sex".
+Flexible attributes are "Embarked", "Fare", "Pclass".
+Target is a Survived that changes from 0.0 to 1.0.
+No nan values.
+Use reduction tables for speeding up.
+Minimal 1 stable antecedent
+Minimal 1 flexible antecedent
+
+
+```python
+from actionrules.actionRulesDiscovery import ActionRulesDiscovery
+import pandas as pd
+
+dataFrame = pd.read_csv("data/titanic.csv", sep="\t")
+actionRulesDiscovery = ActionRulesDiscovery()
+actionRulesDiscovery.load_pandas(dataFrame)
+actionRulesDiscovery.fit(stable_attributes = ["Age", "Sex"],
+                         flexible_attributes = ["Embarked", "Fare", "Pclass"],
+                         consequent = "Survived",
+                         conf=50,
+                         supp=3,
+                         desired_changes = [["0.0", "1.0"]],
+                         is_nan=False,
+                         is_reduction=True,
+                         min_stable_attributes=1,
+                         min_flexible_attributes=1,
+                         max_stable_attributes=5,
+                         max_flexible_attributes=5)
+actionRulesDiscovery.get_pretty_action_rules()
+```
+
+The output is a list of action rules in pretty text form.
```

### Comparing `actionrules-lukassykora-1.1.8/actionrules/actionRules/actionRules.py` & `actionrules-lukassykora-1.1.9/actionrules/actionRules/actionRules.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,367 +1,470 @@
-import pandas as pd
-from typing import List
-from typing import Union
-import itertools
-
-from actionrules.desiredState import DesiredState
-
-
-class ActionRules:
-    """
-    The class ActionRules is the one where the algorithm for action rules discovery is settled.
-
-    ...
-
-    Attributes
-    ----------
-    stable_tables : List[pd.DataFrame]
-        Data frames with stable attributes.
-    flexible_tables : List[pd.DataFrame]
-        Data frames with flexible attributes.
-    decision_tables : List[pd.DataFrame]
-        Data frames with consequent.
-    desired_state : DesiredState()
-        DesiredState object.
-    action_rules : list
-        Discovered action rules.
-    action_rules_pretty_text : list
-        Readable discovered action rules.
-    action_rules_representation : list
-        Math representation of action rules.
-    supp : List[pd.Series]
-        List od supports for classification rules.
-    conf : List[pd.Series]
-        List od confidences for classification rules.
-    is_nan : bool
-        True means NaN values are used, False means NaN values are not used.
-    min_stable_antecedents : int
-        Minimal number of stable pairs.
-    min_flexible_antecedents : int
-        Minimal number of flexible pairs.
-    max_stable_antecedents : int
-        Maximal number of stable pairs.
-    max_flexible_antecedents : int
-        Maximal number of flexible pairs.
-    used_indexes : list
-        Already used indexes.
-    classification_before : list
-        List of before parts of action rules.
-    classification_after : list
-        List of after parts of action rules.
-
-    Methods
-    -------
-    fit(self)
-        Train the model.
-    pretty_text(self)
-        Generate pretty representation of action rules.
-    representation(self)
-        Generate mathematical representation of action rules.
-
-    """
-
-    def __init__(self,
-                 stable_tables: List[pd.DataFrame],
-                 flexible_tables: List[pd.DataFrame],
-                 decision_tables: List[pd.DataFrame],
-                 desired_state: DesiredState,
-                 supp: List[pd.Series],
-                 conf: List[pd.Series],
-                 is_nan: bool = False,
-                 min_stable_antecedents: int = 1,
-                 min_flexible_antecedents: int = 1,
-                 max_stable_antecedents: int = 1,
-                 max_flexible_antecedents: int = 1,
-                 ):
-        """
-        Parameters
-        ----------
-        stable_tables : List[pd.DataFrame]
-            Data frames with stable attributes.
-        flexible_tables : List[pd.DataFrame]
-            Data frames with flexible attributes.
-        decision_tables : List[pd.DataFrame]
-            Data frames with consequent.
-        desired_state : DesiredState()
-            DesiredState object.
-        supp : List[pd.Series]
-            List od supports for classification rules.
-        conf : List[pd.Series]
-            List od confidences for classification rules.
-        is_nan : bool
-            True means NaN values are used, False means NaN values are not used.
-        min_stable_antecedents : int
-            Minimal number of stable pairs.
-        min_flexible_antecedents : int
-            Minimal number of flexible pairs.
-        max_stable_antecedents : int
-            Maximal number of stable pairs.
-        max_flexible_antecedents : int
-            Maximal number of flexible pairs.
-        """
-        self.stable_tables = stable_tables
-        self.flexible_tables = flexible_tables
-        self.decision_tables = decision_tables
-        self.desired_state = desired_state
-        self.action_rules = []
-        self.action_rules_pretty_text = []
-        self.action_rules_representation = []
-        self.supp = supp
-        self.conf = conf
-        self.is_nan = is_nan
-        self.min_stable_antecedents = min_stable_antecedents
-        self.min_flexible_antecedents = min_flexible_antecedents
-        self.max_stable_antecedents = max_stable_antecedents
-        self.max_flexible_antecedents = max_flexible_antecedents
-        self.used_indexes = []
-        self.classification_before = []
-        self.classification_after = []
-
-    def _is_action_couple(self,
-                          before: Union[str, int, float],
-                          after: Union[str, int, float],
-                          attribute_type: str
-                          ) -> tuple:
-        """ Check if the state before and after can make action rule.
-
-        Parameters
-        ----------
-        before : Union[str, int, float]
-            Before part of the candidate.
-        after : Union[str, int, float]
-            After part of the candidate.
-        attribute_type : str
-            Attribute type (stable or flexible).
-
-        Returns
-        -------
-        tuple
-            Returns (bool is_action_pair, (before, after) action_pair, bool break_rule).
-        """
-        before = str(before)
-        after = str(after)
-        if attribute_type == "stable":
-            if before == "nan" and after == "nan":
-                return False, None, False
-            elif before == after and before != "nan":
-                return True, (before,), False
-            elif self.is_nan:
-                if before == "nan" and after != "nan":
-                    return True, (after + "*",), False
-                elif before != "nan" and after == "nan":
-                    return False, None, False
-        elif attribute_type == "flexible":
-            if before == "nan" and after == "nan":
-                return False, None, False
-            elif before != after and before != "nan" and after != "nan":
-                return True, (before, after), False
-            elif self.is_nan:
-                if before != after and before == "nan":
-                    return True, (str(None), after), False
-                if before != after and after == "nan":
-                    return False, None, False
-        return False, None, True
-
-    def _create_action_rules(self,
-                             df: pd.DataFrame,
-                             rule_before_index: int,
-                             rule_after_index: int,
-                             attribute_type: str) -> tuple:
-        """It creates action rules pairs.
-
-        Parameters
-        ----------
-        df : pd.DataFrame
-            Data frame with classification rules.
-        rule_before_index : int
-            Candidate before index.
-        rule_after_index : int
-            Candidate after index.
-        attribute_type : str
-            Type of attributes in the data frame (stable or flexible)
-
-        Returns
-        -------
-        bool
-            Does it break the condition to be an action rule?
-        list
-            Generated part of an action rule.
-        int
-            Number of used attributes in antecedent.
-        """
-        action_rule_part = []
-        count_antecedent = 0
-        columns = list(df)
-        for column in columns:
-            is_action_couple, action_couple, break_rule = self._is_action_couple(
-                before=df[column][rule_before_index],
-                after=df[column][rule_after_index],
-                attribute_type=attribute_type)
-            if break_rule:
-                return False, None, None
-            elif is_action_couple:
-                count_antecedent += 1
-                action_rule_part.append([column, action_couple])
-            else:
-                if action_couple is not None:
-                    action_rule_part.append([column, action_couple])
-        return True, action_rule_part, count_antecedent
-
-    def _add_action_rule(self,
-                         action_rule_stable: list,
-                         action_rule_flexible: list,
-                         action_rule_decision: list,
-                         action_rule_supp: list,
-                         action_rule_conf: list):
-        """This method joins the parts of an action rule and adds the action rule to a list.
-
-        Parameters
-        ----------
-        action_rule_stable : list
-            List of stable attributes.
-        action_rule_flexible : list
-            List of actions in flexible attributes.
-        action_rule_decision : list
-            List of changes in consequent.
-        action_rule_supp : list
-            List of supports.
-        action_rule_conf : list
-            List of confidences.
-        """
-        action_rule = [action_rule_stable, action_rule_flexible, action_rule_decision]
-        uplift = self._get_uplift(action_rule_supp[0], action_rule_conf[0], action_rule_conf[1])
-        self.action_rules.append([action_rule, action_rule_supp, action_rule_conf, uplift])
-
-    def fit(self):
-        """It finds all pairs of classification rules and tries to create action rules.
-
-        """
-        for table in range(len(self.stable_tables)):
-            stable_columns = self.stable_tables.pop(0)
-            flexible_columns = self.flexible_tables.pop(0)
-            decision_column = self.decision_tables.pop(0)
-            supp = self.supp.pop(0)
-            conf = self.conf.pop(0)
-            indexes = list(stable_columns.index.values)
-            for comb in itertools.permutations(indexes, 2):
-                # Check if it is not used twice - just for reduction by nan
-                if self.is_nan:
-                    if comb in self.used_indexes:
-                        continue
-                    self.used_indexes.append(comb)
-                rule_before_index = comb[0]
-                rule_after_index = comb[1]
-                decision_before = decision_column.at[rule_before_index, decision_column.columns[0]]
-                decision_after = decision_column.at[rule_after_index, decision_column.columns[0]]
-                if self.desired_state.is_candidate_decision(decision_before, decision_after):
-                    is_all_stable, action_rule_stable, counted_stable = self._create_action_rules(
-                        stable_columns,
-                        rule_before_index,
-                        rule_after_index,
-                        "stable")
-                    if not is_all_stable:
-                        continue
-                    is_all_flexible, action_rule_flexible, counted_flexible = self._create_action_rules(
-                        flexible_columns,
-                        rule_before_index,
-                        rule_after_index,
-                        "flexible")
-                    if not is_all_flexible:
-                        continue
-                    action_rule_decision = [
-                        decision_column.columns[0], [decision_before, decision_after]]
-                    if counted_flexible >= self.min_flexible_antecedents and \
-                       counted_stable >= self.min_stable_antecedents and \
-                       counted_flexible <= self.max_flexible_antecedents and \
-                       counted_stable <= self.max_stable_antecedents:
-                        action_rule_supp = [supp[rule_before_index],
-                                            supp[rule_after_index],
-                                            min(supp[rule_before_index], supp[rule_after_index])
-                                            ]
-                        action_rule_conf = [conf[rule_before_index],
-                                            conf[rule_after_index],
-                                            conf[rule_before_index] * conf[rule_after_index]
-                                            ]
-                        self._add_action_rule(action_rule_stable,
-                                              action_rule_flexible,
-                                              action_rule_decision,
-                                              action_rule_supp,
-                                              action_rule_conf)
-                        self.classification_before.append(rule_before_index)
-                        self.classification_after.append(rule_after_index)
-
-    def pretty_text(self):
-        """It generates human language representation of action rules.
-
-        """
-        for row in self.action_rules:
-            action_rule = row[0]
-            supp = row[1]
-            conf = row[2]
-            uplift = row[3]
-            text = "If "
-            # Stable part
-            stable_part = action_rule[0]
-            for stable_couple in stable_part:
-                text += "attribute '" + str(stable_couple[0]) + "' is '" + str(stable_couple[1][0]) + "', "
-            # Flexible part
-            flexible_part = action_rule[1]
-            for flexible_couple in flexible_part:
-                text += "attribute '" + str(flexible_couple[0]) + "' value '" + str(flexible_couple[1][0]) + \
-                        "' is changed to '" + str(flexible_couple[1][1]) + "', "
-            # Decision
-            decision = action_rule[2]
-            text += "then '" + str(decision[0]) + "' value '" + str(decision[1][0]) + "' is changed to '" + \
-                    str(decision[1][1]) + "' with support: " + str(supp[2]) + ", confidence: " + str(conf[2]) + \
-            " and uplift: " + str(uplift) + "."
-            self.action_rules_pretty_text.append(text)
-
-    def representation(self):
-        """It generates a mathematical representation of action rules.
-
-        """
-        for row in self.action_rules:
-            action_rule = row[0]
-            supp = row[1]
-            conf = row[2]
-            uplift = row[3]
-            text = "r = [   "
-            # Stable part
-            stable_part = action_rule[0]
-            text = text[:-3]
-            for stable_couple in stable_part:
-                text += "(" + str(stable_couple[0]) + ": " + str(stable_couple[1][0]) + ") ∧ "
-            # Flexible part
-            flexible_part = action_rule[1]
-            text = text[:-3]
-            for flexible_couple in flexible_part:
-                text += " ∧ (" + str(flexible_couple[0]) + ": " + str(flexible_couple[1][0]) + \
-                        " → " + str(flexible_couple[1][1]) + ") "
-            # Decision
-            decision = action_rule[2]
-            text += "] ⇒ [" + str(decision[0]) + ": " + str(decision[1][0]) + " → " + \
-                    str(decision[1][1]) + "] with support: " + str(supp[2]) + ", confidence: " + str(
-                conf[2]) + " and uplift: " + str(uplift) + "."
-            self.action_rules_representation.append(text)
-
-    @staticmethod
-    def _get_uplift(supp_before: float, conf_before: float, conf_after: float) -> float:
-        """Get uplift for action rule.
-
-        Uplift = P(target|treatment) -  P(target|no treatment)
-
-        Parameters
-        ----------
-        supp_before: float
-            Support before.
-        conf_before: float
-            Confidence before.
-        conf_after: float
-            Confidence after.
-
-        Returns
-        -------
-        float
-            An uplift value.
-        """
-        return ((supp_before / conf_before) * conf_after) - ((supp_before / conf_before) - supp_before)
+import pandas as pd
+from typing import List
+from typing import Union
+import itertools
+
+from actionrules.desiredState import DesiredState
+from actionrules.decisions import Decisions
+
+
+class ActionRules:
+    """
+    The class ActionRules is the one where the algorithm for action rules discovery is settled.
+
+    ...
+
+    Attributes
+    ----------
+    stable_tables : List[pd.DataFrame]
+        Data frames with stable attributes.
+    flexible_tables : List[pd.DataFrame]
+        Data frames with flexible attributes.
+    decision_tables : List[pd.DataFrame]
+        Data frames with consequent.
+    desired_state : DesiredState()
+        DesiredState object.
+    action_rules : list
+        Discovered action rules.
+    action_rules_pretty_text : list
+        Readable discovered action rules.
+    action_rules_representation : list
+        Math representation of action rules.
+    supp : List[pd.Series]
+        List od supports for classification rules.
+    conf : List[pd.Series]
+        List od confidences for classification rules.
+    is_nan : bool
+        True means NaN values are used, False means NaN values are not used.
+    min_stable_antecedents : int
+        Minimal number of stable pairs.
+    min_flexible_antecedents : int
+        Minimal number of flexible pairs.
+    max_stable_antecedents : int
+        Maximal number of stable pairs.
+    max_flexible_antecedents : int
+        Maximal number of flexible pairs.
+    used_indexes : list
+        Already used indexes.
+    classification_before : list
+        List of before parts of action rules.
+    classification_after : list
+        List of after parts of action rules.
+    desired_target_classes : List[str]
+        All desired classes.
+    not_default_target_classes : List[str]
+        The target values that are not in the before part.
+    decisions: Decisions()
+        Decisions object.
+
+    Methods
+    -------
+    fit(self)
+        Train the model.
+    pretty_text(self)
+        Generate pretty representation of action rules.
+    representation(self)
+        Generate mathematical representation of action rules.
+
+    """
+
+    def __init__(self,
+                 stable_tables: List[pd.DataFrame],
+                 flexible_tables: List[pd.DataFrame],
+                 decision_tables: List[pd.DataFrame],
+                 desired_state: DesiredState,
+                 decisions: Decisions,
+                 supp: List[pd.Series],
+                 conf: List[pd.Series],
+                 is_nan: bool = False,
+                 min_stable_antecedents: int = 1,
+                 min_flexible_antecedents: int = 1,
+                 max_stable_antecedents: int = 1,
+                 max_flexible_antecedents: int = 1,
+                 ):
+        """
+        Parameters
+        ----------
+        stable_tables : List[pd.DataFrame]
+            Data frames with stable attributes.
+        flexible_tables : List[pd.DataFrame]
+            Data frames with flexible attributes.
+        decision_tables : List[pd.DataFrame]
+            Data frames with consequent.
+        desired_state : DesiredState()
+            DesiredState object.
+        decisions : Decisions()
+            Decisions object.
+        supp : List[pd.Series]
+            List od supports for classification rules.
+        conf : List[pd.Series]
+            List od confidences for classification rules.
+        is_nan : bool
+            True means NaN values are used, False means NaN values are not used.
+        min_stable_antecedents : int
+            Minimal number of stable pairs.
+        min_flexible_antecedents : int
+            Minimal number of flexible pairs.
+        max_stable_antecedents : int
+            Maximal number of stable pairs.
+        max_flexible_antecedents : int
+            Maximal number of flexible pairs.
+
+        """
+        self.stable_tables = stable_tables
+        self.flexible_tables = flexible_tables
+        self.decision_tables = decision_tables
+        self.desired_state = desired_state
+        self.action_rules = []
+        self.action_rules_pretty_text = []
+        self.action_rules_representation = []
+        self.supp = supp
+        self.conf = conf
+        self.is_nan = is_nan
+        self.min_stable_antecedents = min_stable_antecedents
+        self.min_flexible_antecedents = min_flexible_antecedents
+        self.max_stable_antecedents = max_stable_antecedents
+        self.max_flexible_antecedents = max_flexible_antecedents
+        self.used_indexes = []
+        self.classification_before = []
+        self.classification_after = []
+        self.desired_target_classes = self.desired_state.get_destination_classes()
+        self.not_default_target_classes = self.desired_state.get_not_in_default_classes()
+        self.decisions = decisions
+
+    def _is_action_couple(self,
+                          before: Union[str, int, float],
+                          after: Union[str, int, float],
+                          attribute_type: str
+                          ) -> tuple:
+        """ Check if the state before and after can make action rule.
+
+        Parameters
+        ----------
+        before : Union[str, int, float]
+            Before part of the candidate.
+        after : Union[str, int, float]
+            After part of the candidate.
+        attribute_type : str
+            Attribute type (stable or flexible).
+
+        Returns
+        -------
+        tuple
+            Returns (bool is_action_pair, (before, after) action_pair, bool break_rule).
+        """
+        before = str(before)
+        after = str(after)
+        if attribute_type == "stable":
+            if before == "nan" and after == "nan":
+                return False, None, False
+            elif before == after and before != "nan":
+                return True, (before,), False
+            elif self.is_nan:
+                if before == "nan" and after != "nan":
+                    return True, (after + "*",), False
+                elif before != "nan" and after == "nan":
+                    return False, None, False
+        elif attribute_type == "flexible":
+            if before == "nan" and after == "nan":
+                return False, None, False
+            elif before != after and before != "nan" and after != "nan":
+                return True, (before, after), False
+            elif self.is_nan:
+                if before != after and before == "nan":
+                    return True, (str(None), after), False
+                if before != after and after == "nan":
+                    return False, None, False
+        return False, None, True
+
+    def _create_action_rules(self,
+                             df: pd.DataFrame,
+                             rule_before_index: int,
+                             rule_after_index: int,
+                             attribute_type: str) -> tuple:
+        """It creates action rules pairs.
+
+        Parameters
+        ----------
+        df : pd.DataFrame
+            Data frame with classification rules.
+        rule_before_index : int
+            Candidate before index.
+        rule_after_index : int
+            Candidate after index.
+        attribute_type : str
+            Type of attributes in the data frame (stable or flexible)
+
+        Returns
+        -------
+        bool
+            Does it break the condition to be an action rule?
+        list
+            Generated part of an action rule.
+        int
+            Number of used attributes in antecedent.
+        """
+        action_rule_part = []
+        count_antecedent = 0
+        columns = list(df)
+        for column in columns:
+            is_action_couple, action_couple, break_rule = self._is_action_couple(
+                before=df[column][rule_before_index],
+                after=df[column][rule_after_index],
+                attribute_type=attribute_type)
+            if break_rule:
+                return False, None, None
+            elif is_action_couple:
+                count_antecedent += 1
+                action_rule_part.append([column, action_couple])
+            else:
+                if action_couple is not None:
+                    action_rule_part.append([column, action_couple])
+        return True, action_rule_part, count_antecedent
+
+    def _add_action_rule(self,
+                         action_rule_stable: list,
+                         action_rule_flexible: list,
+                         action_rule_decision: list,
+                         action_rule_supp: list,
+                         action_rule_conf: list):
+        """This method joins the parts of an action rule and adds the action rule to a list.
+
+        Parameters
+        ----------
+        action_rule_stable : list
+            List of stable attributes.
+        action_rule_flexible : list
+            List of actions in flexible attributes.
+        action_rule_decision : list
+            List of changes in consequent.
+        action_rule_supp : list
+            List of supports.
+        action_rule_conf : list
+            List of confidences.
+        """
+        action_rule = [action_rule_stable, action_rule_flexible, action_rule_decision]
+        uplift = self._get_uplift(action_rule_supp[0], action_rule_conf[0], action_rule_conf[1])
+        self.action_rules.append([action_rule, action_rule_supp, action_rule_conf, uplift])
+
+    def _split_to_before_after_consequent(self, decision_column: pd.DataFrame) -> tuple:
+        """This method split the table based on consequent.
+
+        Parameters
+        ----------
+        decision_column : pd.DataFrame
+            Target values.
+
+        Returns
+        -------
+        tuple
+            Indexes that can be used in the before part and indexes that can be used in the after part.
+        """
+        before_indexes = decision_column[decision_column.iloc[:, 0] not in self.not_default_target_classes]
+        after_indexes = decision_column[decision_column.iloc[:, 0] in self.desired_target_classes]
+        return (before_indexes.index.values, after_indexes.index.values)
+
+    def fit(self):
+        """It finds all pairs of classification rules and tries to create action rules.
+
+        """
+        for table in range(len(self.stable_tables)):
+            stable_columns = self.stable_tables.pop(0)
+            flexible_columns = self.flexible_tables.pop(0)
+            decision_column = self.decision_tables.pop(0)
+            supp = self.supp.pop(0)
+            conf = self.conf.pop(0)
+            (before_indexes, after_indexes) = self._split_to_before_after_consequent(decision_column)
+            for comb in itertools.product(before_indexes, after_indexes):
+                # Check if it is not used twice - just for reduction by nan
+                if self.is_nan:
+                    if comb in self.used_indexes:
+                        continue
+                    self.used_indexes.append(comb)
+                rule_before_index = comb[0]
+                rule_after_index = comb[1]
+                decision_before = decision_column.at[rule_before_index, decision_column.columns[0]]
+                decision_after = decision_column.at[rule_after_index, decision_column.columns[0]]
+                if self.desired_state.is_candidate_decision(decision_before, decision_after):
+                    is_all_stable, action_rule_stable, counted_stable = self._create_action_rules(
+                        stable_columns,
+                        rule_before_index,
+                        rule_after_index,
+                        "stable")
+                    if not is_all_stable:
+                        continue
+                    is_all_flexible, action_rule_flexible, counted_flexible = self._create_action_rules(
+                        flexible_columns,
+                        rule_before_index,
+                        rule_after_index,
+                        "flexible")
+                    if not is_all_flexible:
+                        continue
+                    action_rule_decision = [
+                        decision_column.columns[0], [decision_before, decision_after]]
+                    if counted_flexible >= self.min_flexible_antecedents and \
+                       counted_stable >= self.min_stable_antecedents and \
+                       counted_flexible <= self.max_flexible_antecedents and \
+                       counted_stable <= self.max_stable_antecedents:
+                        if not self.is_nan:
+                            support = min(supp[rule_before_index], supp[rule_after_index])
+                            confidence = conf[rule_before_index] * conf[rule_after_index]
+                        else:
+                            total = len(self.decisions.data)
+                            if total == 0:
+                                support = None
+                                confidence = None
+                            else:
+                                (left_support_before, support_before) = self._get_frequency_from_mask(action_rule_stable,
+                                                                                                      action_rule_flexible,
+                                                                                                      action_rule_decision,
+                                                                                                      0
+                                                                                                      )
+                                (left_support_after, support_after) = self._get_frequency_from_mask(action_rule_stable,
+                                                                                                    action_rule_flexible,
+                                                                                                    action_rule_decision,
+                                                                                                    1
+                                                                                                    )
+                                support = support_before / total
+                                confidence = (support_before / left_support_before) * (support_after / left_support_after)
+                        action_rule_supp = [supp[rule_before_index],
+                                            supp[rule_after_index],
+                                            support
+                                            ]
+                        action_rule_conf = [conf[rule_before_index],
+                                            conf[rule_after_index],
+                                            confidence
+                                            ]
+                        self._add_action_rule(action_rule_stable,
+                                              action_rule_flexible,
+                                              action_rule_decision,
+                                              action_rule_supp,
+                                              action_rule_conf)
+                        self.classification_before.append(rule_before_index)
+                        self.classification_after.append(rule_after_index)
+
+    def pretty_text(self):
+        """It generates human language representation of action rules.
+
+        """
+        for row in self.action_rules:
+            action_rule = row[0]
+            supp = row[1]
+            conf = row[2]
+            uplift = row[3]
+            text = "If "
+            # Stable part
+            stable_part = action_rule[0]
+            for stable_couple in stable_part:
+                text += "attribute '" + str(stable_couple[0]) + "' is '" + str(stable_couple[1][0]) + "', "
+            # Flexible part
+            flexible_part = action_rule[1]
+            for flexible_couple in flexible_part:
+                text += "attribute '" + str(flexible_couple[0]) + "' value '" + str(flexible_couple[1][0]) + \
+                        "' is changed to '" + str(flexible_couple[1][1]) + "', "
+            # Decision
+            decision = action_rule[2]
+            text += "then '" + str(decision[0]) + "' value '" + str(decision[1][0]) + "' is changed to '" + \
+                    str(decision[1][1]) + "' with support: " + str(supp[2]) + ", confidence: " + str(conf[2]) + \
+            " and uplift: " + str(uplift) + "."
+            self.action_rules_pretty_text.append(text)
+
+    def representation(self):
+        """It generates a mathematical representation of action rules.
+
+        """
+        for row in self.action_rules:
+            action_rule = row[0]
+            supp = row[1]
+            conf = row[2]
+            uplift = row[3]
+            text = "r = [   "
+            # Stable part
+            stable_part = action_rule[0]
+            text = text[:-3]
+            for stable_couple in stable_part:
+                text += "(" + str(stable_couple[0]) + ": " + str(stable_couple[1][0]) + ") ∧ "
+            # Flexible part
+            flexible_part = action_rule[1]
+            text = text[:-3]
+            for flexible_couple in flexible_part:
+                text += " ∧ (" + str(flexible_couple[0]) + ": " + str(flexible_couple[1][0]) + \
+                        " → " + str(flexible_couple[1][1]) + ") "
+            # Decision
+            decision = action_rule[2]
+            text += "] ⇒ [" + str(decision[0]) + ": " + str(decision[1][0]) + " → " + \
+                    str(decision[1][1]) + "] with support: " + str(supp[2]) + ", confidence: " + str(
+                conf[2]) + " and uplift: " + str(uplift) + "."
+            self.action_rules_representation.append(text)
+
+    @staticmethod
+    def _get_uplift(supp_before: float, conf_before: float, conf_after: float) -> float:
+        """Get uplift for action rule.
+
+        Uplift = P(target|treatment) -  P(target|no treatment)
+
+        Parameters
+        ----------
+        supp_before: float
+            Support before.
+        conf_before: float
+            Confidence before.
+        conf_after: float
+            Confidence after.
+
+        Returns
+        -------
+        float
+            An uplift value.
+        """
+        return ((supp_before / conf_before) * conf_after) - ((supp_before / conf_before) - supp_before)
+
+    def _get_frequency_from_mask(self, action_rule_stable: list, action_rule_flexible: list, action_rule_decision: list, part: int) -> tuple:
+        """Get frequency from source data.
+
+        Parameters
+        ----------
+        action_rule_stable: list
+            Extended action rule - stable part.
+        action_rule_flexible: list
+            Extended action rule - flexible part.
+        action_rule_decision: list
+            Extended action rule - target.
+        part: int
+            Part of rule: before or after
+
+        Returns
+        -------
+        tuple
+            An action rule's left support and support (with target)
+        """
+        new_data = self.decisions.data.applymap(str).copy()
+        columns_values = []
+
+        for condition in action_rule_stable:
+            column = condition[0]
+            value = condition[1][0]
+            value = value.replace("*", "")
+            columns_values.append([column, value])
+
+        for condition in action_rule_flexible:
+            column = condition[0]
+            value = condition[1][part]
+            columns_values.append([column, value])
+
+        for column_value in columns_values:
+            col = column_value[0]
+            val = column_value[1]
+            if val is not None:
+                mask = new_data[col] == val
+                new_data = new_data[mask]
+
+        left_support = len(new_data)
+
+        col = action_rule_decision[0]
+        val = action_rule_decision[1][part]
+        mask = new_data[col] == val
+        new_data = new_data[mask]
+
+        support = len(new_data)
+
+        return left_support, support
```

### Comparing `actionrules-lukassykora-1.1.8/actionrules/actionRulesDiscovery/actionRulesDiscovery.py` & `actionrules-lukassykora-1.1.9/actionrules/actionRulesDiscovery/actionRulesDiscovery.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,538 +1,546 @@
-from typing import List
-import pandas as pd
-
-from actionrules.desiredState import DesiredState
-from actionrules.decisions import Decisions
-from actionrules.reduction import Reduction
-from actionrules.actionRules import ActionRules
-
-
-class ActionRulesDiscovery:
-    """
-    The class ActionRulesDiscovery is the main control class where the methods fit or
-    predict can be called. However, there is a minimum logic in the class. It is just an
-    interface that initializes other objects and calls their methods.
-
-    ...
-
-    Attributes
-    ----------
-    decisions : Decisions()
-        Object that runs PyFIM classification rules discovery.
-    action_rules: None or ActionRules
-        Object that runs action rules discovery.
-    desired_state: DesiredState
-        Object that is responsible for handling of desired state.
-    stable_attributes: list
-        List of stable attributes.
-    flexible_attributes: list
-        List of flexible attributes.
-    consequent: str
-        Name of consequent columns.
-
-    Methods
-    -------
-    read_csv(self, file: str, **kwargs)
-        Import data from a CSV file.
-    load_pandas(self, data_frame: pd.DataFrame)
-        Import data from Pandas data frame.
-    fit(self,
-        stable_attributes: List[str],
-        flexible_attributes: List[str],
-        consequent: str,
-        conf: float,
-        supp: float,
-        desired_classes: List[str] = None,
-        desired_changes: List[list] = None,
-        is_nan: bool = False,
-        is_reduction: bool = True,
-        min_stable_attributes: int = 1,
-        min_flexible_attributes: int = 1,
-        max_stable_attributes: int = 5,
-        max_flexible_attributes: int = 5,
-        )
-        Train the model from transaction data.
-    fit_classification_rules(self,
-                             stable_attributes: List[str],
-                             flexible_attributes: List[str],
-                             consequent: str,
-                             conf_col: str,
-                             supp_col: str,
-                             desired_classes: List[str] = None,
-                             desired_changes: List[list] = None,
-                             is_nan: bool = False,
-                             is_reduction: bool = True,
-                             min_stable_attributes: int = 1,
-                             min_flexible_attributes: int = 1,
-                             max_stable_attributes: int = 5,
-                             max_flexible_attributes: int = 5,
-                             )
-        Train the model from classification rules.
-    get_action_rules(self) -> list
-        Get list of action rules (machine representation)
-    get_pretty_action_rules(self) -> list
-        Get human-readable representations of action rules
-    get_action_rules_representation(self) -> list
-        Get math representation of action rules
-    get_source_data_for_ar(self, action_r_number: int, is_before: bool) -> pd.DataFrame
-        Get the source data the action rule is discovered from.
-    predict(self, source_table: pd.DataFrame) -> pd.DataFrame
-        Predicts if new occurrence would need any change.
-
-    """
-    ACTION_RULE = "action rule"
-    ACTION_RULE_TARGET = "action rule target"
-    SUPPORT_BEFORE = "support before"
-    SUPPORT_AFTER = "support after"
-    ACTION_RULE_SUPPORT = "action rule support"
-    CONFIDENCE_BEFORE = "confidence before"
-    CONFIDENCE_AFTER = "confidence after"
-    ACTION_RULE_CONFIDENCE = "action rule confidence"
-    ACTION_RULE_UPLIFT = "uplift"
-    RECOMMENDED = "-recommended"
-
-    def __init__(self):
-        """
-        Initialise
-        """
-        self.decisions = Decisions()
-        self.action_rules = None
-        self.desired_state = None
-        self.stable_attributes = []
-        self.flexible_attributes = []
-        self.consequent = ""
-
-    def _check_columns(self, attributes: List[str], consequent: str):
-        """Checks if inserted data is valid (columns exist, rows exist).
-
-        Parameters
-        ----------
-        attributes : List[str]
-            List of attributes names.
-        consequent : str
-            The name of consequent.
-
-        Raises
-        ------
-        Exception
-            If no data entered or column does not exist in data.
-        """
-        if len(self.decisions.data) == 0:
-            raise Exception("No data entered.")
-        columns = self.decisions.data.columns
-        for col_name in attributes + [consequent]:
-            if col_name not in columns:
-                raise Exception("Column " + str(col_name) + " does not exist in data")
-
-    def read_csv(self, file: str, **kwargs):
-        """Imports data from a CSV file.
-
-        It uses the same optional parameters as read_csv from Pandas.
-
-        Parameters
-        ----------
-        file : str
-            A path to a file.
-        **kwargs :
-            Arbitrary keyword arguments (the same as in Pandas).
-        """
-        self.decisions.read_csv(file, **kwargs)
-
-    def load_pandas(self, data_frame: pd.DataFrame):
-        """Loads a data frame.
-
-        It must be the Pandas data frame.
-
-        Parameters
-        ----------
-        data_frame : pd.DataFrame
-            Pandas data frame.
-        """
-        self.decisions.load_pandas(data_frame)
-
-    def fit(self,
-            stable_attributes: List[str],
-            flexible_attributes: List[str],
-            consequent: str,
-            conf: float,
-            supp: float,
-            desired_classes: List[str] = None,
-            desired_changes: List[list] = None,
-            is_nan: bool = False,
-            is_reduction: bool = True,
-            min_stable_attributes: int = 1,
-            min_flexible_attributes: int = 1,
-            max_stable_attributes: int = 5,
-            max_flexible_attributes: int = 5,
-            ):
-        """Train the model from transaction data.
-
-        Define antecedent and consequent.
-        - stable_attributes
-        - flexible_attributes
-        - consequent
-        Confidence and support.
-        - conf
-        - supp
-        Desired classes or desired changes must be entered.
-        - desired_classes
-        - desired_changes
-        Should NaN values be used?
-        - is_nan
-        Should the reduction table be used?
-        - is_reduction
-        Minimal number of stable and flexible pairs in antecedent.
-        - min_stable_attributes
-        - min_flexible_attributes
-        - max_stable_attributes
-        - max_flexible_attributes
-
-        Parameters
-        ----------
-        stable_attributes : List[str]
-            List of column names.
-        flexible_attributes : List[str]
-            List of column names.
-        consequent : str
-            Name of the consequent column.
-        conf : float
-            Value in % for minimal confidence in classification rules.
-            For example, 60.
-        supp : float
-            Value in % for minimal support of classification rules.
-            For example, 5.
-        desired_classes : List[str] = None
-            List of decision states. For example, ["1"].
-            DEFAULT: None
-        desired_changes : List[list] = None
-            List of desired changes. For example, [["0", "1"]].
-            DEFAULT: None
-        is_nan : bool = False
-            True means NaN values are used, False means NaN values are not used.
-            It means NaN values from classification rules.
-            DEFAULT: FALSE
-        is_reduction : bool = True
-            Is the reduction table used?
-            DEFAULT: TRUE
-        min_stable_attributes : int = 1
-            Minimal number of stable pairs.
-            DEFAULT: 1
-        min_flexible_attributes : int = 1
-            Minimal number of flexible pairs.
-            DEFAULT: 1
-        max_stable_attributes : int = 5
-            Maximal number of stable pairs.
-            DEFAULT: 5
-        max_flexible_attributes : int = 5
-            Maximal number of flexible pairs.
-            DEFAULT: 5
-        """
-        if (self.action_rules):
-            raise Exception("Fit was already called")
-        self.stable_attributes = stable_attributes
-        self.flexible_attributes = flexible_attributes
-        self.consequent = consequent
-        if bool(desired_classes) != bool(desired_changes):
-            self.desired_state = DesiredState(desired_classes=desired_classes, desired_changes=desired_changes)
-        else:
-            raise Exception("Desired classes or desired changes must be entered")
-        attributes = stable_attributes + flexible_attributes
-        self._check_columns(attributes, consequent)
-        self.decisions.prepare_data_fim(attributes, consequent)
-        self.decisions.fit_fim_apriori(conf=conf, support=supp)
-        self.decisions.generate_decision_table()
-        stable = self.decisions.decision_table[stable_attributes]
-        flex = self.decisions.decision_table[flexible_attributes]
-        target = self.decisions.decision_table[[consequent]]
-        supp = self.decisions.support
-        conf = self.decisions.confidence
-        reduced_tables = Reduction(stable, flex, target, self.desired_state, supp, conf, is_nan)
-        if is_reduction:
-            reduced_tables.reduce()
-        self.action_rules = ActionRules(
-            reduced_tables.stable_tables,
-            reduced_tables.flexible_tables,
-            reduced_tables.decision_tables,
-            self.desired_state,
-            reduced_tables.supp,
-            reduced_tables.conf,
-            is_nan,
-            min_stable_attributes,
-            min_flexible_attributes,
-            max_stable_attributes,
-            max_flexible_attributes
-        )
-        self.action_rules.fit()
-
-    def fit_classification_rules(self,
-                                 stable_attributes: List[str],
-                                 flexible_attributes: List[str],
-                                 consequent: str,
-                                 conf_col: str,
-                                 supp_col: str,
-                                 desired_classes: List[str] = None,
-                                 desired_changes: List[list] = None,
-                                 is_nan: bool = False,
-                                 is_reduction: bool = True,
-                                 min_stable_attributes: int = 1,
-                                 min_flexible_attributes: int = 1,
-                                 max_stable_attributes: int = 5,
-                                 max_flexible_attributes: int = 5,
-                                 ):
-        """Train the model from classification rules.
-
-        Define antecedent and consequent.
-        - stable_attributes
-        - flexible_attributes
-        - consequent
-        Confidence and support.
-        - conf_col
-        - supp_col
-        Desired classes or desired changes must be entered.
-        - desired_classes
-        - desired_changes
-        Should NaN values be used?
-        - is_nan
-        Should the reduction table be used?
-        - is_reduction
-        Minimal number of stable and flexible pairs in antecedent.
-        - min_stable_attributes
-        - min_flexible_attributes
-        - max_stable_attributes
-        - max_flexible_attributes
-
-        Parameters
-        ----------
-        stable_attributes: List[str]
-            List of column names.
-        flexible_attributes: List[str]
-            List of column names.
-        consequent: str
-            Name of the consequent column.
-        conf_col: str
-            Name of the column with classification rule confidence -
-            the numbers should be in form 0.1 for 10%.
-        supp_col: str
-            Name of the column with classification rule support -
-            the numbers should be in form 0.1 for 10%.
-        desired_classes: List[str] = None
-            List of decision states. For example ["1"].
-            DEFAULT: None
-        desired_changes: List[list] = None
-            List of desired changes. For example [["0", "1"]].
-            DEFAULT: None
-        is_nan: bool = False
-            True means NaN values are used, False means nan values are not used.
-            DEFAULT: FALSE
-        is_reduction: bool = True
-            Is the reduction table used?
-            DEFAULT: TRUE
-        min_stable_attributes: int = 1
-            Minimal number of stable pairs.
-            DEFAULT: 1
-        min_flexible_attributes: int = 1
-            Minimal number of flexible pairs.
-            DEFAULT: 1
-        max_stable_attributes: int = 5
-            Maximal number of stable pairs.
-            DEFAULT: 5
-        max_flexible_attributes: int = 5
-            Maximal number of flexible pairs.
-            DEFAULT: 5
-        """
-        if (self.action_rules):
-            raise Exception("Fit was already called")
-        self.stable_attributes = stable_attributes
-        self.flexible_attributes = flexible_attributes
-        self.consequent = consequent
-        if bool(desired_classes) != bool(desired_changes):
-            self.desired_state = DesiredState(desired_classes=desired_classes, desired_changes=desired_changes)
-        else:
-            raise Exception("Desired classes or desired changes must be entered")
-        attributes = stable_attributes + flexible_attributes
-        self._check_columns(attributes, consequent)
-        stable = self.decisions.data[stable_attributes]
-        flex = self.decisions.data[flexible_attributes]
-        target = self.decisions.data[[consequent]]
-        supp_df = self.decisions.data[[supp_col]]
-        supp_series = supp_df.iloc[:, 0]
-        supp = supp_series.tolist()
-        conf_df = self.decisions.data[[conf_col]]
-        conf_series = conf_df.iloc[:, 0]
-        conf = conf_series.tolist()
-        reduced_tables = Reduction(stable, flex, target, self.desired_state, supp, conf, is_nan)
-        if is_reduction:
-            reduced_tables.reduce()
-        self.action_rules = ActionRules(
-            reduced_tables.stable_tables,
-            reduced_tables.flexible_tables,
-            reduced_tables.decision_tables,
-            self.desired_state,
-            reduced_tables.supp,
-            reduced_tables.conf,
-            is_nan,
-            min_stable_attributes,
-            min_flexible_attributes,
-            max_stable_attributes,
-            max_flexible_attributes
-        )
-        self.action_rules.fit()
-
-    def get_action_rules(self) -> list:
-        """Get machine representations of action rules.
-
-        The output is a list of action
-        rules. Each action rule is a list where the first part is an action rule itself, and the second part is
-        a tuple of (support before, support after, action rule support), (confidence before, confidence after, action
-        rule confidence) and uplift.
-
-        Returns
-        -------
-        list
-            Returns list of action rules.
-        """
-        return self.action_rules.action_rules
-
-    def get_pretty_action_rules(self) -> list:
-        """Get human-readable representations of action rules.
-
-        Returns
-        -------
-        list
-            Returns list of action rules.
-        """
-        if len(self.action_rules.action_rules_pretty_text) == 0:
-            self.action_rules.pretty_text()
-        return self.action_rules.action_rules_pretty_text
-
-    def get_action_rules_representation(self) -> list:
-        """Get math representation of action rules.
-
-        Returns
-        -------
-        list
-            Returns list of action rules.
-        """
-        if len(self.action_rules.action_rules_representation) == 0:
-            self.action_rules.representation()
-        return self.action_rules.action_rules_representation
-
-    def get_source_data_for_ar(self, action_r_number: int, is_before: bool) -> pd.DataFrame:
-        """ Get data frame with values which the action rule is based on.
-
-        Yellow background - stable attributes
-        Orange background - flexible attributes
-        Red text - Target attribute, undesired state
-        Green text - Target attribute, desired state
-
-        Parameters
-        ----------
-        action_r_number : int
-            The number of action rule - you can figure out from get_action_rules
-        is_before : bool
-            True shows instances in data that match the conditions of the "before" part of the action rule.
-            False show instances in data that match the conditions of the "after" part of the action rule.
-
-        Returns
-        -------
-        pd.DataFrame
-            Returns data frame with transactions data.
-        """
-        if is_before:
-            classification = self.action_rules.classification_before[action_r_number]
-        else:
-            classification = self.action_rules.classification_after[action_r_number]
-        decision = self.decisions.decision_table.loc[
-            classification, self.stable_attributes + self.flexible_attributes]
-        source_table = self._reduce_table_source(decision, self.decisions.data)
-        return source_table.style.applymap(lambda x: 'background-color: yellow',
-                                           subset=self.stable_attributes) \
-            .applymap(lambda x: 'background-color: orange',
-                      subset=self.flexible_attributes) \
-            .applymap(lambda x: 'color: green' if x in self.desired_state.get_destination_classes() else 'color: red',
-                      subset=[self.consequent])
-
-    @staticmethod
-    def _reduce_table_source(decision: pd.Series, source_table: pd.DataFrame) -> pd.DataFrame:
-        """ Get data frame limited by concrete classification rule.
-
-        Parameters
-        ----------
-        decision : pd.Series
-            A classification rule.
-        source_table : pd.DataFrame
-            A source data frame.
-
-        Returns
-        -------
-        pd.DataFrame
-            Returns a limited data frame.
-        """
-        new_data = source_table.applymap(str).copy()
-        for key, value in decision.items():
-            if str(value) != "nan":
-                mask = new_data[key] == value
-                new_data = new_data[mask]
-        return new_data
-
-    def predict(self, source_table: pd.DataFrame) -> pd.DataFrame:
-        """ Predicts if any values would need to change their state.
-
-        Parameters
-        ----------
-        source_table : pd.DataFrame
-            A data frame with new observations.
-
-        Returns
-        -------
-        pd.DataFrame
-            Returns a data frame with recommended actions.
-        """
-        i = 0
-        full_predicted_table = pd.DataFrame()
-        for classification_before in self.action_rules.classification_before:
-            classification_after = self.action_rules.classification_after[i]
-            decision_before = self.decisions.decision_table.loc[
-                classification_before, self.stable_attributes + self.flexible_attributes]
-            decision_after = self.decisions.decision_table.loc[
-                classification_after, self.stable_attributes + self.flexible_attributes]
-            predicted_table = self._reduce_table_source(decision_before, source_table)
-            if len(predicted_table.index) > 0:
-                for key, value in decision_after.items():
-                    if str(value) != "nan" and key in self.flexible_attributes:
-                        column = key + self.RECOMMENDED
-                        predicted_table[column] = [value] * len(predicted_table.index)
-                        predicted_table[self.ACTION_RULE] = [i] * len(predicted_table.index)
-                        predicted_table = predicted_table.astype({self.ACTION_RULE: int})
-                predicted_table[self.ACTION_RULE_TARGET] = \
-                    [self.action_rules.action_rules[i][0][2][1][1]] * len(predicted_table.index)
-                predicted_table[self.SUPPORT_BEFORE] = \
-                    [self.action_rules.action_rules[i][1][0]] * len(predicted_table.index)
-                predicted_table[self.SUPPORT_AFTER] = \
-                    [self.action_rules.action_rules[i][1][1]] * len(predicted_table.index)
-                predicted_table[self.ACTION_RULE_SUPPORT] = \
-                    [self.action_rules.action_rules[i][1][2]] * len(predicted_table.index)
-                predicted_table[self.CONFIDENCE_BEFORE] = \
-                    [self.action_rules.action_rules[i][2][0]] * len(predicted_table.index)
-                predicted_table[self.CONFIDENCE_AFTER] = \
-                    [self.action_rules.action_rules[i][2][1]] * len(predicted_table.index)
-                predicted_table[self.ACTION_RULE_CONFIDENCE] = \
-                    [self.action_rules.action_rules[i][2][2]] * len(predicted_table.index)
-                predicted_table[self.ACTION_RULE_UPLIFT] = \
-                    [self.action_rules.action_rules[i][3]] * len(predicted_table.index)
-            full_predicted_table = pd.concat([full_predicted_table, predicted_table], sort=True)
-            i += 1
-        # New columns always in the end
-        cols = full_predicted_table.columns.tolist()
-        if len(cols)>0:
-            cols.append(cols.pop(cols.index(self.ACTION_RULE)))
-            cols.append(cols.pop(cols.index(self.ACTION_RULE_TARGET)))
-            cols.append(cols.pop(cols.index(self.SUPPORT_BEFORE)))
-            cols.append(cols.pop(cols.index(self.SUPPORT_AFTER)))
-            cols.append(cols.pop(cols.index(self.ACTION_RULE_SUPPORT)))
-            cols.append(cols.pop(cols.index(self.CONFIDENCE_BEFORE)))
-            cols.append(cols.pop(cols.index(self.CONFIDENCE_AFTER)))
-            cols.append(cols.pop(cols.index(self.ACTION_RULE_CONFIDENCE)))
-            cols.append(cols.pop(cols.index(self.ACTION_RULE_UPLIFT)))
-            full_predicted_table = full_predicted_table[cols]
-        return full_predicted_table
+from typing import List
+import pandas as pd
+
+from actionrules.desiredState import DesiredState
+from actionrules.decisions import Decisions
+from actionrules.reduction import Reduction
+from actionrules.actionRules import ActionRules
+
+
+class ActionRulesDiscovery:
+    """
+    The class ActionRulesDiscovery is the main control class where the methods fit or
+    predict can be called. However, there is a minimum logic in the class. It is just an
+    interface that initializes other objects and calls their methods.
+
+    ...
+
+    Attributes
+    ----------
+    decisions : Decisions()
+        Object that runs PyFIM classification rules discovery.
+    action_rules: None or ActionRules
+        Object that runs action rules discovery.
+    desired_state: DesiredState
+        Object that is responsible for handling of desired state.
+    stable_attributes: List[str]
+        List of stable attributes.
+    flexible_attributes: List[str]
+        List of flexible attributes.
+    consequent: str
+        Name of consequent columns.
+
+    Methods
+    -------
+    read_csv(self, file: str, **kwargs)
+        Import data from a CSV file.
+    load_pandas(self, data_frame: pd.DataFrame)
+        Import data from Pandas data frame.
+    fit(self,
+        stable_attributes: List[str],
+        flexible_attributes: List[str],
+        consequent: str,
+        conf: float,
+        supp: float,
+        desired_classes: List[str] = None,
+        desired_changes: List[list] = None,
+        is_nan: bool = False,
+        is_reduction: bool = True,
+        min_stable_attributes: int = 1,
+        min_flexible_attributes: int = 1,
+        max_stable_attributes: int = 5,
+        max_flexible_attributes: int = 5,
+        )
+        Train the model from transaction data.
+    fit_classification_rules(self,
+                             stable_attributes: List[str],
+                             flexible_attributes: List[str],
+                             consequent: str,
+                             conf_col: str,
+                             supp_col: str,
+                             desired_classes: List[str] = None,
+                             desired_changes: List[list] = None,
+                             is_nan: bool = False,
+                             is_reduction: bool = True,
+                             min_stable_attributes: int = 1,
+                             min_flexible_attributes: int = 1,
+                             max_stable_attributes: int = 5,
+                             max_flexible_attributes: int = 5,
+                             )
+        Train the model from classification rules.
+    get_action_rules(self) -> list
+        Get list of action rules (machine representation)
+    get_pretty_action_rules(self) -> list
+        Get human-readable representations of action rules
+    get_action_rules_representation(self) -> list
+        Get math representation of action rules
+    get_source_data_for_ar(self, action_r_number: int, is_before: bool) -> pd.DataFrame
+        Get the source data the action rule is discovered from.
+    predict(self, source_table: pd.DataFrame) -> pd.DataFrame
+        Predicts if new occurrence would need any change.
+
+    """
+    ACTION_RULE = "action rule"
+    ACTION_RULE_TARGET = "action rule target"
+    SUPPORT_BEFORE = "support before"
+    SUPPORT_AFTER = "support after"
+    ACTION_RULE_SUPPORT = "action rule support"
+    CONFIDENCE_BEFORE = "confidence before"
+    CONFIDENCE_AFTER = "confidence after"
+    ACTION_RULE_CONFIDENCE = "action rule confidence"
+    ACTION_RULE_UPLIFT = "uplift"
+    RECOMMENDED = "-recommended"
+
+    def __init__(self):
+        """
+        Initialise
+        """
+        self.decisions = Decisions()
+        self.action_rules = None
+        self.desired_state = None
+        self.stable_attributes = []
+        self.flexible_attributes = []
+        self.consequent = ""
+
+    def _check_columns(self, attributes: List[str], consequent: str):
+        """Checks if inserted data is valid (columns exist, rows exist).
+
+        Parameters
+        ----------
+        attributes : List[str]
+            List of attributes names.
+        consequent : str
+            The name of consequent.
+
+        Raises
+        ------
+        Exception
+            If no data entered or column does not exist in data.
+        """
+        if len(self.decisions.data) == 0:
+            raise Exception("No data entered.")
+        columns = self.decisions.data.columns
+        for col_name in attributes + [consequent]:
+            if col_name not in columns:
+                raise Exception("Column " + str(col_name) + " does not exist in data")
+
+    def read_csv(self, file: str, **kwargs):
+        """Imports data from a CSV file.
+
+        It uses the same optional parameters as read_csv from Pandas.
+
+        Parameters
+        ----------
+        file : str
+            A path to a file.
+        **kwargs :
+            Arbitrary keyword arguments (the same as in Pandas).
+        """
+        self.decisions.read_csv(file, **kwargs)
+
+    def load_pandas(self, data_frame: pd.DataFrame):
+        """Loads a data frame.
+
+        It must be the Pandas data frame.
+
+        Parameters
+        ----------
+        data_frame : pd.DataFrame
+            Pandas data frame.
+        """
+        self.decisions.load_pandas(data_frame)
+
+    def fit(self,
+            stable_attributes: List[str],
+            flexible_attributes: List[str],
+            consequent: str,
+            conf: float,
+            supp: float,
+            desired_classes: List[str] = None,
+            desired_changes: List[list] = None,
+            is_nan: bool = False,
+            is_reduction: bool = True,
+            min_stable_attributes: int = 1,
+            min_flexible_attributes: int = 1,
+            max_stable_attributes: int = 5,
+            max_flexible_attributes: int = 5,
+            ):
+        """Train the model from transaction data.
+
+        Define antecedent and consequent.
+        - stable_attributes
+        - flexible_attributes
+        - consequent
+        Confidence and support.
+        - conf
+        - supp
+        Desired classes or desired changes must be entered.
+        - desired_classes
+        - desired_changes
+        Should uncertainty be used?
+        - is_nan
+        Should the reduction table be used?
+        - is_reduction
+        Minimal number of stable and flexible pairs in antecedent.
+        - min_stable_attributes
+        - min_flexible_attributes
+        - max_stable_attributes
+        - max_flexible_attributes
+
+        Parameters
+        ----------
+        stable_attributes : List[str]
+            List of column names.
+        flexible_attributes : List[str]
+            List of column names.
+        consequent : str
+            Name of the consequent column.
+        conf : float
+            Value in % for minimal confidence in classification rules.
+            For example, 60.
+        supp : float
+            Value in % for minimal support of classification rules.
+            For example, 5.
+        desired_classes : List[str] = None
+            List of decision states. For example, ["1"].
+            DEFAULT: None
+        desired_changes : List[list] = None
+            List of desired changes. For example, [["0", "1"]].
+            DEFAULT: None
+        is_nan : bool = False
+            True means NaN values are used, False means NaN values are not used.
+            It means NaN values from classification rules.
+            If is_nan is true, the uncertainty is used.
+            DEFAULT: FALSE
+        is_reduction : bool = True
+            Is the reduction table used?
+            DEFAULT: TRUE
+        min_stable_attributes : int = 1
+            Minimal number of stable pairs.
+            DEFAULT: 1
+        min_flexible_attributes : int = 1
+            Minimal number of flexible pairs.
+            DEFAULT: 1
+        max_stable_attributes : int = 5
+            Maximal number of stable pairs.
+            DEFAULT: 5
+        max_flexible_attributes : int = 5
+            Maximal number of flexible pairs.
+            DEFAULT: 5
+        """
+        if (self.action_rules):
+            raise Exception("Fit was already called")
+        self.stable_attributes = stable_attributes
+        self.flexible_attributes = flexible_attributes
+        self.consequent = consequent
+        if bool(desired_classes) != bool(desired_changes):
+            self.desired_state = DesiredState(desired_classes=desired_classes, desired_changes=desired_changes)
+        else:
+            raise Exception("Desired classes or desired changes must be entered")
+        attributes = stable_attributes + flexible_attributes
+        self._check_columns(attributes, consequent)
+        self.decisions.prepare_data_fim(attributes, consequent)
+        self.decisions.fit_fim_apriori(conf=conf, support=supp)
+        self.decisions.generate_decision_table()
+        stable = self.decisions.decision_table[stable_attributes]
+        flex = self.decisions.decision_table[flexible_attributes]
+        target = self.decisions.decision_table[[consequent]]
+        supp = self.decisions.support
+        conf = self.decisions.confidence
+        reduced_tables = Reduction(stable, flex, target, self.desired_state, supp, conf, is_nan)
+        if is_reduction:
+            reduced_tables.reduce()
+        self.action_rules = ActionRules(
+            reduced_tables.stable_tables,
+            reduced_tables.flexible_tables,
+            reduced_tables.decision_tables,
+            self.desired_state,
+            self.decisions,
+            reduced_tables.supp,
+            reduced_tables.conf,
+            is_nan,
+            min_stable_attributes,
+            min_flexible_attributes,
+            max_stable_attributes,
+            max_flexible_attributes
+        )
+        self.action_rules.fit()
+
+    def fit_classification_rules(self,
+                                 stable_attributes: List[str],
+                                 flexible_attributes: List[str],
+                                 consequent: str,
+                                 conf_col: str,
+                                 supp_col: str,
+                                 desired_classes: List[str] = None,
+                                 desired_changes: List[list] = None,
+                                 is_nan: bool = False,
+                                 is_reduction: bool = True,
+                                 min_stable_attributes: int = 1,
+                                 min_flexible_attributes: int = 1,
+                                 max_stable_attributes: int = 5,
+                                 max_flexible_attributes: int = 5,
+                                 ):
+        """Train the model from classification rules.
+
+        Define antecedent and consequent.
+        - stable_attributes
+        - flexible_attributes
+        - consequent
+        Confidence and support.
+        - conf_col
+        - supp_col
+        Desired classes or desired changes must be entered.
+        - desired_classes
+        - desired_changes
+        Should uncertainty be used?
+        - is_nan
+        Should the reduction table be used?
+        - is_reduction
+        Minimal number of stable and flexible pairs in antecedent.
+        - min_stable_attributes
+        - min_flexible_attributes
+        - max_stable_attributes
+        - max_flexible_attributes
+
+        Parameters
+        ----------
+        stable_attributes: List[str]
+            List of column names.
+        flexible_attributes: List[str]
+            List of column names.
+        consequent: str
+            Name of the consequent column.
+        conf_col: str
+            Name of the column with classification rule confidence -
+            the numbers should be in form 0.1 for 10%.
+        supp_col: str
+            Name of the column with classification rule support -
+            the numbers should be in form 0.1 for 10%.
+        desired_classes: List[str] = None
+            List of decision states. For example ["1"].
+            DEFAULT: None
+        desired_changes: List[list] = None
+            List of desired changes. For example [["0", "1"]].
+            DEFAULT: None
+        is_nan: bool = False
+            True means NaN values are used, False means nan values are not used.
+            If is_nan is true, the uncertainty is used.
+            DEFAULT: FALSE
+        is_reduction: bool = True
+            Is the reduction table used?
+            DEFAULT: TRUE
+        min_stable_attributes: int = 1
+            Minimal number of stable pairs.
+            DEFAULT: 1
+        min_flexible_attributes: int = 1
+            Minimal number of flexible pairs.
+            DEFAULT: 1
+        max_stable_attributes: int = 5
+            Maximal number of stable pairs.
+            DEFAULT: 5
+        max_flexible_attributes: int = 5
+            Maximal number of flexible pairs.
+            DEFAULT: 5
+        """
+        if (self.action_rules):
+            raise Exception("Fit was already called")
+        self.stable_attributes = stable_attributes
+        self.flexible_attributes = flexible_attributes
+        self.consequent = consequent
+        if bool(desired_classes) != bool(desired_changes):
+            self.desired_state = DesiredState(desired_classes=desired_classes, desired_changes=desired_changes)
+        else:
+            raise Exception("Desired classes or desired changes must be entered")
+        attributes = stable_attributes + flexible_attributes
+        self._check_columns(attributes, consequent)
+        stable = self.decisions.data[stable_attributes]
+        flex = self.decisions.data[flexible_attributes]
+        target = self.decisions.data[[consequent]]
+        supp_df = self.decisions.data[[supp_col]]
+        supp_series = supp_df.iloc[:, 0]
+        supp = supp_series.tolist()
+        conf_df = self.decisions.data[[conf_col]]
+        conf_series = conf_df.iloc[:, 0]
+        conf = conf_series.tolist()
+        reduced_tables = Reduction(stable, flex, target, self.desired_state, supp, conf, is_nan)
+        if is_reduction:
+            reduced_tables.reduce()
+        self.decisions.data = pd.DataFrame()
+        self.action_rules = ActionRules(
+            reduced_tables.stable_tables,
+            reduced_tables.flexible_tables,
+            reduced_tables.decision_tables,
+            self.desired_state,
+            self.decisions,
+            reduced_tables.supp,
+            reduced_tables.conf,
+            is_nan,
+            min_stable_attributes,
+            min_flexible_attributes,
+            max_stable_attributes,
+            max_flexible_attributes
+        )
+        self.action_rules.fit()
+
+    def get_action_rules(self) -> list:
+        """Get machine representations of action rules.
+
+        The output is a list of action
+        rules. Each action rule is a list where the first part is an action rule itself, and the second part is
+        a tuple of (support before, support after, action rule support), (confidence before, confidence after, action
+        rule confidence) and uplift.
+
+        Returns
+        -------
+        list
+            Returns list of action rules.
+        """
+        return self.action_rules.action_rules
+
+    def get_pretty_action_rules(self) -> list:
+        """Get human-readable representations of action rules.
+
+        Returns
+        -------
+        list
+            Returns list of action rules.
+        """
+        if len(self.action_rules.action_rules_pretty_text) == 0:
+            self.action_rules.pretty_text()
+        return self.action_rules.action_rules_pretty_text
+
+    def get_action_rules_representation(self) -> list:
+        """Get math representation of action rules.
+
+        Returns
+        -------
+        list
+            Returns list of action rules.
+        """
+        if len(self.action_rules.action_rules_representation) == 0:
+            self.action_rules.representation()
+        return self.action_rules.action_rules_representation
+
+    def get_source_data_for_ar(self, action_r_number: int, is_before: bool) -> pd.DataFrame:
+        """ Get data frame with values which the action rule is based on.
+
+        Yellow background - stable attributes
+        Orange background - flexible attributes
+        Red text - Target attribute, undesired state
+        Green text - Target attribute, desired state
+
+        Parameters
+        ----------
+        action_r_number : int
+            The number of action rule - you can figure out from get_action_rules
+        is_before : bool
+            True shows instances in data that match the conditions of the "before" part of the action rule.
+            False show instances in data that match the conditions of the "after" part of the action rule.
+
+        Returns
+        -------
+        pd.DataFrame
+            Returns data frame with transactions data.
+        """
+        if len(self.decisions.data) == 0:
+            print('No source data')
+            return pd.DataFrame()
+        if is_before:
+            classification = self.action_rules.classification_before[action_r_number]
+        else:
+            classification = self.action_rules.classification_after[action_r_number]
+        decision = self.decisions.decision_table.loc[
+            classification, self.stable_attributes + self.flexible_attributes]
+        source_table = self._reduce_table_source(decision, self.decisions.data)
+        return source_table.style.applymap(lambda x: 'background-color: yellow',
+                                           subset=self.stable_attributes) \
+            .applymap(lambda x: 'background-color: orange',
+                      subset=self.flexible_attributes) \
+            .applymap(lambda x: 'color: green' if x in self.desired_state.get_destination_classes() else 'color: red',
+                      subset=[self.consequent])
+
+    @staticmethod
+    def _reduce_table_source(decision: pd.Series, source_table: pd.DataFrame) -> pd.DataFrame:
+        """ Get data frame limited by concrete classification rule.
+
+        Parameters
+        ----------
+        decision : pd.Series
+            A classification rule.
+        source_table : pd.DataFrame
+            A source data frame.
+
+        Returns
+        -------
+        pd.DataFrame
+            Returns a limited data frame.
+        """
+        new_data = source_table.applymap(str).copy()
+        for key, value in decision.items():
+            if str(value) != "nan":
+                mask = new_data[key] == value
+                new_data = new_data[mask]
+        return new_data
+
+    def predict(self, source_table: pd.DataFrame) -> pd.DataFrame:
+        """ Predicts if any values would need to change their state.
+
+        Parameters
+        ----------
+        source_table : pd.DataFrame
+            A data frame with new observations.
+
+        Returns
+        -------
+        pd.DataFrame
+            Returns a data frame with recommended actions.
+        """
+        i = 0
+        full_predicted_table = pd.DataFrame()
+        for classification_before in self.action_rules.classification_before:
+            classification_after = self.action_rules.classification_after[i]
+            decision_before = self.decisions.decision_table.loc[
+                classification_before, self.stable_attributes + self.flexible_attributes]
+            decision_after = self.decisions.decision_table.loc[
+                classification_after, self.stable_attributes + self.flexible_attributes]
+            predicted_table = self._reduce_table_source(decision_before, source_table)
+            if len(predicted_table.index) > 0:
+                for key, value in decision_after.items():
+                    if str(value) != "nan" and key in self.flexible_attributes:
+                        column = key + self.RECOMMENDED
+                        predicted_table[column] = [value] * len(predicted_table.index)
+                        predicted_table[self.ACTION_RULE] = [i] * len(predicted_table.index)
+                        predicted_table = predicted_table.astype({self.ACTION_RULE: int})
+                predicted_table[self.ACTION_RULE_TARGET] = \
+                    [self.action_rules.action_rules[i][0][2][1][1]] * len(predicted_table.index)
+                predicted_table[self.SUPPORT_BEFORE] = \
+                    [self.action_rules.action_rules[i][1][0]] * len(predicted_table.index)
+                predicted_table[self.SUPPORT_AFTER] = \
+                    [self.action_rules.action_rules[i][1][1]] * len(predicted_table.index)
+                predicted_table[self.ACTION_RULE_SUPPORT] = \
+                    [self.action_rules.action_rules[i][1][2]] * len(predicted_table.index)
+                predicted_table[self.CONFIDENCE_BEFORE] = \
+                    [self.action_rules.action_rules[i][2][0]] * len(predicted_table.index)
+                predicted_table[self.CONFIDENCE_AFTER] = \
+                    [self.action_rules.action_rules[i][2][1]] * len(predicted_table.index)
+                predicted_table[self.ACTION_RULE_CONFIDENCE] = \
+                    [self.action_rules.action_rules[i][2][2]] * len(predicted_table.index)
+                predicted_table[self.ACTION_RULE_UPLIFT] = \
+                    [self.action_rules.action_rules[i][3]] * len(predicted_table.index)
+            full_predicted_table = pd.concat([full_predicted_table, predicted_table], sort=True)
+            i += 1
+        # New columns always in the end
+        cols = full_predicted_table.columns.tolist()
+        if len(cols)>0:
+            cols.append(cols.pop(cols.index(self.ACTION_RULE)))
+            cols.append(cols.pop(cols.index(self.ACTION_RULE_TARGET)))
+            cols.append(cols.pop(cols.index(self.SUPPORT_BEFORE)))
+            cols.append(cols.pop(cols.index(self.SUPPORT_AFTER)))
+            cols.append(cols.pop(cols.index(self.ACTION_RULE_SUPPORT)))
+            cols.append(cols.pop(cols.index(self.CONFIDENCE_BEFORE)))
+            cols.append(cols.pop(cols.index(self.CONFIDENCE_AFTER)))
+            cols.append(cols.pop(cols.index(self.ACTION_RULE_CONFIDENCE)))
+            cols.append(cols.pop(cols.index(self.ACTION_RULE_UPLIFT)))
+            full_predicted_table = full_predicted_table[cols]
+        return full_predicted_table
```

### Comparing `actionrules-lukassykora-1.1.8/actionrules/decisions/decisions.py` & `actionrules-lukassykora-1.1.9/actionrules/decisions/decisions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,152 +1,154 @@
-import fim
-import pandas as pd
-import numpy as np
-from typing import List
-
-
-class Decisions:
-    """
-    The class Decision is used for classification rules mining. It uses library PyFim. A user
-    can get the classification rules in a different way. In this case, the Decision class just holds
-    classification rules.
-
-    ...
-
-    Attributes
-    ----------
-    data : pd.DataFrame
-        Source transaction data.
-    transactions : list
-        Transactions ready for PyFIM.
-    appearance : set
-        Set of columns ready for PyFIM.
-    rules : tuple
-        Classification rules from PyFIM.
-    decision_table : pd.DataFrame
-        Classification rules in Pandas data frame.
-    support : list
-        List of supports.
-    confidence : list
-        List of confidences.
-    max_length : int
-        Max length of classification rules.
-    Methods
-    -------
-    read_csv(self, file: str, **kwargs)
-        Get transaction data from a CSV file.
-    load_pandas(self, data_frame: pd.DataFrame)
-        Get transaction data from a Pandas data frame.
-    prepare_data_fim(self, antecedent_attributes: List[str], consequent: str)
-        Transform data to be usable in PyFIM.
-    fit_fim_apriori(self, conf: float=70, support: float=10)
-        Train the model with PyFIM.
-    generate_decision_table(self)
-        Generate classification rules from the model.
-    """
-
-    def __init__(self):
-        """Initialise.
-        """
-        self.data = pd.DataFrame()
-        self.transactions = []
-        self.appearance = set()
-        self.rules = ()
-        self.decision_table = pd.DataFrame()
-        self.support = []
-        self.confidence = []
-        self.max_length = 10
-
-    def read_csv(self, file: str, **kwargs):
-        """Loads a data from a CSV file. It uses the Pandas read_csv method.
-
-        Parameters
-        ----------
-        file : str
-            The path to transaction data.
-        **kwargs :
-            Arbitrary keyword arguments (the same as in Pandas).
-        """
-        self.data = pd.read_csv(file, **kwargs)
-
-    def load_pandas(self, data_frame: pd.DataFrame):
-        """Loads a data from a Pandas data frame.
-
-        Parameters
-        ----------
-        data_frame : pd.DataFrame
-            Data frame with transaction data.
-        """
-        self.data = data_frame
-
-    def prepare_data_fim(self, antecedent_attributes: List[str], consequent: str):
-        """Data preparation for PyFIM.
-
-        Parameters
-        ----------
-        antecedent_attributes : List[str]
-            Antecedent columns names.
-        consequent : str
-            Consequent column name.
-        """
-        self.max_length = len(antecedent_attributes) + 1
-        for index, row in self.data.iterrows():
-            transaction_row = []
-            for i, v in row.iteritems():
-                side_type = None
-                if i == consequent:
-                    side_type = "c"
-                elif i in antecedent_attributes:
-                    side_type = "a"
-                if side_type:
-                    self.appearance.add((str(i) + "<:> " + str(v), side_type))
-                    transaction_row.append(str(i) + "<:> " + str(v))
-            self.transactions.append(transaction_row)
-
-    def fit_fim_apriori(self, conf: float=70, support: float=10):
-        """Train the model to be able to get classification rules (PyFIM).
-
-        Parameters
-        ----------
-        conf : float = 70
-            Confidence.
-            DEFAULT: 70%
-        support : float = 10
-            Support.
-            DEFAULT: 10%
-        """
-        self.rules = fim.arules(self.transactions,
-                                supp=support,
-                                conf=conf,
-                                report="sc",
-                                mode="o",
-                                appear=dict(self.appearance),
-                                zmin=2,  # At least one antecedent and consequent
-                                zmax=self.max_length)
-
-    def generate_decision_table(self):
-        """Generates table of classification rules.
-
-        """
-        for rule in self.rules:
-            values = []
-            cols = []
-            # Antecedent
-            for cedent in rule[1]:
-                cols.append(cedent.split("<:> ")[0])
-                value = cedent.split("<:> ")[1]
-                if value == "nan":
-                    values.append(np.NaN)
-                else:
-                    values.append(value)
-            # Subsequent
-            cols.append(rule[0].split("<:> ")[0])
-            value = rule[0].split("<:> ")[1]
-            if value == "nan":
-                values.append(np.NaN)
-            else:
-                values.append(value)
-
-            df2 = pd.DataFrame([values], columns=cols)
-            self.decision_table = self.decision_table.append(df2, sort=False, ignore_index=True)
-            self.support.append(rule[2])
-            self.confidence.append(rule[3])
+import fim
+import pandas as pd
+import numpy as np
+from typing import List
+
+
+class Decisions:
+    """
+    The class Decision is used for classification rules mining. It uses library PyFim. A user
+    can get the classification rules in a different way. In this case, the Decision class just holds
+    classification rules.
+
+    ...
+
+    Attributes
+    ----------
+    data : pd.DataFrame
+        Source transaction data.
+    transactions : list
+        Transactions ready for PyFIM.
+    appearance : set
+        Set of columns ready for PyFIM.
+    rules : tuple
+        Classification rules from PyFIM.
+    decision_table : pd.DataFrame
+        Classification rules in Pandas data frame.
+    support : list
+        List of supports.
+    confidence : list
+        List of confidences.
+    max_length : int
+        Max length of classification rules.
+    Methods
+    -------
+    read_csv(self, file: str, **kwargs)
+        Get transaction data from a CSV file.
+    load_pandas(self, data_frame: pd.DataFrame)
+        Get transaction data from a Pandas data frame.
+    prepare_data_fim(self, antecedent_attributes: List[str], consequent: str)
+        Transform data to be usable in PyFIM.
+    fit_fim_apriori(self, conf: float=70, support: float=10)
+        Train the model with PyFIM.
+    generate_decision_table(self)
+        Generate classification rules from the model.
+    """
+
+    def __init__(self):
+        """Initialise.
+        """
+        self.data = pd.DataFrame()
+        self.transactions = []
+        self.appearance = set()
+        self.rules = ()
+        self.decision_table = pd.DataFrame()
+        self.support = []
+        self.confidence = []
+        self.max_length = 10
+
+    def read_csv(self, file: str, **kwargs):
+        """Loads a data from a CSV file. It uses the Pandas read_csv method.
+
+        Parameters
+        ----------
+        file : str
+            The path to transaction data.
+        **kwargs :
+            Arbitrary keyword arguments (the same as in Pandas).
+        """
+        self.data = pd.read_csv(file, **kwargs)
+        self.data = self.data.applymap(str)
+
+    def load_pandas(self, data_frame: pd.DataFrame):
+        """Loads a data from a Pandas data frame.
+
+        Parameters
+        ----------
+        data_frame : pd.DataFrame
+            Data frame with transaction data.
+        """
+        self.data = data_frame
+        self.data = self.data.applymap(str)
+
+    def prepare_data_fim(self, antecedent_attributes: List[str], consequent: str):
+        """Data preparation for PyFIM.
+
+        Parameters
+        ----------
+        antecedent_attributes : List[str]
+            Antecedent columns names.
+        consequent : str
+            Consequent column name.
+        """
+        self.max_length = len(antecedent_attributes) + 1
+        for index, row in self.data.iterrows():
+            transaction_row = []
+            for i, v in row.iteritems():
+                side_type = None
+                if i == consequent:
+                    side_type = "c"
+                elif i in antecedent_attributes:
+                    side_type = "a"
+                if side_type:
+                    self.appearance.add((str(i) + "<:> " + str(v), side_type))
+                    transaction_row.append(str(i) + "<:> " + str(v))
+            self.transactions.append(transaction_row)
+
+    def fit_fim_apriori(self, conf: float=70, support: float=10):
+        """Train the model to be able to get classification rules (PyFIM).
+
+        Parameters
+        ----------
+        conf : float = 70
+            Confidence.
+            DEFAULT: 70%
+        support : float = 10
+            Support.
+            DEFAULT: 10%
+        """
+        self.rules = fim.arules(self.transactions,
+                                supp=support,
+                                conf=conf,
+                                report="sc",
+                                mode="o",
+                                appear=dict(self.appearance),
+                                zmin=2,  # At least one antecedent and consequent
+                                zmax=self.max_length)
+
+    def generate_decision_table(self):
+        """Generates table of classification rules.
+
+        """
+        for rule in self.rules:
+            values = []
+            cols = []
+            # Antecedent
+            for cedent in rule[1]:
+                cols.append(cedent.split("<:> ")[0])
+                value = cedent.split("<:> ")[1]
+                if value == "nan":
+                    values.append(np.NaN)
+                else:
+                    values.append(value)
+            # Subsequent
+            cols.append(rule[0].split("<:> ")[0])
+            value = rule[0].split("<:> ")[1]
+            if value == "nan":
+                values.append(np.NaN)
+            else:
+                values.append(value)
+
+            df2 = pd.DataFrame([values], columns=cols)
+            self.decision_table = self.decision_table.append(df2, sort=False, ignore_index=True)
+            self.support.append(rule[2])
+            self.confidence.append(rule[3])
```

### Comparing `actionrules-lukassykora-1.1.8/actionrules/desiredState/desiredState.py` & `actionrules-lukassykora-1.1.9/actionrules/desiredState/desiredState.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,184 +1,201 @@
-from typing import List
-import pandas as pd
-
-
-class DesiredState:
-    """
-    The class DesiredState is responsible for all features that are needed to recognize the
-    candidate pair for the target variable.
-
-    ...
-
-    Attributes
-    ----------
-    desired_classes : List[str] or None
-        Desired classes.
-    desired_changes : List[list] or None
-        Desired changes.
-
-    Methods
-    -------
-    is_candidate_decision(self, decision_before: str, decision_after: str) -> bool
-        It checks if a pair of consequent values is a candidate.
-    is_candidate(self, decision_column: pd.DataFrame) -> bool
-        Is it possible to get any action rules (variability, desired classes)?
-    get_destination_classes(self) -> List[str]
-        Get list of possible desired classes.
-    """
-
-    def __init__(self, desired_classes: List[str] = None, desired_changes: List[list] = None):
-        """Initialise the desired state. There are 2 options:
-
-        1) Desired class or desired classes
-        2) Desired changes
-
-        Parameters
-        ----------
-        desired_classes : List[str]
-            List of desired classes. For example: ['survived', 'survived with injury'].
-        desired_changes : List[list]
-            Concrete desired changes. For example: [['death', 'survived'], ['death', 'survived with injury']]
-        """
-        self.desired_classes = desired_classes
-        self.desired_changes = desired_changes
-
-    def is_candidate_decision(self, decision_before: str, decision_after: str) -> bool:
-        """It checks if a pair of consequent is a candidate.
-
-        Parameters
-        ----------
-        decision_before : str
-            The value of a decision before.
-        decision_after : str
-            The value of a decision after.
-
-        Returns
-        -------
-        bool
-            Could it be a candidate pair?
-        """
-        if decision_before == decision_after:
-            return False
-        if self.desired_classes and decision_after not in self.desired_classes:
-            return False
-        if self.desired_changes and \
-                [decision_before, decision_after] not in self.desired_changes:
-            return False
-        return True
-
-    def is_candidate(self, decision_column: pd.DataFrame) -> bool:
-        """Is it possible to get any action rules from a consequent data frame (variability, desired classes)?
-
-        Parameters
-        ----------
-        decision_column : pd.DataFrame
-            Data frame with consequent values.
-
-        Returns
-        -------
-        bool
-            Could action rules be in the data frame?
-        """
-        # decision values are all the same
-        if not self._has_variability(decision_column):
-            return False
-        # does have desired class
-        if self.desired_classes and not self._is_desired_classes_candidate(decision_column):
-            return False
-        # does have desired class
-        if self.desired_changes and not self._is_desired_changes_candidate(decision_column):
-            return False
-        # otherwise
-        return True
-
-    def _is_desired_classes_candidate(self, decision_column: pd.DataFrame) -> bool:
-        """Check if table has at least one desired class.
-
-        Parameters
-        ----------
-        decision_column : pd.DataFrame
-            Data frame with consequent values.
-
-        Returns
-        -------
-        bool
-            Does the data frame contain any desired classes?
-        """
-        is_candidate = False
-        unique_decisions = self._get_unique_values(decision_column, 0)
-        for desired_class in self.desired_classes:
-            if desired_class in unique_decisions:
-                is_candidate = True
-        return is_candidate
-
-    def _is_desired_changes_candidate(self, decision_column: pd.DataFrame) -> bool:
-        """Check if table has at least one desired change of consequent.
-
-        Parameters
-        ----------
-        decision_column : pd.DataFrame
-            Data frame with consequent values.
-
-        Returns
-        -------
-        bool
-            Does the data frame contain any desired changes?
-        """
-        is_candidate = False
-        unique_decisions = self._get_unique_values(decision_column, 0)
-        for desired_change in self.desired_changes:
-            if desired_change[0] in unique_decisions and desired_change[1] in unique_decisions:
-                is_candidate = True
-        return is_candidate
-
-    def _has_variability(self, decision_column: pd.DataFrame) -> bool:
-        """Is there enough variability in desired classes?
-
-        Parameters
-        ----------
-        decision_column : pd.DataFrame
-            Data frame with consequent values.
-
-        Returns
-        -------
-        bool
-            Does the data frame have enough variability?
-        """
-        unique_decisions = self._get_unique_values(decision_column, 0)
-        if len(unique_decisions) == 1:
-            return False
-        return True
-
-    def get_destination_classes(self) -> List[str]:
-        """Get all possible desired classes.
-
-        Returns
-        -------
-        List[str]
-            All possible desired classes.
-        """
-        destination_classes = []
-        if self.desired_classes:
-            destination_classes = destination_classes + self.desired_classes
-        if self.desired_changes:
-            for desired_change in self.desired_changes:
-                destination_classes.append(desired_change[1])
-        return destination_classes
-
-    @staticmethod
-    def _get_unique_values(table: pd.DataFrame, column_number: int) -> list:
-        """Get unique values from column
-
-        Parameters
-        ----------
-        table : pd.DataFrame
-            Data frame with consequent values.
-        column_number : int
-            Column number to be checked,
-
-        Returns
-        -------
-        list
-            All unique values.
-        """
-        return table.iloc[:, column_number].unique()
+from typing import List
+import pandas as pd
+
+
+class DesiredState:
+    """
+    The class DesiredState is responsible for all features that are needed to recognize the
+    candidate pair for the target variable.
+
+    ...
+
+    Attributes
+    ----------
+    desired_classes : List[str] or None
+        Desired classes.
+    desired_changes : List[list] or None
+        Desired changes.
+
+    Methods
+    -------
+    is_candidate_decision(self, decision_before: str, decision_after: str) -> bool
+        It checks if a pair of consequent values is a candidate.
+    is_candidate(self, decision_column: pd.DataFrame) -> bool
+        Is it possible to get any action rules (variability, desired classes)?
+    get_destination_classes(self) -> List[str]
+        Get list of possible desired classes.
+    get_not_in_default_classes
+        Get the possible before part of consequent.
+    """
+
+    def __init__(self, desired_classes: List[str] = None, desired_changes: List[list] = None):
+        """Initialise the desired state. There are 2 options:
+
+        1) Desired class or desired classes
+        2) Desired changes
+
+        Parameters
+        ----------
+        desired_classes : List[str]
+            List of desired classes. For example: ['survived', 'survived with injury'].
+        desired_changes : List[list]
+            Concrete desired changes. For example: [['death', 'survived'], ['death', 'survived with injury']]
+        """
+        self.desired_classes = desired_classes
+        self.desired_changes = desired_changes
+
+    def is_candidate_decision(self, decision_before: str, decision_after: str) -> bool:
+        """It checks if a pair of consequent is a candidate.
+
+        Parameters
+        ----------
+        decision_before : str
+            The value of a decision before.
+        decision_after : str
+            The value of a decision after.
+
+        Returns
+        -------
+        bool
+            Could it be a candidate pair?
+        """
+        if decision_before == decision_after:
+            return False
+        if self.desired_classes and decision_after not in self.desired_classes:
+            return False
+        if self.desired_changes and \
+                [decision_before, decision_after] not in self.desired_changes:
+            return False
+        return True
+
+    def is_candidate(self, decision_column: pd.DataFrame) -> bool:
+        """Is it possible to get any action rules from a consequent data frame (variability, desired classes)?
+
+        Parameters
+        ----------
+        decision_column : pd.DataFrame
+            Data frame with consequent values.
+
+        Returns
+        -------
+        bool
+            Could action rules be in the data frame?
+        """
+        # decision values are all the same
+        if not self._has_variability(decision_column):
+            return False
+        # does have desired class
+        if self.desired_classes and not self._is_desired_classes_candidate(decision_column):
+            return False
+        # does have desired class
+        if self.desired_changes and not self._is_desired_changes_candidate(decision_column):
+            return False
+        # otherwise
+        return True
+
+    def _is_desired_classes_candidate(self, decision_column: pd.DataFrame) -> bool:
+        """Check if table has at least one desired class.
+
+        Parameters
+        ----------
+        decision_column : pd.DataFrame
+            Data frame with consequent values.
+
+        Returns
+        -------
+        bool
+            Does the data frame contain any desired classes?
+        """
+        is_candidate = False
+        unique_decisions = self._get_unique_values(decision_column, 0)
+        for desired_class in self.desired_classes:
+            if desired_class in unique_decisions:
+                is_candidate = True
+        return is_candidate
+
+    def _is_desired_changes_candidate(self, decision_column: pd.DataFrame) -> bool:
+        """Check if table has at least one desired change of consequent.
+
+        Parameters
+        ----------
+        decision_column : pd.DataFrame
+            Data frame with consequent values.
+
+        Returns
+        -------
+        bool
+            Does the data frame contain any desired changes?
+        """
+        is_candidate = False
+        unique_decisions = self._get_unique_values(decision_column, 0)
+        for desired_change in self.desired_changes:
+            if desired_change[0] in unique_decisions and desired_change[1] in unique_decisions:
+                is_candidate = True
+        return is_candidate
+
+    def _has_variability(self, decision_column: pd.DataFrame) -> bool:
+        """Is there enough variability in desired classes?
+
+        Parameters
+        ----------
+        decision_column : pd.DataFrame
+            Data frame with consequent values.
+
+        Returns
+        -------
+        bool
+            Does the data frame have enough variability?
+        """
+        unique_decisions = self._get_unique_values(decision_column, 0)
+        if len(unique_decisions) == 1:
+            return False
+        return True
+
+    def get_destination_classes(self) -> List[str]:
+        """Get all possible desired classes.
+
+        Returns
+        -------
+        List[str]
+            All possible desired classes.
+        """
+        destination_classes = []
+        if self.desired_classes:
+            destination_classes = destination_classes + self.desired_classes
+        if self.desired_changes:
+            for desired_change in self.desired_changes:
+                destination_classes.append(desired_change[1])
+        return destination_classes
+
+    def get_not_in_default_classes(self) -> List[str]:
+        """Get the possible before part of consequent.
+
+        Returns
+        -------
+        List[str]
+            All desired classes that are not in before part.
+        """
+        destination_classes = self.get_destination_classes()
+        if self.desired_changes:
+            for desired_change in self.desired_changes:
+                if desired_change[0] in destination_classes:
+                    destination_classes.remove(desired_change[0])
+        return destination_classes
+
+    @staticmethod
+    def _get_unique_values(table: pd.DataFrame, column_number: int) -> list:
+        """Get unique values from column
+
+        Parameters
+        ----------
+        table : pd.DataFrame
+            Data frame with consequent values.
+        column_number : int
+            Column number to be checked,
+
+        Returns
+        -------
+        list
+            All unique values.
+        """
+        return table.iloc[:, column_number].unique()
```

### Comparing `actionrules-lukassykora-1.1.8/actionrules/reduction/reduction.py` & `actionrules-lukassykora-1.1.9/actionrules/reduction/reduction.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,164 +1,164 @@
-import pandas as pd
-import numpy as np
-
-from actionrules.desiredState import DesiredState
-
-
-class Reduction:
-    """
-    The class Reduction creates the Reduction tree that speed up the discovery process.
-    This feature can be skipped. In this case, the Reduction class is not initialized.
-
-    ...
-
-    Attributes
-    ----------
-    stable_tables : List[pd.DataFrame]
-        List of data frames with stable attributes.
-    flexible_tables : List[pd.DataFrame]
-        List of data frames with flexible attributes.
-    decision_tables : List[pd.DataFrame]
-        List of data frames with consequent.
-    stable_columns_count : int
-        Count of stable attributes.
-    flexible_columns_count : int
-        Count of flexible attributes.
-    desired_state : DesiredState
-        DesiredState object.
-    self.supp : List[pd.Series]
-        List of Pandas Series with support.
-    self.conf : List[pd.Series]
-        List of Pandas Series with confidence.
-    self.is_nan : bool
-        Should uncertainty be used?
-
-    Methods
-    -------
-    reduce(self)
-        Reduce Decision table to many tables.
-    """
-
-    def __init__(self, stable_columns: pd.DataFrame, flexible_columns: pd.DataFrame, decision_column: pd.DataFrame,
-                 desired_state: DesiredState, supp: float, conf: float, is_nan: bool):
-        """Initialise.
-
-        Parameters
-        ----------
-        stable_columns: pd.DataFrame
-            Data frame with stable attributes.
-        flexible_columns: pd.DataFrame
-            Data frame with flexible attributes.
-        decision_column: pd.DataFrame
-            Data frame with consequent.
-        desired_state: DesiredState
-            DesiredState object.
-        supp: float
-            Support, for example 0.1 means 10%.
-        conf: float
-            Confidence, for example 0.8 means 80%.
-        is_nan: bool
-            Should uncertainty be used?
-        """
-        self.stable_tables = [stable_columns]
-        self.flexible_tables = [flexible_columns]
-        self.decision_tables = [decision_column]
-        self.stable_columns_count = self._get_columns_count(stable_columns)
-        self.flexible_columns_count = self._get_columns_count(flexible_columns)
-        self.desired_state = desired_state
-        self.supp = [pd.Series(supp)]
-        self.conf = [pd.Series(conf)]
-        self.is_nan = is_nan
-
-    @staticmethod
-    def _get_columns_count(columns: pd.DataFrame) -> int:
-        """Get the number of columns
-
-        Parameters
-        ----------
-        columns: pd.DataFrame
-            Data frame to check.
-
-        Returns
-        -------
-        int
-            Count of columns.
-        """
-        return len(columns.columns)
-
-    @staticmethod
-    def _get_unique_values(table: pd.DataFrame, column_number: int) -> list:
-        """Get unique values from column
-
-        Parameters
-        ----------
-        table : pd.DataFrame
-            Data frame with consequent values.
-        column_number : int
-            Column number to be checked.
-
-        Returns
-        -------
-        list
-            All unique values.
-        """
-        return table.iloc[:, column_number].unique()
-
-    def _split_tables_by_stable(self, stable_columns: pd.DataFrame, flexible_columns: pd.DataFrame,
-                               decision_column: pd.DataFrame,
-                               split_position: int, supp_series: pd.Series, conf_series: pd.Series):
-        """Split table by stable column.
-
-        Parameters
-        ----------
-        stable_columns : pd.DataFrame
-            Stable attributes.
-        flexible_columns : pd.DataFrame
-            Flexible attributes.
-        decision_column : pd.DataFrame
-            Consequent column.
-        split_position : int
-            The position where the split can be made.
-        supp_series : pd.Series
-            Support column.
-        conf_series : pd.Series
-            Confidence column.
-        """
-        unique_values = self._get_unique_values(stable_columns, split_position)
-        for unique_value in unique_values:
-            if self.is_nan:
-                mask = np.logical_or(stable_columns.iloc[:, split_position] == unique_value,
-                                     stable_columns.iloc[:, split_position].isnull())
-            else:
-                if str(unique_value) == "nan":
-                    mask = stable_columns.iloc[:, split_position].isnull()
-                else:
-                    mask = stable_columns.iloc[:, split_position] == unique_value
-            new_stable_table = stable_columns[mask]
-            new_flexible_table = flexible_columns[mask]
-            new_decision_table = decision_column[mask]
-            new_supp_series = supp_series[mask]
-            new_conf_series = conf_series[mask]
-            if self.desired_state.is_candidate(new_decision_table):
-                self.stable_tables.append(new_stable_table)
-                self.flexible_tables.append(new_flexible_table)
-                self.decision_tables.append(new_decision_table)
-                self.supp.append(new_supp_series)
-                self.conf.append(new_conf_series)
-
-    def reduce(self):
-        """Reduce Decision table to many reduction tables.
-
-        """
-        for split_position in range(self.stable_columns_count):
-            for table in range(len(self.stable_tables)):
-                stable_columns = self.stable_tables.pop(0)
-                flexible_columns = self.flexible_tables.pop(0)
-                decision_column = self.decision_tables.pop(0)
-                supp_series = self.supp.pop(0)
-                conf_series = self.conf.pop(0)
-                self._split_tables_by_stable(stable_columns,
-                                            flexible_columns,
-                                            decision_column,
-                                            split_position,
-                                            supp_series,
-                                            conf_series)
+import pandas as pd
+import numpy as np
+
+from actionrules.desiredState import DesiredState
+
+
+class Reduction:
+    """
+    The class Reduction creates the Reduction tree that speed up the discovery process.
+    This feature can be skipped. In this case, the Reduction class is not initialized.
+
+    ...
+
+    Attributes
+    ----------
+    stable_tables : List[pd.DataFrame]
+        List of data frames with stable attributes.
+    flexible_tables : List[pd.DataFrame]
+        List of data frames with flexible attributes.
+    decision_tables : List[pd.DataFrame]
+        List of data frames with consequent.
+    stable_columns_count : int
+        Count of stable attributes.
+    flexible_columns_count : int
+        Count of flexible attributes.
+    desired_state : DesiredState
+        DesiredState object.
+    self.supp : List[pd.Series]
+        List of Pandas Series with support.
+    self.conf : List[pd.Series]
+        List of Pandas Series with confidence.
+    self.is_nan : bool
+        Should uncertainty be used?
+
+    Methods
+    -------
+    reduce(self)
+        Reduce Decision table to many tables.
+    """
+
+    def __init__(self, stable_columns: pd.DataFrame, flexible_columns: pd.DataFrame, decision_column: pd.DataFrame,
+                 desired_state: DesiredState, supp: float, conf: float, is_nan: bool):
+        """Initialise.
+
+        Parameters
+        ----------
+        stable_columns: pd.DataFrame
+            Data frame with stable attributes.
+        flexible_columns: pd.DataFrame
+            Data frame with flexible attributes.
+        decision_column: pd.DataFrame
+            Data frame with consequent.
+        desired_state: DesiredState
+            DesiredState object.
+        supp: float
+            Support, for example 0.1 means 10%.
+        conf: float
+            Confidence, for example 0.8 means 80%.
+        is_nan: bool
+            Should uncertainty be used?
+        """
+        self.stable_tables = [stable_columns]
+        self.flexible_tables = [flexible_columns]
+        self.decision_tables = [decision_column]
+        self.stable_columns_count = self._get_columns_count(stable_columns)
+        self.flexible_columns_count = self._get_columns_count(flexible_columns)
+        self.desired_state = desired_state
+        self.supp = [pd.Series(supp)]
+        self.conf = [pd.Series(conf)]
+        self.is_nan = is_nan
+
+    @staticmethod
+    def _get_columns_count(columns: pd.DataFrame) -> int:
+        """Get the number of columns
+
+        Parameters
+        ----------
+        columns: pd.DataFrame
+            Data frame to check.
+
+        Returns
+        -------
+        int
+            Count of columns.
+        """
+        return len(columns.columns)
+
+    @staticmethod
+    def _get_unique_values(table: pd.DataFrame, column_number: int) -> list:
+        """Get unique values from column
+
+        Parameters
+        ----------
+        table : pd.DataFrame
+            Data frame with consequent values.
+        column_number : int
+            Column number to be checked.
+
+        Returns
+        -------
+        list
+            All unique values.
+        """
+        return table.iloc[:, column_number].unique()
+
+    def _split_tables_by_stable(self, stable_columns: pd.DataFrame, flexible_columns: pd.DataFrame,
+                               decision_column: pd.DataFrame,
+                               split_position: int, supp_series: pd.Series, conf_series: pd.Series):
+        """Split table by stable column.
+
+        Parameters
+        ----------
+        stable_columns : pd.DataFrame
+            Stable attributes.
+        flexible_columns : pd.DataFrame
+            Flexible attributes.
+        decision_column : pd.DataFrame
+            Consequent column.
+        split_position : int
+            The position where the split can be made.
+        supp_series : pd.Series
+            Support column.
+        conf_series : pd.Series
+            Confidence column.
+        """
+        unique_values = self._get_unique_values(stable_columns, split_position)
+        for unique_value in unique_values:
+            if self.is_nan:
+                mask = np.logical_or(stable_columns.iloc[:, split_position] == unique_value,
+                                     stable_columns.iloc[:, split_position].isnull())
+            else:
+                if str(unique_value) == "nan":
+                    mask = stable_columns.iloc[:, split_position].isnull()
+                else:
+                    mask = stable_columns.iloc[:, split_position] == unique_value
+            new_stable_table = stable_columns[mask]
+            new_flexible_table = flexible_columns[mask]
+            new_decision_table = decision_column[mask]
+            new_supp_series = supp_series[mask]
+            new_conf_series = conf_series[mask]
+            if self.desired_state.is_candidate(new_decision_table):
+                self.stable_tables.append(new_stable_table)
+                self.flexible_tables.append(new_flexible_table)
+                self.decision_tables.append(new_decision_table)
+                self.supp.append(new_supp_series)
+                self.conf.append(new_conf_series)
+
+    def reduce(self):
+        """Reduce Decision table to many reduction tables.
+
+        """
+        for split_position in range(self.stable_columns_count):
+            for table in range(len(self.stable_tables)):
+                stable_columns = self.stable_tables.pop(0)
+                flexible_columns = self.flexible_tables.pop(0)
+                decision_column = self.decision_tables.pop(0)
+                supp_series = self.supp.pop(0)
+                conf_series = self.conf.pop(0)
+                self._split_tables_by_stable(stable_columns,
+                                            flexible_columns,
+                                            decision_column,
+                                            split_position,
+                                            supp_series,
+                                            conf_series)
```

### Comparing `actionrules-lukassykora-1.1.8/actionrules_lukassykora.egg-info/SOURCES.txt` & `actionrules-lukassykora-1.1.9/actionrules_lukassykora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actionrules-lukassykora-1.1.8/setup.py` & `actionrules-lukassykora-1.1.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="actionrules-lukassykora",
-    version="1.1.8",
-    author="Lukas Sykora",
-    author_email="lukassykora@seznam.cz",
-    description="Action rules mining package",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/lukassykora/actionrules",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.6',
-    install_requires=[
-        'pandas',
-        'numpy',
-    ],
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="actionrules-lukassykora",
+    version="1.1.9",
+    author="Lukas Sykora",
+    author_email="lukassykora@seznam.cz",
+    description="Action rules mining package",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/lukassykora/actionrules",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.6',
+    install_requires=[
+        'pandas',
+        'numpy',
+        'pyfim'
+    ],
 )
```

