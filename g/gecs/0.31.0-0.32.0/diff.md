# Comparing `tmp/gecs-0.31.0.tar.gz` & `tmp/gecs-0.32.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gecs-0.31.0.tar", max compression
+gzip compressed data, was "gecs-0.32.0.tar", max compression
```

## Comparing `gecs-0.31.0.tar` & `gecs-0.32.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2023-07-11 17:36:42.496116 gecs-0.31.0/LICENSE
--rw-r--r--   0        0        0     3360 2023-08-01 23:03:40.392463 gecs-0.31.0/README.md
--rw-r--r--   0        0        0      697 2023-08-01 23:03:40.392463 gecs-0.31.0/pyproject.toml
--rw-r--r--   0        0        0    50109 2023-08-01 23:03:40.392463 gecs-0.31.0/src/gecs/gec.py
--rw-r--r--   0        0        0     2152 2023-07-11 18:17:15.906277 gecs-0.31.0/src/gecs/utils/gaussian_process_visualisation.py
--rw-r--r--   0        0        0     4382 1970-01-01 00:00:00.000000 gecs-0.31.0/setup.py
--rw-r--r--   0        0        0     4324 1970-01-01 00:00:00.000000 gecs-0.31.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-07-11 17:36:42.496116 gecs-0.32.0/LICENSE
+-rw-r--r--   0        0        0     3960 2023-08-01 23:03:54.580390 gecs-0.32.0/README.md
+-rw-r--r--   0        0        0      697 2023-08-01 23:03:54.584390 gecs-0.32.0/pyproject.toml
+-rw-r--r--   0        0        0    50182 2023-08-01 23:03:54.584390 gecs-0.32.0/src/gecs/gec.py
+-rw-r--r--   0        0        0     2152 2023-07-11 18:17:15.906277 gecs-0.32.0/src/gecs/utils/gaussian_process_visualisation.py
+-rw-r--r--   0        0        0     5004 1970-01-01 00:00:00.000000 gecs-0.32.0/setup.py
+-rw-r--r--   0        0        0     4924 1970-01-01 00:00:00.000000 gecs-0.32.0/PKG-INFO
```

### Comparing `gecs-0.31.0/LICENSE` & `gecs-0.32.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gecs-0.31.0/README.md` & `gecs-0.32.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -49,27 +49,47 @@
 -   the methods `freeze` and `unfreeze` that turn the `GEC` functionally into a `LGBMClassifier` and back
 
 
 ## Example
 
 The default use of `GEC` would look like this:
 
+    from sklearn.datasets import load_iris
     from gecs.gec import GEC
 
+    X, y = load_iris(return_X_y=True)
+
+
+    # fit and infer GEC
+    gec = GEC()
     gec.fit(X, y)
+    yhat = gec.predict(X)
 
-    gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes
 
+    # manage GEC state
+    path = "./gec.json"
+    gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes
     gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier
+    gec.freeze() # freeze GEC so that it behaves like a LGBMClassifier
+    gec.unfreeze() # unfreeze to enable GEC hyperparameter optimisation
 
-    yhat = gec.predict(X)
 
-    gec.freeze() # freeze GEC so that it behaves like a LGBMClassifier
+    # benchmark against LGBMClassifier
+    from lightgbm import LGBMClassifier
+    from sklearn.model_selection import cross_val_score
+    import numpy as np
 
-    gec.unfreeze() # unfreeze to enable GEC hyperparameter optimisation
+    clf = LGBMClassifier()
+    lgbm_score = np.mean(cross_val_score(clf, X, y))
+
+    gec.freeze()
+    gec_score = np.mean(cross_val_score(gec, X, y))
+
+    print(f"{gec_score = }, {lgbm_score = }")
+    assert gec_score > lgbm_score, "GEC doesn't outperform LGBMClassifier"
 
 
 
 ## Contributing
 
 If you want to contribute, please reach out and I'll design a process around it.
```

### Comparing `gecs-0.31.0/pyproject.toml` & `gecs-0.32.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gecs"
-version = "0.31.0"
+version = "0.32.0"
 authors = ["Leon Luithlen <leontimnaluithlen@gmail.com>"]
 description = "LightGBM Classifier with integrated bayesian hyperparameter optimization"
 keywords = ["lightgbm", "classification", "machine learning", "hyperparameter optimization", "classifier"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/0xideas/sequifier"
 repository = "https://github.com/0xideas/sequifier"
```

### Comparing `gecs-0.31.0/src/gecs/gec.py` & `gecs-0.32.0/src/gecs/gec.py`

 * *Files 5% similar despite different names*

```diff
@@ -212,19 +212,17 @@
         self._classes = None
         self._n_classes = None
         self.set_params(**kwargs)
 
         self._init_kwargs = {
             k: v for k, v in kwargs.items() if k not in ["subsample_freq", "subsample"]
         }
-        self.subsample = kwargs.get("subsample", None)
-        self.subsample_freq = kwargs.get("subsample_freq", None)
 
-        self.fix_bagging = False
-        self.fix_boosting_type = False
+        self.fix_bagging_ = False
+        self.fix_boosting_type_ = False
 
         self.frozen = frozen
         non_optimized_init_args = [
             "max_depth",
             "subsample_for_bin",
             "objective",
             "class_weight",
@@ -234,15 +232,15 @@
             "random_state",
             "n_jobs",
             "silent",
             "importance_type",
         ]
         self._init_args = {arg: getattr(self, arg) for arg in non_optimized_init_args}
 
-        self.gec_hyperparameters = {
+        self.gec_hyperparameters_ = {
             "l": 1.0,
             "l_bagging": 0.1,
             "hyperparams_acquisition_percentile": 0.7,
             "bagging_acquisition_percentile": 0.7,
             "bandit_greediness": 1.0,
             "n_random_exploration": 10,
             "n_sample": 1000,
@@ -270,26 +268,26 @@
         ]
 
         self._categorical_hyperparameter_names, _ = zip(
             *self.categorical_hyperparameters
         )
 
         prohibited_combinations = ["rf-no_bagging"]
-        if self.fix_bagging and (self.subsample is None or self.subsample_freq is None):
+        if self.fix_bagging_ and (self.subsample is None or self.subsample_freq is None):
             prohibited_combinations += ["rf-yes_bagging"]
 
         self._categorical_hyperparameter_combinations = [
             "-".join(y)
             for y in itertools.product(
                 *[x[1] for x in self.categorical_hyperparameters]
             )
             if "-".join(y) not in prohibited_combinations
         ]
 
-        if self.fix_boosting_type:
+        if self.fix_boosting_type_:
             self._categorical_hyperparameter_combinations = [
                 hp_comb
                 for hp_comb in self._categorical_hyperparameter_combinations
                 if hp_comb.startswith(self.boosting_type)
             ]
 
         ten_to_ten_thousand = np.concatenate(
@@ -339,21 +337,21 @@
             ("min_child_samples", np.arange(2, 50, 1)),
             ("colsample_bytree", np.arange(0.1, 1.00, 0.01)),
         ]
 
         self.fixed_params = {
             hyperparameter: getattr(self, hyperparameter)
             for hyperparameter, _ in self._real_hyperparameters_all
-            if hyperparameter not in self.gec_hyperparameters["hyperparameters"]
+            if hyperparameter not in self.gec_hyperparameters_["hyperparameters"]
         }
 
         self._real_hyperparameters = [
             (hp_name, range_)
             for hp_name, range_ in self._real_hyperparameters_all
-            if hp_name in self.gec_hyperparameters["hyperparameters"]
+            if hp_name in self.gec_hyperparameters_["hyperparameters"]
         ]
         self._real_hyperparameters_linear = [
             (name, np.arange(-1.0, 1.0, 2 / len(values)).round(4).astype(np.float16))
             for name, values in self._real_hyperparameters
         ]
 
         self._real_hyperparameters_map = {
@@ -376,26 +374,27 @@
             *self._real_hyperparameters_linear
         )
 
         self._real_hypermarameter_types = [
             np.array(s).dtype for _, s in self._real_hyperparameters
         ]
 
+
     def _set_gec_fields(self) -> None:
-        self.kernel = RBF(self.gec_hyperparameters["l"])
-        self.hyperparameter_scores = {
+        self.kernel = RBF(self.gec_hyperparameters_["l"])
+        self.hyperparameter_scores_ = {
             "inputs": [],
             "output": [],
             "means": [],
             "sigmas": [],
         }
 
-        self.kernel_bagging = RBF(self.gec_hyperparameters["l_bagging"])
+        self.kernel_bagging = RBF(self.gec_hyperparameters_["l_bagging"])
 
-        self.bagging_scores = {"inputs": [], "output": [], "means": [], "sigmas": []}
+        self.bagging_scores_ = {"inputs": [], "output": [], "means": [], "sigmas": []}
 
         self._bagging_combinations = list(
             itertools.product(
                 *[
                     list(range(1, 11, 1)),
                     np.arange(0.5, 1.0, 0.01),
                 ]
@@ -411,24 +410,27 @@
             ((frac + 3) / 4),
         )
         self._bagging_combinations_rescaled = [
             self._rescale_bagging_combination(freq, frac)
             for freq, frac in self._bagging_combinations
         ]
 
-        self.best_score = None
+        self.best_score_gec_ = None
         self.best_params_ = None
-        self.fit_params = None
+        self.gec_fit_params_ = None
         self.n_iterations = 0
 
         # parameters for bandit
-        self.rewards = {
+        self.rewards_ = {
             c: {"a": 1, "b": 1} for c in self._categorical_hyperparameter_combinations
         }
-        self.selected_arms = []
+        self.selected_arms_ = []
+
+        self.best_scores_gec_ = {}
+        self.best_params_gec_ = {}
 
     @property
     def kernel(self):
         return self._kernel
 
     @kernel.setter
     def kernel(self, value):
@@ -443,16 +445,16 @@
     def kernel_bagging(self, value):
         self._kernel_bagging = value
         self.gaussian_bagging = GaussianProcessRegressor(
             kernel=value, n_restarts_optimizer=9
         )
 
     @property
-    def gec_iter(self) -> int:
-        return len(self.hyperparameter_scores["output"])
+    def gec_iter_(self) -> int:
+        return len(self.hyperparameter_scores_["output"])
 
     @classmethod
     def _cast_to_type(cls, value, type_):
         if type_ == np.float64:
             return float(value)
         elif type_ == np.int64:
             return int(value)
@@ -477,30 +479,30 @@
             gec : GEC
                 deserialized model object
         """
         with open(path, "r") as f:
             representation = json.loads(f.read())
 
         gec = cls()
-        gec.gec_hyperparameters = representation["gec_hyperparameters"]
-        gec.rewards = representation["rewards"]
-        gec.selected_arms = representation["selected_arms"]
-        gec.hyperparameter_scores = (
+        gec.gec_hyperparameters_ = representation["gec_hyperparameters"]
+        gec.rewards_ = representation["rewards"]
+        gec.selected_arms_ = representation["selected_arms"]
+        gec.hyperparameter_scores_ = (
             gec._convert_gaussian_process_data_from_deserialisation(
                 representation["hyperparameter_scores"]
             )
         )
-        gec.bagging_scores = gec._convert_gaussian_process_data_from_deserialisation(
+        gec.bagging_scores_ = gec._convert_gaussian_process_data_from_deserialisation(
             representation["bagging_scores"]
         )
-        gec.best_params_ = representation["best_params_"]
-        gec.best_score = float(representation["best_score"])
-        gec.best_params_gec = representation["best_params_gec"]
-        gec.best_scores_gec = representation["best_scores_gec"]
-        gec.fit_params = representation["fit_params"]
+        gec.best_params_ = representation["best_params"]
+        gec.best_score_gec_ = float(representation["best_score_gec"])
+        gec.best_params_gec_ = representation["best_params_gec"]
+        gec.best_scores_gec_ = representation["best_scores_gec"]
+        gec.gec_fit_params_ = representation["gec_fit_params"]
 
         if X is not None and y is not None:
             gec._fit_best_params(X, y)
         else:
             warnings.warn(
                 "If X and y are not provided, the GEC model is not fitted for inference"
             )
@@ -553,31 +555,31 @@
             k2: [process_value(k2, vv) for vv in v] for k2, v in data_dict.items()
         }
 
         return converted_dict
 
     def _get_representation(self) -> Dict[str, Any]:
         hyperparameter_scores = self._convert_gaussian_process_data_for_serialisation(
-            self.hyperparameter_scores
+            self.hyperparameter_scores_
         )
         bagging_scores = self._convert_gaussian_process_data_for_serialisation(
-            self.bagging_scores
+            self.bagging_scores_
         )
         representation = {
-            "gec_hyperparameters": self.gec_hyperparameters,
-            "rewards": self.rewards,
-            "selected_arms": self.selected_arms,
+            "gec_hyperparameters": self.gec_hyperparameters_,
+            "rewards": self.rewards_,
+            "selected_arms": self.selected_arms_,
             "hyperparameter_scores": hyperparameter_scores,
             "bagging_scores": bagging_scores,
-            "best_params_": self.best_params_,
-            "best_score": self.best_score,
-            "best_params_gec": self.best_params_gec,
-            "best_scores_gec": self.best_scores_gec,
-            "gec_iter": self.gec_iter,
-            "fit_params": self.fit_params,
+            "best_params": self.best_params_,
+            "best_score_gec": self.best_score_gec_,
+            "best_params_gec": self.best_params_gec_,
+            "best_scores_gec": self.best_scores_gec_,
+            "gec_iter": self.gec_iter_,
+            "gec_fit_params": self.gec_fit_params_,
         }
         return representation
 
     def _validate_parameter_maps(self) -> None:
         real_to_linear_to_real = {
             v: self._real_hyperparameters_map[hp][
                 self._real_hyperparameters_map_reverse[hp][v]
@@ -607,22 +609,22 @@
         self, gec_hyperparameters: Dict[str, Union[int, float, List[str]]]
     ) -> None:
         """Set the hyperparameters of the GEC optimisation process
 
         Parameters
         ----------
             gec_hyperparameters : dict[str, float]
-                dictionary with keys that are in self.gec_hyperparameters
+                dictionary with keys that are in self.gec_hyperparameters_
         """
         assert np.all(
             np.array(
-                [hp in self.gec_hyperparameters for hp in gec_hyperparameters.keys()]
+                [hp in self.gec_hyperparameters_ for hp in gec_hyperparameters.keys()]
             )
         )
-        self.gec_hyperparameters.update(gec_hyperparameters)
+        self.gec_hyperparameters_.update(gec_hyperparameters)
         self._set_gec_attributes()
 
     def freeze(self):
         self.frozen = True
         return self
 
     def unfreeze(self):
@@ -680,96 +682,94 @@
         ----------
             n_iter : int
                 number of optimization steps
             fixed_hyperparameters : list[str]
                 list of hyperparameters that should not be optimised
         """
 
-        self.fit_params = {
+        self.gec_fit_params_ = {
             "sample_weight": sample_weight,
             "init_score": init_score,
             "eval_set": eval_set,
             "eval_names": eval_names,
             "eval_sample_weight": eval_sample_weight,
             "eval_class_weight": eval_class_weight,
             "eval_init_score": eval_init_score,
             "eval_metric": eval_metric,
             "feature_name": feature_name,
             "categorical_feature": categorical_feature,
             "callbacks": callbacks,
             "init_model": init_model,
         }
 
-        self.fix_boosting_type = "boosting_type" in fixed_hyperparameters
+        self.fix_boosting_type_ = "boosting_type" in fixed_hyperparameters
         fixed_hyperparameters = [
             hp for hp in fixed_hyperparameters if hp != "boosting_type"
         ]
 
-        self.fix_bagging = "bagging" in fixed_hyperparameters
+        self.fix_bagging_ = "bagging" in fixed_hyperparameters
         fixed_hyperparameters = [hp for hp in fixed_hyperparameters if hp != "bagging"]
 
         assert (
-            (not self.fix_bagging)
+            (not self.fix_bagging_)
             or (self.subsample_freq is not None)
             or (self.boosting_type != "rf")
-            or (not self.fix_boosting_type)
+            or (not self.fix_boosting_type_)
         ), 'boosting_type="rf" requires bagging'
         if not self.frozen:
             filtered_hyperparameters = list(
-                set(self.gec_hyperparameters["hyperparameters"]).difference(
+                set(self.gec_hyperparameters_["hyperparameters"]).difference(
                     set(fixed_hyperparameters)
                 )
             )
             self.set_gec_hyperparameters({"hyperparameters": filtered_hyperparameters})
 
-            self.best_scores_gec = {}
-            self.best_params_gec = {}
             (
-                self.best_params_gec["search"],
-                self.best_scores_gec["search"],
+                self.best_params_gec_["search"],
+                self.best_scores_gec_["search"],
             ) = self._optimise_hyperparameters(n_iter, X, y)
 
             best_params_grid = self._find_best_parameters()
-            self.best_params_gec["grid"] = self._replace_fixed_args(best_params_grid)
-            self.best_scores_gec["grid"] = self._calculate_cv_score(
-                X, y, self.best_params_gec["grid"]
+            self.best_params_gec_["grid"] = self._replace_fixed_args(best_params_grid)
+            self.best_scores_gec_["grid"] = self._calculate_cv_score(
+                X, y, self.best_params_gec_["grid"]
             )
 
-            best_params_prep = copy.deepcopy(self.best_params_gec["search"])
+            best_params_prep = copy.deepcopy(self.best_params_gec_["search"])
             best_params_grid_from_search = self._find_best_parameters_from_search(
                 best_params_prep
             )
-            self.best_params_gec["grid_from_search"] = self._replace_fixed_args(
+            self.best_params_gec_["grid_from_search"] = self._replace_fixed_args(
                 best_params_grid_from_search
             )
-            self.best_scores_gec["grid_from_search"] = self._calculate_cv_score(
-                X, y, self.best_params_gec["grid_from_search"]
+            self.best_scores_gec_["grid_from_search"] = self._calculate_cv_score(
+                X, y, self.best_params_gec_["grid_from_search"]
             )
 
-            for source, score in self.best_scores_gec.items():
-                if self.best_score is None or score > self.best_score:
-                    self.best_score = score
-                    self.best_params_ = self.best_params_gec[source]
+            for source, score in self.best_scores_gec_.items():
+                if self.best_score_gec_ is None or score > self.best_score_gec_:
+                    self.best_score_gec_ = score
+                    self.best_params_ = self.best_params_gec_[source]
 
         self._fit_best_params(X, y)
 
         return self
 
     def _replace_fixed_args(self, params):
-        if self.fix_boosting_type:
+        if self.fix_boosting_type_:
             params["boosting_type"] = self.boosting_type
-        self.selected_arms = []
-        if self.fix_bagging and "subsample" in params and "subsample_freq" in params:
+        self.selected_arms_ = []
+        if self.fix_bagging_ and "subsample" in params and "subsample_freq" in params:
             if self.subsample is not None and self.subsample_freq is not None:
                 params["subsample"] = self.subsample
                 params["subsample_freq"] = self.subsample_freq
             else:
                 del params["subsample"]
                 del params["subsample_freq"]
-            self.bagging_scores = {
+            self.bagging_scores_ = {
                 "inputs": [],
                 "output": [],
                 "means": [],
                 "sigmas": [],
             }
         return params
 
@@ -779,15 +779,15 @@
         y: ndarray,
         params: Dict[str, Optional[Union[str, float, int, float64]]],
     ) -> float64:
         clf = LGBMClassifier(**params)
         try:
             with open(os.devnull, "w") as f, contextlib.redirect_stdout(f):
                 cross_val_scores = cross_val_score(
-                    clf, X, y, cv=5, fit_params=self.fit_params
+                    clf, X, y, cv=5, fit_params=self.gec_fit_params_
                 )
                 score = np.mean(cross_val_scores)
         except:
             warnings.warn(
                 f"Could not calculate cross val scores for parameters: {params}"
             )
             score = 0.0
@@ -797,23 +797,23 @@
         self,
         n_iter: int,
         X: ndarray,
         Y: ndarray,
         **kwargs,
     ) -> Tuple[Dict[str, Optional[Union[int, float, str]]], float64]:
 
-        if self.gec_hyperparameters["randomize"]:
+        if self.gec_hyperparameters_["randomize"]:
             np.random.seed(int(datetime.now().timestamp() % 1 * 1e7))
 
         n_random_exploration = min(
-            self.gec_hyperparameters["n_random_exploration"], int(n_iter / 2)
+            self.gec_hyperparameters_["n_random_exploration"], int(n_iter / 2)
         )
 
         for i in tqdm(list(range(n_iter))):
-            if (i + self.gec_iter) < n_random_exploration:
+            if (i + self.gec_iter_) < n_random_exploration:
                 (
                     selected_arm,
                     selected_combination,
                     selected_combination_bagging,
                     arguments,
                 ) = self._get_random_hyperparameter_configuration()
 
@@ -852,15 +852,15 @@
             )
 
             if "yes_bagging" in selected_arm:
                 self._update_gec_fields_bagging(
                     score, selected_combination_bagging, mean_bagging, sigma_bagging
                 )
 
-        return (self.best_params_, self.best_score)
+        return (self.best_params_, self.best_score_gec_)
 
     def _get_random_hyperparameter_configuration(
         self,
     ) -> Tuple[
         str_,
         ndarray,
         Tuple[int, float64],
@@ -897,89 +897,89 @@
         )
 
     def _select_parameters(self) -> Tuple[str, ndarray, ndarray, ndarray]:
 
         sampled_reward = np.array(
             [
                 beta.rvs(reward["a"], reward["b"])
-                for arm, reward in self.rewards.items()
+                for arm, reward in self.rewards_.items()
                 if arm in self._categorical_hyperparameter_combinations
             ]
         )
         selected_arm_index = sampled_reward.argmax()
         selected_arm = self._categorical_hyperparameter_combinations[selected_arm_index]
 
         sets = np.array(
             [
-                np.random.choice(range_, self.gec_hyperparameters["n_sample_initial"])
+                np.random.choice(range_, self.gec_hyperparameters_["n_sample_initial"])
                 for _, range_ in self._real_hyperparameters_linear
             ]
         )
 
         combinations = self._get_combinations_to_score(sets)
 
         assert len(combinations), sets
 
-        if len(self.hyperparameter_scores["inputs"]) > 0:
+        if len(self.hyperparameter_scores_["inputs"]) > 0:
             self._fit_gaussian()
 
         mean, sigma = self.gaussian.predict(combinations, return_std=True)
 
         predicted_rewards = np.array(
             [
                 scipy.stats.norm.ppf(
-                    self.gec_hyperparameters["hyperparams_acquisition_percentile"],
+                    self.gec_hyperparameters_["hyperparams_acquisition_percentile"],
                     loc=m,
                     scale=s,
                 )
                 for m, s in zip(mean, sigma)
             ]
         )
 
         selected_combination = combinations[np.argmax(predicted_rewards)]
 
         return (selected_arm, selected_combination, mean, sigma)
 
     def _get_combinations_to_score(self, sets: ndarray) -> List[ndarray]:
-        if len(self.hyperparameter_scores["inputs"]):
-            n_best = max(3, int(self.gec_iter * self.gec_hyperparameters["best_share"]))
+        if len(self.hyperparameter_scores_["inputs"]):
+            n_best = max(3, int(self.gec_iter_ * self.gec_hyperparameters_["best_share"]))
             best_interactions = np.argsort(
-                np.array(self.hyperparameter_scores["output"])
+                np.array(self.hyperparameter_scores_["output"])
             )[::-1][:n_best]
 
-            best_hyperparameters = np.array(self.hyperparameter_scores["inputs"])[
+            best_hyperparameters = np.array(self.hyperparameter_scores_["inputs"])[
                 best_interactions, :
             ]
 
             closest_hyperparameters = best_hyperparameters.dot(sets).argsort(1)[
-                :, : self.gec_hyperparameters["n_sample"]
+                :, : self.gec_hyperparameters_["n_sample"]
             ]
             selected_hyperparameter_indices = np.unique(
                 closest_hyperparameters.flatten()
             )
 
             combinations = list(sets[:, selected_hyperparameter_indices].T)
         else:
-            combinations = list(sets[:, : self.gec_hyperparameters["n_sample"]].T)
+            combinations = list(sets[:, : self.gec_hyperparameters_["n_sample"]].T)
 
         return combinations
 
     def _select_bagging_parameters(
         self,
     ) -> Tuple[Tuple[int, float64], ndarray, ndarray]:
-        if len(self.bagging_scores["inputs"]) > 0:
+        if len(self.bagging_scores_["inputs"]) > 0:
             self._fit_gaussian_bagging()
         mean_bagging, sigma_bagging = self.gaussian_bagging.predict(
             self._bagging_combinations_rescaled, return_std=True
         )
 
         predicted_rewards_bagging = np.array(
             [
                 scipy.stats.norm.ppf(
-                    self.gec_hyperparameters["bagging_acquisition_percentile"],
+                    self.gec_hyperparameters_["bagging_acquisition_percentile"],
                     loc=m,
                     scale=s,
                 )
                 for m, s in zip(mean_bagging, sigma_bagging)
             ]
         )
         best_predicted_combination_bagging = self._bagging_combinations[
@@ -993,57 +993,57 @@
         arguments: Dict[str, Optional[Union[str, float, int, float64]]],
         selected_arm: Union[str, str_],
         selected_combination: ndarray,
         mean: Optional[ndarray],
         sigma: Optional[ndarray],
     ) -> None:
 
-        self.selected_arms.append(selected_arm)
-        self.hyperparameter_scores["inputs"].append(
+        self.selected_arms_.append(selected_arm)
+        self.hyperparameter_scores_["inputs"].append(
             [float(f) for f in selected_combination]
         )
-        self.hyperparameter_scores["output"].append(score)
+        self.hyperparameter_scores_["output"].append(score)
 
         if mean is not None:
-            self.hyperparameter_scores["means"].append(mean)
-            self.hyperparameter_scores["sigmas"].append(sigma)
+            self.hyperparameter_scores_["means"].append(mean)
+            self.hyperparameter_scores_["sigmas"].append(sigma)
 
-        if self.best_score is not None:
-            score_delta = score - self.best_score
+        if self.best_score_gec_ is not None:
+            score_delta = score - self.best_score_gec_
             weighted_score_delta = (
-                score_delta * self.gec_hyperparameters["bandit_greediness"]
+                score_delta * self.gec_hyperparameters_["bandit_greediness"]
             )
             if score_delta > 0:
-                self.rewards[selected_arm]["a"] = (
-                    self.rewards[selected_arm]["a"] + weighted_score_delta
+                self.rewards_[selected_arm]["a"] = (
+                    self.rewards_[selected_arm]["a"] + weighted_score_delta
                 )
                 self.best_params_ = arguments
-                self.best_score = score
+                self.best_score_gec_ = score
             else:
-                self.rewards[selected_arm]["b"] = (
-                    self.rewards[selected_arm]["b"] - weighted_score_delta
+                self.rewards_[selected_arm]["b"] = (
+                    self.rewards_[selected_arm]["b"] - weighted_score_delta
                 )
         else:
-            self.best_score = score
+            self.best_score_gec_ = score
             self.best_params_ = arguments
 
     def _update_gec_fields_bagging(
         self,
         score: float64,
         selected_combination_bagging: Tuple[int, float64],
         mean_bagging: Optional[ndarray],
         sigma_bagging: Optional[ndarray],
     ) -> None:
-        self.bagging_scores["inputs"].append(
+        self.bagging_scores_["inputs"].append(
             list(self._rescale_bagging_combination(*selected_combination_bagging))
         )
-        self.bagging_scores["output"].append(score)
+        self.bagging_scores_["output"].append(score)
         if mean_bagging is not None:
-            self.bagging_scores["means"].append(mean_bagging)
-            self.bagging_scores["sigmas"].append(sigma_bagging)
+            self.bagging_scores_["means"].append(mean_bagging)
+            self.bagging_scores_["sigmas"].append(sigma_bagging)
 
     def _build_arguments(
         self, categorical_combination: List[str], real_combination_linear: ndarray
     ) -> Dict[str, Optional[Union[int, float, str]]]:
         best_predicted_combination_converted = [
             self._real_hyperparameters_map[name][value]
             for name, value in zip(
@@ -1072,43 +1072,43 @@
             **self.fixed_params,
             **self._init_args,
             **self._init_kwargs,
         }
 
     def _fit_best_params(self, X: ndarray, y: ndarray) -> None:
 
-        if hasattr(self, "best_params_") and self.best_params_ is not None:
+        if hasattr(self, "best_params") and self.best_params_ is not None:
             for k, v in self.best_params_.items():
                 setattr(self, k, v)
             setattr(self, "random_state", 101)
 
-        super().fit(X, y, **self.fit_params)
+        super().fit(X, y, **self.gec_fit_params_)
 
     @ignore_warnings(category=ConvergenceWarning)
     def _fit_gaussian(self) -> None:
         self.gaussian.fit(
-            np.array(self.hyperparameter_scores["inputs"]),
-            np.array(self.hyperparameter_scores["output"])
-            - np.mean(self.hyperparameter_scores["output"]),
+            np.array(self.hyperparameter_scores_["inputs"]),
+            np.array(self.hyperparameter_scores_["output"])
+            - np.mean(self.hyperparameter_scores_["output"]),
         )
 
     @ignore_warnings(category=ConvergenceWarning)
     def _fit_gaussian_bagging(self) -> None:
-        if len(self.bagging_scores["output"]):
+        if len(self.bagging_scores_["output"]):
             self.gaussian_bagging.fit(
-                np.array(self.bagging_scores["inputs"]),
-                np.array(self.bagging_scores["output"])
-                - np.mean(self.bagging_scores["output"]),
+                np.array(self.bagging_scores_["inputs"]),
+                np.array(self.bagging_scores_["output"])
+                - np.mean(self.bagging_scores_["output"]),
             )
 
     def _get_best_arm(self) -> str:
         mean_reward = np.array(
             [
                 reward["a"] / (reward["a"] + reward["b"])
-                for arm, reward in self.rewards.items()
+                for arm, reward in self.rewards_.items()
                 if arm in self._categorical_hyperparameter_combinations
             ]
         )
         best_arm = self._categorical_hyperparameter_combinations[mean_reward.argmax()]
         return best_arm
 
     def _find_best_parameters(
@@ -1257,63 +1257,63 @@
         figs = {}
 
         fig, axes = plt.subplots(
             nrows=2, ncols=2, sharex=True, sharey=False, figsize=(12, 12)
         )
         ax1, ax2, ax3, ax4 = axes.flatten()
 
-        x = np.arange(len(self.hyperparameter_scores["means"]))
+        x = np.arange(len(self.hyperparameter_scores_["means"]))
         self._plot_mean_prediction_and_mean_variance(ax1, x)
         self._plot_prediction_std_and_variance_std(ax2, x)
         self._plot_prediction_mean_variance_correlation(ax3, x)
         self._plot_linear_scaled_parameter_samples(ax4)
 
         figs["parameters"] = fig
 
         fig2 = self._plot_boosting_parameter_surface()
         figs["bagging"] = fig2
 
         return figs
 
     def _plot_mean_prediction_and_mean_variance(self, ax: Axes, x: ndarray) -> None:
-        gp_mean_prediction = [np.mean(x) for x in self.hyperparameter_scores["means"]]
-        gp_mean_sigma = [np.mean(x) for x in self.hyperparameter_scores["sigmas"]]
+        gp_mean_prediction = [np.mean(x) for x in self.hyperparameter_scores_["means"]]
+        gp_mean_sigma = [np.mean(x) for x in self.hyperparameter_scores_["sigmas"]]
 
         ax.plot(x, gp_mean_prediction, label="mean_prediction")
         ax.plot(x, gp_mean_sigma, label="mean_sigma")
         ax.legend(loc="upper right")
 
     def _plot_prediction_std_and_variance_std(self, ax: Axes, x: ndarray) -> None:
         gp_prediction_variance = [
-            np.std(x) for x in self.hyperparameter_scores["means"]
+            np.std(x) for x in self.hyperparameter_scores_["means"]
         ]
-        gp_sigma_variance = [np.std(x) for x in self.hyperparameter_scores["sigmas"]]
+        gp_sigma_variance = [np.std(x) for x in self.hyperparameter_scores_["sigmas"]]
 
         ax.plot(x, gp_prediction_variance, label="prediction_variance")
         ax.plot(x, gp_sigma_variance, label="sigma_variance")
         ax.legend(loc="lower right")
 
     def _plot_prediction_mean_variance_correlation(self, ax: Axes, x: ndarray) -> None:
         correlation = [
             np.corrcoef(
-                self.hyperparameter_scores["means"][i],
-                self.hyperparameter_scores["sigmas"][i],
+                self.hyperparameter_scores_["means"][i],
+                self.hyperparameter_scores_["sigmas"][i],
             )[0, 1]
             for i in x
         ]
 
         ax.plot(
             x,
             correlation,
             label="corr(preds mean, preds variance)",
         )
         ax.legend(loc="lower right")
 
     def _plot_linear_scaled_parameter_samples(self, ax: Axes) -> None:
-        inputs_ = np.array(self.hyperparameter_scores["inputs"])
+        inputs_ = np.array(self.hyperparameter_scores_["inputs"])
         x = np.arange(inputs_.shape[0])
         assert (
             (len(self._real_hyperparameter_names) == inputs_.shape[1]),
             f"{len(self._real_hyperparameter_names)}!={inputs_.shape[1]}",
         )
         for i in range(inputs_.shape[1]):
             ax.plot(x, inputs_[:, i], label=self._real_hyperparameter_names[i])
```

### Comparing `gecs-0.31.0/src/gecs/utils/gaussian_process_visualisation.py` & `gecs-0.32.0/src/gecs/utils/gaussian_process_visualisation.py`

 * *Files identical despite different names*

### Comparing `gecs-0.31.0/setup.py` & `gecs-0.32.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,17 @@
  'scikit-learn==1.2.2',
  'scipy==1.10.1',
  'tqdm==4.65.0',
  'typer==0.9.0']
 
 setup_kwargs = {
     'name': 'gecs',
-    'version': '0.31.0',
+    'version': '0.32.0',
     'description': 'LightGBM Classifier with integrated bayesian hyperparameter optimization',
-    'long_description': "![a gecko looking at the camera with bayesian math in white on a pink and green background](documentation/assets/header.png)\n\n\n# (100)gecs\n\nBayesian hyperparameter tuning for LGBMClassifier with a scikit-learn API\n\n\n## Table of Contents\n\n- [Project Overview](#project-overview)\n- [Introduction](#introduction)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Example](#example)\n- [Contributing](#contributing)\n- [License](#license)\n\n\n## Project Overview\n\n`gecs` is a tool to help automate the process of hyperparameter tuning for LightGBM classifiers, which can potentially save significant time and computational resources in model building and optimization processes. The `GEC` stands for **G**ood **E**nough **C**lassifier, which allows you to focus on other tasks such as feature engineering. If you deploy 100 of them, you get 100GECs.\n\n\n## Introduction\n\nThe primary class in this package is `GEC`, which is derived from `LGBMClassifier`. Like its parent, GEC can be used to build and train gradient boosting models, but with the added feature of **automated bayesian hyperparameter optimization**. It can be imported from `gecs.gec` and then used in place of `LGBMClassifier`, with the same API.\n\nBy default, `GEC` optimizes `boosting_type`, `learning_rate`, `reg_alpha`, `reg_lambda`, `min_child_samples`, `min_child_weight`, `colsample_bytree`, `subsample_freq`, `subsample` and optionally `num_leaves` and `n_estimators`. Which hyperparameters to tune is fully customizable.\n\n\n## Installation\n\n    pip install gecs\n\n\n## Usage\n\n\nThe `GEC` class provides the same API to the user as the `LGBMClassifier` class of `lightgbm`, and additionally:\n\n-   the two additional parameters to the fit method:\n    - `n_iter`: Defines the number of hyperparameter combinations that the model should try. More iterations could lead to better model performance, but at the expense of computational resources\n\n    - `fixed_hyperparameters`: Allows the user to specify hyperparameters that the GEC should not optimize. By default, these are `n_estimators` and `num_leaves`. Any of the LGBMClassifier init arguments can be fixed, and so can  `subsample_freq` and `subsample`, but only jointly. This is done by passing the value `bagging`.\n\n-   the methods `serialize` and `deserialize`, which stores the `GEC` state for the hyperparameter optimization process, **but not the fitted** `LGBMClassifier` **parameters**, to a json file. To store the boosted tree model itself, you have to provide your own serialization or use `pickle`\n\n-   the methods `freeze` and `unfreeze` that turn the `GEC` functionally into a `LGBMClassifier` and back\n\n\n## Example\n\nThe default use of `GEC` would look like this:\n\n    from gecs.gec import GEC\n\n    gec.fit(X, y)\n\n    gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes\n\n    gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier\n\n    yhat = gec.predict(X)\n\n    gec.freeze() # freeze GEC so that it behaves like a LGBMClassifier\n\n    gec.unfreeze() # unfreeze to enable GEC hyperparameter optimisation\n\n\n\n## Contributing\n\nIf you want to contribute, please reach out and I'll design a process around it.\n\n## License\n\nMIT\n\n## Contact Information\n\nYou can find my contact information on my website: [https://leonluithlen.eu](https://leonluithlen.eu)",
+    'long_description': '![a gecko looking at the camera with bayesian math in white on a pink and green background](documentation/assets/header.png)\n\n\n# (100)gecs\n\nBayesian hyperparameter tuning for LGBMClassifier with a scikit-learn API\n\n\n## Table of Contents\n\n- [Project Overview](#project-overview)\n- [Introduction](#introduction)\n- [Installation](#installation)\n- [Usage](#usage)\n- [Example](#example)\n- [Contributing](#contributing)\n- [License](#license)\n\n\n## Project Overview\n\n`gecs` is a tool to help automate the process of hyperparameter tuning for LightGBM classifiers, which can potentially save significant time and computational resources in model building and optimization processes. The `GEC` stands for **G**ood **E**nough **C**lassifier, which allows you to focus on other tasks such as feature engineering. If you deploy 100 of them, you get 100GECs.\n\n\n## Introduction\n\nThe primary class in this package is `GEC`, which is derived from `LGBMClassifier`. Like its parent, GEC can be used to build and train gradient boosting models, but with the added feature of **automated bayesian hyperparameter optimization**. It can be imported from `gecs.gec` and then used in place of `LGBMClassifier`, with the same API.\n\nBy default, `GEC` optimizes `boosting_type`, `learning_rate`, `reg_alpha`, `reg_lambda`, `min_child_samples`, `min_child_weight`, `colsample_bytree`, `subsample_freq`, `subsample` and optionally `num_leaves` and `n_estimators`. Which hyperparameters to tune is fully customizable.\n\n\n## Installation\n\n    pip install gecs\n\n\n## Usage\n\n\nThe `GEC` class provides the same API to the user as the `LGBMClassifier` class of `lightgbm`, and additionally:\n\n-   the two additional parameters to the fit method:\n    - `n_iter`: Defines the number of hyperparameter combinations that the model should try. More iterations could lead to better model performance, but at the expense of computational resources\n\n    - `fixed_hyperparameters`: Allows the user to specify hyperparameters that the GEC should not optimize. By default, these are `n_estimators` and `num_leaves`. Any of the LGBMClassifier init arguments can be fixed, and so can  `subsample_freq` and `subsample`, but only jointly. This is done by passing the value `bagging`.\n\n-   the methods `serialize` and `deserialize`, which stores the `GEC` state for the hyperparameter optimization process, **but not the fitted** `LGBMClassifier` **parameters**, to a json file. To store the boosted tree model itself, you have to provide your own serialization or use `pickle`\n\n-   the methods `freeze` and `unfreeze` that turn the `GEC` functionally into a `LGBMClassifier` and back\n\n\n## Example\n\nThe default use of `GEC` would look like this:\n\n    from sklearn.datasets import load_iris\n    from gecs.gec import GEC\n\n    X, y = load_iris(return_X_y=True)\n\n\n    # fit and infer GEC\n    gec = GEC()\n    gec.fit(X, y)\n    yhat = gec.predict(X)\n\n\n    # manage GEC state\n    path = "./gec.json"\n    gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes\n    gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier\n    gec.freeze() # freeze GEC so that it behaves like a LGBMClassifier\n    gec.unfreeze() # unfreeze to enable GEC hyperparameter optimisation\n\n\n    # benchmark against LGBMClassifier\n    from lightgbm import LGBMClassifier\n    from sklearn.model_selection import cross_val_score\n    import numpy as np\n\n    clf = LGBMClassifier()\n    lgbm_score = np.mean(cross_val_score(clf, X, y))\n\n    gec.freeze()\n    gec_score = np.mean(cross_val_score(gec, X, y))\n\n    print(f"{gec_score = }, {lgbm_score = }")\n    assert gec_score > lgbm_score, "GEC doesn\'t outperform LGBMClassifier"\n\n\n\n## Contributing\n\nIf you want to contribute, please reach out and I\'ll design a process around it.\n\n## License\n\nMIT\n\n## Contact Information\n\nYou can find my contact information on my website: [https://leonluithlen.eu](https://leonluithlen.eu)',
     'author': 'Leon Luithlen',
     'author_email': 'leontimnaluithlen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xideas/sequifier',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `gecs-0.31.0/PKG-INFO` & `gecs-0.32.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gecs
-Version: 0.31.0
+Version: 0.32.0
 Summary: LightGBM Classifier with integrated bayesian hyperparameter optimization
 Home-page: https://github.com/0xideas/sequifier
 License: MIT
 Keywords: lightgbm,classification,machine learning,hyperparameter optimization,classifier
 Author: Leon Luithlen
 Author-email: leontimnaluithlen@gmail.com
 Requires-Python: >=3.10.0,<3.11.0
@@ -75,27 +75,47 @@
 -   the methods `freeze` and `unfreeze` that turn the `GEC` functionally into a `LGBMClassifier` and back
 
 
 ## Example
 
 The default use of `GEC` would look like this:
 
+    from sklearn.datasets import load_iris
     from gecs.gec import GEC
 
+    X, y = load_iris(return_X_y=True)
+
+
+    # fit and infer GEC
+    gec = GEC()
     gec.fit(X, y)
+    yhat = gec.predict(X)
 
-    gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes
 
+    # manage GEC state
+    path = "./gec.json"
+    gec.serialize(path) # stores gec data and settings, but not underlying LGBMClassifier attributes
     gec2 = GEC.deserialize(path, X, y) # X and y are necessary to fit the underlying LGBMClassifier
+    gec.freeze() # freeze GEC so that it behaves like a LGBMClassifier
+    gec.unfreeze() # unfreeze to enable GEC hyperparameter optimisation
 
-    yhat = gec.predict(X)
 
-    gec.freeze() # freeze GEC so that it behaves like a LGBMClassifier
+    # benchmark against LGBMClassifier
+    from lightgbm import LGBMClassifier
+    from sklearn.model_selection import cross_val_score
+    import numpy as np
 
-    gec.unfreeze() # unfreeze to enable GEC hyperparameter optimisation
+    clf = LGBMClassifier()
+    lgbm_score = np.mean(cross_val_score(clf, X, y))
+
+    gec.freeze()
+    gec_score = np.mean(cross_val_score(gec, X, y))
+
+    print(f"{gec_score = }, {lgbm_score = }")
+    assert gec_score > lgbm_score, "GEC doesn't outperform LGBMClassifier"
 
 
 
 ## Contributing
 
 If you want to contribute, please reach out and I'll design a process around it.
```

