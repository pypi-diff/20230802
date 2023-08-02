# Comparing `tmp/crcf-0.0.3.tar.gz` & `tmp/crcf-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crcf-0.0.3.tar", last modified: Mon Jun 13 15:42:52 2022, max compression
+gzip compressed data, was "crcf-1.0.0.tar", last modified: Wed Aug  2 02:12:15 2023, max compression
```

## Comparing `crcf-0.0.3.tar` & `crcf-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2022-06-13 15:42:52.815511 crcf-0.0.3/
--rw-r--r--   0 jhughes  (1624782681) 1567826318     2432 2022-06-13 15:42:52.815729 crcf-0.0.3/PKG-INFO
-drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2022-06-13 15:42:52.810260 crcf-0.0.3/crcf/
--rw-r--r--   0 jhughes  (1624782681) 1567826318      103 2022-06-13 15:38:04.000000 crcf-0.0.3/crcf/__init__.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318     5937 2022-06-13 15:38:04.000000 crcf-0.0.3/crcf/forest.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318     9748 2022-06-13 15:38:04.000000 crcf-0.0.3/crcf/rule.py
--rw-r--r--   0 jhughes  (1624782681) 1567826318    20286 2022-06-13 15:38:04.000000 crcf-0.0.3/crcf/tree.py
-drwxr-xr-x   0 jhughes  (1624782681) 1567826318        0 2022-06-13 15:42:52.814815 crcf-0.0.3/crcf.egg-info/
--rw-r--r--   0 jhughes  (1624782681) 1567826318     2432 2022-06-13 15:42:52.000000 crcf-0.0.3/crcf.egg-info/PKG-INFO
--rw-r--r--   0 jhughes  (1624782681) 1567826318      215 2022-06-13 15:42:52.000000 crcf-0.0.3/crcf.egg-info/SOURCES.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318        1 2022-06-13 15:42:52.000000 crcf-0.0.3/crcf.egg-info/dependency_links.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318       15 2022-06-13 15:42:52.000000 crcf-0.0.3/crcf.egg-info/requires.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318        5 2022-06-13 15:42:52.000000 crcf-0.0.3/crcf.egg-info/top_level.txt
--rw-r--r--   0 jhughes  (1624782681) 1567826318       63 2022-06-13 15:42:52.817454 crcf-0.0.3/setup.cfg
--rw-r--r--   0 jhughes  (1624782681) 1567826318      569 2022-06-13 15:42:40.000000 crcf-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:12:15.682875 crcf-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-02 02:12:04.000000 crcf-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-08-02 02:12:15.682875 crcf-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-02 02:12:04.000000 crcf-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:12:15.682875 crcf-1.0.0/crcf/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-02 02:12:04.000000 crcf-1.0.0/crcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-08-02 02:12:04.000000 crcf-1.0.0/crcf/forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-08-02 02:12:04.000000 crcf-1.0.0/crcf/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-08-02 02:12:04.000000 crcf-1.0.0/crcf/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:12:15.682875 crcf-1.0.0/crcf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-08-02 02:12:15.000000 crcf-1.0.0/crcf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-02 02:12:15.000000 crcf-1.0.0/crcf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 02:12:15.000000 crcf-1.0.0/crcf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 02:12:15.000000 crcf-1.0.0/crcf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 02:12:15.000000 crcf-1.0.0/crcf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-02 02:12:04.000000 crcf-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-02 02:12:15.682875 crcf-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 02:12:15.682875 crcf-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-08-02 02:12:04.000000 crcf-1.0.0/tests/test_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-08-02 02:12:04.000000 crcf-1.0.0/tests/test_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-08-02 02:12:04.000000 crcf-1.0.0/tests/test_tree.py
```

### Comparing `crcf-0.0.3/PKG-INFO` & `crcf-1.0.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,37 @@
-Metadata-Version: 2.1
-Name: crcf
-Version: 0.0.3
-Summary: Combination Robust Cut Forests
-Home-page: UNKNOWN
-Author: J. Marcus Hughes
-Author-email: hughes.jmb@gmail.com
-License: LICENSE.txt
-Description: # Combination Robust Cut Forests
-        [![CodeFactor](https://www.codefactor.io/repository/github/jmbhughes/crcf/badge)](https://www.codefactor.io/repository/github/jmbhughes/crcf)
-        [![PyPI version](https://badge.fury.io/py/crcf.svg)](https://badge.fury.io/py/crcf)
-        
-        Isolation Forests **[Liu+2008]** and Robust Random Cut Trees **[Guha+2016]** are very similar in many ways, 
-        as outlined in the [supporting overview](overview.pdf). Most notably, they are extremes
-        of the same outlier scoring function: 
-        
-        $$\theta \textrm{Depth} + (1 - \theta) \textrm{[Co]Disp}$$ 
-        
-        The combination robust cut forest allows you to combine both scores by using an theta other than 0 or 1. 
-        
-        # Install
-        You can install with through `pip install crcf`. Alternatively, you can download the repository and run 
-        `python3 setup.py install` or `pip3 install .` Please note that this package uses features from Python 3.7+
-        and is not compatible with earlier Python versions. 
-        
-        The tests can be run from `pytest` with `python3 setup.py test`.
-        
-        # Tasks
-        - [X] complete basic implementation
-        - [X] provide clear documentation and usage instructions
-        - [ ] implement tree down in cython
-        - [ ] accelerate forests with multi-threading
-        - [ ] incorporate categorical variable support, including categorical rules
-        - [ ] complete the write-up document with a benchmarking of performance
-        
-        # References
-        - **[Liu+2008]**: [Liu, Fei Tony, Kai Ming Ting, and Zhi-Hua Zhou. 
-        "Isolation forest." In 2008 Eighth IEEE International Conference on Data Mining, 
-        pp. 413-422. IEEE, 2008.](https://cs.nju.edu.cn/zhouzh/zhouzh.files/publication/icdm08b.pdf?q=isolation-forest)
-        - **[Guha+2016]**: [Guha, Sudipto, Nina Mishra, Gourav Roy, and Okke Schrijvers. 
-        "Robust random cut forest based anomaly detection on streams." 
-        In International conference on machine learning, pp. 2712-2721. 2016.](http://proceedings.mlr.press/v48/guha16.pdf)
-        
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+# Combination Robust Cut Forests
+[![CodeFactor](https://www.codefactor.io/repository/github/jmbhughes/crcf/badge)](https://www.codefactor.io/repository/github/jmbhughes/crcf)
+[![PyPI version](https://badge.fury.io/py/crcf.svg)](https://badge.fury.io/py/crcf)
+[![codecov](https://codecov.io/gh/jmbhughes/crcf/branch/main/graph/badge.svg?token=YBZERHDU75)](https://codecov.io/gh/jmbhughes/crcf)
+
+Isolation Forests **[Liu+2008]** and Robust Random Cut Trees **[Guha+2016]** are very similar in many ways, 
+as outlined in the [supporting overview](overview.pdf). Most notably, they are extremes
+of the same outlier scoring function: 
+
+$$\theta \textrm{Depth} + (1 - \theta) \textrm{[Co]Disp}$$ 
+
+The combination robust cut forest allows you to combine both scores by using an theta other than 0 or 1. 
+
+# Install
+You can install with through `pip install crcf`. Alternatively, you can download the repository and run 
+`python3 setup.py install` or `pip3 install .` Please note that this package uses features from Python 3.7+
+and is not compatible with earlier Python versions. 
+
+
+# Tasks
+- [X] complete basic implementation
+- [X] provide clear documentation and usage instructions
+- [ ] ensure interface allows for fitting and scoring on multiple points at the same time
+- [ ] implement a better saving method than pickling
+- [ ] use random tests with hypothesis
+- [ ] implement tree down in cython
+- [ ] accelerate forests with multi-threading
+- [ ] incorporate categorical variable support, including categorical rules
+- [ ] complete the write-up document with a benchmarking of performance
+
+# References
+- **[Liu+2008]**: [Liu, Fei Tony, Kai Ming Ting, and Zhi-Hua Zhou. 
+"Isolation forest." In 2008 Eighth IEEE International Conference on Data Mining, 
+pp. 413-422. IEEE, 2008.](https://cs.nju.edu.cn/zhouzh/zhouzh.files/publication/icdm08b.pdf?q=isolation-forest)
+- **[Guha+2016]**: [Guha, Sudipto, Nina Mishra, Gourav Roy, and Okke Schrijvers. 
+"Robust random cut forest based anomaly detection on streams." 
+In International conference on machine learning, pp. 2712-2721. 2016.](http://proceedings.mlr.press/v48/guha16.pdf)
```

### Comparing `crcf-0.0.3/crcf/rule.py` & `crcf-1.0.0/crcf/rule.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,210 +17,288 @@
         - _generate_uniform(bounding_box): generates a new rule at uniform from the bounding box
         - _generate_biased(bounding_box): generates a new biased sample rule from the bounding box
     """
     def __init__(self) -> None:
         pass
 
     def evaluate(self, x: np.ndarray) -> np.ndarray:
-        """
-        Decide the path of a set of points using the rule
-        :param x: a set of points, e.g. np.array([[1,2,3],[4,5,6]])
-        :return: true if goes to left side, false for right side
+        """Decide the path of a set of points using the rule
+
+
+        Parameters
+        ----------
+        x : np.ndarray
+            a set of points, e.g. np.array([[1,2,3],[4,5,6]])
+
+        Returns
+        -------
+        np.ndarray of bool
+            True if point goes to left side, False for right side
         """
         return np.array([self._evaluate(xx) for xx in x])
+        # TODO: this is much slower than it has to be, use array methods
 
     @abstractmethod
     def _evaluate(self, x: np.ndarray) -> bool:
-        """
-        Score a single point
-        :param x: a single example, e.g. np.ndarray([1,2,3])
-        :return: true if goes to left side, false for right side
+        """Score a single point
+
+        Parameters
+        ----------
+        x : np.ndarray
+            a single example, 1-D numpy array
+
+        Returns
+        -------
+        bool
+            True if point goes to left side, False for right side
         """
         pass
 
     @classmethod
     def generate(cls, bounding_box: np.ndarray, mode: str = "uniform") -> Rule:
-        """
-        Generates a new rule from the bounding box.
-        The mode determines the strategy of picking a dimension.
+        """Generates a new rule from the bounding box.
 
-        :param bounding_box: the minimal axis parallel bounding box that contains all the data points
+        Parameters
+        ----------
+        bounding_box : np.ndarray
+            the minimal axis parallel bounding box that contains all the data points
             for a given node, e.g. [[1,2], [1,10]] this means the value in first dimension has values
             from 1 to 2 and in the second dimension 1 to 10.
-        :param mode: the strategy of picking a dimension:
+        mode : str
+            the strategy of picking a dimension:
             - "uniform": all dimensions are equally considered
             - "biased": dimensions with larger value ranges are weighted proportionally more
                 in two dimensions if the bounding box were [[1,2], [1,10]] this means the
                 value in first dimension has values from 1 to 2 and in the second dimension 1 to 10.
                 In the biased setting the first dimension has a weight of 2-1=1 and the second dimension
                 has weight 10-1=9. The second dimension is 9 times more likely to be chosen.
-        :return: a new rule
+
+
+        Returns
+        -------
+        Rule
+            a new rule
         """
 
         # switch on the mode and call the appropriate function
         if mode == "uniform":
             return cls._generate_uniform(bounding_box)
         elif mode == "biased":
             return cls._generate_biased(bounding_box)
         else:
             raise RuntimeError("mode must either be uniform or biased, not {}".format(mode))
 
     @classmethod
     @abstractmethod
     def _generate_uniform(cls, bounding_box: np.ndarray) -> Rule:
-        """
-        Generate a rule with no special attention to the bounding box, i.e. all dimeensions are equally important
-        :param bounding_box: the minimal axis parallel bounding box that contains all the data points
+        """Generate a rule with no special attention to the bounding box, i.e. all dimeensions are equally important
+
+
+        Parameters
+        ----------
+        bounding_box : np.ndarray
+            the minimal axis parallel bounding box that contains all the data points
             for a given node, e.g. [[1,2], [1,10]] this means the value in first dimension has values
             from 1 to 2 and in the second dimension 1 to 10.
-        :return: a new rule
+
+        Returns
+        -------
+        Rule
+            a new random rule
         """
         pass
 
     @classmethod
     @abstractmethod
     def _generate_biased(cls, bounding_box: np.ndarray) -> Rule:
-        """
-        Generate a rule with no weighted attention to the bounding box, i.e. wider dimensions are more important
-        :param bounding_box: the minimal axis parallel bounding box that contains all the data points
+        """Generate a rule with no weighted attention to the bounding box, i.e. wider dimensions are more important
+
+
+        Parameters
+        ----------
+        bounding_box : np.ndarray
+            the minimal axis parallel bounding box that contains all the data points
             for a given node, e.g. [[1,2], [1,10]] this means the value in first dimension has values
             from 1 to 2 and in the second dimension 1 to 10.
-        :return: a new rule
+
+        Returns
+        -------
+        Rule
+            a new random rule
         """
         pass
 
     @abstractmethod
     def __str__(self) -> str:
-        """
-        :return: string representation
-        """
         pass
 
     @abstractmethod
     def __eq__(self, other: Type[Rule]) -> bool:
-        """
-        :param other: other node to check
-        :return: whether the two nodes are same
-        """
         pass
 
 
 class AxisAlignedRule(Rule):
     """
     This rule uses cuts that are axis aligned. Thus, the rule is defined by its dimension and what threshold value
     for that dimension
     """
     def __init__(self, dimension: int, value: float):
-        """
-        :param dimension: the number, 0-indexed, describing the dimension of the cut
-        :param value: the  value to threshold on, i.e. x < value is true
+        """Initialize an AxisAlignedRule
+
+        Parameters
+        ----------
+        dimension : int
+            the number, 0-indexed, describing the dimension of the cut
+        value : float
+            the  value to threshold on, i.e. x < value is true
         """
         super().__init__()
         self.dimension, self.value = dimension, value
 
     def _evaluate(self, x: np.ndarray) -> bool:
-        """
-        Determine the path for a single point, points less than the threshold value are true
-        :param x: a single example, e.g. np.ndarray([1,2,3])
-        :return: true if x[dimension] < value and false if x[dimension] >= value
+        """Determine the path for a single point, points less than the threshold value are true
+
+
+        Parameters
+        ----------
+        x : np.ndarray
+             single example, e.g. np.ndarray([1,2,3])
+
+        Returns
+        -------
+        bool
+            true if x[dimension] < value and false if x[dimension] >= value
         """
         return x[self.dimension] < self.value
 
     @classmethod
     def _generate_uniform(cls, bounding_box: np.ndarray) -> AxisAlignedRule:
-        """
-        Generate a rule with no special attention to the bounding box, i.e. all dimensions are equally important
-        :param bounding_box: the minimal axis parallel bounding box that contains all the data points
+        """Generate a rule with no special attention to the bounding box, i.e. all dimeensions are equally important
+
+
+        Parameters
+        ----------
+        bounding_box : np.ndarray
+            the minimal axis parallel bounding box that contains all the data points
             for a given node, e.g. [[1,2], [1,10]] this means the value in first dimension has values
             from 1 to 2 and in the second dimension 1 to 10.
-        :return: a new rule
+
+        Returns
+        -------
+        Rule
+            a new random rule
         """
         dimension = np.random.randint(0, bounding_box.shape[0])
         value = np.random.uniform(bounding_box[dimension][0], bounding_box[dimension][1])
         return AxisAlignedRule(dimension, value)
 
     @classmethod
     def _generate_biased(cls, bounding_box: np.ndarray) -> AxisAlignedRule:
-        """
-        Generate a rule with no weighted attention to the bounding box, i.e. wider dimensions are more important
-        :param bounding_box: the minimal axis parallel bounding box that contains all the data points
+        """Generate a rule with no weighted attention to the bounding box, i.e. wider dimensions are more important
+
+
+        Parameters
+        ----------
+        bounding_box : np.ndarray
+            the minimal axis parallel bounding box that contains all the data points
             for a given node, e.g. [[1,2], [1,10]] this means the value in first dimension has values
             from 1 to 2 and in the second dimension 1 to 10.
-        :return: a new rule
+
+        Returns
+        -------
+        Rule
+            a new random rule
         """
         lengths = np.diff(bounding_box)
         dimension = np.random.choice(np.arange(bounding_box.shape[0]),
                                      p=lengths.flatten()/np.sum(lengths))
         value = np.random.uniform(bounding_box[dimension][0], bounding_box[dimension][1])
         return AxisAlignedRule(dimension, value)
 
     def __str__(self) -> str:
-        """
-        customized string output
-        :return: description of rule
-        """
-        return "x[{}]<{:.2f}".format(self.dimension, self.value)
+        return f"x[{self.dimension}]<{self.value:.2f}"
 
     def __eq__(self, other: AxisAlignedRule) -> bool:
-        """
-        :param other: rule to test equality against
-        :return: whether the rules are equivalent
-        """
         return isinstance(other, AxisAlignedRule) and other.dimension == self.dimension and other.value == self.value
 
 
 class NonAxisAlignedRule(Rule):
     """
     A cut is instead a hyperplane that divides the space. This hyperplane is thus a linear combination of dimensions.
     It is described by a normal vector to the hyperplane and a point the hyperplane passes through.
     """
     def __init__(self, normal: np.ndarray, point: np.ndarray):
-        """
-        Create a non-axis aligned rule
-        :param normal: the normal vector for the hyperplane
-        :param point: a point the hyperplane must pass through
+        """Create a non-axis-aligned rule
+
+        Parameters
+        ----------
+        normal : np.ndarray
+            the normal vector for the hyperplane
+        point : np.ndarray
+            a point the hyperplane must pass through
         """
         super().__init__()
         self.normal, self.point = normal, point
         self.offset = normal.dot(point)  # the offset used in calculations
 
     def _evaluate(self, x: np.ndarray) -> bool:
-        """
-        Determine the path for a single point, points less than the threshold value are true
-        :param x: a single example, e.g. np.ndarray([1,2,3])
-        :return: true if x[dimension] < value and false if x[dimension] >= value
+        """Score a single point
+
+        Parameters
+        ----------
+        x : np.ndarray
+            a single example, 1-D numpy array
+
+        Returns
+        -------
+        bool
+            True if point goes to left side, False for right side
         """
         return np.inner(self.normal, x) < self.offset
 
     @classmethod
     def _generate_uniform(cls, bounding_box: np.ndarray) -> NonAxisAlignedRule:
-        """
-        Generate a rule with no special attention to the bounding box, i.e. all dimensions are equally important
-        :param bounding_box: the minimal axis parallel bounding box that contains all the data points
+        """Generate a rule with no special attention to the bounding box, i.e. all dimeensions are equally important
+
+
+        Parameters
+        ----------
+        bounding_box : np.ndarray
+            the minimal axis parallel bounding box that contains all the data points
             for a given node, e.g. [[1,2], [1,10]] this means the value in first dimension has values
             from 1 to 2 and in the second dimension 1 to 10.
-        :return: a new rule
+
+        Returns
+        -------
+        Rule
+            a new random rule
         """
         normal = np.random.uniform(-1, 1, size=bounding_box.shape[0])
         point = np.array(np.random.uniform(low, high) for low, high in bounding_box)
         return NonAxisAlignedRule(normal, point)
 
     @classmethod
     def _generate_biased(cls, bounding_box: np.ndarray) -> NonAxisAlignedRule:
-        # TODO: figure out how to generate biased
+        """Generate a rule with no weighted attention to the bounding box, i.e. wider dimensions are more important
+
+
+        Parameters
+        ----------
+        bounding_box : np.ndarray
+            the minimal axis parallel bounding box that contains all the data points
+            for a given node, e.g. [[1,2], [1,10]] this means the value in first dimension has values
+            from 1 to 2 and in the second dimension 1 to 10.
+
+        Returns
+        -------
+        Rule
+            a new random rule
+        """
         raise NotImplementedError("Will be added in a later version.")
 
     def __str__(self) -> str:
-        """
-        customized string output
-        :return: description of rule
-        """
         return "x^T{}<{:.2f}".format("[" + ("{:.2f},"*self.normal.shape[0]).format(self.normal) + "]",
                                      self.offset)
 
     def __eq__(self, other: NonAxisAlignedRule) -> bool:
-        """
-        :param other: rule to test equality against
-        :return: whether the rules are equivalent
-        """
         return isinstance(other, NonAxisAlignedRule) and np.all(other.normal == self.normal) and\
             np.all(other.point == self.point)
```

