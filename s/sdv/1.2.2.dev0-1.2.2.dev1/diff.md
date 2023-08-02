# Comparing `tmp/sdv-1.2.2.dev0.tar.gz` & `tmp/sdv-1.2.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdv-1.2.2.dev0.tar", last modified: Fri Jul 21 02:24:52 2023, max compression
+gzip compressed data, was "sdv-1.2.2.dev1.tar", last modified: Wed Aug  2 17:40:55 2023, max compression
```

## Comparing `sdv-1.2.2.dev0.tar` & `sdv-1.2.2.dev1.tar`

### file list

```diff
@@ -1,657 +1,658 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.656209 sdv-1.2.2.dev0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-24 21:06:49.000000 sdv-1.2.2.dev0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8110 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    70434 2023-07-13 19:59:39.000000 sdv-1.2.2.dev0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4818 2023-01-24 21:06:49.000000 sdv-1.2.2.dev0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    81220 2023-07-21 02:24:52.656490 sdv-1.2.2.dev0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9801 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.504224 sdv-1.2.2.dev0/docs/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      604 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/Makefile
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.505149 sdv-1.2.2.dev0/docs/api_reference/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.505688 sdv-1.2.2.dev0/docs/api_reference/constraints/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.526239 sdv-1.2.2.dev0/docs/api_reference/constraints/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      666 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      627 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      117 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      131 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Range.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      588 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.fit_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.is_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      523 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      359 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/base.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2609 2022-07-22 02:55:50.000000 sdv-1.2.2.dev0/docs/api_reference/constraints/tabular.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      353 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/evaluation.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      347 2022-07-22 02:55:50.000000 sdv-1.2.2.dev0/docs/api_reference/index.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.526825 sdv-1.2.2.dev0/docs/api_reference/lite/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.528782 sdv-1.2.2.dev0/docs/api_reference/lite/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      205 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.list_available_presets.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      502 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.2.2.dev0/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       94 2022-07-22 02:55:50.000000 sdv-1.2.2.dev0/docs/api_reference/lite/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      348 2022-07-22 02:55:50.000000 sdv-1.2.2.dev0/docs/api_reference/lite/tabular.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.529579 sdv-1.2.2.dev0/docs/api_reference/metadata/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.538520 sdv-1.2.2.dev0/docs/api_reference/metadata/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_field.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_relationship.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_table.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_children.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_dtypes.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_field_meta.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_fields.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      184 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_foreign_keys.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_parents.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_primary_key.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_table_meta.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_tables.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_table.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_tables.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      877 2022-09-29 22:36:12.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.set_primary_key.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_json.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.validate.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.visualize.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.filter_valid.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_json.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_dtypes.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_fields.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_model_kwargs.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.reverse_transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      668 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_model_kwargs.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_primary_key.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_dict.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_json.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.transform.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      854 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/dataset.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      116 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      583 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/metadata/table.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.539701 sdv-1.2.2.dev0/docs/api_reference/metrics/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.583210 sdv-1.2.2.dev0/docs/api_reference/metrics/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.demos.load_multi_table_demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.demos.load_single_table_demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.demos.load_timeseries_demo.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:23.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      614 2022-08-30 22:45:23.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      506 2022-08-30 22:45:24.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      573 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-08-30 23:02:40.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-08-30 23:02:40.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 23:02:40.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-08-30 23:02:15.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-08-30 23:02:15.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      534 2022-08-30 23:02:15.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      638 2022-08-30 22:45:24.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      242 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2022-08-30 22:45:24.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      236 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      582 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:24.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      204 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      661 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      210 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      897 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      811 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      762 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      565 2022-08-30 22:45:24.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      734 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      818 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      842 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      720 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      192 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      788 2022-10-05 00:20:25.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      760 2022-10-05 00:20:25.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-08-30 23:02:40.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-08-30 23:02:40.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      649 2022-08-30 23:02:40.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-08-30 23:02:15.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-08-30 23:02:15.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-08-30 23:02:15.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      717 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      657 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      688 2022-10-05 00:20:25.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      701 2022-08-30 22:45:24.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      222 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      957 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      195 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      822 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      819 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      239 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      895 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      257 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      857 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.compute.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      551 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      683 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      230 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      672 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.get_subclasses.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      213 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/demos.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1402 2022-09-22 23:47:45.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/relational.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4109 2022-09-22 23:47:45.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/tabular.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      735 2022-12-21 22:30:23.000000 sdv-1.2.2.dev0/docs/api_reference/metrics/timeseries.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.583745 sdv-1.2.2.dev0/docs/api_reference/relational/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.584991 sdv-1.2.2.dev0/docs/api_reference/relational/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      416 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/relational/api/sdv.relational.hma.HMA1.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/relational/hma1.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/relational/index.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.585316 sdv-1.2.2.dev0/docs/api_reference/sampling/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.585825 sdv-1.2.2.dev0/docs/api_reference/sampling/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/sampling/api/sdv.sampling.Condition.get_column_values.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      151 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/sampling/api/sdv.sampling.Condition.get_num_rows.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      417 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/sampling/api/sdv.sampling.Condition.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/sampling/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/sampling/tabular.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/sdv.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.586981 sdv-1.2.2.dev0/docs/api_reference/tabular/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.594399 sdv-1.2.2.dev0/docs/api_reference/tabular/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_distributions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      655 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_distributions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_likelihood.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_parameters.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      663 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.set_parameters.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      463 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      450 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      129 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_conditions.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      187 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_remaining_columns.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      339 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/copulagan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      489 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/copulas.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      260 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/ctgan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      136 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      249 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/tabular/tvae.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.594751 sdv-1.2.2.dev0/docs/api_reference/timeseries/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.596168 sdv-1.2.2.dev0/docs/api_reference/timeseries/api/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.fit.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.get_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.load.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      338 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.sample.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.2.dev0/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.save.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      108 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/timeseries/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/api_reference/timeseries/par.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6934 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/docs/conf.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.596873 sdv-1.2.2.dev0/docs/developer_guides/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8613 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/docs/developer_guides/contributing.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      364 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/developer_guides/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2905 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/developer_guides/overview.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.597652 sdv-1.2.2.dev0/docs/developer_guides/sdv/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5889 2022-07-22 02:55:50.000000 sdv-1.2.2.dev0/docs/developer_guides/sdv/constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      292 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/developer_guides/sdv/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7480 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/developer_guides/sdv/metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9508 2023-02-02 20:58:41.000000 sdv-1.2.2.dev0/docs/developer_guides/sdv/tabular.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.598276 sdv-1.2.2.dev0/docs/getting_started/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      113 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/getting_started/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2557 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/getting_started/install.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3664 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/getting_started/quickstart.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/history.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.610131 sdv-1.2.2.dev0/docs/images/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    52078 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/images/CTGAN-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    50900 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/images/Copulas-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60600 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/images/DataCebo-Blue.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    54065 2023-04-20 22:38:57.000000 sdv-1.2.2.dev0/docs/images/DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    46250 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/images/DeepEcho-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    25573 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/images/RDT-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   243101 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/docs/images/Real-vs-Synthetic-Evaluation.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    27285 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/images/SDGym-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    35670 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/images/SDMetrics-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22394 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/images/SDV-DataCebo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    64162 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/docs/images/SDV-logo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8765 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/images/SDV.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   412158 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/docs/images/Single-Table-Metadata-Example.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    99815 2022-07-22 02:55:50.000000 sdv-1.2.2.dev0/docs/images/custom_constraint.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    50140 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/docs/images/datacebo-logo-dark-mode.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    50481 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/docs/images/datacebo-logo.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      547 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/images/google_colab.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.2.2.dev0/docs/images/hma1_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8748 2022-12-08 23:36:42.000000 sdv-1.2.2.dev0/docs/images/metadata_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67425 2022-12-08 23:36:42.000000 sdv-1.2.2.dev0/docs/images/metadata_2.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2497 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/images/mybinder.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.2.2.dev0/docs/images/quickstart_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   176980 2023-01-24 21:06:49.000000 sdv-1.2.2.dev0/docs/images/rdt_main_tranformation.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2283 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/images/slack.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6075 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/docs/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      765 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/make.bat
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.612424 sdv-1.2.2.dev0/docs/savefig/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:00:09.000000 sdv-1.2.2.dev0/docs/savefig/copulagan_experience_years_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12668 2022-12-08 23:00:10.000000 sdv-1.2.2.dev0/docs/savefig/copulagan_experience_years_2.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10277 2022-12-08 23:00:37.000000 sdv-1.2.2.dev0/docs/savefig/copulagan_experience_years_3.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:05:15.000000 sdv-1.2.2.dev0/docs/savefig/experience_years_1.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10270 2022-12-08 23:05:16.000000 sdv-1.2.2.dev0/docs/savefig/experience_years_2.png
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12415 2022-12-08 23:05:16.000000 sdv-1.2.2.dev0/docs/savefig/experience_years_3.png
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.497298 sdv-1.2.2.dev0/docs/sdv_theme/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.612766 sdv-1.2.2.dev0/docs/sdv_theme/static/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1046 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/sdv_theme/static/slack-32.png
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.613208 sdv-1.2.2.dev0/docs/user_guides/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.615989 sdv-1.2.2.dev0/docs/user_guides/benchmarking/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4753 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/benchmarking/datasets.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1885 2023-02-02 20:58:41.000000 sdv-1.2.2.dev0/docs/user_guides/benchmarking/docker.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      563 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/benchmarking/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2562 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/benchmarking/install.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7764 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/benchmarking/run.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1731 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/benchmarking/synthesizers.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.616972 sdv-1.2.2.dev0/docs/user_guides/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3240 2022-12-21 22:30:23.000000 sdv-1.2.2.dev0/docs/user_guides/evaluation/evaluation_framework.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      504 2022-12-21 22:30:23.000000 sdv-1.2.2.dev0/docs/user_guides/evaluation/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-12-21 22:30:23.000000 sdv-1.2.2.dev0/docs/user_guides/evaluation/synthetic_data_metrics.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      277 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/index.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.618705 sdv-1.2.2.dev0/docs/user_guides/relational/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2131 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/relational/constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      141 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/relational/data_description.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8143 2022-12-21 22:30:23.000000 sdv-1.2.2.dev0/docs/user_guides/relational/hma1.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/relational/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       79 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/relational/models.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6906 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/relational/relational_metadata.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.623679 sdv-1.2.2.dev0/docs/user_guides/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/single_table/constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    24765 2023-02-02 20:58:41.000000 sdv-1.2.2.dev0/docs/user_guides/single_table/copulagan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18899 2023-02-02 20:58:41.000000 sdv-1.2.2.dev0/docs/user_guides/single_table/ctgan.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6108 2022-09-22 23:47:45.000000 sdv-1.2.2.dev0/docs/user_guides/single_table/custom_constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      121 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/single_table/data_description.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20259 2023-02-02 20:58:41.000000 sdv-1.2.2.dev0/docs/user_guides/single_table/gaussian_copula.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14530 2022-09-22 23:47:45.000000 sdv-1.2.2.dev0/docs/user_guides/single_table/handling_constraints.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      980 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/single_table/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/single_table/models.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       65 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/single_table/table_metadata.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8354 2022-07-22 02:55:50.000000 sdv-1.2.2.dev0/docs/user_guides/single_table/tabular_preset.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18149 2023-02-02 20:58:41.000000 sdv-1.2.2.dev0/docs/user_guides/single_table/tvae.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.624674 sdv-1.2.2.dev0/docs/user_guides/timeseries/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       92 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/timeseries/index.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       78 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/docs/user_guides/timeseries/models.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14863 2022-12-21 22:30:23.000000 sdv-1.2.2.dev0/docs/user_guides/timeseries/par.rst
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.625380 sdv-1.2.2.dev0/sdv/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2988 2023-07-13 20:00:04.000000 sdv-1.2.2.dev0/sdv/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.628198 sdv-1.2.2.dev0/sdv/constraints/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      542 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/sdv/constraints/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18056 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/sdv/constraints/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      799 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/constraints/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    54000 2023-07-13 19:59:39.000000 sdv-1.2.2.dev0/sdv/constraints/tabular.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5830 2023-07-13 19:59:39.000000 sdv-1.2.2.dev0/sdv/constraints/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.631034 sdv-1.2.2.dev0/sdv/data_processing/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/data_processing/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    34331 2023-07-21 02:23:44.000000 sdv-1.2.2.dev0/sdv/data_processing/data_processor.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1526 2023-04-20 18:31:25.000000 sdv-1.2.2.dev0/sdv/data_processing/datetime_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      522 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/data_processing/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4010 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/data_processing/numerical_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      726 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/data_processing/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.631625 sdv-1.2.2.dev0/sdv/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       43 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6625 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/datasets/demo.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1117 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/datasets/local.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      694 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/errors.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.632660 sdv-1.2.2.dev0/sdv/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       49 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/evaluation/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3701 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/evaluation/multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3239 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/evaluation/single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.633113 sdv-1.2.2.dev0/sdv/lite/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      145 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/lite/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7153 2023-05-10 21:10:34.000000 sdv-1.2.2.dev0/sdv/lite/single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.634858 sdv-1.2.2.dev0/sdv/metadata/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      400 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/metadata/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3060 2023-05-10 21:10:34.000000 sdv-1.2.2.dev0/sdv/metadata/anonymization.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      238 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/metadata/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10362 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/metadata/metadata_upgrader.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    29106 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/sdv/metadata/multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21941 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/sdv/metadata/single_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      793 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/metadata/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-04-20 18:31:25.000000 sdv-1.2.2.dev0/sdv/metadata/visualization.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.636226 sdv-1.2.2.dev0/sdv/metrics/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      252 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/sdv/metrics/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/sdv/metrics/demos.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/sdv/metrics/relational.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/sdv/metrics/tabular.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/sdv/metrics/timeseries.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.636691 sdv-1.2.2.dev0/sdv/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/sdv/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    20683 2023-07-13 19:59:39.000000 sdv-1.2.2.dev0/sdv/multi_table/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    15744 2023-07-13 19:59:39.000000 sdv-1.2.2.dev0/sdv/multi_table/hma.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.637424 sdv-1.2.2.dev0/sdv/sampling/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      302 2023-07-13 19:59:39.000000 sdv-1.2.2.dev0/sdv/sampling/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8640 2023-07-13 19:59:39.000000 sdv-1.2.2.dev0/sdv/sampling/hierarchical_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5578 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/sdv/sampling/independent_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      913 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/sdv/sampling/tabular.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.637714 sdv-1.2.2.dev0/sdv/sequential/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/sequential/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14850 2023-05-10 21:10:34.000000 sdv-1.2.2.dev0/sdv/sequential/par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.638909 sdv-1.2.2.dev0/sdv/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      358 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/sdv/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    45468 2023-07-13 19:59:39.000000 sdv-1.2.2.dev0/sdv/single_table/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11161 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/sdv/single_table/copulagan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14901 2023-05-10 21:10:34.000000 sdv-1.2.2.dev0/sdv/single_table/copulas.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9895 2023-05-10 21:10:34.000000 sdv-1.2.2.dev0/sdv/single_table/ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      341 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/single_table/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10141 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/sdv/single_table/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5800 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/sdv/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.627040 sdv-1.2.2.dev0/sdv.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    81220 2023-07-21 02:24:52.000000 sdv-1.2.2.dev0/sdv.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    35730 2023-07-21 02:24:52.000000 sdv-1.2.2.dev0/sdv.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-21 02:24:52.000000 sdv-1.2.2.dev0/sdv.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-21 02:24:52.000000 sdv-1.2.2.dev0/sdv.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1491 2023-07-21 02:24:52.000000 sdv-1.2.2.dev0/sdv.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-07-21 02:24:52.000000 sdv-1.2.2.dev0/sdv.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1233 2023-07-21 02:24:52.657038 sdv-1.2.2.dev0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3816 2023-07-21 02:23:44.000000 sdv-1.2.2.dev0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.639739 sdv-1.2.2.dev0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/tests/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.640209 sdv-1.2.2.dev0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/tests/integration/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.640405 sdv-1.2.2.dev0/tests/integration/data_processing/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12132 2023-05-10 21:10:34.000000 sdv-1.2.2.dev0/tests/integration/data_processing/test_data_processor.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/dataset.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.640729 sdv-1.2.2.dev0/tests/integration/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3324 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/datasets/test_demo.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.642544 sdv-1.2.2.dev0/tests/integration/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/evaluation/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1133 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/evaluation/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1131 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/evaluation/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.643869 sdv-1.2.2.dev0/tests/integration/lite/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.2.2.dev0/tests/integration/lite/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1447 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/lite/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.645644 sdv-1.2.2.dev0/tests/integration/metadata/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/metadata/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      596 2023-05-10 21:10:34.000000 sdv-1.2.2.dev0/tests/integration/metadata/test_anonymization.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4369 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/metadata/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6200 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/metadata/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.645954 sdv-1.2.2.dev0/tests/integration/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    23356 2023-07-13 19:59:39.000000 sdv-1.2.2.dev0/tests/integration/multi_table/test_hma.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.646260 sdv-1.2.2.dev0/tests/integration/sequential/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/sequential/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6268 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/sequential/test_par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.646990 sdv-1.2.2.dev0/tests/integration/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1769 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/single_table/custom_constraints.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    36264 2023-07-13 19:59:39.000000 sdv-1.2.2.dev0/tests/integration/single_table/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12402 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/tests/integration/single_table/test_copulas.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2528 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/integration/single_table/test_ctgan.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.647132 sdv-1.2.2.dev0/tests/readme_test/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13973 2022-08-16 22:57:14.000000 sdv-1.2.2.dev0/tests/readme_test/README.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.647923 sdv-1.2.2.dev0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/tests/unit/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.649344 sdv-1.2.2.dev0/tests/unit/constraints/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/tests/unit/constraints/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    32384 2023-04-20 22:38:57.000000 sdv-1.2.2.dev0/tests/unit/constraints/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   162819 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/tests/unit/constraints/test_tabular.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6848 2023-07-13 19:59:39.000000 sdv-1.2.2.dev0/tests/unit/constraints/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.650870 sdv-1.2.2.dev0/tests/unit/data_processing/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/unit/data_processing/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    80948 2023-07-21 02:23:44.000000 sdv-1.2.2.dev0/tests/unit/data_processing/test_data_processor.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2765 2023-04-20 18:31:25.000000 sdv-1.2.2.dev0/tests/unit/data_processing/test_datetime_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    14718 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/unit/data_processing/test_numerical_formatter.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      926 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/unit/data_processing/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.651835 sdv-1.2.2.dev0/tests/unit/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/unit/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9876 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/unit/datasets/test_demo.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2498 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/unit/datasets/test_local.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.652182 sdv-1.2.2.dev0/tests/unit/evaluation/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2865 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/unit/evaluation/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2533 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/unit/evaluation/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.652504 sdv-1.2.2.dev0/tests/unit/lite/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/tests/unit/lite/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10135 2023-05-10 21:10:34.000000 sdv-1.2.2.dev0/tests/unit/lite/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.653496 sdv-1.2.2.dev0/tests/unit/metadata/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/tests/unit/metadata/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5258 2023-05-10 21:10:34.000000 sdv-1.2.2.dev0/tests/unit/metadata/test_anonymization.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22557 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/unit/metadata/test_metadata_upgrader.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    75538 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/tests/unit/metadata/test_multi_table.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    66306 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/tests/unit/metadata/test_single_table.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.653995 sdv-1.2.2.dev0/tests/unit/multi_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/unit/multi_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    41567 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/tests/unit/multi_table/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19731 2023-07-13 19:59:39.000000 sdv-1.2.2.dev0/tests/unit/multi_table/test_hma.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.654570 sdv-1.2.2.dev0/tests/unit/sampling/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.2.2.dev0/tests/unit/sampling/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13827 2023-07-13 19:59:39.000000 sdv-1.2.2.dev0/tests/unit/sampling/test_hierarchical_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11155 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/tests/unit/sampling/test_independent_sampler.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2140 2022-06-21 19:18:25.000000 sdv-1.2.2.dev0/tests/unit/sampling/test_tabular.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.654865 sdv-1.2.2.dev0/tests/unit/sequential/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       50 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/unit/sequential/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    29331 2023-05-10 21:10:34.000000 sdv-1.2.2.dev0/tests/unit/sequential/test_par.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-21 02:24:52.656079 sdv-1.2.2.dev0/tests/unit/single_table/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/unit/single_table/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    77568 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/tests/unit/single_table/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13803 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/tests/unit/single_table/test_copulagan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18091 2023-05-10 21:10:34.000000 sdv-1.2.2.dev0/tests/unit/single_table/test_copulas.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10328 2023-05-10 21:10:34.000000 sdv-1.2.2.dev0/tests/unit/single_table/test_ctgan.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8358 2023-03-28 20:22:54.000000 sdv-1.2.2.dev0/tests/unit/single_table/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4604 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5572 2023-06-07 20:46:09.000000 sdv-1.2.2.dev0/tests/unit/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3051 2023-05-10 21:10:34.000000 sdv-1.2.2.dev0/tests/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.162732 sdv-1.2.2.dev1/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-24 21:06:49.000000 sdv-1.2.2.dev1/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8110 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    70434 2023-07-13 19:59:39.000000 sdv-1.2.2.dev1/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4818 2023-01-24 21:06:49.000000 sdv-1.2.2.dev1/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    81220 2023-08-02 17:40:55.163012 sdv-1.2.2.dev1/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9801 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.035230 sdv-1.2.2.dev1/docs/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      604 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/Makefile
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.036180 sdv-1.2.2.dev1/docs/api_reference/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.036727 sdv-1.2.2.dev1/docs/api_reference/constraints/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.057059 sdv-1.2.2.dev1/docs/api_reference/constraints/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      666 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      575 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      627 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      158 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      549 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      117 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      131 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Range.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      653 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      588 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.fit_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      137 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.is_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      523 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      134 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      359 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/base.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2609 2022-07-22 02:55:50.000000 sdv-1.2.2.dev1/docs/api_reference/constraints/tabular.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      353 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/evaluation.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      347 2022-07-22 02:55:50.000000 sdv-1.2.2.dev1/docs/api_reference/index.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.057541 sdv-1.2.2.dev1/docs/api_reference/lite/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.059764 sdv-1.2.2.dev1/docs/api_reference/lite/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      205 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.list_available_presets.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      502 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      211 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-29 17:31:16.000000 sdv-1.2.2.dev1/docs/api_reference/lite/api/sdv.lite.tabular.TabularPreset.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       94 2022-07-22 02:55:50.000000 sdv-1.2.2.dev1/docs/api_reference/lite/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      348 2022-07-22 02:55:50.000000 sdv-1.2.2.dev1/docs/api_reference/lite/tabular.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.060598 sdv-1.2.2.dev1/docs/api_reference/metadata/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.069145 sdv-1.2.2.dev1/docs/api_reference/metadata/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_field.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_relationship.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      161 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.add_table.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_children.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_dtypes.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_field_meta.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_fields.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      184 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_foreign_keys.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_parents.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_primary_key.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      178 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_table_meta.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.get_tables.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_table.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.load_tables.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      877 2022-09-29 22:36:12.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      181 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.set_primary_key.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.to_json.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.validate.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.visualize.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      155 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.filter_valid.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      146 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.from_json.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_dtypes.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_fields.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.get_model_kwargs.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.reverse_transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      668 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      169 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_model_kwargs.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.set_primary_key.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_dict.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      140 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.to_json.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.transform.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      854 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/dataset.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      116 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      583 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/metadata/table.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.070541 sdv-1.2.2.dev1/docs/api_reference/metrics/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.106525 sdv-1.2.2.dev1/docs/api_reference/metrics/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.demos.load_multi_table_demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      170 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.demos.load_single_table_demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.demos.load_timeseries_demo.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:23.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      614 2022-08-30 22:45:23.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      506 2022-08-30 22:45:24.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.CSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      573 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-08-30 23:02:40.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-08-30 23:02:40.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 23:02:40.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-08-30 23:02:15.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-08-30 23:02:15.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      534 2022-08-30 23:02:15.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      638 2022-08-30 22:45:24.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      242 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2022-08-30 22:45:24.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      236 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      582 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      578 2022-08-30 22:45:24.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      204 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      661 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      210 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      897 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      811 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      198 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      837 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      762 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      565 2022-08-30 22:45:24.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      183 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      734 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      818 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      221 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      842 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      168 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      664 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      180 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      203 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      720 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      192 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      788 2022-10-05 00:20:25.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      209 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      760 2022-10-05 00:20:25.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      171 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      194 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-08-30 23:02:40.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-08-30 23:02:40.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      649 2022-08-30 23:02:40.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-08-30 23:02:15.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      179 2022-08-30 23:02:15.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      605 2022-08-30 23:02:15.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      717 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      716 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      657 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      688 2022-10-05 00:20:25.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      701 2022-08-30 22:45:24.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      222 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      245 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      957 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      195 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      218 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      822 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      182 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      215 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      819 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      216 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      239 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      895 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      643 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      875 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      162 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      569 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      257 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      857 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      629 2022-12-08 22:56:17.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      201 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      224 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      650 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      174 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.compute.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      197 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      551 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      233 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      683 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      230 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      672 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      206 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.get_subclasses.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      584 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      213 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/demos.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      143 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1402 2022-09-22 23:47:45.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/relational.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4109 2022-09-22 23:47:45.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/tabular.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      735 2022-12-21 22:30:23.000000 sdv-1.2.2.dev1/docs/api_reference/metrics/timeseries.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.106983 sdv-1.2.2.dev1/docs/api_reference/relational/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.108015 sdv-1.2.2.dev1/docs/api_reference/relational/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      416 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/relational/api/sdv.relational.hma.HMA1.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      173 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/relational/hma1.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/relational/index.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.108425 sdv-1.2.2.dev1/docs/api_reference/sampling/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.109039 sdv-1.2.2.dev1/docs/api_reference/sampling/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      166 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/sampling/api/sdv.sampling.Condition.get_column_values.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      151 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/sampling/api/sdv.sampling.Condition.get_num_rows.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      417 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/sampling/api/sdv.sampling.Condition.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      109 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/sampling/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      227 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/sampling/tabular.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/sdv.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.110092 sdv-1.2.2.dev1/docs/api_reference/tabular/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.118114 sdv-1.2.2.dev1/docs/api_reference/tabular/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      147 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_distributions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      176 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      655 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      214 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      150 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_distributions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_likelihood.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      185 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.get_parameters.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      663 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      165 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      200 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      223 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      159 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      191 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.set_parameters.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      152 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      463 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      167 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.CTGAN.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      120 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      149 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      450 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      129 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_conditions.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      187 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.sample_remaining_columns.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      123 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.ctgan.TVAE.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      339 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/copulagan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      489 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/copulas.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      260 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/ctgan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      136 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      249 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/tabular/tvae.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.118523 sdv-1.2.2.dev1/docs/api_reference/timeseries/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.119803 sdv-1.2.2.dev1/docs/api_reference/timeseries/api/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.fit.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      164 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.get_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.load.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      338 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      144 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.sample.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      138 2022-06-22 20:44:18.000000 sdv-1.2.2.dev1/docs/api_reference/timeseries/api/sdv.timeseries.deepecho.PAR.save.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      108 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/timeseries/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/api_reference/timeseries/par.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6934 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/docs/conf.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.120448 sdv-1.2.2.dev1/docs/developer_guides/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8613 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/docs/developer_guides/contributing.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      364 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/developer_guides/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2905 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/developer_guides/overview.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.121285 sdv-1.2.2.dev1/docs/developer_guides/sdv/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5889 2022-07-22 02:55:50.000000 sdv-1.2.2.dev1/docs/developer_guides/sdv/constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      292 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/developer_guides/sdv/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7480 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/developer_guides/sdv/metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9508 2023-02-02 20:58:41.000000 sdv-1.2.2.dev1/docs/developer_guides/sdv/tabular.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.121936 sdv-1.2.2.dev1/docs/getting_started/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      113 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/getting_started/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2557 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/getting_started/install.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3664 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/getting_started/quickstart.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       29 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/history.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.132788 sdv-1.2.2.dev1/docs/images/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    52078 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/images/CTGAN-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50900 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/images/Copulas-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60600 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/images/DataCebo-Blue.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    54065 2023-04-20 22:38:57.000000 sdv-1.2.2.dev1/docs/images/DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    46250 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/images/DeepEcho-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    25573 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/images/RDT-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   243101 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/docs/images/Real-vs-Synthetic-Evaluation.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    27285 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/images/SDGym-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    35670 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/images/SDMetrics-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22394 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/images/SDV-DataCebo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    64162 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/docs/images/SDV-logo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8765 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/images/SDV.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   412158 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/docs/images/Single-Table-Metadata-Example.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    99815 2022-07-22 02:55:50.000000 sdv-1.2.2.dev1/docs/images/custom_constraint.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50140 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/docs/images/datacebo-logo-dark-mode.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    50481 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/docs/images/datacebo-logo.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      547 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/images/google_colab.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.2.2.dev1/docs/images/hma1_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8748 2022-12-08 23:36:42.000000 sdv-1.2.2.dev1/docs/images/metadata_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    67425 2022-12-08 23:36:42.000000 sdv-1.2.2.dev1/docs/images/metadata_2.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2497 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/images/mybinder.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    67403 2022-12-08 23:36:42.000000 sdv-1.2.2.dev1/docs/images/quickstart_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   176980 2023-01-24 21:06:49.000000 sdv-1.2.2.dev1/docs/images/rdt_main_tranformation.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2283 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/images/slack.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6075 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/docs/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      765 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/make.bat
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.134608 sdv-1.2.2.dev1/docs/savefig/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:00:09.000000 sdv-1.2.2.dev1/docs/savefig/copulagan_experience_years_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12668 2022-12-08 23:00:10.000000 sdv-1.2.2.dev1/docs/savefig/copulagan_experience_years_2.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10277 2022-12-08 23:00:37.000000 sdv-1.2.2.dev1/docs/savefig/copulagan_experience_years_3.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10974 2022-12-08 23:05:15.000000 sdv-1.2.2.dev1/docs/savefig/experience_years_1.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10270 2022-12-08 23:05:16.000000 sdv-1.2.2.dev1/docs/savefig/experience_years_2.png
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12415 2022-12-08 23:05:16.000000 sdv-1.2.2.dev1/docs/savefig/experience_years_3.png
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.027234 sdv-1.2.2.dev1/docs/sdv_theme/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.134871 sdv-1.2.2.dev1/docs/sdv_theme/static/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1046 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/sdv_theme/static/slack-32.png
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.135105 sdv-1.2.2.dev1/docs/user_guides/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.136358 sdv-1.2.2.dev1/docs/user_guides/benchmarking/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4753 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/benchmarking/datasets.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1885 2023-02-02 20:58:41.000000 sdv-1.2.2.dev1/docs/user_guides/benchmarking/docker.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      563 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/benchmarking/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2562 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/benchmarking/install.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7764 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/benchmarking/run.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1731 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/benchmarking/synthesizers.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.137112 sdv-1.2.2.dev1/docs/user_guides/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3240 2022-12-21 22:30:23.000000 sdv-1.2.2.dev1/docs/user_guides/evaluation/evaluation_framework.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      504 2022-12-21 22:30:23.000000 sdv-1.2.2.dev1/docs/user_guides/evaluation/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      219 2022-12-21 22:30:23.000000 sdv-1.2.2.dev1/docs/user_guides/evaluation/synthetic_data_metrics.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      277 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/index.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.138119 sdv-1.2.2.dev1/docs/user_guides/relational/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2131 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/relational/constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      141 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/relational/data_description.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8143 2022-12-21 22:30:23.000000 sdv-1.2.2.dev1/docs/user_guides/relational/hma1.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      177 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/relational/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       79 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/relational/models.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6906 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/relational/relational_metadata.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.141357 sdv-1.2.2.dev1/docs/user_guides/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      135 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/single_table/constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    24765 2023-02-02 20:58:41.000000 sdv-1.2.2.dev1/docs/user_guides/single_table/copulagan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18899 2023-02-02 20:58:41.000000 sdv-1.2.2.dev1/docs/user_guides/single_table/ctgan.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6108 2022-09-22 23:47:45.000000 sdv-1.2.2.dev1/docs/user_guides/single_table/custom_constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      121 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/single_table/data_description.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    20259 2023-02-02 20:58:41.000000 sdv-1.2.2.dev1/docs/user_guides/single_table/gaussian_copula.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14530 2022-09-22 23:47:45.000000 sdv-1.2.2.dev1/docs/user_guides/single_table/handling_constraints.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      980 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/single_table/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      510 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/single_table/models.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       65 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/single_table/table_metadata.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8354 2022-07-22 02:55:50.000000 sdv-1.2.2.dev1/docs/user_guides/single_table/tabular_preset.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18149 2023-02-02 20:58:41.000000 sdv-1.2.2.dev1/docs/user_guides/single_table/tvae.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.141957 sdv-1.2.2.dev1/docs/user_guides/timeseries/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       92 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/timeseries/index.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       78 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/docs/user_guides/timeseries/models.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14863 2022-12-21 22:30:23.000000 sdv-1.2.2.dev1/docs/user_guides/timeseries/par.rst
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.142454 sdv-1.2.2.dev1/sdv/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2988 2023-07-21 02:25:14.000000 sdv-1.2.2.dev1/sdv/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.144320 sdv-1.2.2.dev1/sdv/constraints/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      542 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/sdv/constraints/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18056 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/sdv/constraints/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      799 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/constraints/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    54000 2023-07-13 19:59:39.000000 sdv-1.2.2.dev1/sdv/constraints/tabular.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5830 2023-07-13 19:59:39.000000 sdv-1.2.2.dev1/sdv/constraints/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.145220 sdv-1.2.2.dev1/sdv/data_processing/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      132 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/data_processing/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    34767 2023-08-02 17:39:54.000000 sdv-1.2.2.dev1/sdv/data_processing/data_processor.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1526 2023-04-20 18:31:25.000000 sdv-1.2.2.dev1/sdv/data_processing/datetime_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      522 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/data_processing/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4010 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/data_processing/numerical_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      726 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/data_processing/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.145692 sdv-1.2.2.dev1/sdv/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       43 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6625 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/datasets/demo.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1117 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/datasets/local.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      694 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/errors.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.146146 sdv-1.2.2.dev1/sdv/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       49 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/evaluation/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3701 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/evaluation/multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3239 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/evaluation/single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.146428 sdv-1.2.2.dev1/sdv/lite/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      145 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/lite/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7153 2023-05-10 21:10:34.000000 sdv-1.2.2.dev1/sdv/lite/single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.147690 sdv-1.2.2.dev1/sdv/metadata/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      400 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/metadata/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3060 2023-05-10 21:10:34.000000 sdv-1.2.2.dev1/sdv/metadata/anonymization.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      238 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/metadata/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10362 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/metadata/metadata_upgrader.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    29106 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/sdv/metadata/multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21941 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/sdv/metadata/single_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      793 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/metadata/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2475 2023-04-20 18:31:25.000000 sdv-1.2.2.dev1/sdv/metadata/visualization.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.148417 sdv-1.2.2.dev1/sdv/metrics/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      252 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/sdv/metrics/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      156 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/sdv/metrics/demos.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/sdv/metrics/relational.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      186 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/sdv/metrics/tabular.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      188 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/sdv/metrics/timeseries.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.148879 sdv-1.2.2.dev1/sdv/multi_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      126 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/sdv/multi_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    20683 2023-07-13 19:59:39.000000 sdv-1.2.2.dev1/sdv/multi_table/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    15744 2023-07-13 19:59:39.000000 sdv-1.2.2.dev1/sdv/multi_table/hma.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.149496 sdv-1.2.2.dev1/sdv/sampling/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      302 2023-07-13 19:59:39.000000 sdv-1.2.2.dev1/sdv/sampling/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8640 2023-07-13 19:59:39.000000 sdv-1.2.2.dev1/sdv/sampling/hierarchical_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5578 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/sdv/sampling/independent_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      913 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/sdv/sampling/tabular.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.149764 sdv-1.2.2.dev1/sdv/sequential/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      124 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/sequential/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14850 2023-05-10 21:10:34.000000 sdv-1.2.2.dev1/sdv/sequential/par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.150879 sdv-1.2.2.dev1/sdv/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      358 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/sdv/single_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    45510 2023-08-02 17:39:54.000000 sdv-1.2.2.dev1/sdv/single_table/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11161 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/sdv/single_table/copulagan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14901 2023-05-10 21:10:34.000000 sdv-1.2.2.dev1/sdv/single_table/copulas.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9895 2023-05-10 21:10:34.000000 sdv-1.2.2.dev1/sdv/single_table/ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      341 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/single_table/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10141 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/sdv/single_table/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5800 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/sdv/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.143502 sdv-1.2.2.dev1/sdv.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    81220 2023-08-02 17:40:54.000000 sdv-1.2.2.dev1/sdv.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    35781 2023-08-02 17:40:54.000000 sdv-1.2.2.dev1/sdv.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-08-02 17:40:54.000000 sdv-1.2.2.dev1/sdv.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-08-02 17:40:54.000000 sdv-1.2.2.dev1/sdv.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1491 2023-08-02 17:40:54.000000 sdv-1.2.2.dev1/sdv.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-08-02 17:40:54.000000 sdv-1.2.2.dev1/sdv.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1233 2023-08-02 17:40:55.163557 sdv-1.2.2.dev1/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3816 2023-07-21 02:25:14.000000 sdv-1.2.2.dev1/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.151150 sdv-1.2.2.dev1/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/tests/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.151451 sdv-1.2.2.dev1/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/tests/integration/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.151614 sdv-1.2.2.dev1/tests/integration/data_processing/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12132 2023-05-10 21:10:34.000000 sdv-1.2.2.dev1/tests/integration/data_processing/test_data_processor.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      598 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/dataset.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.151941 sdv-1.2.2.dev1/tests/integration/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3324 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/datasets/test_demo.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.152497 sdv-1.2.2.dev1/tests/integration/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/evaluation/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1133 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/evaluation/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1131 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/evaluation/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.153033 sdv-1.2.2.dev1/tests/integration/lite/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.2.2.dev1/tests/integration/lite/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1447 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/lite/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.153556 sdv-1.2.2.dev1/tests/integration/metadata/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/metadata/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      596 2023-05-10 21:10:34.000000 sdv-1.2.2.dev1/tests/integration/metadata/test_anonymization.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4369 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/metadata/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6200 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/metadata/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.153809 sdv-1.2.2.dev1/tests/integration/multi_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/multi_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    23356 2023-07-13 19:59:39.000000 sdv-1.2.2.dev1/tests/integration/multi_table/test_hma.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.154086 sdv-1.2.2.dev1/tests/integration/sequential/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/sequential/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6268 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/sequential/test_par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.155191 sdv-1.2.2.dev1/tests/integration/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/single_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1769 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/single_table/custom_constraints.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13998 2023-08-02 17:39:54.000000 sdv-1.2.2.dev1/tests/integration/single_table/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    24051 2023-08-02 17:39:54.000000 sdv-1.2.2.dev1/tests/integration/single_table/test_constraints.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12402 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/tests/integration/single_table/test_copulas.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2528 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/integration/single_table/test_ctgan.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.155366 sdv-1.2.2.dev1/tests/readme_test/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13973 2022-08-16 22:57:14.000000 sdv-1.2.2.dev1/tests/readme_test/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.156070 sdv-1.2.2.dev1/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/tests/unit/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.156845 sdv-1.2.2.dev1/tests/unit/constraints/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/tests/unit/constraints/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    32384 2023-04-20 22:38:57.000000 sdv-1.2.2.dev1/tests/unit/constraints/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   162819 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/tests/unit/constraints/test_tabular.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6848 2023-07-13 19:59:39.000000 sdv-1.2.2.dev1/tests/unit/constraints/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.157793 sdv-1.2.2.dev1/tests/unit/data_processing/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/unit/data_processing/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    81548 2023-08-02 17:39:54.000000 sdv-1.2.2.dev1/tests/unit/data_processing/test_data_processor.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2765 2023-04-20 18:31:25.000000 sdv-1.2.2.dev1/tests/unit/data_processing/test_datetime_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14718 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/unit/data_processing/test_numerical_formatter.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      926 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/unit/data_processing/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.158287 sdv-1.2.2.dev1/tests/unit/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/unit/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9876 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/unit/datasets/test_demo.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2498 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/unit/datasets/test_local.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.158621 sdv-1.2.2.dev1/tests/unit/evaluation/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2865 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/unit/evaluation/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2533 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/unit/evaluation/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.158947 sdv-1.2.2.dev1/tests/unit/lite/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/tests/unit/lite/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10135 2023-05-10 21:10:34.000000 sdv-1.2.2.dev1/tests/unit/lite/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.159826 sdv-1.2.2.dev1/tests/unit/metadata/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/tests/unit/metadata/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5258 2023-05-10 21:10:34.000000 sdv-1.2.2.dev1/tests/unit/metadata/test_anonymization.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22557 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/unit/metadata/test_metadata_upgrader.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    75538 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/tests/unit/metadata/test_multi_table.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    66306 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/tests/unit/metadata/test_single_table.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.160382 sdv-1.2.2.dev1/tests/unit/multi_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/unit/multi_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    42043 2023-08-02 17:39:54.000000 sdv-1.2.2.dev1/tests/unit/multi_table/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19731 2023-07-13 19:59:39.000000 sdv-1.2.2.dev1/tests/unit/multi_table/test_hma.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.161022 sdv-1.2.2.dev1/tests/unit/sampling/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2022-07-22 02:55:50.000000 sdv-1.2.2.dev1/tests/unit/sampling/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13827 2023-07-13 19:59:39.000000 sdv-1.2.2.dev1/tests/unit/sampling/test_hierarchical_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11155 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/tests/unit/sampling/test_independent_sampler.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2140 2022-06-21 19:18:25.000000 sdv-1.2.2.dev1/tests/unit/sampling/test_tabular.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.161332 sdv-1.2.2.dev1/tests/unit/sequential/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       50 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/unit/sequential/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    29331 2023-05-10 21:10:34.000000 sdv-1.2.2.dev1/tests/unit/sequential/test_par.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 17:40:55.162564 sdv-1.2.2.dev1/tests/unit/single_table/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        0 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/unit/single_table/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    77568 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/tests/unit/single_table/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13803 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/tests/unit/single_table/test_copulagan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18091 2023-05-10 21:10:34.000000 sdv-1.2.2.dev1/tests/unit/single_table/test_copulas.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10328 2023-05-10 21:10:34.000000 sdv-1.2.2.dev1/tests/unit/single_table/test_ctgan.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8358 2023-03-28 20:22:54.000000 sdv-1.2.2.dev1/tests/unit/single_table/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4604 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5572 2023-06-07 20:46:09.000000 sdv-1.2.2.dev1/tests/unit/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3051 2023-05-10 21:10:34.000000 sdv-1.2.2.dev1/tests/utils.py
```

### Comparing `sdv-1.2.2.dev0/CONTRIBUTING.rst` & `sdv-1.2.2.dev1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/HISTORY.md` & `sdv-1.2.2.dev1/HISTORY.md`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/LICENSE` & `sdv-1.2.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/PKG-INFO` & `sdv-1.2.2.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdv
-Version: 1.2.2.dev0
+Version: 1.2.2.dev1
 Summary: Generate synthetic data for single table, multi table and sequential data
 Home-page: https://github.com/sdv-dev/SDV
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: sdv synthetic-data synhtetic-data-generation timeseries single-table multi-table
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sdv Version: 1.2.2.dev0 Summary: Generate synthetic
+Metadata-Version: 2.1 Name: sdv Version: 1.2.2.dev1 Summary: Generate synthetic
 data for single table, multi table and sequential data Home-page: https://
 github.com/sdv-dev/SDV Author: DataCebo, Inc. Author-email: info@sdv.dev
 License: BSL-1.1 Keywords: sdv synthetic-data synhtetic-data-generation
 timeseries single-table multi-table Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: Free for non-commercial use Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `sdv-1.2.2.dev0/README.md` & `sdv-1.2.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/Makefile` & `sdv-1.2.2.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst` & `sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Constraint.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst` & `sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.CustomConstraint.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst` & `sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.FixedCombinations.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst` & `sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Inequality.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Negative.rst` & `sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Negative.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst` & `sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.OneHotEncoding.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Positive.rst` & `sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Positive.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst` & `sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarInequality.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst` & `sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.ScalarRange.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/constraints/api/sdv.constraints.Unique.rst` & `sdv-1.2.2.dev1/docs/api_reference/constraints/api/sdv.constraints.Unique.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/constraints/tabular.rst` & `sdv-1.2.2.dev1/docs/api_reference/constraints/tabular.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst` & `sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.dataset.Metadata.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst` & `sdv-1.2.2.dev1/docs/api_reference/metadata/api/sdv.metadata.table.Table.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metadata/dataset.rst` & `sdv-1.2.2.dev1/docs/api_reference/metadata/dataset.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metadata/table.rst` & `sdv-1.2.2.dev1/docs/api_reference/metadata/table.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.BNLogLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.DetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSComplement.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.KSTest.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.LogisticParentChildDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiSingleTableMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.MultiTableMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.ParentChildDetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.relational.SVCParentChildDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BNLogLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryAdaBoostClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryDecisionTreeClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryLogisticRegression.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.BinaryMLPClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CSTest.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalCAP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalEnsemble.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalGeneralizedCAP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalKNN.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalNB.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalPrivacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalRF.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalSVM.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.CategoricalZeroCAP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ContinuousKLDivergence.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.DiscreteKLDivergence.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.GMLogLikelihood.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSComplement.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.KSTest.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LinearRegression.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.LogisticDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MLPRegressor.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiColumnPairsMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MultiSingleColumnMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassDecisionTreeClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.MulticlassMLPClassifier.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalLR.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalMLP.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalPrivacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalRadiusNearestNeighbor.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.NumericalSVR.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.RegressionEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SVCDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.ScikitLearnClassifierDetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.tabular.SingleTableMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMClassifierEfficacy.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.LSTMDetection.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesDetectionMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesEfficacyMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/api/sdv.metrics.timeseries.TimeSeriesMetric.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/relational.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/relational.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/tabular.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/tabular.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/metrics/timeseries.rst` & `sdv-1.2.2.dev1/docs/api_reference/metrics/timeseries.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst` & `sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulagan.CopulaGAN.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst` & `sdv-1.2.2.dev1/docs/api_reference/tabular/api/sdv.tabular.copulas.GaussianCopula.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/conf.py` & `sdv-1.2.2.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/developer_guides/contributing.rst` & `sdv-1.2.2.dev1/docs/developer_guides/contributing.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/developer_guides/overview.rst` & `sdv-1.2.2.dev1/docs/developer_guides/overview.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/developer_guides/sdv/constraints.rst` & `sdv-1.2.2.dev1/docs/developer_guides/sdv/constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/developer_guides/sdv/metadata.rst` & `sdv-1.2.2.dev1/docs/developer_guides/sdv/metadata.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/developer_guides/sdv/tabular.rst` & `sdv-1.2.2.dev1/docs/developer_guides/sdv/tabular.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/getting_started/install.rst` & `sdv-1.2.2.dev1/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/getting_started/quickstart.rst` & `sdv-1.2.2.dev1/docs/getting_started/quickstart.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/CTGAN-DataCebo.png` & `sdv-1.2.2.dev1/docs/images/CTGAN-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/Copulas-DataCebo.png` & `sdv-1.2.2.dev1/docs/images/Copulas-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/DataCebo-Blue.png` & `sdv-1.2.2.dev1/docs/images/DataCebo-Blue.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/DataCebo.png` & `sdv-1.2.2.dev1/docs/images/DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/DeepEcho-DataCebo.png` & `sdv-1.2.2.dev1/docs/images/DeepEcho-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/RDT-DataCebo.png` & `sdv-1.2.2.dev1/docs/images/RDT-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/Real-vs-Synthetic-Evaluation.png` & `sdv-1.2.2.dev1/docs/images/Real-vs-Synthetic-Evaluation.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/SDGym-DataCebo.png` & `sdv-1.2.2.dev1/docs/images/SDGym-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/SDMetrics-DataCebo.png` & `sdv-1.2.2.dev1/docs/images/SDMetrics-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/SDV-DataCebo.png` & `sdv-1.2.2.dev1/docs/images/SDV-DataCebo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/SDV-logo.png` & `sdv-1.2.2.dev1/docs/images/SDV-logo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/SDV.png` & `sdv-1.2.2.dev1/docs/images/SDV.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/Single-Table-Metadata-Example.png` & `sdv-1.2.2.dev1/docs/images/Single-Table-Metadata-Example.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/custom_constraint.png` & `sdv-1.2.2.dev1/docs/images/custom_constraint.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/datacebo-logo-dark-mode.png` & `sdv-1.2.2.dev1/docs/images/datacebo-logo-dark-mode.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/datacebo-logo.png` & `sdv-1.2.2.dev1/docs/images/datacebo-logo.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/google_colab.png` & `sdv-1.2.2.dev1/docs/images/google_colab.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/hma1_1.png` & `sdv-1.2.2.dev1/docs/images/hma1_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/metadata_1.png` & `sdv-1.2.2.dev1/docs/images/metadata_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/metadata_2.png` & `sdv-1.2.2.dev1/docs/images/metadata_2.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/mybinder.png` & `sdv-1.2.2.dev1/docs/images/mybinder.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/quickstart_1.png` & `sdv-1.2.2.dev1/docs/images/quickstart_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/rdt_main_tranformation.png` & `sdv-1.2.2.dev1/docs/images/rdt_main_tranformation.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/images/slack.png` & `sdv-1.2.2.dev1/docs/images/slack.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/index.rst` & `sdv-1.2.2.dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/make.bat` & `sdv-1.2.2.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/savefig/copulagan_experience_years_1.png` & `sdv-1.2.2.dev1/docs/savefig/copulagan_experience_years_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/savefig/copulagan_experience_years_2.png` & `sdv-1.2.2.dev1/docs/savefig/copulagan_experience_years_2.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/savefig/copulagan_experience_years_3.png` & `sdv-1.2.2.dev1/docs/savefig/copulagan_experience_years_3.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/savefig/experience_years_1.png` & `sdv-1.2.2.dev1/docs/savefig/experience_years_1.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/savefig/experience_years_2.png` & `sdv-1.2.2.dev1/docs/savefig/experience_years_2.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/savefig/experience_years_3.png` & `sdv-1.2.2.dev1/docs/savefig/experience_years_3.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/sdv_theme/static/slack-32.png` & `sdv-1.2.2.dev1/docs/sdv_theme/static/slack-32.png`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/benchmarking/datasets.rst` & `sdv-1.2.2.dev1/docs/user_guides/benchmarking/datasets.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/benchmarking/docker.rst` & `sdv-1.2.2.dev1/docs/user_guides/benchmarking/docker.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/benchmarking/index.rst` & `sdv-1.2.2.dev1/docs/user_guides/benchmarking/index.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/benchmarking/install.rst` & `sdv-1.2.2.dev1/docs/user_guides/benchmarking/install.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/benchmarking/run.rst` & `sdv-1.2.2.dev1/docs/user_guides/benchmarking/run.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/benchmarking/synthesizers.rst` & `sdv-1.2.2.dev1/docs/user_guides/benchmarking/synthesizers.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/evaluation/evaluation_framework.rst` & `sdv-1.2.2.dev1/docs/user_guides/evaluation/evaluation_framework.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/relational/constraints.rst` & `sdv-1.2.2.dev1/docs/user_guides/relational/constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/relational/hma1.rst` & `sdv-1.2.2.dev1/docs/user_guides/relational/hma1.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/relational/relational_metadata.rst` & `sdv-1.2.2.dev1/docs/user_guides/relational/relational_metadata.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/single_table/copulagan.rst` & `sdv-1.2.2.dev1/docs/user_guides/single_table/copulagan.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/single_table/ctgan.rst` & `sdv-1.2.2.dev1/docs/user_guides/single_table/ctgan.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/single_table/custom_constraints.rst` & `sdv-1.2.2.dev1/docs/user_guides/single_table/custom_constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/single_table/gaussian_copula.rst` & `sdv-1.2.2.dev1/docs/user_guides/single_table/gaussian_copula.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/single_table/handling_constraints.rst` & `sdv-1.2.2.dev1/docs/user_guides/single_table/handling_constraints.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/single_table/index.rst` & `sdv-1.2.2.dev1/docs/user_guides/single_table/index.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/single_table/tabular_preset.rst` & `sdv-1.2.2.dev1/docs/user_guides/single_table/tabular_preset.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/single_table/tvae.rst` & `sdv-1.2.2.dev1/docs/user_guides/single_table/tvae.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/docs/user_guides/timeseries/par.rst` & `sdv-1.2.2.dev1/docs/user_guides/timeseries/par.rst`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/__init__.py` & `sdv-1.2.2.dev1/sdv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # configure logging for the library with a null handler (nothing is printed by default). See
 # http://docs.python-guide.org/en/latest/writing/logging/
 
 """Top-level package for SDV."""
 
 __author__ = 'DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
-__version__ = '1.2.2.dev0'
+__version__ = '1.2.2.dev1'
 
 
 import sys
 import warnings
 from operator import attrgetter
 
 from pkg_resources import iter_entry_points
```

### Comparing `sdv-1.2.2.dev0/sdv/constraints/__init__.py` & `sdv-1.2.2.dev1/sdv/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/constraints/base.py` & `sdv-1.2.2.dev1/sdv/constraints/base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/constraints/errors.py` & `sdv-1.2.2.dev1/sdv/constraints/errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/constraints/tabular.py` & `sdv-1.2.2.dev1/sdv/constraints/tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/constraints/utils.py` & `sdv-1.2.2.dev1/sdv/constraints/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/data_processing/data_processor.py` & `sdv-1.2.2.dev1/sdv/data_processing/data_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -695,36 +695,43 @@
             if not data.empty:
                 reversed_data = self._hyper_transformer.reverse_transform_subset(
                     data[reversible_columns]
                 )
         except rdt.errors.NotFittedError:
             LOGGER.info(f'HyperTransformer has not been fitted for table {self.table_name}')
 
-        for constraint in reversed(self._constraints_to_reverse):
-            reversed_data = constraint.reverse_transform(reversed_data)
-
         num_rows = len(reversed_data)
         sampled_columns = list(reversed_data.columns)
         missing_columns = [
             column
             for column in self.metadata.columns.keys() - set(sampled_columns + self._keys)
             if self._hyper_transformer.field_transformers.get(column)
         ]
         if missing_columns and num_rows:
             anonymized_data = self._hyper_transformer.create_anonymized_columns(
                 num_rows=num_rows,
                 column_names=missing_columns
             )
             sampled_columns.extend(missing_columns)
+            reversed_data[anonymized_data.columns] = anonymized_data[anonymized_data.notna()]
 
         if self._keys and num_rows:
             generated_keys = self.generate_keys(num_rows, reset_keys)
             sampled_columns.extend(self._keys)
+            reversed_data[generated_keys.columns] = generated_keys[generated_keys.notna()]
+
+        for constraint in reversed(self._constraints_to_reverse):
+            reversed_data = constraint.reverse_transform(reversed_data)
+
+        # Add new columns generated by the constraint
+        new_columns = list(set(reversed_data.columns) - set(sampled_columns))
+        sampled_columns.extend(new_columns)
 
-        # Sort the sampled columns in the order of the metadata
+        # Sort the sampled columns in the order of the metadata.
+        # Any extra columns not present in the metadata will be dropped.
         # In multitable there may be missing columns in the sample such as foreign keys
         # And alternate keys. Thats the reason of ensuring that the metadata column is within
         # The sampled columns.
         sampled_columns = [
             column for column in self.metadata.columns.keys()
             if column in sampled_columns
         ]
```

### Comparing `sdv-1.2.2.dev0/sdv/data_processing/datetime_formatter.py` & `sdv-1.2.2.dev1/sdv/data_processing/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/data_processing/errors.py` & `sdv-1.2.2.dev1/sdv/data_processing/errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/data_processing/numerical_formatter.py` & `sdv-1.2.2.dev1/sdv/data_processing/numerical_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/data_processing/utils.py` & `sdv-1.2.2.dev1/sdv/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/datasets/demo.py` & `sdv-1.2.2.dev1/sdv/datasets/demo.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/datasets/local.py` & `sdv-1.2.2.dev1/sdv/datasets/local.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/errors.py` & `sdv-1.2.2.dev1/sdv/errors.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/evaluation/multi_table.py` & `sdv-1.2.2.dev1/sdv/evaluation/multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/evaluation/single_table.py` & `sdv-1.2.2.dev1/sdv/evaluation/single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/lite/single_table.py` & `sdv-1.2.2.dev1/sdv/lite/single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/metadata/anonymization.py` & `sdv-1.2.2.dev1/sdv/metadata/anonymization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/metadata/metadata_upgrader.py` & `sdv-1.2.2.dev1/sdv/metadata/metadata_upgrader.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/metadata/multi_table.py` & `sdv-1.2.2.dev1/sdv/metadata/multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/metadata/single_table.py` & `sdv-1.2.2.dev1/sdv/metadata/single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/metadata/utils.py` & `sdv-1.2.2.dev1/sdv/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/metadata/visualization.py` & `sdv-1.2.2.dev1/sdv/metadata/visualization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/multi_table/base.py` & `sdv-1.2.2.dev1/sdv/multi_table/base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/multi_table/hma.py` & `sdv-1.2.2.dev1/sdv/multi_table/hma.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/sampling/hierarchical_sampler.py` & `sdv-1.2.2.dev1/sdv/sampling/hierarchical_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/sampling/independent_sampler.py` & `sdv-1.2.2.dev1/sdv/sampling/independent_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/sampling/tabular.py` & `sdv-1.2.2.dev1/sdv/sampling/tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/sequential/par.py` & `sdv-1.2.2.dev1/sdv/sequential/par.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/single_table/base.py` & `sdv-1.2.2.dev1/sdv/single_table/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,15 +464,17 @@
     def fit_processed_data(self, processed_data):
         """Fit this model to the transformed data.
 
         Args:
             processed_data (pandas.DataFrame):
                 The transformed data used to fit the model to.
         """
-        self._fit(processed_data)
+        if not processed_data.empty:
+            self._fit(processed_data)
+
         self._fitted = True
         self._fitted_date = datetime.datetime.today().strftime('%Y-%m-%d')
         self._fitted_sdv_version = pkg_resources.get_distribution('sdv').version
 
     def fit(self, data):
         """Fit this model to the original data.
```

### Comparing `sdv-1.2.2.dev0/sdv/single_table/copulagan.py` & `sdv-1.2.2.dev1/sdv/single_table/copulagan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/single_table/copulas.py` & `sdv-1.2.2.dev1/sdv/single_table/copulas.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/single_table/ctgan.py` & `sdv-1.2.2.dev1/sdv/single_table/ctgan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/single_table/utils.py` & `sdv-1.2.2.dev1/sdv/single_table/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv/utils.py` & `sdv-1.2.2.dev1/sdv/utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/sdv.egg-info/PKG-INFO` & `sdv-1.2.2.dev1/sdv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdv
-Version: 1.2.2.dev0
+Version: 1.2.2.dev1
 Summary: Generate synthetic data for single table, multi table and sequential data
 Home-page: https://github.com/sdv-dev/SDV
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: sdv synthetic-data synhtetic-data-generation timeseries single-table multi-table
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sdv Version: 1.2.2.dev0 Summary: Generate synthetic
+Metadata-Version: 2.1 Name: sdv Version: 1.2.2.dev1 Summary: Generate synthetic
 data for single table, multi table and sequential data Home-page: https://
 github.com/sdv-dev/SDV Author: DataCebo, Inc. Author-email: info@sdv.dev
 License: BSL-1.1 Keywords: sdv synthetic-data synhtetic-data-generation
 timeseries single-table multi-table Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: Free for non-commercial use Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `sdv-1.2.2.dev0/sdv.egg-info/SOURCES.txt` & `sdv-1.2.2.dev1/sdv.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -541,14 +541,15 @@
 tests/integration/multi_table/__init__.py
 tests/integration/multi_table/test_hma.py
 tests/integration/sequential/__init__.py
 tests/integration/sequential/test_par.py
 tests/integration/single_table/__init__.py
 tests/integration/single_table/custom_constraints.py
 tests/integration/single_table/test_base.py
+tests/integration/single_table/test_constraints.py
 tests/integration/single_table/test_copulas.py
 tests/integration/single_table/test_ctgan.py
 tests/readme_test/README.md
 tests/unit/__init__.py
 tests/unit/test___init__.py
 tests/unit/test_utils.py
 tests/unit/constraints/__init__.py
```

### Comparing `sdv-1.2.2.dev0/sdv.egg-info/requires.txt` & `sdv-1.2.2.dev1/sdv.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/setup.cfg` & `sdv-1.2.2.dev1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.2.dev0
+current_version = 1.2.2.dev1
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `sdv-1.2.2.dev0/setup.py` & `sdv-1.2.2.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,10 +131,10 @@
     name='sdv',
     packages=find_packages(include=['sdv', 'sdv.*']),
     python_requires='>=3.8,<3.11',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/SDV',
-    version='1.2.2.dev0',
+    version='1.2.2.dev1',
     zip_safe=False,
 )
```

### Comparing `sdv-1.2.2.dev0/tests/integration/data_processing/test_data_processor.py` & `sdv-1.2.2.dev1/tests/integration/data_processing/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/integration/dataset.py` & `sdv-1.2.2.dev1/tests/integration/dataset.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/integration/datasets/test_demo.py` & `sdv-1.2.2.dev1/tests/integration/datasets/test_demo.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/integration/evaluation/test_multi_table.py` & `sdv-1.2.2.dev1/tests/integration/evaluation/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/integration/evaluation/test_single_table.py` & `sdv-1.2.2.dev1/tests/integration/evaluation/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/integration/lite/test_single_table.py` & `sdv-1.2.2.dev1/tests/integration/lite/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/integration/metadata/test_anonymization.py` & `sdv-1.2.2.dev1/tests/integration/metadata/test_anonymization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/integration/metadata/test_multi_table.py` & `sdv-1.2.2.dev1/tests/integration/metadata/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/integration/metadata/test_single_table.py` & `sdv-1.2.2.dev1/tests/integration/metadata/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/integration/multi_table/test_hma.py` & `sdv-1.2.2.dev1/tests/integration/multi_table/test_hma.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/integration/sequential/test_par.py` & `sdv-1.2.2.dev1/tests/integration/sequential/test_par.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/integration/single_table/custom_constraints.py` & `sdv-1.2.2.dev1/tests/integration/single_table/custom_constraints.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/integration/single_table/test_copulas.py` & `sdv-1.2.2.dev1/tests/integration/single_table/test_copulas.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/integration/single_table/test_ctgan.py` & `sdv-1.2.2.dev1/tests/integration/single_table/test_ctgan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/readme_test/README.md` & `sdv-1.2.2.dev1/tests/readme_test/README.md`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/constraints/test_base.py` & `sdv-1.2.2.dev1/tests/unit/constraints/test_base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/constraints/test_tabular.py` & `sdv-1.2.2.dev1/tests/unit/constraints/test_tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/constraints/test_utils.py` & `sdv-1.2.2.dev1/tests/unit/constraints/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/data_processing/test_data_processor.py` & `sdv-1.2.2.dev1/tests/unit/data_processing/test_data_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from sdv.data_processing.data_processor import DataProcessor
 from sdv.data_processing.datetime_formatter import DatetimeFormatter
 from sdv.data_processing.errors import InvalidConstraintsError, NotFittedError
 from sdv.data_processing.numerical_formatter import NumericalFormatter
 from sdv.errors import SynthesizerInputError
 from sdv.metadata.single_table import SingleTableMetadata
 from sdv.single_table.base import BaseSynthesizer
+from tests.utils import DataFrameMatcher
 
 
 class TestDataProcessor:
 
     def test__update_numerical_transformer(self):
         """Test the ``_update_numerical_transformer`` method.
 
@@ -1842,54 +1843,68 @@
             - The reverse transformed data.
         """
         # Setup
         constraint_mock = Mock()
         dp = DataProcessor(SingleTableMetadata())
         dp.fitted = True
         dp.metadata = Mock()
-        dp.metadata.columns = {'a': None, 'b': None, 'c': None, 'd': None}
+        dp.metadata.columns = {'a': None, 'b': None, 'c': None, 'key': None, 'd': None}
         data = pd.DataFrame({
             'a': [1, 2, 3],
             'b': [True, True, False],
             'c': ['d', 'e', 'f'],
+
         })
+        dp._keys = ['key']
         dp._hyper_transformer = Mock()
-        dp._hyper_transformer.create_anonymized_columns.return_value = pd.DataFrame({
-            'd': ['a@gmail.com', 'b@gmail.com', 'c@gmail.com']
-        })
+        dp._hyper_transformer.create_anonymized_columns.side_effect = [
+            pd.DataFrame({'d': ['a@gmail.com', 'b@gmail.com', 'c@gmail.com']}),
+            pd.DataFrame({'key': ['sdv_0', 'sdv_1', 'sdv_2']})
+        ]
         dp._constraints_to_reverse = [constraint_mock]
-        dp._hyper_transformer.reverse_transform_subset.return_value = data
+        dp._hyper_transformer.reverse_transform_subset.return_value = data.copy()
         dp._hyper_transformer._output_columns = ['a', 'b', 'c']
         dp._dtypes = pd.Series(
-            [np.float64, np.bool_, np.object_, np.object_], index=['a', 'b', 'c', 'd'])
+            [np.float64, np.bool_, np.object_, np.object_, np.object_],
+            index=['a', 'b', 'c', 'd', 'key']
+        )
         constraint_mock.reverse_transform.return_value = data
 
         # Run
         reverse_transformed = dp.reverse_transform(data)
 
         # Assert
         input_data = pd.DataFrame({
             'a': [1, 2, 3],
             'b': [True, True, False],
             'c': ['d', 'e', 'f']
         })
-        constraint_mock.reverse_transform.assert_called_once_with(data)
+        expected_constraint_input = pd.DataFrame({
+            'a': [1, 2, 3],
+            'b': [True, True, False],
+            'c': ['d', 'e', 'f'],
+            'd': ['a@gmail.com', 'b@gmail.com', 'c@gmail.com'],
+            'key': ['sdv_0', 'sdv_1', 'sdv_2']
+        })
+        constraint_mock.reverse_transform.assert_called_once_with(
+            DataFrameMatcher(expected_constraint_input))
         data_from_call = dp._hyper_transformer.reverse_transform_subset.mock_calls[0][1][0]
         pd.testing.assert_frame_equal(input_data, data_from_call)
         dp._hyper_transformer.reverse_transform_subset.assert_called_once()
+        dp._hyper_transformer.create_anonymized_columns.has_calls(
+            call(num_rows=3, column_names=['d']),
+            call(num_rows=3, column_names=['key'])
+        )
         expected_output = pd.DataFrame({
             'a': [1., 2., 3.],
             'b': [True, True, False],
             'c': ['d', 'e', 'f'],
-            'd': ['a@gmail.com', 'b@gmail.com', 'c@gmail.com']
+            'key': ['sdv_0', 'sdv_1', 'sdv_2'],
+            'd': ['a@gmail.com', 'b@gmail.com', 'c@gmail.com'],
         })
-        dp._hyper_transformer.create_anonymized_columns.assert_called_once_with(
-            num_rows=3,
-            column_names=['d']
-        )
         pd.testing.assert_frame_equal(reverse_transformed, expected_output)
 
     @patch('sdv.data_processing.data_processor.LOGGER')
     def test_reverse_transform_hyper_transformer_errors(self, log_mock):
         """Test the ``reverse_transform`` method.
 
         A message should be logged if the ``HyperTransformer`` errors.
```

### Comparing `sdv-1.2.2.dev0/tests/unit/data_processing/test_datetime_formatter.py` & `sdv-1.2.2.dev1/tests/unit/data_processing/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/data_processing/test_numerical_formatter.py` & `sdv-1.2.2.dev1/tests/unit/data_processing/test_numerical_formatter.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/data_processing/test_utils.py` & `sdv-1.2.2.dev1/tests/unit/data_processing/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/datasets/test_demo.py` & `sdv-1.2.2.dev1/tests/unit/datasets/test_demo.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/datasets/test_local.py` & `sdv-1.2.2.dev1/tests/unit/datasets/test_local.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/evaluation/test_multi_table.py` & `sdv-1.2.2.dev1/tests/unit/evaluation/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/evaluation/test_single_table.py` & `sdv-1.2.2.dev1/tests/unit/evaluation/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/lite/test_single_table.py` & `sdv-1.2.2.dev1/tests/unit/lite/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/metadata/test_anonymization.py` & `sdv-1.2.2.dev1/tests/unit/metadata/test_anonymization.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/metadata/test_metadata_upgrader.py` & `sdv-1.2.2.dev1/tests/unit/metadata/test_metadata_upgrader.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/metadata/test_multi_table.py` & `sdv-1.2.2.dev1/tests/unit/metadata/test_multi_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/metadata/test_single_table.py` & `sdv-1.2.2.dev1/tests/unit/metadata/test_single_table.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/multi_table/test_base.py` & `sdv-1.2.2.dev1/tests/unit/multi_table/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -714,14 +714,29 @@
         BaseMultiTableSynthesizer.fit_processed_data(instance, data)
 
         # Assert
         instance._augment_tables.assert_called_once_with(data)
         instance._model_tables.assert_called_once_with(instance._augment_tables.return_value)
         assert instance._fitted
 
+    def test_fit_processed_data_empty_table(self):
+        """Test attributes are properly set when data is empty and that _fit is not called."""
+        # Setup
+        instance = Mock()
+        data = pd.DataFrame()
+
+        # Run
+        BaseMultiTableSynthesizer.fit_processed_data(instance, data)
+
+        # Assert
+        instance._fit.assert_not_called()
+        assert instance._fitted
+        assert instance._fitted_date
+        assert instance._fitted_sdv_version
+
     def test_fit(self):
         """Test that ``fit`` calls ``preprocess`` and then ``fit_processed_data``."""
         # Setup
         instance = Mock()
         data = Mock()
 
         # Run
```

### Comparing `sdv-1.2.2.dev0/tests/unit/multi_table/test_hma.py` & `sdv-1.2.2.dev1/tests/unit/multi_table/test_hma.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/sampling/test_hierarchical_sampler.py` & `sdv-1.2.2.dev1/tests/unit/sampling/test_hierarchical_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/sampling/test_independent_sampler.py` & `sdv-1.2.2.dev1/tests/unit/sampling/test_independent_sampler.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/sampling/test_tabular.py` & `sdv-1.2.2.dev1/tests/unit/sampling/test_tabular.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/sequential/test_par.py` & `sdv-1.2.2.dev1/tests/unit/sequential/test_par.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/single_table/test_base.py` & `sdv-1.2.2.dev1/tests/unit/single_table/test_base.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/single_table/test_copulagan.py` & `sdv-1.2.2.dev1/tests/unit/single_table/test_copulagan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/single_table/test_copulas.py` & `sdv-1.2.2.dev1/tests/unit/single_table/test_copulas.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/single_table/test_ctgan.py` & `sdv-1.2.2.dev1/tests/unit/single_table/test_ctgan.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/single_table/test_utils.py` & `sdv-1.2.2.dev1/tests/unit/single_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/test___init__.py` & `sdv-1.2.2.dev1/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/unit/test_utils.py` & `sdv-1.2.2.dev1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `sdv-1.2.2.dev0/tests/utils.py` & `sdv-1.2.2.dev1/tests/utils.py`

 * *Files identical despite different names*

