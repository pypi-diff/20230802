# Comparing `tmp/botorch-0.8.5.tar.gz` & `tmp/botorch-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botorch-0.8.5.tar", last modified: Mon May  8 17:50:32 2023, max compression
+gzip compressed data, was "botorch-0.9.1.tar", last modified: Wed Aug  2 01:34:20 2023, max compression
```

## Comparing `botorch-0.8.5.tar` & `botorch-0.9.1.tar`

### file list

```diff
@@ -1,238 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.704423 botorch-0.8.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.636422 botorch-0.8.5/.conda/
--rwxr-xr-x   0 runner    (1001) docker     (123)      436 2023-05-08 17:48:07.000000 botorch-0.8.5/.conda/build_conda.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-08 17:48:07.000000 botorch-0.8.5/.conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.636422 botorch-0.8.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.636422 botorch-0.8.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.640423 botorch-0.8.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/deploy_on_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/nightly.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/reusable_tutorials.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/reusable_website.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/test_stable.yml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/tutorials_smoke_test_on_pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-08 17:48:07.000000 botorch-0.8.5/.github/workflows/tutorials_smoke_test_on_push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-08 17:48:07.000000 botorch-0.8.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    50315 2023-05-08 17:48:07.000000 botorch-0.8.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-08 17:48:07.000000 botorch-0.8.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-08 17:48:07.000000 botorch-0.8.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-08 17:48:07.000000 botorch-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-08 17:48:07.000000 botorch-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-08 17:50:32.704423 botorch-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-05-08 17:48:07.000000 botorch-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.644423 botorch-0.8.5/botorch/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.648423 botorch-0.8.5/botorch/acquisition/
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/active_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)    47072 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/cached_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/cost_aware.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/fixed_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    45389 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/input_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/joint_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    26678 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/knowledge_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    42642 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/max_value_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    23047 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/monte_carlo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.652423 botorch-0.8.5/botorch/acquisition/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)    31296 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/joint_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15949 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/max_value_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    33366 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/monte_carlo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)    35301 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/multi_output_risk_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    48822 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/predictive_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_objective/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/multi_step_lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)    23534 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/penalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/predictive_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/preference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/proximal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13908 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/risk_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    20846 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/acquisition/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/cross_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.652423 botorch-0.8.5/botorch/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/exceptions/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/exceptions/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.652423 botorch-0.8.5/botorch/generation/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/generation/gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    15203 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/generation/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/generation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.660423 botorch-0.8.5/botorch/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/approximate_gp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/contextual_multioutput.py
--rw-r--r--   0 runner    (1001) docker     (123)    17742 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)    15141 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/fully_bayesian_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    20346 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    15061 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/gp_regression_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/gp_regression_mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)    35032 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/gpytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24436 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/higher_order_gp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.664423 botorch-0.8.5/botorch/models/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/contextual_lcea.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/contextual_sac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/downsampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/exponential_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/kernels/linear_truncated_fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.664423 botorch-0.8.5/botorch/models/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/likelihoods/pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21037 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/model_list_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    33200 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    46993 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/pairwise_gp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.668423 botorch-0.8.5/botorch/models/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/transforms/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    63408 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/transforms/input.py
--rw-r--r--   0 runner    (1001) docker     (123)    30293 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/transforms/outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/transforms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.668423 botorch-0.8.5/botorch/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/utils/assorted.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/utils/inducing_point_allocators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/models/utils/parse_training_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.672423 botorch-0.8.5/botorch/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.676423 botorch-0.8.5/botorch/optim/closures/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/closures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/closures/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/closures/model_closures.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    42398 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/numpy_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)    56043 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18385 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/parameter_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/stopping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.676423 botorch-0.8.5/botorch/optim/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/utils/acquisition_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/optim/utils/timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.680423 botorch-0.8.5/botorch/posteriors/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/base_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/gpytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/higher_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/posterior_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/posteriors/transformed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.684423 botorch-0.8.5/botorch/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/get_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/index_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/list_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pairwise_samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.688423 botorch-0.8.5/botorch/sampling/pathwise/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.688423 botorch-0.8.5/botorch/sampling/pathwise/features/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/features/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/features/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/posterior_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/prior_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/update_strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/pathwise/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/qmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/sampling/stochastic_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.692423 botorch-0.8.5/botorch/test_functions/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)    48773 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/multi_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/multi_objective_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/sensitivity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    24915 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/test_functions/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.700423 botorch-0.8.5/botorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/feasible_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    20040 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/gp_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/low_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.700423 botorch-0.8.5/botorch/utils/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.704423 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/box_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/dominated.py
--rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/non_dominated.py
--rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/hypervolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/pareto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/multi_objective/scalarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/objective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.704423 botorch-0.8.5/botorch/utils/probability/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/bvn.py
--rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/lin_ess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/mvnxpb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/truncated_multivariate_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/unified_skew_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/probability/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/rounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/safe_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    36647 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    14905 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 17:50:32.000000 botorch-0.8.5/botorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.644423 botorch-0.8.5/botorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-08 17:50:32.000000 botorch-0.8.5/botorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-05-08 17:50:32.000000 botorch-0.8.5/botorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:50:32.000000 botorch-0.8.5/botorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-08 17:50:32.000000 botorch-0.8.5/botorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 17:50:32.000000 botorch-0.8.5/botorch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    79395 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch_logo_lockup.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    63261 2023-05-08 17:48:07.000000 botorch-0.8.5/botorch_logo_lockup.svg
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 17:48:07.000000 botorch-0.8.5/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:50:32.704423 botorch-0.8.5/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    15796 2023-05-08 17:48:07.000000 botorch-0.8.5/notebooks/tutorials_performance_tracking.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-08 17:48:07.000000 botorch-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-08 17:48:07.000000 botorch-0.8.5/requirements-fmt.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-08 17:48:07.000000 botorch-0.8.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-08 17:50:32.704423 botorch-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-08 17:48:07.000000 botorch-0.8.5/setup.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.089427 botorch-0.9.1/
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:19.992789 botorch-0.9.1/.conda/
+-rwxr-xr-x   0 balandat   (501) staff       (20)      436 2023-04-01 23:17:12.000000 botorch-0.9.1/.conda/build_conda.sh
+-rw-r--r--   0 balandat   (501) staff       (20)     1107 2023-08-01 22:52:12.000000 botorch-0.9.1/.conda/meta.yaml
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:19.994379 botorch-0.9.1/.github/
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:19.995560 botorch-0.9.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 balandat   (501) staff       (20)      874 2019-10-29 21:48:18.000000 botorch-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 balandat   (501) staff       (20)      951 2019-10-29 21:48:18.000000 botorch-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 balandat   (501) staff       (20)      519 2019-10-29 21:48:18.000000 botorch-0.9.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 balandat   (501) staff       (20)      877 2022-03-10 21:59:17.000000 botorch-0.9.1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.005488 botorch-0.9.1/.github/workflows/
+-rw-r--r--   0 balandat   (501) staff       (20)     3528 2023-08-01 14:24:19.000000 botorch-0.9.1/.github/workflows/deploy_on_release.yml
+-rw-r--r--   0 balandat   (501) staff       (20)     1030 2023-08-01 14:24:19.000000 botorch-0.9.1/.github/workflows/docs.yml
+-rw-r--r--   0 balandat   (501) staff       (20)      994 2023-08-01 14:24:19.000000 botorch-0.9.1/.github/workflows/lint.yml
+-rw-r--r--   0 balandat   (501) staff       (20)     4744 2023-08-01 14:24:19.000000 botorch-0.9.1/.github/workflows/nightly.yml
+-rw-r--r--   0 balandat   (501) staff       (20)     4289 2023-08-01 14:24:19.000000 botorch-0.9.1/.github/workflows/reusable_tutorials.yml
+-rw-r--r--   0 balandat   (501) staff       (20)     1926 2023-08-01 14:24:19.000000 botorch-0.9.1/.github/workflows/reusable_website.yml
+-rw-r--r--   0 balandat   (501) staff       (20)     2277 2023-08-01 14:24:19.000000 botorch-0.9.1/.github/workflows/test.yml
+-rw-r--r--   0 balandat   (501) staff       (20)     3837 2023-08-02 01:29:03.000000 botorch-0.9.1/.github/workflows/test_stable.yml
+-rw-r--r--   0 balandat   (501) staff       (20)      385 2023-04-01 23:17:12.000000 botorch-0.9.1/.github/workflows/tutorials_smoke_test_on_pr.yml
+-rw-r--r--   0 balandat   (501) staff       (20)      378 2023-04-01 23:17:12.000000 botorch-0.9.1/.github/workflows/tutorials_smoke_test_on_push.yml
+-rw-r--r--   0 balandat   (501) staff       (20)     1416 2021-12-04 18:00:52.000000 botorch-0.9.1/.gitignore
+-rw-r--r--   0 balandat   (501) staff       (20)    53112 2023-08-01 22:52:12.000000 botorch-0.9.1/CHANGELOG.md
+-rw-r--r--   0 balandat   (501) staff       (20)     3466 2022-03-10 21:59:17.000000 botorch-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 balandat   (501) staff       (20)     4324 2023-08-01 14:24:19.000000 botorch-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0 balandat   (501) staff       (20)     1088 2022-03-10 21:59:17.000000 botorch-0.9.1/LICENSE
+-rw-r--r--   0 balandat   (501) staff       (20)      179 2022-03-10 21:59:17.000000 botorch-0.9.1/MANIFEST.in
+-rw-r--r--   0 balandat   (501) staff       (20)     9967 2023-08-02 01:34:20.089547 botorch-0.9.1/PKG-INFO
+-rw-r--r--   0 balandat   (501) staff       (20)     9159 2023-08-01 22:52:12.000000 botorch-0.9.1/README.md
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.011153 botorch-0.9.1/botorch/
+-rw-r--r--   0 balandat   (501) staff       (20)     2057 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/__init__.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.031259 botorch-0.9.1/botorch/acquisition/
+-rw-r--r--   0 balandat   (501) staff       (20)     4104 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/acquisition/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5985 2023-07-03 14:23:54.000000 botorch-0.9.1/botorch/acquisition/acquisition.py
+-rw-r--r--   0 balandat   (501) staff       (20)     8122 2023-06-07 21:20:45.000000 botorch-0.9.1/botorch/acquisition/active_learning.py
+-rw-r--r--   0 balandat   (501) staff       (20)    46601 2023-06-07 21:20:45.000000 botorch-0.9.1/botorch/acquisition/analytic.py
+-rw-r--r--   0 balandat   (501) staff       (20)     7369 2023-05-03 15:06:10.000000 botorch-0.9.1/botorch/acquisition/cached_cholesky.py
+-rw-r--r--   0 balandat   (501) staff       (20)     8906 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/acquisition/cost_aware.py
+-rw-r--r--   0 balandat   (501) staff       (20)     6923 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/acquisition/decoupled.py
+-rw-r--r--   0 balandat   (501) staff       (20)     7984 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/acquisition/fixed_feature.py
+-rw-r--r--   0 balandat   (501) staff       (20)    54160 2023-08-01 22:52:12.000000 botorch-0.9.1/botorch/acquisition/input_constructors.py
+-rw-r--r--   0 balandat   (501) staff       (20)    15009 2023-06-07 21:20:45.000000 botorch-0.9.1/botorch/acquisition/joint_entropy_search.py
+-rw-r--r--   0 balandat   (501) staff       (20)    26255 2023-06-07 21:20:45.000000 botorch-0.9.1/botorch/acquisition/knowledge_gradient.py
+-rw-r--r--   0 balandat   (501) staff       (20)    22644 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/acquisition/logei.py
+-rw-r--r--   0 balandat   (501) staff       (20)    42642 2023-05-08 14:38:07.000000 botorch-0.9.1/botorch/acquisition/max_value_entropy_search.py
+-rw-r--r--   0 balandat   (501) staff       (20)    36283 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/acquisition/monte_carlo.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.035088 botorch-0.9.1/botorch/acquisition/multi_objective/
+-rw-r--r--   0 balandat   (501) staff       (20)     1719 2023-06-07 21:20:45.000000 botorch-0.9.1/botorch/acquisition/multi_objective/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)    10079 2023-06-07 21:20:45.000000 botorch-0.9.1/botorch/acquisition/multi_objective/analytic.py
+-rw-r--r--   0 balandat   (501) staff       (20)    31296 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/acquisition/multi_objective/joint_entropy_search.py
+-rw-r--r--   0 balandat   (501) staff       (20)    15949 2023-05-03 15:06:10.000000 botorch-0.9.1/botorch/acquisition/multi_objective/max_value_entropy_search.py
+-rw-r--r--   0 balandat   (501) staff       (20)    33579 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/acquisition/multi_objective/monte_carlo.py
+-rw-r--r--   0 balandat   (501) staff       (20)     6611 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/acquisition/multi_objective/multi_fidelity.py
+-rw-r--r--   0 balandat   (501) staff       (20)    35301 2023-05-03 15:06:10.000000 botorch-0.9.1/botorch/acquisition/multi_objective/multi_output_risk_measures.py
+-rw-r--r--   0 balandat   (501) staff       (20)    10923 2023-06-07 21:20:45.000000 botorch-0.9.1/botorch/acquisition/multi_objective/objective.py
+-rw-r--r--   0 balandat   (501) staff       (20)    48822 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/acquisition/multi_objective/predictive_entropy_search.py
+-rw-r--r--   0 balandat   (501) staff       (20)    15526 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/acquisition/multi_objective/utils.py
+-rw-r--r--   0 balandat   (501) staff       (20)    29304 2023-06-07 21:20:45.000000 botorch-0.9.1/botorch/acquisition/multi_step_lookahead.py
+-rw-r--r--   0 balandat   (501) staff       (20)    22827 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/acquisition/objective.py
+-rw-r--r--   0 balandat   (501) staff       (20)    14396 2023-07-15 04:59:07.000000 botorch-0.9.1/botorch/acquisition/penalized.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4235 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/acquisition/predictive_entropy_search.py
+-rw-r--r--   0 balandat   (501) staff       (20)     7676 2023-06-04 22:52:24.000000 botorch-0.9.1/botorch/acquisition/preference.py
+-rw-r--r--   0 balandat   (501) staff       (20)     3750 2023-07-11 21:08:20.000000 botorch-0.9.1/botorch/acquisition/prior_guided.py
+-rw-r--r--   0 balandat   (501) staff       (20)     8229 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/acquisition/proximal.py
+-rw-r--r--   0 balandat   (501) staff       (20)    13908 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/acquisition/risk_measures.py
+-rw-r--r--   0 balandat   (501) staff       (20)    27167 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/acquisition/utils.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5925 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/cross_validation.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.036377 botorch-0.9.1/botorch/exceptions/
+-rw-r--r--   0 balandat   (501) staff       (20)     1076 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/exceptions/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)     1603 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/exceptions/errors.py
+-rw-r--r--   0 balandat   (501) staff       (20)     1180 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/exceptions/warnings.py
+-rw-r--r--   0 balandat   (501) staff       (20)    16563 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/fit.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.037927 botorch-0.9.1/botorch/generation/
+-rw-r--r--   0 balandat   (501) staff       (20)      552 2022-03-10 21:59:17.000000 botorch-0.9.1/botorch/generation/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)    20101 2023-07-09 15:09:08.000000 botorch-0.9.1/botorch/generation/gen.py
+-rw-r--r--   0 balandat   (501) staff       (20)    14479 2023-06-07 21:20:45.000000 botorch-0.9.1/botorch/generation/sampling.py
+-rw-r--r--   0 balandat   (501) staff       (20)     6660 2023-07-09 15:09:08.000000 botorch-0.9.1/botorch/generation/utils.py
+-rw-r--r--   0 balandat   (501) staff       (20)     1170 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/logging.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.044806 botorch-0.9.1/botorch/models/
+-rw-r--r--   0 balandat   (501) staff       (20)     1867 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)    19333 2023-07-03 14:23:54.000000 botorch-0.9.1/botorch/models/approximate_gp.py
+-rw-r--r--   0 balandat   (501) staff       (20)     3693 2023-07-09 15:09:08.000000 botorch-0.9.1/botorch/models/contextual.py
+-rw-r--r--   0 balandat   (501) staff       (20)     8035 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/contextual_multioutput.py
+-rw-r--r--   0 balandat   (501) staff       (20)    17742 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/converter.py
+-rw-r--r--   0 balandat   (501) staff       (20)     3157 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/cost.py
+-rw-r--r--   0 balandat   (501) staff       (20)     7548 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/deterministic.py
+-rw-r--r--   0 balandat   (501) staff       (20)     3374 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/ensemble.py
+-rw-r--r--   0 balandat   (501) staff       (20)    22032 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/models/fully_bayesian.py
+-rw-r--r--   0 balandat   (501) staff       (20)    18188 2023-06-07 21:20:45.000000 botorch-0.9.1/botorch/models/fully_bayesian_multitask.py
+-rw-r--r--   0 balandat   (501) staff       (20)    19499 2023-07-03 14:23:54.000000 botorch-0.9.1/botorch/models/gp_regression.py
+-rw-r--r--   0 balandat   (501) staff       (20)    15061 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/gp_regression_fidelity.py
+-rw-r--r--   0 balandat   (501) staff       (20)     8431 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/gp_regression_mixed.py
+-rw-r--r--   0 balandat   (501) staff       (20)    34654 2023-06-07 21:20:45.000000 botorch-0.9.1/botorch/models/gpytorch.py
+-rw-r--r--   0 balandat   (501) staff       (20)    24087 2023-07-03 14:23:54.000000 botorch-0.9.1/botorch/models/higher_order_gp.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.047970 botorch-0.9.1/botorch/models/kernels/
+-rw-r--r--   0 balandat   (501) staff       (20)      645 2022-03-10 21:59:17.000000 botorch-0.9.1/botorch/models/kernels/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)     1198 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/kernels/categorical.py
+-rw-r--r--   0 balandat   (501) staff       (20)    17647 2023-07-09 15:09:08.000000 botorch-0.9.1/botorch/models/kernels/contextual_lcea.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4275 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/kernels/contextual_sac.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4251 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/kernels/downsampling.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4247 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/kernels/exponential_decay.py
+-rw-r--r--   0 balandat   (501) staff       (20)    10226 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/kernels/linear_truncated_fidelity.py
+-rw-r--r--   0 balandat   (501) staff       (20)    12106 2023-06-08 01:49:29.000000 botorch-0.9.1/botorch/models/kernels/orthogonal_additive_kernel.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.048789 botorch-0.9.1/botorch/models/likelihoods/
+-rw-r--r--   0 balandat   (501) staff       (20)      393 2022-06-10 04:39:40.000000 botorch-0.9.1/botorch/models/likelihoods/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)     9127 2023-07-09 15:09:08.000000 botorch-0.9.1/botorch/models/likelihoods/pairwise.py
+-rw-r--r--   0 balandat   (501) staff       (20)    25250 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/models/model.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5686 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/model_list_gp_regression.py
+-rw-r--r--   0 balandat   (501) staff       (20)    34117 2023-07-03 14:23:54.000000 botorch-0.9.1/botorch/models/multitask.py
+-rw-r--r--   0 balandat   (501) staff       (20)    47232 2023-07-09 15:09:08.000000 botorch-0.9.1/botorch/models/pairwise_gp.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.051198 botorch-0.9.1/botorch/models/transforms/
+-rw-r--r--   0 balandat   (501) staff       (20)      726 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/transforms/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4660 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/transforms/factory.py
+-rw-r--r--   0 balandat   (501) staff       (20)    63902 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/models/transforms/input.py
+-rw-r--r--   0 balandat   (501) staff       (20)    31087 2023-07-03 14:23:54.000000 botorch-0.9.1/botorch/models/transforms/outcome.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4421 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/transforms/utils.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.052869 botorch-0.9.1/botorch/models/utils/
+-rw-r--r--   0 balandat   (501) staff       (20)     1038 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/utils/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)    13894 2023-07-09 15:09:08.000000 botorch-0.9.1/botorch/models/utils/assorted.py
+-rw-r--r--   0 balandat   (501) staff       (20)     1936 2023-07-03 14:23:54.000000 botorch-0.9.1/botorch/models/utils/gpytorch_modules.py
+-rw-r--r--   0 balandat   (501) staff       (20)    12753 2023-07-03 14:23:54.000000 botorch-0.9.1/botorch/models/utils/inducing_point_allocators.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4572 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/models/utils/parse_training_data.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.056345 botorch-0.9.1/botorch/optim/
+-rw-r--r--   0 balandat   (501) staff       (20)     1803 2023-07-09 15:09:08.000000 botorch-0.9.1/botorch/optim/__init__.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.057352 botorch-0.9.1/botorch/optim/closures/
+-rw-r--r--   0 balandat   (501) staff       (20)      555 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/optim/closures/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)     7789 2023-06-07 21:20:19.000000 botorch-0.9.1/botorch/optim/closures/core.py
+-rw-r--r--   0 balandat   (501) staff       (20)     7375 2023-06-07 21:20:19.000000 botorch-0.9.1/botorch/optim/closures/model_closures.py
+-rw-r--r--   0 balandat   (501) staff       (20)     9132 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/optim/core.py
+-rw-r--r--   0 balandat   (501) staff       (20)    15498 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/optim/fit.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5800 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/optim/homotopy.py
+-rw-r--r--   0 balandat   (501) staff       (20)    42398 2023-06-07 21:20:45.000000 botorch-0.9.1/botorch/optim/initializers.py
+-rw-r--r--   0 balandat   (501) staff       (20)     7365 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/optim/numpy_converter.py
+-rw-r--r--   0 balandat   (501) staff       (20)    56151 2023-07-11 21:08:20.000000 botorch-0.9.1/botorch/optim/optimize.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5718 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/optim/optimize_homotopy.py
+-rw-r--r--   0 balandat   (501) staff       (20)    19687 2023-07-09 15:09:08.000000 botorch-0.9.1/botorch/optim/parameter_constraints.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4405 2023-07-03 14:23:54.000000 botorch-0.9.1/botorch/optim/stopping.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.059422 botorch-0.9.1/botorch/optim/utils/
+-rw-r--r--   0 balandat   (501) staff       (20)     1344 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/optim/utils/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5144 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/optim/utils/acquisition_utils.py
+-rw-r--r--   0 balandat   (501) staff       (20)     2954 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/optim/utils/common.py
+-rw-r--r--   0 balandat   (501) staff       (20)     7412 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/optim/utils/model_utils.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5930 2023-05-29 17:24:44.000000 botorch-0.9.1/botorch/optim/utils/numpy_utils.py
+-rw-r--r--   0 balandat   (501) staff       (20)     3684 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/optim/utils/timeout.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.063315 botorch-0.9.1/botorch/posteriors/
+-rw-r--r--   0 balandat   (501) staff       (20)     1000 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/posteriors/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)     1581 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/posteriors/base_samples.py
+-rw-r--r--   0 balandat   (501) staff       (20)     2733 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/posteriors/deterministic.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5027 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/posteriors/ensemble.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5375 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/posteriors/fully_bayesian.py
+-rw-r--r--   0 balandat   (501) staff       (20)    14827 2023-04-12 11:57:17.000000 botorch-0.9.1/botorch/posteriors/gpytorch.py
+-rw-r--r--   0 balandat   (501) staff       (20)    11379 2023-05-03 15:06:10.000000 botorch-0.9.1/botorch/posteriors/higher_order.py
+-rw-r--r--   0 balandat   (501) staff       (20)    12403 2023-05-03 15:06:10.000000 botorch-0.9.1/botorch/posteriors/multitask.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5626 2023-04-12 11:57:17.000000 botorch-0.9.1/botorch/posteriors/posterior.py
+-rw-r--r--   0 balandat   (501) staff       (20)     7217 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/posteriors/posterior_list.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4253 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/posteriors/torch.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5751 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/posteriors/transformed.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.067486 botorch-0.9.1/botorch/sampling/
+-rw-r--r--   0 balandat   (501) staff       (20)     1210 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)     6419 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/base.py
+-rw-r--r--   0 balandat   (501) staff       (20)     1331 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/deterministic.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4964 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/get_sampler.py
+-rw-r--r--   0 balandat   (501) staff       (20)     2289 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/index_sampler.py
+-rw-r--r--   0 balandat   (501) staff       (20)     2657 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/list_sampler.py
+-rw-r--r--   0 balandat   (501) staff       (20)     8627 2023-07-03 14:23:54.000000 botorch-0.9.1/botorch/sampling/normal.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4474 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/pairwise_samplers.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.069588 botorch-0.9.1/botorch/sampling/pathwise/
+-rw-r--r--   0 balandat   (501) staff       (20)      977 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/pathwise/__init__.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.070483 botorch-0.9.1/botorch/sampling/pathwise/features/
+-rw-r--r--   0 balandat   (501) staff       (20)      512 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/pathwise/features/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)     6229 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/pathwise/features/generators.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4458 2023-05-18 00:21:43.000000 botorch-0.9.1/botorch/sampling/pathwise/features/maps.py
+-rw-r--r--   0 balandat   (501) staff       (20)     6195 2023-05-18 00:21:43.000000 botorch-0.9.1/botorch/sampling/pathwise/paths.py
+-rw-r--r--   0 balandat   (501) staff       (20)     6416 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/pathwise/posterior_samplers.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5420 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/pathwise/prior_samplers.py
+-rw-r--r--   0 balandat   (501) staff       (20)     7069 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/pathwise/update_strategies.py
+-rw-r--r--   0 balandat   (501) staff       (20)    10536 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/pathwise/utils.py
+-rw-r--r--   0 balandat   (501) staff       (20)     6555 2022-03-10 21:59:17.000000 botorch-0.9.1/botorch/sampling/qmc.py
+-rw-r--r--   0 balandat   (501) staff       (20)     2232 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/sampling/stochastic_samplers.py
+-rw-r--r--   0 balandat   (501) staff       (20)     2944 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/settings.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.073507 botorch-0.9.1/botorch/test_functions/
+-rw-r--r--   0 balandat   (501) staff       (20)     2195 2023-05-21 00:44:53.000000 botorch-0.9.1/botorch/test_functions/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)     6296 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/test_functions/base.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5330 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/test_functions/multi_fidelity.py
+-rw-r--r--   0 balandat   (501) staff       (20)    49438 2023-05-21 00:44:53.000000 botorch-0.9.1/botorch/test_functions/multi_objective.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4803 2022-06-10 04:39:40.000000 botorch-0.9.1/botorch/test_functions/multi_objective_multi_fidelity.py
+-rw-r--r--   0 balandat   (501) staff       (20)     8869 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/test_functions/sensitivity_analysis.py
+-rw-r--r--   0 balandat   (501) staff       (20)    31639 2023-05-21 00:44:53.000000 botorch-0.9.1/botorch/test_functions/synthetic.py
+-rw-r--r--   0 balandat   (501) staff       (20)     1112 2023-05-21 00:44:53.000000 botorch-0.9.1/botorch/test_functions/utils.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.080003 botorch-0.9.1/botorch/utils/
+-rw-r--r--   0 balandat   (501) staff       (20)     1082 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)     1202 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/constants.py
+-rw-r--r--   0 balandat   (501) staff       (20)     3475 2023-07-03 14:23:54.000000 botorch-0.9.1/botorch/utils/constraints.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4433 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/containers.py
+-rw-r--r--   0 balandat   (501) staff       (20)     6217 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/context_managers.py
+-rw-r--r--   0 balandat   (501) staff       (20)     7184 2023-07-11 21:08:20.000000 botorch-0.9.1/botorch/utils/datasets.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5613 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/dispatcher.py
+-rw-r--r--   0 balandat   (501) staff       (20)     7854 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/feasible_volume.py
+-rw-r--r--   0 balandat   (501) staff       (20)    20040 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/gp_sampling.py
+-rw-r--r--   0 balandat   (501) staff       (20)     6290 2023-04-04 13:42:04.000000 botorch-0.9.1/botorch/utils/low_rank.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.081778 botorch-0.9.1/botorch/utils/multi_objective/
+-rw-r--r--   0 balandat   (501) staff       (20)      565 2022-03-10 21:59:17.000000 botorch-0.9.1/botorch/utils/multi_objective/__init__.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.084016 botorch-0.9.1/botorch/utils/multi_objective/box_decompositions/
+-rw-r--r--   0 balandat   (501) staff       (20)      972 2022-03-10 21:59:17.000000 botorch-0.9.1/botorch/utils/multi_objective/box_decompositions/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)    13382 2023-05-09 15:17:51.000000 botorch-0.9.1/botorch/utils/multi_objective/box_decompositions/box_decomposition.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4479 2022-03-10 21:59:17.000000 botorch-0.9.1/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py
+-rw-r--r--   0 balandat   (501) staff       (20)     2554 2023-05-09 15:17:51.000000 botorch-0.9.1/botorch/utils/multi_objective/box_decompositions/dominated.py
+-rw-r--r--   0 balandat   (501) staff       (20)    18402 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/multi_objective/box_decompositions/non_dominated.py
+-rw-r--r--   0 balandat   (501) staff       (20)    12735 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/multi_objective/box_decompositions/utils.py
+-rw-r--r--   0 balandat   (501) staff       (20)    14870 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/multi_objective/hypervolume.py
+-rw-r--r--   0 balandat   (501) staff       (20)     3534 2022-05-15 20:07:15.000000 botorch-0.9.1/botorch/utils/multi_objective/pareto.py
+-rw-r--r--   0 balandat   (501) staff       (20)     4711 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/multi_objective/scalarization.py
+-rw-r--r--   0 balandat   (501) staff       (20)     9469 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/utils/objective.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.087367 botorch-0.9.1/botorch/utils/probability/
+-rw-r--r--   0 balandat   (501) staff       (20)      777 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/probability/__init__.py
+-rw-r--r--   0 balandat   (501) staff       (20)    11159 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/probability/bvn.py
+-rw-r--r--   0 balandat   (501) staff       (20)    22921 2023-07-03 14:23:54.000000 botorch-0.9.1/botorch/utils/probability/lin_ess.py
+-rw-r--r--   0 balandat   (501) staff       (20)     7815 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/utils/probability/linalg.py
+-rw-r--r--   0 balandat   (501) staff       (20)    16553 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/utils/probability/mvnxpb.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5675 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/probability/truncated_multivariate_normal.py
+-rw-r--r--   0 balandat   (501) staff       (20)    10727 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/probability/unified_skew_normal.py
+-rw-r--r--   0 balandat   (501) staff       (20)    11385 2023-07-09 15:09:08.000000 botorch-0.9.1/botorch/utils/probability/utils.py
+-rw-r--r--   0 balandat   (501) staff       (20)     3107 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/rounding.py
+-rw-r--r--   0 balandat   (501) staff       (20)     9414 2023-08-01 14:24:19.000000 botorch-0.9.1/botorch/utils/safe_math.py
+-rw-r--r--   0 balandat   (501) staff       (20)    35566 2023-06-02 23:50:48.000000 botorch-0.9.1/botorch/utils/sampling.py
+-rw-r--r--   0 balandat   (501) staff       (20)    16945 2023-06-07 21:20:45.000000 botorch-0.9.1/botorch/utils/testing.py
+-rw-r--r--   0 balandat   (501) staff       (20)     5641 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/torch.py
+-rw-r--r--   0 balandat   (501) staff       (20)    12649 2023-06-02 23:50:48.000000 botorch-0.9.1/botorch/utils/transforms.py
+-rw-r--r--   0 balandat   (501) staff       (20)      610 2023-04-01 23:17:12.000000 botorch-0.9.1/botorch/utils/types.py
+-rw-r--r--   0 balandat   (501) staff       (20)      160 2023-08-02 01:34:19.000000 botorch-0.9.1/botorch/version.py
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.016548 botorch-0.9.1/botorch.egg-info/
+-rw-r--r--   0 balandat   (501) staff       (20)     9967 2023-08-02 01:34:19.000000 botorch-0.9.1/botorch.egg-info/PKG-INFO
+-rw-r--r--   0 balandat   (501) staff       (20)     7508 2023-08-02 01:34:19.000000 botorch-0.9.1/botorch.egg-info/SOURCES.txt
+-rw-r--r--   0 balandat   (501) staff       (20)        1 2023-08-02 01:34:19.000000 botorch-0.9.1/botorch.egg-info/dependency_links.txt
+-rw-r--r--   0 balandat   (501) staff       (20)      308 2023-08-02 01:34:19.000000 botorch-0.9.1/botorch.egg-info/requires.txt
+-rw-r--r--   0 balandat   (501) staff       (20)        8 2023-08-02 01:34:19.000000 botorch-0.9.1/botorch.egg-info/top_level.txt
+-rwxr-xr-x   0 balandat   (501) staff       (20)    79395 2022-03-10 21:59:17.000000 botorch-0.9.1/botorch_logo_lockup.png
+-rwxr-xr-x   0 balandat   (501) staff       (20)    63261 2019-10-29 21:48:18.000000 botorch-0.9.1/botorch_logo_lockup.svg
+-rw-r--r--   0 balandat   (501) staff       (20)      196 2023-08-01 22:52:13.000000 botorch-0.9.1/environment.yml
+drwxr-xr-x   0 balandat   (501) staff       (20)        0 2023-08-02 01:34:20.087730 botorch-0.9.1/notebooks/
+-rw-r--r--   0 balandat   (501) staff       (20)    15796 2023-04-01 23:17:12.000000 botorch-0.9.1/notebooks/tutorials_performance_tracking.ipynb
+-rw-r--r--   0 balandat   (501) staff       (20)      246 2023-04-01 23:17:12.000000 botorch-0.9.1/pyproject.toml
+-rw-r--r--   0 balandat   (501) staff       (20)       65 2023-04-01 23:17:12.000000 botorch-0.9.1/requirements-fmt.txt
+-rw-r--r--   0 balandat   (501) staff       (20)       91 2023-08-01 22:52:13.000000 botorch-0.9.1/requirements.txt
+-rw-r--r--   0 balandat   (501) staff       (20)      236 2023-08-02 01:34:20.091445 botorch-0.9.1/setup.cfg
+-rw-r--r--   0 balandat   (501) staff       (20)     3379 2023-08-01 14:24:19.000000 botorch-0.9.1/setup.py
```

### Comparing `botorch-0.8.5/.conda/meta.yaml` & `botorch-0.9.1/.conda/meta.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 build:
   noarch: python
   script: "$PYTHON setup.py install --single-version-externally-managed --record=record.txt"
 
 requirements:
   host:
-    - python>=3.8
+    - python>=3.9
     - setuptools
     - setuptools_scm
   run:
-    - pytorch >=1.12
-    - gpytorch ==1.10
-    - linear_operator ==0.4.0
+    - pytorch >=1.13.1
+    - gpytorch ==1.11
+    - linear_operator ==0.5.1
     - scipy
     - multipledispatch
     - pyro-ppl >=1.8.4
 
 test:
   imports:
     - botorch
```

### Comparing `botorch-0.8.5/.github/ISSUE_TEMPLATE/bug_report.md` & `botorch-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/.github/ISSUE_TEMPLATE/feature_request.md` & `botorch-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/.github/ISSUE_TEMPLATE.md` & `botorch-0.9.1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/.github/PULL_REQUEST_TEMPLATE.md` & `botorch-0.9.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/.github/workflows/deploy_on_release.yml` & `botorch-0.9.1/.github/workflows/deploy_on_release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,29 @@
   tests-and-coverage-pip:
     name: Tests and coverage (pip, Python ${{ matrix.python-version }}, ${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest", "macos-latest", "windows-latest"]
-        python-version: ["3.8", "3.10"]
+        python-version: ["3.9", "3.11"]
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install (auto-install dependencies)
       run: |
         pip install .[test]
     - name: Unit tests and coverage
       run: |
         pytest -ra --cov=. --cov-report term-missing
     - name: Upload coverage
-      if: ${{ runner.os == 'Linux' && matrix.python-version == 3.8 }}
+      if: ${{ runner.os == 'Linux' && matrix.python-version == 3.9 }}
       run: |
         bash <(curl -s https://codecov.io/bash)
 
   package-deploy-pypi:
     name: Package and deploy to pypi.org
     runs-on: ubuntu-latest
     needs: tests-and-coverage-pip
@@ -72,15 +72,15 @@
       fail-fast: true
     steps:
     - uses: actions/checkout@v3
     - uses: conda-incubator/setup-miniconda@v2
       with:
         miniconda-version: "latest"
         activate-environment: test
-        python-version: "3.8"
+        python-version: "3.9"
     - name: Fetch all history for all tags and branches
       run: git fetch --prune --unshallow
     - name: Install dependencies
       shell: bash -l {0}
       run: |
         conda install -y setuptools_scm conda-build conda-verify anaconda-client
         conda install -y scipy sphinx pytest flake8 multipledispatch
@@ -103,7 +103,8 @@
   publish-versioned-website:
     name: Publish versioned website
     needs: [package-deploy-pypi, package-deploy-conda]
     uses: ./.github/workflows/reusable_website.yml
     with:
       publish_versioned_website: true
       release_tag: ${{ github.event.release.tag_name }}
+    secrets: inherit
```

### Comparing `botorch-0.8.5/.github/workflows/docs.yml` & `botorch-0.9.1/.github/workflows/docs.yml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     strategy:
       fail-fast: false
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: "3.8"
+        python-version: "3.9"
     - name: Install dependencies
       env:
         ALLOW_LATEST_GPYTORCH_LINOP: true
       run: |
         pip install git+https://github.com/cornellius-gp/linear_operator.git
         pip install git+https://github.com/cornellius-gp/gpytorch.git
         pip install .[dev]
```

### Comparing `botorch-0.8.5/.github/workflows/lint.yml` & `botorch-0.9.1/.github/workflows/lint.yml`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     strategy:
       fail-fast: false
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: "3.8"
+        python-version: "3.9"
     - name: Install dependencies
       run: |
         # pin dependencies to match Meta-internal versions
         pip install -r requirements-fmt.txt
         pip install ufmt
     - name: ufmt
       run: |
@@ -36,14 +36,14 @@
     strategy:
       fail-fast: false
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: "3.8"
+        python-version: "3.9"
     - name: Install dependencies
       run: |
         pip install flake8 flake8-docstrings
     - name: Flake8
       run: |
         flake8
```

### Comparing `botorch-0.8.5/.github/workflows/nightly.yml` & `botorch-0.9.1/.github/workflows/nightly.yml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   tests-and-coverage-nightly:
     name: Tests and coverage (pip, Python ${{ matrix.python-version }}, ${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest", "macos-latest", "windows-latest"]
-        python-version: ["3.8", "3.10"]
+        python-version: ["3.9", "3.11"]
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
@@ -30,15 +30,15 @@
         pip install git+https://github.com/cornellius-gp/linear_operator.git
         pip install git+https://github.com/cornellius-gp/gpytorch.git
         pip install .[test]
     - name: Unit tests and coverage
       run: |
         pytest -ra --cov=. --cov-report term-missing
     - name: Upload coverage
-      if: ${{ runner.os == 'Linux' && matrix.python-version == 3.8 }}
+      if: ${{ runner.os == 'Linux' && matrix.python-version == 3.9 }}
       run: |
         bash <(curl -s https://codecov.io/bash)
 
   package-test-deploy-pypi:
     name: Package and test deployment to test.pypi.org
     runs-on: ubuntu-latest
     strategy:
@@ -46,15 +46,15 @@
     steps:
     - uses: actions/checkout@v3
     - name: Fetch all history for all tags and branches
       run: git fetch --prune --unshallow
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: 3.9
     - name: Install dependencies
       env:
         ALLOW_LATEST_GPYTORCH_LINOP: true
       run: |
         pip install --pre torch -f https://download.pytorch.org/whl/nightly/cpu/torch_nightly.html
         pip install git+https://github.com/cornellius-gp/linear_operator.git
         pip install git+https://github.com/cornellius-gp/gpytorch.git
@@ -92,15 +92,15 @@
       fail-fast: true
     steps:
     - uses: actions/checkout@v3
     - uses: conda-incubator/setup-miniconda@v2
       with:
         miniconda-version: "latest"
         activate-environment: test
-        python-version: "3.8"
+        python-version: "3.9"
     - name: Fetch all history for all tags and branches
       run: git fetch --prune --unshallow
     - name: Install dependencies
       shell: bash -l {0}
       env:
         ALLOW_LATEST_GPYTORCH_LINOP: true
       # Don't need most deps for conda build, but need them for testing
@@ -119,14 +119,15 @@
 
   publish-latest-website:
     name: Publish latest website
     needs: [tests-and-coverage-nightly, package-test-deploy-pypi, package-conda]
     uses: ./.github/workflows/reusable_website.yml
     with:
       publish_versioned_website: false
+    secrets: inherit
 
   run_tutorials:
     name: Run tutorials without smoke test on latest PyTorch / GPyTorch / Ax
     uses: ./.github/workflows/reusable_tutorials.yml
     with:
       smoke_test: false
       use_stable_pytorch_gpytorch: false
```

### Comparing `botorch-0.8.5/.github/workflows/reusable_tutorials.yml` & `botorch-0.9.1/.github/workflows/reusable_tutorials.yml`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     name: Run tutorials
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: "3.8"
+        python-version: "3.9"
     - name: Fetch all history for all tags and branches
       # We need to do this so setuptools_scm knows how to set the BoTorch version.
       run: git fetch --prune --unshallow
     - if: ${{ !inputs.use_stable_pytorch_gpytorch }}
       name: Install latest PyTorch & GPyTorch
       run: |
         pip install --pre torch torchvision -f https://download.pytorch.org/whl/nightly/cpu/torch_nightly.html
```

### Comparing `botorch-0.8.5/.github/workflows/reusable_website.yml` & `botorch-0.9.1/.github/workflows/reusable_website.yml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     strategy:
       fail-fast: true
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: 3.9
     - name: Fetch all history for all tags and branches
       run: git fetch --prune --unshallow
     - if: ${{ !inputs.publish_versioned_website }}
       name: Install latest GPyTorch and Linear Operator
       run: |
         pip install git+https://github.com/cornellius-gp/linear_operator.git
         pip install git+https://github.com/cornellius-gp/gpytorch.git
```

### Comparing `botorch-0.8.5/.github/workflows/test.yml` & `botorch-0.9.1/.github/workflows/test.yml`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   tests-and-coverage-pip:
     name: Tests and coverage (pip, Python ${{ matrix.python-version }}, ${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest", "macos-latest", "windows-latest"]
-        python-version: ["3.8", "3.10"]
+        python-version: ["3.9", "3.11"]
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
@@ -33,26 +33,26 @@
         pip install git+https://github.com/cornellius-gp/linear_operator.git
         pip install git+https://github.com/cornellius-gp/gpytorch.git
         pip install .[test]
     - name: Unit tests and coverage
       run: |
         pytest -ra --cov=. --cov-report term-missing
     - name: Upload coverage
-      if: ${{ runner.os == 'Linux' && matrix.python-version == 3.8 }}
+      if: ${{ runner.os == 'Linux' && matrix.python-version == 3.9 }}
       run: |
         bash <(curl -s https://codecov.io/bash)
 
   tests-conda:
     name: Tests (conda, ${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest", "macos-latest", "windows-latest"]
-        python-version: ["3.8", "3.10"]
+        python-version: ["3.9", "3.11"]
     steps:
     - uses: actions/checkout@v3
     - uses: conda-incubator/setup-miniconda@v2
       with:
         miniconda-version: "latest"
         activate-environment: test
         python-version: ${{ matrix.python-version }}
```

### Comparing `botorch-0.8.5/.github/workflows/test_stable.yml` & `botorch-0.9.1/.github/workflows/test_stable.yml`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   tests-and-coverage-pip-stable:
     name: Tests and coverage (pip, Python ${{ matrix.python-version }}, ${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest", "macos-latest", "windows-latest"]
-        python-version: ["3.8", "3.10"]
+        python-version: ["3.9", "3.11"]
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
@@ -30,15 +30,15 @@
   tests-conda-stable:
     name: Tests (conda, ${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest", "macos-latest", "windows-latest"]
-        python-version: ["3.8", "3.10"]
+        python-version: ["3.9", "3.11"]
     steps:
     - uses: actions/checkout@v3
     - uses: conda-incubator/setup-miniconda@v2
       with:
         miniconda-version: "latest"
         activate-environment: test
         python-version: ${{ matrix.python-version }}
@@ -58,26 +58,31 @@
   tests-and-coverage-min-req-pip:
     name: Tests and coverage min req. torch, gpytorch & linear_operator versions (pip, Python ${{ matrix.python-version }}, ${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest", "macos-latest"]
-        python-version: ["3.8", "3.10"]
+        python-version: ["3.9", "3.11"]
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
+      env:
+        PYTHON_VERSION: ${{ matrix.python-version }}
+        OS: ${{ matrix.os }}
       run: |
         python setup.py egg_info
         req_txt="botorch.egg-info/requires.txt"
         min_torch_version=$(grep '\btorch[>=]=' ${req_txt} | sed 's/[^0-9.]//g')
+        # HACK around the fact that pytorch does not offer a mac binary for 1.13.1 for py3.11 - TODO: Remove when bumping torch to 2.0.1
+        min_torch_version=$(if [[ "${min_torch_version}"=="1.13.1" ]] && [[ "${PYTHON_VERSION}"=="3.11" ]] && [[ "${OS}"=="macos-latest" ]]; then echo "2.0.1"; else echo "${min_torch_version}"; fi)
         min_gpytorch_version=$(grep '\bgpytorch[>=]=' ${req_txt} | sed 's/[^0-9.]//g')
         min_linear_operator_version=$(grep '\blinear_operator[>=]=' ${req_txt} | sed 's/[^0-9.]//g')
         pip install "torch==${min_torch_version}" "gpytorch==${min_gpytorch_version}" "linear_operator==${min_linear_operator_version}"
         pip install .[test]
     - name: Unit tests and coverage
       run: |
         pytest -ra --cov=. --cov-report term-missing
```

### Comparing `botorch-0.8.5/.gitignore` & `botorch-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/CHANGELOG.md` & `botorch-0.9.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,62 @@
 # Changelog
 
 The release log for BoTorch.
 
+## [0.9.1] - Aug 1, 2023
+
+* Require linear_operator == 0.5.1 (#1963).
+
+
+## [0.9.0] - Aug 1, 2023
+
+#### Compatibility
+* Require Python >= 3.9.0 (#1924).
+* Require PyTorch >= 1.13.1 (#1960).
+* Require linear_operator == 0.5.0 (#1961).
+* Require GPyTorch == 1.11 (#1961).
+
+#### Highlights
+* Introduce `OrthogonalAdditiveKernel` (#1869).
+* Speed up LCE-A kernel by over an order of magnitude (#1910).
+* Introduce `optimize_acqf_homotopy`, for optimizing acquisition functions with homotopy (#1915).
+* Introduce `PriorGuidedAcquisitionFunction` (PiBO) (#1920).
+* Introduce `qLogExpectedImprovement`, which provides more accurate numerics than `qExpectedImprovement` and can lead to significant optimization improvements (#1936).
+* Similarly, introduce `qLogNoisyExpectedImprovement`, which is analogous to `qNoisyExpectedImprovement` (#1937).
+
+#### New Features
+* Add constrained synthetic test functions `PressureVesselDesign`, `WeldedBeam`, `SpeedReducer`, and `TensionCompressionString` (#1832).
+* Support decoupled fantasization (#1853) and decoupled evaluations in cost-aware utilities (#1949).
+* Add `PairwiseBayesianActiveLearningByDisagreement`, an active learning acquisition function for PBO and BOPE (#1855).
+* Support custom mean and likelihood in `MultiTaskGP` (#1909).
+* Enable candidate generation (via `optimize_acqf`) with both `non_linear_constraints` and `fixed_features` (#1912).
+* Introduce `L0PenaltyApproxObjective` to support L0 regularization (#1916).
+* Enable batching in `PriorGuidedAcquisitionFunction` (#1925).
+
+#### Other changes
+* Deprecate `FixedNoiseMultiTaskGP`; allow `train_Yvar` optionally in `MultiTaskGP` (#1818).
+* Implement `load_state_dict` for SAAS multi-task GP (#1825).
+* Improvements to `LinearEllipticalSliceSampler` (#1859, #1878, #1879, #1883).
+* Allow passing in task features as part of X in MTGP.posterior (#1868).
+* Improve numerical stability of log densities in pairwise GPs (#1919).
+* Python 3.11 compliance (#1927).
+* Enable using constraints with `SampleReducingMCAcquisitionFunction`s when using `input_constructor`s and `get_acquisition_function` (#1932).
+* Enable use of `qLogExpectedImprovement` and `qLogNoisyExpectedImprovement` with Ax (#1941).
+
+#### Bug Fixes
+* Enable pathwise sampling modules to be converted to GPU  (#1821).
+* Allow `Standardize` modules to be loaded once trained (#1874).
+* Fix memory leak in Inducing Point Allocators (#1890).
+* Correct einsum computation in `LCEAKernel` (#1918).
+* Properly whiten bounds in MVNXPB (#1933).
+* Make `FixedFeatureAcquisitionFunction` convert floats to double-precision tensors rather than single-precision (#1944).
+* Fix memory leak in `FullyBayesianPosterior` (#1951).
+* Make `AnalyticExpectedUtilityOfBestOption` input constructor work correctionly with multi-task GPs (#1955).
+
+
 ## [0.8.5] - May 8, 2023
 
 #### New Features
 * Support inferred noise in `SaasFullyBayesianMultiTaskGP` (#1809).
 
 #### Other Changes
 * More informative error message when `Standardize` has wrong batch shape (#1807).
```

### Comparing `botorch-0.8.5/CODE_OF_CONDUCT.md` & `botorch-0.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/CONTRIBUTING.md` & `botorch-0.9.1/CONTRIBUTING.md`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 `__init__` function contains an `Args:` block. We use the `flake8-docstrings`
 plugin to check this - install via `pip install flake8-docstrings` and
 run `flake8` as above to check.
 
 
 #### Type Hints
 
-BoTorch is fully typed using python 3.8+
+BoTorch is fully typed using python 3.9+
 [type hints](https://www.python.org/dev/peps/pep-0484/).
 We expect any contributions to also use proper type annotations. While we
 currently do not enforce full consistency of these in our continuous integration
 test, you should strive to type check your code locally. For this we recommend
 using [pyre](https://pyre-check.org/).
```

### Comparing `botorch-0.8.5/LICENSE` & `botorch-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/PKG-INFO` & `botorch-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: botorch
-Version: 0.8.5
+Version: 0.9.1
 Summary: Bayesian Optimization in PyTorch
 Home-page: https://botorch.org
 Author: Meta Platforms, Inc.
 License: MIT
 Project-URL: Documentation, https://botorch.org
 Project-URL: Source, https://github.com/pytorch/botorch
 Project-URL: conda, https://anaconda.org/pytorch/botorch
 Keywords: Bayesian optimization,PyTorch
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: tutorials
 License-File: LICENSE
 
 <a href="https://botorch.org">
@@ -75,18 +75,18 @@
 We recommend that end-users who are not actively doing research on Bayesian
 Optimization simply use Ax.
 
 
 ## Installation
 
 **Installation Requirements**
-- Python >= 3.8
-- PyTorch >= 1.12
-- gpytorch == 1.10
-- linear_operator == 0.4.0
+- Python >= 3.9
+- PyTorch >= 1.13.1
+- gpytorch == 1.11
+- linear_operator == 0.5.1
 - pyro-ppl >= 1.8.4
 - scipy
 - multiple-dispatch
 
 ### Prerequisite only for MacOS users with Intel processors:
 Before installing BoTorch, we recommend first manually installing PyTorch, a required dependency of
 BoTorch. Installing it according to the [PyTorch installation instructions](https://pytorch.org/get-started/locally/)
@@ -173,15 +173,17 @@
 1. Fit a Gaussian Process model to data
   ```python
   import torch
   from botorch.models import SingleTaskGP
   from botorch.fit import fit_gpytorch_mll
   from gpytorch.mlls import ExactMarginalLogLikelihood
 
-  train_X = torch.rand(10, 2)
+  # Double precision is highly recommended for GPs.
+  # See https://github.com/pytorch/botorch/discussions/1444
+  train_X = torch.rand(10, 2, dtype=torch.double)
   Y = 1 - (train_X - 0.5).norm(dim=-1, keepdim=True)  # explicit output dimension
   Y += 0.1 * torch.rand_like(Y)
   train_Y = (Y - Y.mean()) / Y.std()
 
   gp = SingleTaskGP(train_X, train_Y)
   mll = ExactMarginalLogLikelihood(gp.likelihood, gp)
   fit_gpytorch_mll(mll)
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: botorch Version: 0.8.5 Summary: Bayesian
+Metadata-Version: 2.1 Name: botorch Version: 0.9.1 Summary: Bayesian
 Optimization in PyTorch Home-page: https://botorch.org Author: Meta Platforms,
 Inc. License: MIT Project-URL: Documentation, https://botorch.org Project-URL:
 Source, https://github.com/pytorch/botorch Project-URL: conda, https://
 anaconda.org/pytorch/botorch Keywords: Bayesian optimization,PyTorch
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Developers Requires-Python:
->=3.8 Description-Content-Type: text/markdown Provides-Extra: dev Provides-
+>=3.9 Description-Content-Type: text/markdown Provides-Extra: dev Provides-
 Extra: test Provides-Extra: tutorials License-File: LICENSE [BoTorch_Logo]
 ===============================================================================
 [![Support Ukraine](https://img.shields.io/badge/Support-Ukraine-
 FFD500?style=flat&labelColor=005BBB)](https://opensource.fb.com/support-
 ukraine) [![Lint](https://github.com/pytorch/botorch/workflows/Lint/badge.svg)]
 (https://github.com/pytorch/botorch/actions?query=workflow%3ALint) [![Test]
 (https://github.com/pytorch/botorch/workflows/Test/badge.svg)](https://
@@ -43,16 +43,16 @@
 researchers and sophisticated practitioners in Bayesian Optimization and AI. We
 recommend using BoTorch as a low-level API for implementing new algorithms for
 [Ax](https://ax.dev). Ax has been designed to be an easy-to-use platform for
 end-users, which at the same time is flexible enough for Bayesian Optimization
 researchers to plug into for handling of feature transformations, (meta-)data
 management, storage, etc. We recommend that end-users who are not actively
 doing research on Bayesian Optimization simply use Ax. ## Installation
-**Installation Requirements** - Python >= 3.8 - PyTorch >= 1.12 - gpytorch ==
-1.10 - linear_operator == 0.4.0 - pyro-ppl >= 1.8.4 - scipy - multiple-dispatch
+**Installation Requirements** - Python >= 3.9 - PyTorch >= 1.13.1 - gpytorch ==
+1.11 - linear_operator == 0.5.1 - pyro-ppl >= 1.8.4 - scipy - multiple-dispatch
 ### Prerequisite only for MacOS users with Intel processors: Before installing
 BoTorch, we recommend first manually installing PyTorch, a required dependency
 of BoTorch. Installing it according to the [PyTorch installation instructions]
 (https://pytorch.org/get-started/locally/) ensures that it is properly linked
 against MKL, a library that optimizes mathematical computation for Intel
 processors. This will result in up to an order-of-magnitude speed-up for
 Bayesian optimization, as at the moment, installing PyTorch from pip does not
@@ -98,30 +98,32 @@
 notebooks. * You can also install either the dev or tutorials dependencies
 without installing both, e.g. by changing the last command to `pip install -
 e ".[dev]"`. ## Getting Started Here's a quick run down of the main components
 of a Bayesian optimization loop. For more details see our [Documentation]
 (https://botorch.org/docs/introduction) and the [Tutorials](https://
 botorch.org/tutorials). 1. Fit a Gaussian Process model to data ```python
 import torch from botorch.models import SingleTaskGP from botorch.fit import
-fit_gpytorch_mll from gpytorch.mlls import ExactMarginalLogLikelihood train_X =
-torch.rand(10, 2) Y = 1 - (train_X - 0.5).norm(dim=-1, keepdim=True) # explicit
-output dimension Y += 0.1 * torch.rand_like(Y) train_Y = (Y - Y.mean()) / Y.std
-() gp = SingleTaskGP(train_X, train_Y) mll = ExactMarginalLogLikelihood
-(gp.likelihood, gp) fit_gpytorch_mll(mll) ``` 2. Construct an acquisition
-function ```python from botorch.acquisition import UpperConfidenceBound UCB =
-UpperConfidenceBound(gp, beta=0.1) ``` 3. Optimize the acquisition function
-```python from botorch.optim import optimize_acqf bounds = torch.stack(
-[torch.zeros(2), torch.ones(2)]) candidate, acq_value = optimize_acqf( UCB,
-bounds=bounds, q=1, num_restarts=5, raw_samples=20, ) ``` ## Citing BoTorch If
-you use BoTorch, please cite the following paper: > [M. Balandat, B. Karrer, D.
-R. Jiang, S. Daulton, B. Letham, A. G. Wilson, and E. Bakshy. BoTorch: A
-Framework for Efficient Monte-Carlo Bayesian Optimization. Advances in Neural
-Information Processing Systems 33, 2020.](https://arxiv.org/abs/1910.06403) ```
-@inproceedings{balandat2020botorch, title={{BoTorch: A Framework for Efficient
-Monte-Carlo Bayesian Optimization}}, author={Balandat, Maximilian and Karrer,
-Brian and Jiang, Daniel R. and Daulton, Samuel and Letham, Benjamin and Wilson,
-Andrew Gordon and Bakshy, Eytan}, booktitle = {Advances in Neural Information
+fit_gpytorch_mll from gpytorch.mlls import ExactMarginalLogLikelihood # Double
+precision is highly recommended for GPs. # See https://github.com/pytorch/
+botorch/discussions/1444 train_X = torch.rand(10, 2, dtype=torch.double) Y = 1
+- (train_X - 0.5).norm(dim=-1, keepdim=True) # explicit output dimension Y +=
+0.1 * torch.rand_like(Y) train_Y = (Y - Y.mean()) / Y.std() gp = SingleTaskGP
+(train_X, train_Y) mll = ExactMarginalLogLikelihood(gp.likelihood, gp)
+fit_gpytorch_mll(mll) ``` 2. Construct an acquisition function ```python from
+botorch.acquisition import UpperConfidenceBound UCB = UpperConfidenceBound(gp,
+beta=0.1) ``` 3. Optimize the acquisition function ```python from botorch.optim
+import optimize_acqf bounds = torch.stack([torch.zeros(2), torch.ones(2)])
+candidate, acq_value = optimize_acqf( UCB, bounds=bounds, q=1, num_restarts=5,
+raw_samples=20, ) ``` ## Citing BoTorch If you use BoTorch, please cite the
+following paper: > [M. Balandat, B. Karrer, D. R. Jiang, S. Daulton, B. Letham,
+A. G. Wilson, and E. Bakshy. BoTorch: A Framework for Efficient Monte-Carlo
+Bayesian Optimization. Advances in Neural Information Processing Systems 33,
+2020.](https://arxiv.org/abs/1910.06403) ``` @inproceedings
+{balandat2020botorch, title={{BoTorch: A Framework for Efficient Monte-Carlo
+Bayesian Optimization}}, author={Balandat, Maximilian and Karrer, Brian and
+Jiang, Daniel R. and Daulton, Samuel and Letham, Benjamin and Wilson, Andrew
+Gordon and Bakshy, Eytan}, booktitle = {Advances in Neural Information
 Processing Systems 33}, year={2020}, url = {http://arxiv.org/abs/1910.06403} }
 ``` See [here](https://botorch.org/docs/papers) for an incomplete selection of
 peer-reviewed papers that build off of BoTorch. ## Contributing See the
 [CONTRIBUTING](CONTRIBUTING.md) file for how to help out. ## License BoTorch is
 MIT licensed, as found in the [LICENSE](LICENSE) file.
```

### Comparing `botorch-0.8.5/README.md` & `botorch-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,18 @@
 We recommend that end-users who are not actively doing research on Bayesian
 Optimization simply use Ax.
 
 
 ## Installation
 
 **Installation Requirements**
-- Python >= 3.8
-- PyTorch >= 1.12
-- gpytorch == 1.10
-- linear_operator == 0.4.0
+- Python >= 3.9
+- PyTorch >= 1.13.1
+- gpytorch == 1.11
+- linear_operator == 0.5.1
 - pyro-ppl >= 1.8.4
 - scipy
 - multiple-dispatch
 
 ### Prerequisite only for MacOS users with Intel processors:
 Before installing BoTorch, we recommend first manually installing PyTorch, a required dependency of
 BoTorch. Installing it according to the [PyTorch installation instructions](https://pytorch.org/get-started/locally/)
@@ -149,15 +149,17 @@
 1. Fit a Gaussian Process model to data
   ```python
   import torch
   from botorch.models import SingleTaskGP
   from botorch.fit import fit_gpytorch_mll
   from gpytorch.mlls import ExactMarginalLogLikelihood
 
-  train_X = torch.rand(10, 2)
+  # Double precision is highly recommended for GPs.
+  # See https://github.com/pytorch/botorch/discussions/1444
+  train_X = torch.rand(10, 2, dtype=torch.double)
   Y = 1 - (train_X - 0.5).norm(dim=-1, keepdim=True)  # explicit output dimension
   Y += 0.1 * torch.rand_like(Y)
   train_Y = (Y - Y.mean()) / Y.std()
 
   gp = SingleTaskGP(train_X, train_Y)
   mll = ExactMarginalLogLikelihood(gp.likelihood, gp)
   fit_gpytorch_mll(mll)
```

#### html2text {}

```diff
@@ -33,16 +33,16 @@
 researchers and sophisticated practitioners in Bayesian Optimization and AI. We
 recommend using BoTorch as a low-level API for implementing new algorithms for
 [Ax](https://ax.dev). Ax has been designed to be an easy-to-use platform for
 end-users, which at the same time is flexible enough for Bayesian Optimization
 researchers to plug into for handling of feature transformations, (meta-)data
 management, storage, etc. We recommend that end-users who are not actively
 doing research on Bayesian Optimization simply use Ax. ## Installation
-**Installation Requirements** - Python >= 3.8 - PyTorch >= 1.12 - gpytorch ==
-1.10 - linear_operator == 0.4.0 - pyro-ppl >= 1.8.4 - scipy - multiple-dispatch
+**Installation Requirements** - Python >= 3.9 - PyTorch >= 1.13.1 - gpytorch ==
+1.11 - linear_operator == 0.5.1 - pyro-ppl >= 1.8.4 - scipy - multiple-dispatch
 ### Prerequisite only for MacOS users with Intel processors: Before installing
 BoTorch, we recommend first manually installing PyTorch, a required dependency
 of BoTorch. Installing it according to the [PyTorch installation instructions]
 (https://pytorch.org/get-started/locally/) ensures that it is properly linked
 against MKL, a library that optimizes mathematical computation for Intel
 processors. This will result in up to an order-of-magnitude speed-up for
 Bayesian optimization, as at the moment, installing PyTorch from pip does not
@@ -88,30 +88,32 @@
 notebooks. * You can also install either the dev or tutorials dependencies
 without installing both, e.g. by changing the last command to `pip install -
 e ".[dev]"`. ## Getting Started Here's a quick run down of the main components
 of a Bayesian optimization loop. For more details see our [Documentation]
 (https://botorch.org/docs/introduction) and the [Tutorials](https://
 botorch.org/tutorials). 1. Fit a Gaussian Process model to data ```python
 import torch from botorch.models import SingleTaskGP from botorch.fit import
-fit_gpytorch_mll from gpytorch.mlls import ExactMarginalLogLikelihood train_X =
-torch.rand(10, 2) Y = 1 - (train_X - 0.5).norm(dim=-1, keepdim=True) # explicit
-output dimension Y += 0.1 * torch.rand_like(Y) train_Y = (Y - Y.mean()) / Y.std
-() gp = SingleTaskGP(train_X, train_Y) mll = ExactMarginalLogLikelihood
-(gp.likelihood, gp) fit_gpytorch_mll(mll) ``` 2. Construct an acquisition
-function ```python from botorch.acquisition import UpperConfidenceBound UCB =
-UpperConfidenceBound(gp, beta=0.1) ``` 3. Optimize the acquisition function
-```python from botorch.optim import optimize_acqf bounds = torch.stack(
-[torch.zeros(2), torch.ones(2)]) candidate, acq_value = optimize_acqf( UCB,
-bounds=bounds, q=1, num_restarts=5, raw_samples=20, ) ``` ## Citing BoTorch If
-you use BoTorch, please cite the following paper: > [M. Balandat, B. Karrer, D.
-R. Jiang, S. Daulton, B. Letham, A. G. Wilson, and E. Bakshy. BoTorch: A
-Framework for Efficient Monte-Carlo Bayesian Optimization. Advances in Neural
-Information Processing Systems 33, 2020.](https://arxiv.org/abs/1910.06403) ```
-@inproceedings{balandat2020botorch, title={{BoTorch: A Framework for Efficient
-Monte-Carlo Bayesian Optimization}}, author={Balandat, Maximilian and Karrer,
-Brian and Jiang, Daniel R. and Daulton, Samuel and Letham, Benjamin and Wilson,
-Andrew Gordon and Bakshy, Eytan}, booktitle = {Advances in Neural Information
+fit_gpytorch_mll from gpytorch.mlls import ExactMarginalLogLikelihood # Double
+precision is highly recommended for GPs. # See https://github.com/pytorch/
+botorch/discussions/1444 train_X = torch.rand(10, 2, dtype=torch.double) Y = 1
+- (train_X - 0.5).norm(dim=-1, keepdim=True) # explicit output dimension Y +=
+0.1 * torch.rand_like(Y) train_Y = (Y - Y.mean()) / Y.std() gp = SingleTaskGP
+(train_X, train_Y) mll = ExactMarginalLogLikelihood(gp.likelihood, gp)
+fit_gpytorch_mll(mll) ``` 2. Construct an acquisition function ```python from
+botorch.acquisition import UpperConfidenceBound UCB = UpperConfidenceBound(gp,
+beta=0.1) ``` 3. Optimize the acquisition function ```python from botorch.optim
+import optimize_acqf bounds = torch.stack([torch.zeros(2), torch.ones(2)])
+candidate, acq_value = optimize_acqf( UCB, bounds=bounds, q=1, num_restarts=5,
+raw_samples=20, ) ``` ## Citing BoTorch If you use BoTorch, please cite the
+following paper: > [M. Balandat, B. Karrer, D. R. Jiang, S. Daulton, B. Letham,
+A. G. Wilson, and E. Bakshy. BoTorch: A Framework for Efficient Monte-Carlo
+Bayesian Optimization. Advances in Neural Information Processing Systems 33,
+2020.](https://arxiv.org/abs/1910.06403) ``` @inproceedings
+{balandat2020botorch, title={{BoTorch: A Framework for Efficient Monte-Carlo
+Bayesian Optimization}}, author={Balandat, Maximilian and Karrer, Brian and
+Jiang, Daniel R. and Daulton, Samuel and Letham, Benjamin and Wilson, Andrew
+Gordon and Bakshy, Eytan}, booktitle = {Advances in Neural Information
 Processing Systems 33}, year={2020}, url = {http://arxiv.org/abs/1910.06403} }
 ``` See [here](https://botorch.org/docs/papers) for an incomplete selection of
 peer-reviewed papers that build off of BoTorch. ## Contributing See the
 [CONTRIBUTING](CONTRIBUTING.md) file for how to help out. ## License BoTorch is
 MIT licensed, as found in the [LICENSE](LICENSE) file.
```

### Comparing `botorch-0.8.5/botorch/__init__.py` & `botorch-0.9.1/botorch/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/acquisition/__init__.py` & `botorch-0.9.1/botorch/acquisition/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,78 +12,98 @@
     PairwiseMCPosteriorVariance,
     qNegIntegratedPosteriorVariance,
 )
 from botorch.acquisition.analytic import (
     AnalyticAcquisitionFunction,
     ConstrainedExpectedImprovement,
     ExpectedImprovement,
+    LogExpectedImprovement,
+    LogNoisyExpectedImprovement,
     NoisyExpectedImprovement,
     PosteriorMean,
     ProbabilityOfImprovement,
     qAnalyticProbabilityOfImprovement,
     UpperConfidenceBound,
 )
 from botorch.acquisition.cost_aware import (
     GenericCostAwareUtility,
     InverseCostWeightedUtility,
 )
+from botorch.acquisition.decoupled import DecoupledAcquisitionFunction
 from botorch.acquisition.fixed_feature import FixedFeatureAcquisitionFunction
 from botorch.acquisition.input_constructors import get_acqf_input_constructor
 from botorch.acquisition.knowledge_gradient import (
     qKnowledgeGradient,
     qMultiFidelityKnowledgeGradient,
 )
+from botorch.acquisition.logei import (
+    LogImprovementMCAcquisitionFunction,
+    qLogExpectedImprovement,
+    qLogNoisyExpectedImprovement,
+)
 from botorch.acquisition.max_value_entropy_search import (
     MaxValueBase,
     qLowerBoundMaxValueEntropy,
     qMaxValueEntropy,
     qMultiFidelityLowerBoundMaxValueEntropy,
     qMultiFidelityMaxValueEntropy,
 )
 from botorch.acquisition.monte_carlo import (
     MCAcquisitionFunction,
     qExpectedImprovement,
     qNoisyExpectedImprovement,
     qProbabilityOfImprovement,
     qSimpleRegret,
     qUpperConfidenceBound,
+    SampleReducingMCAcquisitionFunction,
 )
 from botorch.acquisition.multi_step_lookahead import qMultiStepLookahead
 from botorch.acquisition.objective import (
     ConstrainedMCObjective,
     GenericMCObjective,
     IdentityMCObjective,
     LearnedObjective,
     LinearMCObjective,
     MCAcquisitionObjective,
-    ScalarizedObjective,
     ScalarizedPosteriorTransform,
 )
-from botorch.acquisition.preference import AnalyticExpectedUtilityOfBestOption
+from botorch.acquisition.preference import (
+    AnalyticExpectedUtilityOfBestOption,
+    PairwiseBayesianActiveLearningByDisagreement,
+)
+from botorch.acquisition.prior_guided import PriorGuidedAcquisitionFunction
 from botorch.acquisition.proximal import ProximalAcquisitionFunction
 from botorch.acquisition.utils import get_acquisition_function
 
 __all__ = [
     "AcquisitionFunction",
     "AnalyticAcquisitionFunction",
     "AnalyticExpectedUtilityOfBestOption",
     "ConstrainedExpectedImprovement",
+    "DecoupledAcquisitionFunction",
     "ExpectedImprovement",
+    "LogExpectedImprovement",
+    "LogNoisyExpectedImprovement",
     "FixedFeatureAcquisitionFunction",
     "GenericCostAwareUtility",
     "InverseCostWeightedUtility",
     "NoisyExpectedImprovement",
     "OneShotAcquisitionFunction",
+    "PairwiseBayesianActiveLearningByDisagreement",
     "PairwiseMCPosteriorVariance",
     "PosteriorMean",
+    "PriorGuidedAcquisitionFunction",
     "ProbabilityOfImprovement",
     "ProximalAcquisitionFunction",
     "UpperConfidenceBound",
     "qAnalyticProbabilityOfImprovement",
     "qExpectedImprovement",
+    "LogImprovementMCAcquisitionFunction",
+    "qLogExpectedImprovement",
+    "qLogNoisyExpectedImprovement",
     "qKnowledgeGradient",
     "MaxValueBase",
     "qMultiFidelityKnowledgeGradient",
     "qMaxValueEntropy",
     "qMultiFidelityLowerBoundMaxValueEntropy",
     "qLowerBoundMaxValueEntropy",
     "qMultiFidelityMaxValueEntropy",
@@ -95,13 +115,13 @@
     "qUpperConfidenceBound",
     "ConstrainedMCObjective",
     "GenericMCObjective",
     "IdentityMCObjective",
     "LearnedObjective",
     "LinearMCObjective",
     "MCAcquisitionFunction",
+    "SampleReducingMCAcquisitionFunction",
     "MCAcquisitionObjective",
-    "ScalarizedObjective",
     "ScalarizedPosteriorTransform",
     "get_acquisition_function",
     "get_acqf_input_constructor",
 ]
```

### Comparing `botorch-0.8.5/botorch/acquisition/acquisition.py` & `botorch-0.9.1/botorch/acquisition/acquisition.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 r"""Abstract base module for all botorch acquisition functions."""
 
 from __future__ import annotations
 
 import warnings
 from abc import ABC, abstractmethod
-from typing import Callable, Optional
+from typing import Optional
 
 import torch
-from botorch.exceptions import BotorchWarning, UnsupportedError
+from botorch.exceptions import BotorchWarning
 from botorch.models.model import Model, ModelDict
 from botorch.posteriors.posterior import Posterior
 from botorch.sampling.base import MCSampler
 from botorch.sampling.get_sampler import get_sampler
 from torch import Tensor
 from torch.nn import Module
 
@@ -37,43 +37,14 @@
 
         Args:
             model: A fitted model.
         """
         super().__init__()
         self.model: Model = model
 
-    @classmethod
-    def _deprecate_acqf_objective(
-        cls,
-        posterior_transform: Optional[Callable[[Posterior], Posterior]],
-        objective: Optional[Module],
-    ) -> Optional[Callable[[Posterior], Posterior]]:
-        from botorch.acquisition.objective import (
-            ScalarizedObjective,
-            ScalarizedPosteriorTransform,
-        )
-
-        if objective is None:
-            return posterior_transform
-        warnings.warn(
-            f"{cls.__name__} got a non-MC `objective`. The non-MC "
-            "AcquisitionObjectives and the `objective` argument to"
-            "AnalyticAcquisitionFunctions are DEPRECATED and will be removed in the"
-            "next version. Use `posterior_transform` instead.",
-            DeprecationWarning,
-        )
-        if not isinstance(objective, ScalarizedObjective):
-            raise UnsupportedError(
-                f"{cls.__name__} only supports ScalarizedObjective "
-                "(DEPRECATED) type objectives."
-            )
-        return ScalarizedPosteriorTransform(
-            weights=objective.weights, offset=objective.offset
-        )
-
     def set_X_pending(self, X_pending: Optional[Tensor] = None) -> None:
         r"""Informs the acquisition function about pending design points.
 
         Args:
             X_pending: `n x d` Tensor with `n` `d`-dim design points that have
                 been submitted for evaluation but have not yet been evaluated.
         """
@@ -165,14 +136,22 @@
         """
         if self.sampler is None:
             self.sampler = get_sampler(
                 posterior=posterior, sample_shape=self._default_sample_shape
             )
         return self.sampler(posterior=posterior)
 
+    @property
+    def sample_shape(self) -> torch.Size:
+        return (
+            self.sampler.sample_shape
+            if self.sampler is not None
+            else self._default_sample_shape
+        )
+
 
 class MultiModelAcquisitionFunction(AcquisitionFunction, ABC):
     r"""Abstract base class for acquisition functions that require
     multiple types of models.
 
     The intended use case for these acquisition functions are those
     where we have multiple models, each serving a distinct purpose.
```

### Comparing `botorch-0.8.5/botorch/acquisition/active_learning.py` & `botorch-0.9.1/botorch/acquisition/active_learning.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     def __init__(
         self,
         model: Model,
         mc_points: Tensor,
         sampler: Optional[MCSampler] = None,
         posterior_transform: Optional[PosteriorTransform] = None,
         X_pending: Optional[Tensor] = None,
-        **kwargs,
     ) -> None:
         r"""q-Integrated Negative Posterior Variance.
 
         Args:
             model: A fitted model.
             mc_points: A `batch_shape x N x d` tensor of points to use for
                 MC-integrating the posterior variance. Usually, these are qMC
@@ -72,15 +71,15 @@
             posterior_transform: A PosteriorTransform. If using a multi-output model,
                 a PosteriorTransform that transforms the multi-output posterior into a
                 single-output posterior is required.
             X_pending: A `n' x d`-dim Tensor of `n'` design points that have
                 points that have been submitted for function evaluation but
                 have not yet been evaluated.
         """
-        super().__init__(model=model, posterior_transform=posterior_transform, **kwargs)
+        super().__init__(model=model, posterior_transform=posterior_transform)
         if sampler is None:
             # If no sampler is provided, we use the following dummy sampler for the
             # fantasize() method in forward. IMPORTANT: This assumes that the posterior
             # variance does not depend on the samples y (only on x), which is true for
             # standard GP models, but not in general (e.g. for other likelihoods or
             # heteroskedastic GPs using a separate noise model fit on data).
             sampler = SobolQMCNormalSampler(sample_shape=torch.Size([1]))
```

### Comparing `botorch-0.8.5/botorch/acquisition/analytic.py` & `botorch-0.9.1/botorch/acquisition/analytic.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     phi,
 )
 from botorch.utils.safe_math import log1mexp, logmeanexp
 from botorch.utils.transforms import convert_to_target_pre_hook, t_batch_mode_transform
 from torch import Tensor
 from torch.nn.functional import pad
 
-_sqrt_2pi = math.sqrt(2 * math.pi)
 # the following two numbers are needed for _log_ei_helper
 _neg_inv_sqrt2 = -(2**-0.5)
 _log_sqrt_pi_div_2 = math.log(math.pi / 2) / 2
 
 
 class AnalyticAcquisitionFunction(AcquisitionFunction, ABC):
     r"""
@@ -54,29 +53,24 @@
     :meta private:
     """
 
     def __init__(
         self,
         model: Model,
         posterior_transform: Optional[PosteriorTransform] = None,
-        **kwargs,
     ) -> None:
         r"""Base constructor for analytic acquisition functions.
 
         Args:
             model: A fitted single-outcome model.
             posterior_transform: A PosteriorTransform. If using a multi-output model,
                 a PosteriorTransform that transforms the multi-output posterior into a
                 single-output posterior is required.
         """
         super().__init__(model=model)
-        posterior_transform = self._deprecate_acqf_objective(
-            posterior_transform=posterior_transform,
-            objective=kwargs.get("objective"),
-        )
         if posterior_transform is None:
             if model.num_outputs != 1:
                 raise UnsupportedError(
                     "Must specify a posterior transform when using a "
                     "multi-output model."
                 )
         else:
@@ -142,28 +136,27 @@
 
     def __init__(
         self,
         model: Model,
         best_f: Union[float, Tensor],
         posterior_transform: Optional[PosteriorTransform] = None,
         maximize: bool = True,
-        **kwargs,
     ):
         r"""Single-outcome Probability of Improvement.
 
         Args:
             model: A fitted single-outcome model.
             best_f: Either a scalar or a `b`-dim Tensor (batch mode) representing
                 the best function value observed so far (assumed noiseless).
             posterior_transform: A PosteriorTransform. If using a multi-output model,
                 a PosteriorTransform that transforms the multi-output posterior into a
                 single-output posterior is required.
             maximize: If True, consider the problem a maximization problem.
         """
-        super().__init__(model=model, posterior_transform=posterior_transform, **kwargs)
+        super().__init__(model=model, posterior_transform=posterior_transform)
         self.register_buffer("best_f", torch.as_tensor(best_f))
         self.maximize = maximize
 
     @t_batch_mode_transform(expected_q=1)
     def forward(self, X: Tensor) -> Tensor:
         r"""Evaluate the Log Probability of Improvement on the candidate set X.
 
@@ -197,28 +190,27 @@
 
     def __init__(
         self,
         model: Model,
         best_f: Union[float, Tensor],
         posterior_transform: Optional[PosteriorTransform] = None,
         maximize: bool = True,
-        **kwargs,
     ):
         r"""Single-outcome Probability of Improvement.
 
         Args:
             model: A fitted single-outcome model.
             best_f: Either a scalar or a `b`-dim Tensor (batch mode) representing
                 the best function value observed so far (assumed noiseless).
             posterior_transform: A PosteriorTransform. If using a multi-output model,
                 a PosteriorTransform that transforms the multi-output posterior into a
                 single-output posterior is required.
             maximize: If True, consider the problem a maximization problem.
         """
-        super().__init__(model=model, posterior_transform=posterior_transform, **kwargs)
+        super().__init__(model=model, posterior_transform=posterior_transform)
         self.register_buffer("best_f", torch.as_tensor(best_f))
         self.maximize = maximize
 
     @t_batch_mode_transform(expected_q=1)
     def forward(self, X: Tensor) -> Tensor:
         r"""Evaluate the Probability of Improvement on the candidate set X.
 
@@ -246,28 +238,27 @@
 
     def __init__(
         self,
         model: Model,
         best_f: Union[float, Tensor],
         posterior_transform: Optional[PosteriorTransform] = None,
         maximize: bool = True,
-        **kwargs,
     ) -> None:
         """qPI using an analytic approximation.
 
         Args:
             model: A fitted single-outcome model.
             best_f: Either a scalar or a `b`-dim Tensor (batch mode) representing
                 the best function value observed so far (assumed noiseless).
             posterior_transform: A PosteriorTransform. If using a multi-output model,
                 a PosteriorTransform that transforms the multi-output posterior into a
                 single-output posterior is required.
             maximize: If True, consider the problem a maximization problem.
         """
-        super().__init__(model=model, posterior_transform=posterior_transform, **kwargs)
+        super().__init__(model=model, posterior_transform=posterior_transform)
         self.maximize = maximize
         if not torch.is_tensor(best_f):
             best_f = torch.tensor(best_f)
         self.register_buffer("best_f", best_f)
 
     @t_batch_mode_transform()
     def forward(self, X: Tensor) -> Tensor:
@@ -324,28 +315,27 @@
 
     def __init__(
         self,
         model: Model,
         best_f: Union[float, Tensor],
         posterior_transform: Optional[PosteriorTransform] = None,
         maximize: bool = True,
-        **kwargs,
     ):
         r"""Single-outcome Expected Improvement (analytic).
 
         Args:
             model: A fitted single-outcome model.
             best_f: Either a scalar or a `b`-dim Tensor (batch mode) representing
                 the best function value observed so far (assumed noiseless).
             posterior_transform: A PosteriorTransform. If using a multi-output model,
                 a PosteriorTransform that transforms the multi-output posterior into a
                 single-output posterior is required.
             maximize: If True, consider the problem a maximization problem.
         """
-        super().__init__(model=model, posterior_transform=posterior_transform, **kwargs)
+        super().__init__(model=model, posterior_transform=posterior_transform)
         self.register_buffer("best_f", torch.as_tensor(best_f))
         self.maximize = maximize
 
     @t_batch_mode_transform(expected_q=1)
     def forward(self, X: Tensor) -> Tensor:
         r"""Evaluate Expected Improvement on the candidate set X.
 
@@ -384,28 +374,27 @@
 
     def __init__(
         self,
         model: Model,
         best_f: Union[float, Tensor],
         posterior_transform: Optional[PosteriorTransform] = None,
         maximize: bool = True,
-        **kwargs,
     ):
         r"""Logarithm of single-outcome Expected Improvement (analytic).
 
         Args:
             model: A fitted single-outcome model.
             best_f: Either a scalar or a `b`-dim Tensor (batch mode) representing
                 the best function value observed so far (assumed noiseless).
             posterior_transform: A PosteriorTransform. If using a multi-output model,
                 a PosteriorTransform that transforms the multi-output posterior into a
                 single-output posterior is required.
             maximize: If True, consider the problem a maximization problem.
         """
-        super().__init__(model=model, posterior_transform=posterior_transform, **kwargs)
+        super().__init__(model=model, posterior_transform=posterior_transform)
         self.register_buffer("best_f", torch.as_tensor(best_f))
         self.maximize = maximize
 
     @t_batch_mode_transform(expected_q=1)
     def forward(self, X: Tensor) -> Tensor:
         r"""Evaluate logarithm of Expected Improvement on the candidate set X.
 
@@ -595,15 +584,14 @@
     def __init__(
         self,
         model: GPyTorchModel,
         X_observed: Tensor,
         num_fantasies: int = 20,
         maximize: bool = True,
         posterior_transform: Optional[PosteriorTransform] = None,
-        **kwargs,
     ) -> None:
         r"""Single-outcome Noisy Log Expected Improvement (via fantasies).
 
         Args:
             model: A fitted single-outcome model.
             X_observed: A `n x d` Tensor of observed points that are likely to
                 be the best observed points so far.
@@ -628,17 +616,15 @@
         sampler = SobolQMCNormalSampler(sample_shape=torch.Size([num_fantasies]))
         Y_fantasized = sampler(posterior).squeeze(-1)
         batch_X_observed = X_observed.expand(num_fantasies, *X_observed.shape)
         # The fantasy model will operate in batch mode
         fantasy_model = _get_noiseless_fantasy_model(
             model=model, batch_X_observed=batch_X_observed, Y_fantasized=Y_fantasized
         )
-        super().__init__(
-            model=fantasy_model, posterior_transform=posterior_transform, **kwargs
-        )
+        super().__init__(model=fantasy_model, posterior_transform=posterior_transform)
         best_f, _ = Y_fantasized.max(dim=-1) if maximize else Y_fantasized.min(dim=-1)
         self.best_f, self.maximize = best_f, maximize
 
     @t_batch_mode_transform(expected_q=1)
     def forward(self, X: Tensor) -> Tensor:
         r"""Evaluate logarithm of the mean Expected Improvement on the candidate set X.
 
@@ -754,29 +740,28 @@
 
     def __init__(
         self,
         model: Model,
         beta: Union[float, Tensor],
         posterior_transform: Optional[PosteriorTransform] = None,
         maximize: bool = True,
-        **kwargs,
     ) -> None:
         r"""Single-outcome Upper Confidence Bound.
 
         Args:
             model: A fitted single-outcome GP model (must be in batch mode if
                 candidate sets X will be)
             beta: Either a scalar or a one-dim tensor with `b` elements (batch mode)
                 representing the trade-off parameter between mean and covariance
             posterior_transform: A PosteriorTransform. If using a multi-output model,
                 a PosteriorTransform that transforms the multi-output posterior into a
                 single-output posterior is required.
             maximize: If True, consider the problem a maximization problem.
         """
-        super().__init__(model=model, posterior_transform=posterior_transform, **kwargs)
+        super().__init__(model=model, posterior_transform=posterior_transform)
         self.register_buffer("beta", torch.as_tensor(beta))
         self.maximize = maximize
 
     @t_batch_mode_transform(expected_q=1)
     def forward(self, X: Tensor) -> Tensor:
         r"""Evaluate the Upper Confidence Bound on the candidate set X.
 
@@ -848,27 +833,26 @@
     """
 
     def __init__(
         self,
         model: Model,
         weights: Tensor,
         posterior_transform: Optional[PosteriorTransform] = None,
-        **kwargs,
     ) -> None:
         r"""Scalarized Posterior Mean.
 
         Args:
             model: A fitted single-outcome model.
             weights: A tensor of shape `q` for scalarization. In order to minimize
                 the scalarized posterior mean, pass -weights.
             posterior_transform: A PosteriorTransform. If using a multi-output model,
                 a PosteriorTransform that transforms the multi-output posterior into a
                 single-output posterior is required.
         """
-        super().__init__(model=model, posterior_transform=posterior_transform, **kwargs)
+        super().__init__(model=model, posterior_transform=posterior_transform)
         self.register_buffer("weights", weights)
 
     @t_batch_mode_transform()
     def forward(self, X: Tensor) -> Tensor:
         r"""Evaluate the scalarized posterior mean on the candidate set X.
 
         Args:
```

### Comparing `botorch-0.8.5/botorch/acquisition/cached_cholesky.py` & `botorch-0.9.1/botorch/acquisition/cached_cholesky.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/acquisition/cost_aware.py` & `botorch-0.9.1/botorch/acquisition/cost_aware.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,26 @@
 To be used in a context where there is an objective/cost tradeoff.
 """
 
 from __future__ import annotations
 
 import warnings
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Optional, Union
 
 import torch
 from botorch import settings
-from botorch.acquisition.objective import IdentityMCObjective, MCAcquisitionObjective
+from botorch.acquisition.objective import (
+    GenericMCObjective,
+    IdentityMCObjective,
+    MCAcquisitionObjective,
+)
 from botorch.exceptions.warnings import CostAwareWarning
-from botorch.models.model import Model
+from botorch.models.deterministic import DeterministicModel
+from botorch.models.gpytorch import GPyTorchModel
 from botorch.sampling.base import MCSampler
 from torch import Tensor
 from torch.nn import Module
 
 
 class CostAwareUtility(Module, ABC):
     r"""
@@ -90,70 +95,97 @@
     `weighted utility = mean(u_1 / c_1, ..., u_N / c_N)`.
 
     The cost is additive across multiple elements of a q-batch.
     """
 
     def __init__(
         self,
-        cost_model: Model,
+        cost_model: Union[DeterministicModel, GPyTorchModel],
         use_mean: bool = True,
         cost_objective: Optional[MCAcquisitionObjective] = None,
         min_cost: float = 1e-2,
     ) -> None:
         r"""Cost-aware utility that weights increase in utiltiy by inverse cost.
 
         Args:
-            cost_model: A Model modeling the cost of evaluating a candidate
+            cost_model: A model of the cost of evaluating a candidate
                 set `X`, where `X` are the same features as in the model for the
                 acquisition function this is to be used with. If no cost_objective
                 is specified, the outputs are required to be non-negative.
             use_mean: If True, use the posterior mean, otherwise use posterior
                 samples from the cost model.
             cost_objective: If specified, transform the posterior mean / the
                 posterior samples from the cost model. This can be used e.g. to
                 un-transform predictions/samples of a cost model fit on the
-                log-transformed cost (often done to ensure non-negativity).
+                log-transformed cost (often done to ensure non-negativity). If the
+                cost model is multi-output, then by default this will sum the cost
+                across outputs.
             min_cost: A value used to clamp the cost samples so that they are not
                 too close to zero, which may cause numerical issues.
         Returns:
             The inverse-cost-weighted utiltiy.
         """
         super().__init__()
         if cost_objective is None:
-            cost_objective = IdentityMCObjective()
+            if cost_model.num_outputs == 1:
+                cost_objective = IdentityMCObjective()
+            else:
+                # sum over outputs
+                cost_objective = GenericMCObjective(lambda Y, X: Y.sum(dim=-1))
+
         self.cost_model = cost_model
         self.cost_objective = cost_objective
         self._use_mean = use_mean
         self._min_cost = min_cost
 
     def forward(
         self,
         X: Tensor,
         deltas: Tensor,
         sampler: Optional[MCSampler] = None,
+        X_evaluation_mask: Optional[Tensor] = None,
         **kwargs: Any,
     ) -> Tensor:
         r"""Evaluate the cost function on the candidates and improvements.
 
         Args:
             X: A `batch_shape x q x d`-dim Tensor of with `q` `d`-dim design
                 points each for each t-batch.
             deltas: A `num_fantasies x batch_shape`-dim Tensor of `num_fantasy`
                 samples from the marginal improvement in utility over the
                 current state at `X` for each t-batch.
             sampler: A sampler used for sampling from the posterior of the cost
                 model (required if `use_mean=False`, ignored if `use_mean=True`).
+            X_evaluation_mask: A `q x m`-dim boolean tensor indicating which
+                outcomes should be evaluated for each design in the batch.
 
         Returns:
             A `num_fantasies x batch_shape`-dim Tensor of cost-weighted utilities.
         """
         if not self._use_mean and sampler is None:
             raise RuntimeError("Must provide `sampler` if `use_mean=False`")
-
-        cost_posterior = self.cost_model.posterior(X)
+        if X_evaluation_mask is not None:
+            # TODO: support different evaluation masks for each X. This requires
+            # either passing evaluation_mask to `cost_model.posterior`
+            # or assuming that evalauting `cost_model.posterior(X)` on all
+            # `q` points and then only selecting the costs for relevant points
+            # does not change the cost function for each point. This would not be
+            # true for instance if the incremental cost of evalauting an additional
+            # point decreased as the number of points increased.
+            if not all(
+                torch.equal(X_evaluation_mask[0], X_evaluation_mask[i])
+                for i in range(1, X_evaluation_mask.shape[0])
+            ):
+                raise NotImplementedError(
+                    "Currently, all candidates must be evaluated on the same outputs."
+                )
+            output_indices = X_evaluation_mask[0].nonzero().view(-1).tolist()
+        else:
+            output_indices = None
+        cost_posterior = self.cost_model.posterior(X, output_indices=output_indices)
         if self._use_mean:
             cost = cost_posterior.mean  # batch_shape x q x m'
         else:
             # This will be of shape num_fantasies x batch_shape x q x m'
             cost = sampler(cost_posterior)
             # TODO: Make sure this doesn't change base samples in-place
         cost = self.cost_objective(cost)
```

### Comparing `botorch-0.8.5/botorch/acquisition/fixed_feature.py` & `botorch-0.9.1/botorch/acquisition/fixed_feature.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,43 @@
 
 import torch
 from botorch.acquisition.acquisition import AcquisitionFunction
 from torch import Tensor
 from torch.nn import Module
 
 
+def get_dtype_of_sequence(values: Sequence[Union[Tensor, float]]) -> torch.dtype:
+    """
+    Return torch.float32 if everything is single-precision and torch.float64
+    otherwise.
+
+    Numbers (non-tensors) are double-precision.
+    """
+
+    def _is_single(value: Union[Tensor, float]) -> bool:
+        return isinstance(value, Tensor) and value.dtype == torch.float32
+
+    all_single_precision = all(_is_single(value) for value in values)
+    return torch.float32 if all_single_precision else torch.float64
+
+
+def get_device_of_sequence(values: Sequence[Union[Tensor, float]]) -> torch.dtype:
+    """
+    CPU if everything is on the CPU; Cuda otherwise.
+
+    Numbers (non-tensors) are considered to be on the CPU.
+    """
+
+    def _is_cuda(value: Union[Tensor, float]) -> bool:
+        return hasattr(value, "device") and value.device == torch.device("cuda")
+
+    any_cuda = any(_is_cuda(value) for value in values)
+    return torch.device("cuda") if any_cuda else torch.device("cpu")
+
+
 class FixedFeatureAcquisitionFunction(AcquisitionFunction):
     """A wrapper around AquisitionFunctions to fix a subset of features.
 
     Example:
         >>> model = SingleTaskGP(train_X, train_Y)  # d = 5
         >>> qEI = qExpectedImprovement(model, best_f=0.0)
         >>> columns = [2, 4]
@@ -54,35 +83,33 @@
                 `q`-batch dimensions, e.g. a list of length `d_f` if values
                 are the same across all `t` and `q`-batch dimensions, or a
                 combination of `Tensor`s and numbers which can be broadcasted
                 to form a tensor with trailing dimension size of `d_f`.
         """
         Module.__init__(self)
         self.acq_func = acq_function
-        dtype = torch.float
-        device = torch.device("cpu")
         self.d = d
+
         if isinstance(values, Tensor):
             new_values = values.detach().clone()
         else:
+
+            dtype = get_dtype_of_sequence(values)
+            device = get_device_of_sequence(values)
+
             new_values = []
             for value in values:
                 if isinstance(value, Number):
-                    new_values.append(torch.tensor([float(value)]))
+                    value = torch.tensor([value], dtype=dtype)
                 else:
-                    # if any value uses double, use double for all values
-                    # likewise if any value uses cuda, use cuda for all values
-                    dtype = value.dtype if value.dtype == torch.double else dtype
-                    device = value.device if value.device.type == "cuda" else device
                     if value.ndim == 0:  # since we can't broadcast with zero-d tensors
                         value = value.unsqueeze(0)
-                    new_values.append(value.detach().clone())
-            # move all values to same device
-            for i, val in enumerate(new_values):
-                new_values[i] = val.to(dtype=dtype, device=device)
+                    value = value.detach().clone()
+
+                new_values.append(value.to(dtype=dtype, device=device))
 
             # There are 3 cases for when `values` is a `Sequence`.
             # 1) `values` == list of floats as earlier.
             # 2) `values` == combination of floats and `Tensor`s.
             # 3) `values` == a list of `Tensor`s.
             # For 1), the below step creates a vector of length `len(values)`
             # For 2), the below step creates a `Tensor` of shape `batch_shape x q x d_f`
```

### Comparing `botorch-0.8.5/botorch/acquisition/input_constructors.py` & `botorch-0.9.1/botorch/acquisition/input_constructors.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 r"""
 A registry of helpers for generating inputs to acquisition function
 constructors programmatically from a consistent input format.
 """
 
 from __future__ import annotations
 
-import warnings
 from typing import (
     Any,
     Callable,
     Dict,
     Hashable,
     Iterable,
     List,
@@ -44,14 +43,20 @@
 from botorch.acquisition.cost_aware import InverseCostWeightedUtility
 from botorch.acquisition.fixed_feature import FixedFeatureAcquisitionFunction
 from botorch.acquisition.joint_entropy_search import qJointEntropySearch
 from botorch.acquisition.knowledge_gradient import (
     qKnowledgeGradient,
     qMultiFidelityKnowledgeGradient,
 )
+from botorch.acquisition.logei import (
+    qLogExpectedImprovement,
+    qLogNoisyExpectedImprovement,
+    TAU_MAX,
+    TAU_RELU,
+)
 from botorch.acquisition.max_value_entropy_search import (
     qMaxValueEntropy,
     qMultiFidelityMaxValueEntropy,
 )
 from botorch.acquisition.monte_carlo import (
     qExpectedImprovement,
     qNoisyExpectedImprovement,
@@ -68,24 +73,22 @@
 from botorch.acquisition.multi_objective.objective import (
     AnalyticMultiOutputObjective,
     IdentityAnalyticMultiOutputObjective,
     IdentityMCMultiOutputObjective,
 )
 from botorch.acquisition.multi_objective.utils import get_default_partitioning_alpha
 from botorch.acquisition.objective import (
-    AcquisitionObjective,
     IdentityMCObjective,
     MCAcquisitionObjective,
     PosteriorTransform,
-    ScalarizedObjective,
-    ScalarizedPosteriorTransform,
 )
 from botorch.acquisition.preference import AnalyticExpectedUtilityOfBestOption
 from botorch.acquisition.risk_measures import RiskMeasureMCObjective
 from botorch.acquisition.utils import (
+    compute_best_feasible_objective,
     expand_trace_observations,
     get_optimal_samples,
     project_to_target_fidelity,
 )
 from botorch.exceptions.errors import UnsupportedError
 from botorch.models.cost import AffineFidelityCostModel
 from botorch.models.deterministic import FixedSingleSampleModel
@@ -209,76 +212,37 @@
 def _register_acqf_input_constructor(
     acqf_cls: Type[AcquisitionFunction],
     input_constructor: Callable[..., Dict[str, Any]],
 ) -> None:
     ACQF_INPUT_CONSTRUCTOR_REGISTRY[acqf_cls] = input_constructor
 
 
-# ------------------------- Deprecation Helpers ------------------------- #
-
-
-def _deprecate_objective_arg(
-    posterior_transform: Optional[PosteriorTransform] = None,
-    objective: Optional[AcquisitionObjective] = None,
-) -> Optional[PosteriorTransform]:
-    if posterior_transform is not None:
-        if objective is None:
-            return posterior_transform
-        else:
-            raise RuntimeError(
-                "Got both a non-MC objective (DEPRECATED) and a posterior "
-                "transform. Use only a posterior transform instead."
-            )
-    elif objective is not None:
-        warnings.warn(
-            "The `objective` argument to AnalyticAcquisitionFunctions is deprecated "
-            "and will be removed in the next version. Use `posterior_transform` "
-            "instead.",
-            DeprecationWarning,
-        )
-        if not isinstance(objective, ScalarizedObjective):
-            raise UnsupportedError(
-                "Analytic acquisition functions only support ScalarizedObjective "
-                "(DEPRECATED) type objectives."
-            )
-        return ScalarizedPosteriorTransform(
-            weights=objective.weights, offset=objective.offset
-        )
-    else:
-        return None
-
-
 # --------------------- Input argument constructors --------------------- #
 
 
 @acqf_input_constructor(PosteriorMean)
 def construct_inputs_analytic_base(
     model: Model,
     training_data: MaybeDict[SupervisedDataset],
     posterior_transform: Optional[PosteriorTransform] = None,
     **kwargs: Any,
 ) -> Dict[str, Any]:
     r"""Construct kwargs for basic analytic acquisition functions.
 
     Args:
         model: The model to be used in the acquisition function.
-        training_data: Dataset(s) used to train the model.
+        training_data: Dataset(s) used to train the model. Not used.
         posterior_transform: The posterior transform to be used in the
             acquisition function.
+        kwargs: Not used.
 
     Returns:
         A dict mapping kwarg names of the constructor to values.
     """
-    return {
-        "model": model,
-        "posterior_transform": _deprecate_objective_arg(
-            posterior_transform=posterior_transform,
-            objective=kwargs.get("objective"),
-        ),
-    }
+    return {"model": model, "posterior_transform": posterior_transform}
 
 
 @acqf_input_constructor(
     ExpectedImprovement,
     LogExpectedImprovement,
     ProbabilityOfImprovement,
     LogProbabilityOfImprovement,
@@ -297,28 +261,27 @@
         model: The model to be used in the acquisition function.
         training_data: Dataset(s) used to train the model.
             Used to determine default value for `best_f`.
         best_f: Threshold above (or below) which improvement is defined.
         posterior_transform: The posterior transform to be used in the
             acquisition function.
         maximize: If True, consider the problem a maximization problem.
+        kwargs: Not used.
 
     Returns:
         A dict mapping kwarg names of the constructor to values.
     """
     base_inputs = construct_inputs_analytic_base(
         model=model,
         training_data=training_data,
         posterior_transform=posterior_transform,
-        **kwargs,
     )
     if best_f is None:
         best_f = get_best_f_analytic(
             training_data=training_data,
-            objective=kwargs.get("objective"),
             posterior_transform=posterior_transform,
         )
 
     return {**base_inputs, "best_f": best_f, "maximize": maximize}
 
 
 @acqf_input_constructor(UpperConfidenceBound)
@@ -330,29 +293,29 @@
     maximize: bool = True,
     **kwargs: Any,
 ) -> Dict[str, Any]:
     r"""Construct kwargs for `UpperConfidenceBound`.
 
     Args:
         model: The model to be used in the acquisition function.
-        training_data: Dataset(s) used to train the model.
+        training_data: Dataset(s) used to train the model. Not used.
         posterior_transform: The posterior transform to be used in the
             acquisition function.
         beta: Either a scalar or a one-dim tensor with `b` elements (batch mode)
             representing the trade-off parameter between mean and covariance
         maximize: If True, consider the problem a maximization problem.
+        kwargs: Not used.
 
     Returns:
         A dict mapping kwarg names of the constructor to values.
     """
     base_inputs = construct_inputs_analytic_base(
         model=model,
         training_data=training_data,
         posterior_transform=posterior_transform,
-        **kwargs,
     )
     return {**base_inputs, "beta": beta, "maximize": maximize}
 
 
 @acqf_input_constructor(
     ConstrainedExpectedImprovement, LogConstrainedExpectedImprovement
 )
@@ -370,14 +333,15 @@
         model: The model to be used in the acquisition function.
         training_data: Dataset(s) used to train the model.
         objective_index: The index of the objective.
         constraints: A dictionary of the form `{i: [lower, upper]}`, where
             `i` is the output index, and `lower` and `upper` are lower and upper
             bounds on that output (resp. interpreted as -Inf / Inf if None)
         maximize: If True, consider the problem a maximization problem.
+        kwargs: Additional keyword arguments.
 
     Returns:
         A dict mapping kwarg names of the constructor to values.
     """
     # TODO: Implement best point computation from training data
     # best_f =
     # return {
@@ -403,43 +367,40 @@
     Args:
         model: The model to be used in the acquisition function.
         training_data: Dataset(s) used to train the model.
         num_fantasies: The number of fantasies to generate. The higher this
             number the more accurate the model (at the expense of model
             complexity and performance).
         maximize: If True, consider the problem a maximization problem.
+        kwargs: Not used.
 
     Returns:
         A dict mapping kwarg names of the constructor to values.
     """
     # TODO: Add prune_baseline functionality as for qNEI
     X = _get_dataset_field(training_data, "X", first_only=True, assert_shared=True)
     return {
         "model": model,
         "X_observed": X(),
         "num_fantasies": num_fantasies,
         "maximize": maximize,
     }
 
 
-@acqf_input_constructor(qSimpleRegret)
-def construct_inputs_mc_base(
+def _construct_inputs_mc_base(
     model: Model,
-    training_data: MaybeDict[SupervisedDataset],
     objective: Optional[MCAcquisitionObjective] = None,
     posterior_transform: Optional[PosteriorTransform] = None,
     X_pending: Optional[Tensor] = None,
     sampler: Optional[MCSampler] = None,
-    **kwargs: Any,
 ) -> Dict[str, Any]:
     r"""Construct kwargs for basic MC acquisition functions.
 
     Args:
         model: The model to be used in the acquisition function.
-        training_data: Dataset(s) used to train the model.
         objective: The objective to be used in the acquisition function.
         posterior_transform: The posterior transform to be used in the
             acquisition function.
         X_pending: A `batch_shape, m x d`-dim Tensor of `m` design points
             that have points that have been submitted for function evaluation
             but have not yet been evaluated.
         sampler: The sampler used to draw base samples. If omitted, uses
@@ -453,24 +414,63 @@
         "objective": objective,
         "posterior_transform": posterior_transform,
         "X_pending": X_pending,
         "sampler": sampler,
     }
 
 
+@acqf_input_constructor(qSimpleRegret)
+def construct_inputs_qSimpleRegret(
+    model: Model,
+    training_data: MaybeDict[SupervisedDataset],
+    objective: Optional[MCAcquisitionObjective] = None,
+    posterior_transform: Optional[PosteriorTransform] = None,
+    X_pending: Optional[Tensor] = None,
+    sampler: Optional[MCSampler] = None,
+    **kwargs: Any,
+) -> Dict[str, Any]:
+    r"""Construct kwargs for qSimpleRegret.
+
+    Args:
+        model: The model to be used in the acquisition function.
+        training_data: Dataset(s) used to train the model. Not used.
+        objective: The objective to be used in the acquisition function.
+        posterior_transform: The posterior transform to be used in the
+            acquisition function.
+        X_pending: A `batch_shape, m x d`-dim Tensor of `m` design points
+            that have points that have been submitted for function evaluation
+            but have not yet been evaluated.
+        sampler: The sampler used to draw base samples. If omitted, uses
+            the acquisition functions's default sampler.
+        kwargs: Not used.
+
+    Returns:
+        A dict mapping kwarg names of the constructor to values.
+    """
+    return _construct_inputs_mc_base(
+        model=model,
+        objective=objective,
+        posterior_transform=posterior_transform,
+        X_pending=X_pending,
+        sampler=sampler,
+    )
+
+
 @acqf_input_constructor(qExpectedImprovement)
 def construct_inputs_qEI(
     model: Model,
     training_data: MaybeDict[SupervisedDataset],
     objective: Optional[MCAcquisitionObjective] = None,
     posterior_transform: Optional[PosteriorTransform] = None,
     X_pending: Optional[Tensor] = None,
     sampler: Optional[MCSampler] = None,
     best_f: Optional[Union[float, Tensor]] = None,
-    **kwargs: Any,
+    constraints: Optional[List[Callable[[Tensor], Tensor]]] = None,
+    eta: Union[Tensor, float] = 1e-3,
+    **ignored: Any,
 ) -> Dict[str, Any]:
     r"""Construct kwargs for the `qExpectedImprovement` constructor.
 
     Args:
         model: The model to be used in the acquisition function.
         training_data: Dataset(s) used to train the model.
         objective: The objective to be used in the acquisition function.
@@ -478,47 +478,125 @@
             acquisition function.
         X_pending: A `m x d`-dim Tensor of `m` design points that have been
             submitted for function evaluation but have not yet been evaluated.
             Concatenated into X upon forward call.
         sampler: The sampler used to draw base samples. If omitted, uses
             the acquisition functions's default sampler.
         best_f: Threshold above (or below) which improvement is defined.
+        constraints: A list of constraint callables which map a Tensor of posterior
+            samples of dimension `sample_shape x batch-shape x q x m`-dim to a
+            `sample_shape x batch-shape x q`-dim Tensor. The associated constraints
+            are considered satisfied if the output is less than zero.
+        eta: Temperature parameter(s) governing the smoothness of the sigmoid
+            approximation to the constraint indicators. For more details, on this
+            parameter, see the docs of `compute_smoothed_feasibility_indicator`.
+        ignored: Not used.
+
     Returns:
         A dict mapping kwarg names of the constructor to values.
     """
-    base_inputs = construct_inputs_mc_base(
+    base_inputs = _construct_inputs_mc_base(
         model=model,
-        training_data=training_data,
         objective=objective,
         posterior_transform=posterior_transform,
         sampler=sampler,
         X_pending=X_pending,
     )
     if best_f is None:
         best_f = get_best_f_mc(
             training_data=training_data,
             objective=objective,
             posterior_transform=posterior_transform,
+            constraints=constraints,
+            model=model,
         )
 
-    return {**base_inputs, "best_f": best_f}
+    return {**base_inputs, "best_f": best_f, "constraints": constraints, "eta": eta}
+
+
+@acqf_input_constructor(qLogExpectedImprovement)
+def construct_inputs_qLogEI(
+    model: Model,
+    training_data: MaybeDict[SupervisedDataset],
+    objective: Optional[MCAcquisitionObjective] = None,
+    posterior_transform: Optional[PosteriorTransform] = None,
+    X_pending: Optional[Tensor] = None,
+    sampler: Optional[MCSampler] = None,
+    best_f: Optional[Union[float, Tensor]] = None,
+    constraints: Optional[List[Callable[[Tensor], Tensor]]] = None,
+    eta: Union[Tensor, float] = 1e-3,
+    fat: bool = True,
+    tau_max: float = TAU_MAX,
+    tau_relu: float = TAU_RELU,
+    **ignored: Any,
+) -> Dict[str, Any]:
+    r"""Construct kwargs for the `qExpectedImprovement` constructor.
+
+    Args:
+        model: The model to be used in the acquisition function.
+        training_data: Dataset(s) used to train the model.
+        objective: The objective to be used in the acquisition function.
+        posterior_transform: The posterior transform to be used in the
+            acquisition function.
+        X_pending: A `m x d`-dim Tensor of `m` design points that have been
+            submitted for function evaluation but have not yet been evaluated.
+            Concatenated into X upon forward call.
+        sampler: The sampler used to draw base samples. If omitted, uses
+            the acquisition functions's default sampler.
+        best_f: Threshold above (or below) which improvement is defined.
+        constraints: A list of constraint callables which map a Tensor of posterior
+            samples of dimension `sample_shape x batch-shape x q x m`-dim to a
+            `sample_shape x batch-shape x q`-dim Tensor. The associated constraints
+            are considered satisfied if the output is less than zero.
+        eta: Temperature parameter(s) governing the smoothness of the sigmoid
+            approximation to the constraint indicators. For more details, on this
+            parameter, see the docs of `compute_smoothed_feasibility_indicator`.
+        fat: Toggles the logarithmic / linear asymptotic behavior of the smooth
+            approximation to the ReLU.
+        tau_max: Temperature parameter controlling the sharpness of the smooth
+            approximations to max.
+        tau_relu: Temperature parameter controlling the sharpness of the smooth
+            approximations to ReLU.
+        ignored: Not used.
+
+    Returns:
+        A dict mapping kwarg names of the constructor to values.
+    """
+    return {
+        **construct_inputs_qEI(
+            model=model,
+            training_data=training_data,
+            objective=objective,
+            posterior_transform=posterior_transform,
+            X_pending=X_pending,
+            sampler=sampler,
+            best_f=best_f,
+            constraints=constraints,
+            eta=eta,
+        ),
+        "fat": fat,
+        "tau_max": tau_max,
+        "tau_relu": tau_relu,
+    }
 
 
 @acqf_input_constructor(qNoisyExpectedImprovement)
 def construct_inputs_qNEI(
     model: Model,
     training_data: MaybeDict[SupervisedDataset],
     objective: Optional[MCAcquisitionObjective] = None,
     posterior_transform: Optional[PosteriorTransform] = None,
     X_pending: Optional[Tensor] = None,
     sampler: Optional[MCSampler] = None,
     X_baseline: Optional[Tensor] = None,
     prune_baseline: Optional[bool] = True,
     cache_root: Optional[bool] = True,
-    **kwargs: Any,
+    constraints: Optional[List[Callable[[Tensor], Tensor]]] = None,
+    eta: Union[Tensor, float] = 1e-3,
+    **ignored: Any,
 ) -> Dict[str, Any]:
     r"""Construct kwargs for the `qNoisyExpectedImprovement` constructor.
 
     Args:
         model: The model to be used in the acquisition function.
         training_data: Dataset(s) used to train the model.
         objective: The objective to be used in the acquisition function.
@@ -532,54 +610,140 @@
         X_baseline: A `batch_shape x r x d`-dim Tensor of `r` design points
             that have already been observed. These points are considered as
             the potential best design point. If omitted, checks that all
             training_data have the same input features and take the first `X`.
         prune_baseline: If True, remove points in `X_baseline` that are
             highly unlikely to be the best point. This can significantly
             improve performance and is generally recommended.
+        constraints: A list of constraint callables which map a Tensor of posterior
+            samples of dimension `sample_shape x batch-shape x q x m`-dim to a
+            `sample_shape x batch-shape x q`-dim Tensor. The associated constraints
+            are considered satisfied if the output is less than zero.
+        eta: Temperature parameter(s) governing the smoothness of the sigmoid
+            approximation to the constraint indicators. For more details, on this
+            parameter, see the docs of `compute_smoothed_feasibility_indicator`.
+        ignored: Not used.
 
     Returns:
         A dict mapping kwarg names of the constructor to values.
     """
-    base_inputs = construct_inputs_mc_base(
+    base_inputs = _construct_inputs_mc_base(
         model=model,
-        training_data=training_data,
         objective=objective,
         posterior_transform=posterior_transform,
         sampler=sampler,
         X_pending=X_pending,
     )
     if X_baseline is None:
         X_baseline = _get_dataset_field(
             training_data,
             fieldname="X",
             transform=lambda field: field(),
             assert_shared=True,
             first_only=True,
         )
-
     return {
         **base_inputs,
         "X_baseline": X_baseline,
         "prune_baseline": prune_baseline,
         "cache_root": cache_root,
+        "constraints": constraints,
+        "eta": eta,
+    }
+
+
+@acqf_input_constructor(qLogNoisyExpectedImprovement)
+def construct_inputs_qLogNEI(
+    model: Model,
+    training_data: MaybeDict[SupervisedDataset],
+    objective: Optional[MCAcquisitionObjective] = None,
+    posterior_transform: Optional[PosteriorTransform] = None,
+    X_pending: Optional[Tensor] = None,
+    sampler: Optional[MCSampler] = None,
+    X_baseline: Optional[Tensor] = None,
+    prune_baseline: Optional[bool] = True,
+    cache_root: Optional[bool] = True,
+    constraints: Optional[List[Callable[[Tensor], Tensor]]] = None,
+    eta: Union[Tensor, float] = 1e-3,
+    fat: bool = True,
+    tau_max: float = TAU_MAX,
+    tau_relu: float = TAU_RELU,
+    **ignored: Any,
+):
+    r"""Construct kwargs for the `qNoisyExpectedImprovement` constructor.
+
+    Args:
+        model: The model to be used in the acquisition function.
+        training_data: Dataset(s) used to train the model.
+        objective: The objective to be used in the acquisition function.
+        posterior_transform: The posterior transform to be used in the
+            acquisition function.
+        X_pending: A `m x d`-dim Tensor of `m` design points that have been
+            submitted for function evaluation but have not yet been evaluated.
+            Concatenated into X upon forward call.
+        sampler: The sampler used to draw base samples. If omitted, uses
+            the acquisition functions's default sampler.
+        X_baseline: A `batch_shape x r x d`-dim Tensor of `r` design points
+            that have already been observed. These points are considered as
+            the potential best design point. If omitted, checks that all
+            training_data have the same input features and take the first `X`.
+        prune_baseline: If True, remove points in `X_baseline` that are
+            highly unlikely to be the best point. This can significantly
+            improve performance and is generally recommended.
+        constraints: A list of constraint callables which map a Tensor of posterior
+            samples of dimension `sample_shape x batch-shape x q x m`-dim to a
+            `sample_shape x batch-shape x q`-dim Tensor. The associated constraints
+            are considered satisfied if the output is less than zero.
+        eta: Temperature parameter(s) governing the smoothness of the sigmoid
+            approximation to the constraint indicators. For more details, on this
+            parameter, see the docs of `compute_smoothed_feasibility_indicator`.
+        fat: Toggles the logarithmic / linear asymptotic behavior of the smooth
+            approximation to the ReLU.
+        tau_max: Temperature parameter controlling the sharpness of the smooth
+            approximations to max.
+        tau_relu: Temperature parameter controlling the sharpness of the smooth
+            approximations to ReLU.
+        ignored: Not used.
+
+    Returns:
+        A dict mapping kwarg names of the constructor to values.
+    """
+    return {
+        **construct_inputs_qNEI(
+            model=model,
+            training_data=training_data,
+            objective=objective,
+            posterior_transform=posterior_transform,
+            X_pending=X_pending,
+            sampler=sampler,
+            X_baseline=X_baseline,
+            prune_baseline=prune_baseline,
+            cache_root=cache_root,
+            constraint=constraints,
+            eta=eta,
+        ),
+        "fat": fat,
+        "tau_max": tau_max,
+        "tau_relu": tau_relu,
     }
 
 
 @acqf_input_constructor(qProbabilityOfImprovement)
 def construct_inputs_qPI(
     model: Model,
     training_data: MaybeDict[SupervisedDataset],
     objective: Optional[MCAcquisitionObjective] = None,
     posterior_transform: Optional[PosteriorTransform] = None,
     X_pending: Optional[Tensor] = None,
     sampler: Optional[MCSampler] = None,
     tau: float = 1e-3,
     best_f: Optional[Union[float, Tensor]] = None,
-    **kwargs: Any,
+    constraints: Optional[List[Callable[[Tensor], Tensor]]] = None,
+    eta: Union[Tensor, float] = 1e-3,
+    **ignored: Any,
 ) -> Dict[str, Any]:
     r"""Construct kwargs for the `qProbabilityOfImprovement` constructor.
 
     Args:
         model: The model to be used in the acquisition function.
         training_data: Dataset(s) used to train the model.
         objective: The objective to be used in the acquisition function.
@@ -593,42 +757,61 @@
         tau: The temperature parameter used in the sigmoid approximation
             of the step function. Smaller values yield more accurate
             approximations of the function, but result in gradients
             estimates with higher variance.
         best_f: The best objective value observed so far (assumed noiseless). Can
             be a `batch_shape`-shaped tensor, which in case of a batched model
             specifies potentially different values for each element of the batch.
+        constraints: A list of constraint callables which map a Tensor of posterior
+            samples of dimension `sample_shape x batch-shape x q x m`-dim to a
+            `sample_shape x batch-shape x q`-dim Tensor. The associated constraints
+            are considered satisfied if the output is less than zero.
+        eta: Temperature parameter(s) governing the smoothness of the sigmoid
+            approximation to the constraint indicators. For more details, on this
+            parameter, see the docs of `compute_smoothed_feasibility_indicator`.
+        ignored: Not used.
+
     Returns:
         A dict mapping kwarg names of the constructor to values.
     """
     if best_f is None:
-        best_f = get_best_f_mc(training_data=training_data, objective=objective)
-
-    base_inputs = construct_inputs_mc_base(
+        best_f = get_best_f_mc(
+            training_data=training_data,
+            objective=objective,
+            posterior_transform=posterior_transform,
+            constraints=constraints,
+            model=model,
+        )
+    base_inputs = _construct_inputs_mc_base(
         model=model,
-        training_data=training_data,
         objective=objective,
         posterior_transform=posterior_transform,
         sampler=sampler,
         X_pending=X_pending,
     )
 
-    return {**base_inputs, "tau": tau, "best_f": best_f}
+    return {
+        **base_inputs,
+        "tau": tau,
+        "best_f": best_f,
+        "constraints": constraints,
+        "eta": eta,
+    }
 
 
 @acqf_input_constructor(qUpperConfidenceBound)
 def construct_inputs_qUCB(
     model: Model,
     training_data: MaybeDict[SupervisedDataset],
     objective: Optional[MCAcquisitionObjective] = None,
     posterior_transform: Optional[PosteriorTransform] = None,
     X_pending: Optional[Tensor] = None,
     sampler: Optional[MCSampler] = None,
     beta: float = 0.2,
-    **kwargs: Any,
+    **ignored: Any,
 ) -> Dict[str, Any]:
     r"""Construct kwargs for the `qUpperConfidenceBound` constructor.
 
     Args:
         model: The model to be used in the acquisition function.
         training_data: Dataset(s) used to train the model.
         objective: The objective to be used in the acquisition function.
@@ -636,21 +819,21 @@
             acquisition function.
         X_pending: A `m x d`-dim Tensor of `m` design points that have been
             submitted for function evaluation but have not yet been evaluated.
             Concatenated into X upon forward call.
         sampler: The sampler used to draw base samples. If omitted, uses
             the acquisition functions's default sampler.
         beta: Controls tradeoff between mean and standard deviation in UCB.
+        ignored: Not used.
 
     Returns:
         A dict mapping kwarg names of the constructor to values.
     """
-    base_inputs = construct_inputs_mc_base(
+    base_inputs = _construct_inputs_mc_base(
         model=model,
-        training_data=training_data,
         objective=objective,
         posterior_transform=posterior_transform,
         sampler=sampler,
         X_pending=X_pending,
     )
     return {**base_inputs, "beta": beta}
 
@@ -799,15 +982,14 @@
         X_baseline = _get_dataset_field(
             training_data,
             fieldname="X",
             transform=lambda field: field(),
             first_only=True,
             assert_shared=True,
         )
-
     # This selects the objectives (a subset of the outcomes) and set each
     # objective threhsold to have the proper optimization direction.
     if objective is None:
         objective = IdentityMCMultiOutputObjective()
 
     outcome_constraints = kwargs.pop("outcome_constraints", None)
     if outcome_constraints is None:
@@ -827,25 +1009,27 @@
         )
 
     if isinstance(objective, RiskMeasureMCObjective):
         ref_point = objective.preprocessing_function(objective_thresholds)
     else:
         ref_point = objective(objective_thresholds)
 
+    num_objectives = objective_thresholds[~torch.isnan(objective_thresholds)].shape[0]
+
     return {
         "model": model,
         "ref_point": ref_point,
         "X_baseline": X_baseline,
         "sampler": sampler,
         "objective": objective,
         "constraints": cons_tfs,
         "X_pending": kwargs.get("X_pending"),
         "eta": kwargs.get("eta", 1e-3),
         "prune_baseline": kwargs.get("prune_baseline", True),
-        "alpha": kwargs.get("alpha", get_default_partitioning_alpha(model.num_outputs)),
+        "alpha": kwargs.get("alpha", get_default_partitioning_alpha(num_objectives)),
         "cache_pending": kwargs.get("cache_pending", True),
         "max_iep": kwargs.get("max_iep", 0),
         "incremental_nehvi": kwargs.get("incremental_nehvi", True),
         "cache_root": kwargs.get("cache_root", True),
     }
 
 
@@ -856,19 +1040,17 @@
     bounds: List[Tuple[float, float]],
     objective: Optional[MCAcquisitionObjective] = None,
     posterior_transform: Optional[PosteriorTransform] = None,
     candidate_size: int = 1000,
     **kwargs: Any,
 ) -> Dict[str, Any]:
     r"""Construct kwargs for `qMaxValueEntropy` constructor."""
-    inputs_mc = construct_inputs_mc_base(
+    inputs_mc = _construct_inputs_mc_base(
         model=model,
-        training_data=training_data,
         objective=objective,
-        **kwargs,
     )
 
     X = _get_dataset_field(training_data, "X", first_only=True)
     _kw = {"device": X.device, "dtype": X.dtype}
     _rvs = torch.rand(candidate_size, len(bounds), **_kw)
     _bounds = torch.tensor(bounds, **_kw).transpose(0, 1)
     return {
@@ -927,30 +1109,27 @@
     posterior_transform: Optional[PosteriorTransform] = None,
     target_fidelities: Optional[Dict[int, float]] = None,
     num_fantasies: int = 64,
     **kwargs: Any,
 ) -> Dict[str, Any]:
     r"""Construct kwargs for `qKnowledgeGradient` constructor."""
 
-    inputs_mc = construct_inputs_mc_base(
+    inputs_mc = _construct_inputs_mc_base(
         model=model,
-        training_data=training_data,
         objective=objective,
         posterior_transform=posterior_transform,
-        **kwargs,
     )
 
     X = _get_dataset_field(training_data, "X", first_only=True)
     _bounds = torch.tensor(bounds, dtype=X.dtype, device=X.device)
 
     _, current_value = optimize_objective(
         model=model,
         bounds=_bounds.t(),
         q=1,
-        target_fidelities=target_fidelities,
         objective=objective,
         posterior_transform=posterior_transform,
         **kwargs,
     )
 
     return {
         **inputs_mc,
@@ -1021,15 +1200,14 @@
     _bounds = torch.tensor(bounds, dtype=X.dtype, device=X.device)
     _, current_value = optimize_objective(
         model=model,
         bounds=_bounds.t(),
         q=1,
         objective=objective,
         posterior_transform=posterior_transform,
-        target_fidelities=target_fidelities,
         **kwargs,
     )
 
     return {
         **inputs_mf,
         **inputs_qmes,
         "current_value": current_value.detach().cpu().max(),
@@ -1054,77 +1232,79 @@
 
     Returns:
         A dict mapping kwarg names of the constructor to values.
     """
     # construct a deterministic fixed single sample model from `model`
     # i.e., performing EUBO-zeta by default as described
     # in https://arxiv.org/abs/2203.11382
-    w = torch.randn(model.num_outputs) * sample_multiplier
+    # using pref_model.dim instead of model.num_outputs here as MTGP's
+    # num_outputs could be tied to the number of tasks
+    w = torch.randn(pref_model.dim) * sample_multiplier
     one_sample_outcome_model = FixedSingleSampleModel(model=model, w=w)
 
     return {
         "pref_model": pref_model,
         "outcome_model": one_sample_outcome_model,
         "previous_winner": previous_winner,
     }
 
 
 def get_best_f_analytic(
     training_data: MaybeDict[SupervisedDataset],
     posterior_transform: Optional[PosteriorTransform] = None,
-    **kwargs,
 ) -> Tensor:
     if isinstance(training_data, dict) and not _field_is_shared(
         training_data, fieldname="X"
     ):
         raise NotImplementedError("Currently only block designs are supported.")
 
     Y = _get_dataset_field(
         training_data,
         fieldname="Y",
         transform=lambda field: field(),
         join_rule=lambda field_tensors: torch.cat(field_tensors, dim=-1),
     )
 
-    posterior_transform = _deprecate_objective_arg(
-        posterior_transform=posterior_transform, objective=kwargs.get("objective", None)
-    )
     if posterior_transform is not None:
         return posterior_transform.evaluate(Y).max(-1).values
     if Y.shape[-1] > 1:
         raise NotImplementedError(
             "Analytic acquisition functions currently only work with "
             "multi-output models if provided with a `ScalarizedObjective`."
         )
     return Y.max(-2).values.squeeze(-1)
 
 
 def get_best_f_mc(
     training_data: MaybeDict[SupervisedDataset],
     objective: Optional[MCAcquisitionObjective] = None,
     posterior_transform: Optional[PosteriorTransform] = None,
+    constraints: Optional[List[Callable[[Tensor], Tensor]]] = None,
+    model: Optional[Model] = None,
 ) -> Tensor:
     if isinstance(training_data, dict) and not _field_is_shared(
         training_data, fieldname="X"
     ):
         raise NotImplementedError("Currently only block designs are supported.")
 
+    X_baseline = _get_dataset_field(
+        training_data,
+        fieldname="X",
+        transform=lambda field: field(),
+        assert_shared=True,
+        first_only=True,
+    )
+
     Y = _get_dataset_field(
         training_data,
         fieldname="Y",
         transform=lambda field: field(),
         join_rule=lambda field_tensors: torch.cat(field_tensors, dim=-1),
-    )
+    )  # batch_shape x n x d
 
-    posterior_transform = _deprecate_objective_arg(
-        posterior_transform=posterior_transform,
-        objective=objective
-        if not isinstance(objective, MCAcquisitionObjective)
-        else None,
-    )
     if posterior_transform is not None:
         # retain the original tensor dimension since objective expects explicit
         # output dimension.
         Y_dim = Y.dim()
         Y = posterior_transform.evaluate(Y)
         if Y.dim() < Y_dim:
             Y = Y.unsqueeze(-1)
@@ -1132,30 +1312,38 @@
         if Y.shape[-1] > 1:
             raise UnsupportedError(
                 "Acquisition functions require an objective when "
                 "used with multi-output models (execpt for multi-objective"
                 "acquisition functions)."
             )
         objective = IdentityMCObjective()
-    return objective(Y).max(-1).values
+    obj = objective(Y, X=X_baseline)  # batch_shape x n
+    return compute_best_feasible_objective(
+        samples=Y,
+        obj=obj,
+        constraints=constraints,
+        model=model,
+        objective=objective,
+        posterior_transform=posterior_transform,
+        X_baseline=X_baseline,
+    )
 
 
 def optimize_objective(
     model: Model,
     bounds: Tensor,
     q: int,
     objective: Optional[MCAcquisitionObjective] = None,
     posterior_transform: Optional[PosteriorTransform] = None,
     linear_constraints: Optional[Tuple[Tensor, Tensor]] = None,
     fixed_features: Optional[Dict[int, float]] = None,
-    target_fidelities: Optional[Dict[int, float]] = None,
     qmc: bool = True,
     mc_samples: int = 512,
     seed_inner: Optional[int] = None,
-    optimizer_options: Dict[str, Any] = None,
+    optimizer_options: Optional[Dict[str, Any]] = None,
     post_processing_func: Optional[Callable[[Tensor], Tensor]] = None,
     batch_initial_conditions: Optional[Tensor] = None,
     sequential: bool = False,
     **ignore,
 ) -> Tuple[Tensor, Tensor]:
     r"""Optimize an objective under the given model.
 
@@ -1167,25 +1355,24 @@
         posterior_transform: The posterior transform to be used in the
             acquisition function.
         linear_constraints: A tuple of (A, b). Given `k` linear constraints on a
             `d`-dimensional space, `A` is `k x d` and `b` is `k x 1` such that
             `A x <= b`. (Not used by single task models).
         fixed_features: A dictionary of feature assignments `{feature_index: value}` to
             hold fixed during generation.
-        target_fidelities: A dictionary mapping input feature indices to fidelity
-            values. Defaults to `{-1: 1.0}`.
         qmc: Toggle for enabling (qmc=1) or disabling (qmc=0) use of Quasi Monte Carlo.
         mc_samples: Integer number of samples used to estimate Monte Carlo objectives.
         seed_inner: Integer seed used to initialize the sampler passed to MCObjective.
         optimizer_options: Table used to lookup keyword arguments for the optimizer.
         post_processing_func: A function that post-processes an optimization
             result appropriately (i.e. according to `round-trip` transformations).
         batch_initial_conditions: A Tensor of initial values for the optimizer.
         sequential: If False, uses joint optimization, otherwise uses sequential
             optimization.
+        ignore: Any other arguments are ignored.
 
     Returns:
         A tuple containing the best input locations and corresponding objective values.
     """
     if optimizer_options is None:
         optimizer_options = {}
```

### Comparing `botorch-0.8.5/botorch/acquisition/joint_entropy_search.py` & `botorch-0.9.1/botorch/acquisition/joint_entropy_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,17 +135,17 @@
         # which raises a BotorchTensorDimensionWarning.
         if isinstance(model, SaasFullyBayesianSingleTaskGP):
             raise NotImplementedError(FULLY_BAYESIAN_ERROR_MSG)
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore")
             with fantasize_flag():
                 with settings.propagate_grads(False):
-                    # We must do a forward pass one before conditioning
+                    # We must do a forward pass one before conditioning.
                     self.initial_model.posterior(
-                        self.model.train_inputs[0], observation_noise=False
+                        self.optimal_inputs[:1], observation_noise=False
                     )
 
                 # This equates to the JES version proposed by Hvarfner et. al.
                 if self.condition_noiseless:
                     opt_noise = torch.full_like(
                         self.optimal_outputs, MIN_INFERRED_NOISE_LEVEL
                     )
```

### Comparing `botorch-0.8.5/botorch/acquisition/knowledge_gradient.py` & `botorch-0.9.1/botorch/acquisition/knowledge_gradient.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,26 +122,18 @@
         MCSamplerMixin.__init__(self, sampler=sampler)
         # if not explicitly specified, we use the posterior mean for linear objs
         if isinstance(objective, MCAcquisitionObjective) and inner_sampler is None:
             inner_sampler = SobolQMCNormalSampler(sample_shape=torch.Size([128]))
         elif objective is not None and not isinstance(
             objective, MCAcquisitionObjective
         ):
-            # TODO: clean this up after removing AcquisitionObjective.
-            if posterior_transform is None:
-                posterior_transform = self._deprecate_acqf_objective(
-                    posterior_transform=posterior_transform,
-                    objective=objective,
-                )
-                objective = None
-            else:
-                raise RuntimeError(
-                    "Got both a non-MC objective (DEPRECATED) and a posterior "
-                    "transform. Use only a posterior transform instead."
-                )
+            raise UnsupportedError(
+                "Objectives that are not an `MCAcquisitionObjective` are not supported."
+            )
+
         if objective is None and model.num_outputs != 1:
             if posterior_transform is None:
                 raise UnsupportedError(
                     "Must specify an objective or a posterior transform when using "
                     "a multi-output model."
                 )
             elif not posterior_transform.scalarize:
```

### Comparing `botorch-0.8.5/botorch/acquisition/max_value_entropy_search.py` & `botorch-0.9.1/botorch/acquisition/max_value_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/acquisition/monte_carlo.py` & `botorch-0.9.1/botorch/acquisition/objective.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,548 +1,586 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-r"""
-Batch acquisition functions using the reparameterization trick in combination
-with (quasi) Monte-Carlo sampling. See [Rezende2014reparam]_, [Wilson2017reparam]_ and
-[Balandat2020botorch]_.
-
-.. [Rezende2014reparam]
-    D. J. Rezende, S. Mohamed, and D. Wierstra. Stochastic backpropagation and
-    approximate inference in deep generative models. ICML 2014.
-
-.. [Wilson2017reparam]
-    J. T. Wilson, R. Moriconi, F. Hutter, and M. P. Deisenroth.
-    The reparameterization trick for acquisition functions. ArXiv 2017.
-"""
+r"""Objective Modules to be used with acquisition functions."""
 
 from __future__ import annotations
 
-import math
+import inspect
+import warnings
 from abc import ABC, abstractmethod
-from copy import deepcopy
-from typing import Any, Optional, Union
+from typing import Callable, List, Optional, TYPE_CHECKING, Union
 
 import torch
-from botorch.acquisition.acquisition import AcquisitionFunction, MCSamplerMixin
-from botorch.acquisition.cached_cholesky import CachedCholeskyMCAcquisitionFunction
-from botorch.acquisition.objective import (
-    IdentityMCObjective,
-    MCAcquisitionObjective,
-    PosteriorTransform,
-)
-from botorch.acquisition.utils import prune_inferior_points
-from botorch.exceptions.errors import UnsupportedError
+from botorch.exceptions.errors import BotorchTensorDimensionError, UnsupportedError
 from botorch.models.model import Model
-from botorch.posteriors.posterior import Posterior
-from botorch.sampling.base import MCSampler
-from botorch.utils.transforms import (
-    concatenate_pending_points,
-    match_batch_shape,
-    t_batch_mode_transform,
-)
+from botorch.models.transforms.outcome import Standardize
+from botorch.posteriors.gpytorch import GPyTorchPosterior, scalarize_posterior
+from botorch.sampling import IIDNormalSampler, MCSampler
+from botorch.utils import apply_constraints
+from gpytorch.distributions import MultitaskMultivariateNormal, MultivariateNormal
+from linear_operator.operators.dense_linear_operator import to_linear_operator
 from torch import Tensor
+from torch.nn import Module
 
+if TYPE_CHECKING:
+    from botorch.posteriors.posterior import Posterior  # pragma: no cover
+    from botorch.posteriors.posterior_list import PosteriorList  # pragma: no cover
 
-class MCAcquisitionFunction(AcquisitionFunction, MCSamplerMixin, ABC):
+
+class PosteriorTransform(Module, ABC):
     r"""
-    Abstract base class for Monte-Carlo based batch acquisition functions.
+    Abstract base class for objectives that transform the posterior.
 
     :meta private:
     """
 
-    def __init__(
-        self,
-        model: Model,
-        sampler: Optional[MCSampler] = None,
-        objective: Optional[MCAcquisitionObjective] = None,
-        posterior_transform: Optional[PosteriorTransform] = None,
-        X_pending: Optional[Tensor] = None,
-    ) -> None:
-        r"""
+    @abstractmethod
+    def evaluate(self, Y: Tensor) -> Tensor:
+        r"""Evaluate the transform on a set of outcomes.
+
         Args:
-            model: A fitted model.
-            sampler: The sampler used to draw base samples. If not given,
-                a sampler is generated using `get_sampler`.
-                NOTE: For posteriors that do not support base samples,
-                a sampler compatible with intended use case must be provided.
-                See `ForkedRNGSampler` and `StochasticSampler` as examples.
-            objective: The MCAcquisitionObjective under which the samples are
-                evaluated. Defaults to `IdentityMCObjective()`.
-            posterior_transform: A PosteriorTransform (optional).
-            X_pending: A `batch_shape, m x d`-dim Tensor of `m` design points
-                that have points that have been submitted for function evaluation
-                but have not yet been evaluated.
-        """
-        super().__init__(model=model)
-        MCSamplerMixin.__init__(self, sampler=sampler)
-        if objective is None and model.num_outputs != 1:
-            if posterior_transform is None:
-                raise UnsupportedError(
-                    "Must specify an objective or a posterior transform when using "
-                    "a multi-output model."
-                )
-            elif not posterior_transform.scalarize:
-                raise UnsupportedError(
-                    "If using a multi-output model without an objective, "
-                    "posterior_transform must scalarize the output."
-                )
-        if objective is None:
-            objective = IdentityMCObjective()
-        self.posterior_transform = posterior_transform
-        self.objective: MCAcquisitionObjective = objective
-        self.set_X_pending(X_pending)
+            Y: A `batch_shape x q x m`-dim tensor of outcomes.
+
+        Returns:
+            A `batch_shape x q' [x m']`-dim tensor of transformed outcomes.
+        """
+        pass  # pragma: no cover
 
     @abstractmethod
-    def forward(self, X: Tensor) -> Tensor:
-        r"""Takes in a `batch_shape x q x d` X Tensor of t-batches with `q` `d`-dim
-        design points each, and returns a Tensor with shape `batch_shape'`, where
-        `batch_shape'` is the broadcasted batch shape of model and input `X`. Should
-        utilize the result of `set_X_pending` as needed to account for pending function
-        evaluations.
+    def forward(self, posterior) -> Posterior:
+        r"""Compute the transformed posterior.
+
+        Args:
+            posterior: The posterior to be transformed.
+
+        Returns:
+            The transformed posterior object.
         """
         pass  # pragma: no cover
 
 
-class qExpectedImprovement(MCAcquisitionFunction):
-    r"""MC-based batch Expected Improvement.
+# import DeterministicModel after PosteriorTransform to avoid circular import
+from botorch.models.deterministic import DeterministicModel  # noqa
+
 
-    This computes qEI by
-    (1) sampling the joint posterior over q points
-    (2) evaluating the improvement over the current best for each sample
-    (3) maximizing over q
-    (4) averaging over the samples
+class ScalarizedPosteriorTransform(PosteriorTransform):
+    r"""An affine posterior transform for scalarizing multi-output posteriors.
 
-    `qEI(X) = E(max(max Y - best_f, 0)), Y ~ f(X), where X = (x_1,...,x_q)`
+    For a Gaussian posterior at a single point (`q=1`) with mean `mu` and
+    covariance matrix `Sigma`, this yields a single-output posterior with mean
+    `weights^T * mu` and variance `weights^T Sigma w`.
 
     Example:
-        >>> model = SingleTaskGP(train_X, train_Y)
-        >>> best_f = train_Y.max()[0]
-        >>> sampler = SobolQMCNormalSampler(1024)
-        >>> qEI = qExpectedImprovement(model, best_f, sampler)
-        >>> qei = qEI(test_X)
+        Example for a model with two outcomes:
+
+        >>> weights = torch.tensor([0.5, 0.25])
+        >>> posterior_transform = ScalarizedPosteriorTransform(weights)
+        >>> EI = ExpectedImprovement(
+        ... model, best_f=0.1, posterior_transform=posterior_transform
+        ... )
     """
 
-    def __init__(
-        self,
-        model: Model,
-        best_f: Union[float, Tensor],
-        sampler: Optional[MCSampler] = None,
-        objective: Optional[MCAcquisitionObjective] = None,
-        posterior_transform: Optional[PosteriorTransform] = None,
-        X_pending: Optional[Tensor] = None,
-        **kwargs: Any,
-    ) -> None:
-        r"""q-Expected Improvement.
+    scalarize: bool = True
 
+    def __init__(self, weights: Tensor, offset: float = 0.0) -> None:
+        r"""
         Args:
-            model: A fitted model.
-            best_f: The best objective value observed so far (assumed noiseless). Can be
-                a `batch_shape`-shaped tensor, which in case of a batched model
-                specifies potentially different values for each element of the batch.
-            sampler: The sampler used to draw base samples. See `MCAcquisitionFunction`
-                more details.
-            objective: The MCAcquisitionObjective under which the samples are evaluated.
-                Defaults to `IdentityMCObjective()`.
-            posterior_transform: A PosteriorTransform (optional).
-            X_pending:  A `m x d`-dim Tensor of `m` design points that have been
-                submitted for function evaluation but have not yet been evaluated.
-                Concatenated into X upon forward call. Copied and set to have no
-                gradient.
-        """
-        super().__init__(
-            model=model,
-            sampler=sampler,
-            objective=objective,
-            posterior_transform=posterior_transform,
-            X_pending=X_pending,
-        )
-        self.register_buffer("best_f", torch.as_tensor(best_f, dtype=float))
+            weights: A one-dimensional tensor with `m` elements representing the
+                linear weights on the outputs.
+            offset: An offset to be added to posterior mean.
+        """
+        if weights.dim() != 1:
+            raise ValueError("weights must be a one-dimensional tensor.")
+        super().__init__()
+        self.register_buffer("weights", weights)
+        self.offset = offset
 
-    @concatenate_pending_points
-    @t_batch_mode_transform()
-    def forward(self, X: Tensor) -> Tensor:
-        r"""Evaluate qExpectedImprovement on the candidate set `X`.
+    def evaluate(self, Y: Tensor) -> Tensor:
+        r"""Evaluate the transform on a set of outcomes.
 
         Args:
-            X: A `batch_shape x q x d`-dim Tensor of t-batches with `q` `d`-dim design
-                points each.
+            Y: A `batch_shape x q x m`-dim tensor of outcomes.
 
         Returns:
-            A `batch_shape'`-dim Tensor of Expected Improvement values at the given
-            design points `X`, where `batch_shape'` is the broadcasted batch shape of
-            model and input `X`.
+            A `batch_shape x q`-dim tensor of transformed outcomes.
         """
-        posterior = self.model.posterior(
-            X=X, posterior_transform=self.posterior_transform
+        return self.offset + Y @ self.weights
+
+    def forward(
+        self, posterior: Union[GPyTorchPosterior, PosteriorList]
+    ) -> GPyTorchPosterior:
+        r"""Compute the posterior of the affine transformation.
+
+        Args:
+            posterior: A posterior with the same number of outputs as the
+                elements in `self.weights`.
+
+        Returns:
+            A single-output posterior.
+        """
+        return scalarize_posterior(
+            posterior=posterior, weights=self.weights, offset=self.offset
         )
-        samples = self.get_posterior_samples(posterior)
-        obj = self.objective(samples, X=X)
-        obj = (obj - self.best_f.unsqueeze(-1).to(obj)).clamp_min(0)
-        q_ei = obj.max(dim=-1)[0].mean(dim=0)
-        return q_ei
-
-
-class qNoisyExpectedImprovement(
-    MCAcquisitionFunction, CachedCholeskyMCAcquisitionFunction
-):
-    r"""MC-based batch Noisy Expected Improvement.
-
-    This function does not assume a `best_f` is known (which would require
-    noiseless observations). Instead, it uses samples from the joint posterior
-    over the `q` test points and previously observed points. The improvement
-    over previously observed points is computed for each sample and averaged.
 
-    `qNEI(X) = E(max(max Y - max Y_baseline, 0))`, where
-    `(Y, Y_baseline) ~ f((X, X_baseline)), X = (x_1,...,x_q)`
 
-    Example:
-        >>> model = SingleTaskGP(train_X, train_Y)
-        >>> sampler = SobolQMCNormalSampler(1024)
-        >>> qNEI = qNoisyExpectedImprovement(model, train_X, sampler)
-        >>> qnei = qNEI(test_X)
+class ExpectationPosteriorTransform(PosteriorTransform):
+    r"""Transform the `batch x (q * n_w) x m` posterior into a `batch x q x m`
+    posterior of the expectation. The expectation is calculated over each
+    consecutive `n_w` block of points in the posterior.
+
+    This is intended for use with `InputPerturbation` or `AppendFeatures` for
+    optimizing the expectation over `n_w` points. This should not be used when
+    there are constraints present, since this does not take into account
+    the feasibility of the objectives.
+
+    Note: This is different than `ScalarizedPosteriorTransform` in that
+    this operates over the q-batch dimension.
     """
 
-    def __init__(
-        self,
-        model: Model,
-        X_baseline: Tensor,
-        sampler: Optional[MCSampler] = None,
-        objective: Optional[MCAcquisitionObjective] = None,
-        posterior_transform: Optional[PosteriorTransform] = None,
-        X_pending: Optional[Tensor] = None,
-        prune_baseline: bool = True,
-        cache_root: bool = True,
-        **kwargs: Any,
-    ) -> None:
-        r"""q-Noisy Expected Improvement.
+    def __init__(self, n_w: int, weights: Optional[Tensor] = None) -> None:
+        r"""A posterior transform calculating the expectation over the q-batch
+        dimension.
+
+        Args:
+            n_w: The number of points in the q-batch of the posterior to compute
+                the expectation over. This corresponds to the size of the
+                `feature_set` of `AppendFeatures` or the size of the `perturbation_set`
+                of `InputPerturbation`.
+            weights: An optional `n_w x m`-dim tensor of weights. Can be used to
+                compute a weighted expectation. Weights are normalized before use.
+        """
+        super().__init__()
+        if weights is not None:
+            if weights.dim() != 2 or weights.shape[0] != n_w:
+                raise ValueError("`weights` must be a tensor of size `n_w x m`.")
+            if torch.any(weights < 0):
+                raise ValueError("`weights` must be non-negative.")
+        else:
+            weights = torch.ones(n_w, 1)
+        # Normalize the weights.
+        weights = weights / weights.sum(dim=0)
+        self.register_buffer("weights", weights)
+        self.n_w = n_w
+
+    def evaluate(self, Y: Tensor) -> Tensor:
+        r"""Evaluate the expectation of a set of outcomes.
+
+        Args:
+            Y: A `batch_shape x (q * n_w) x m`-dim tensor of outcomes.
+
+        Returns:
+            A `batch_shape x q x m`-dim tensor of expectation outcomes.
+        """
+        batch_shape, m = Y.shape[:-2], Y.shape[-1]
+        weighted_Y = Y.view(*batch_shape, -1, self.n_w, m) * self.weights.to(Y)
+        return weighted_Y.sum(dim=-2)
+
+    def forward(self, posterior: GPyTorchPosterior) -> GPyTorchPosterior:
+        r"""Compute the posterior of the expectation.
 
         Args:
-            model: A fitted model.
-            X_baseline: A `batch_shape x r x d`-dim Tensor of `r` design points
-                that have already been observed. These points are considered as
-                the potential best design point.
-            sampler: The sampler used to draw base samples. See `MCAcquisitionFunction`
-                more details.
-            objective: The MCAcquisitionObjective under which the samples are
-                evaluated. Defaults to `IdentityMCObjective()`.
-            posterior_transform: A PosteriorTransform (optional).
-            X_pending: A `batch_shape x m x d`-dim Tensor of `m` design points
-                that have points that have been submitted for function evaluation
-                but have not yet been evaluated. Concatenated into `X` upon
-                forward call. Copied and set to have no gradient.
-            prune_baseline: If True, remove points in `X_baseline` that are
-                highly unlikely to be the best point. This can significantly
-                improve performance and is generally recommended. In order to
-                customize pruning parameters, instead manually call
-                `botorch.acquisition.utils.prune_inferior_points` on `X_baseline`
-                before instantiating the acquisition function.
-            cache_root: A boolean indicating whether to cache the root
-                decomposition over `X_baseline` and use low-rank updates.
-
-        TODO: similar to qNEHVI, when we are using sequential greedy candidate
-        selection, we could incorporate pending points X_baseline and compute
-        the incremental qNEI from the new point. This would greatly increase
-        efficiency for large batches.
-        """
-        super().__init__(
-            model=model,
-            sampler=sampler,
-            objective=objective,
-            posterior_transform=posterior_transform,
-            X_pending=X_pending,
+            posterior: An `m`-outcome joint posterior over `q * n_w` points.
+
+        Returns:
+            An `m`-outcome joint posterior over `q` expectations.
+        """
+        org_mvn = posterior.distribution
+        if getattr(org_mvn, "_interleaved", False):
+            raise UnsupportedError(
+                "`ExpectationPosteriorTransform` does not support "
+                "interleaved posteriors."
+            )
+        # Initialize the weight matrix of shape compatible with the mvn.
+        org_event_shape = org_mvn.event_shape
+        batch_shape = org_mvn.batch_shape
+        q = org_event_shape[0] // self.n_w
+        m = 1 if len(org_event_shape) == 1 else org_event_shape[-1]
+        tkwargs = {"device": org_mvn.loc.device, "dtype": org_mvn.loc.dtype}
+        weights = torch.zeros(q * m, q * self.n_w * m, **tkwargs)
+        # Make sure self.weights has the correct dtype/device and shape.
+        self.weights = self.weights.to(org_mvn.loc).expand(self.n_w, m)
+        # Fill in the non-zero entries of the weight matrix.
+        # We want each row to have non-zero weights for the corresponding
+        # `n_w` sized diagonal. The `m` outcomes are not interleaved.
+        for i in range(q * m):
+            weights[i, self.n_w * i : self.n_w * (i + 1)] = self.weights[:, i // q]
+        # Trasform the mean.
+        new_loc = (
+            (weights @ org_mvn.loc.unsqueeze(-1))
+            .view(*batch_shape, m, q)
+            .transpose(-1, -2)
         )
-        self._setup(model=model, cache_root=cache_root)
-        if prune_baseline:
-            X_baseline = prune_inferior_points(
-                model=model,
-                X=X_baseline,
-                objective=objective,
-                posterior_transform=posterior_transform,
-                marginalize_dim=kwargs.get("marginalize_dim"),
+        # Transform the covariance matrix.
+        org_cov = (
+            org_mvn.lazy_covariance_matrix
+            if org_mvn.islazy
+            else org_mvn.covariance_matrix
+        )
+        new_cov = weights @ (org_cov @ weights.t())
+        if m == 1:
+            new_mvn = MultivariateNormal(
+                new_loc.squeeze(-1), to_linear_operator(new_cov)
             )
-        self.register_buffer("X_baseline", X_baseline)
-
-        if self._cache_root:
-            self.q_in = -1
-            # set baseline samples
-            with torch.no_grad():
-                posterior = self.model.posterior(
-                    X_baseline, posterior_transform=self.posterior_transform
-                )
-                # Note: The root decomposition is cached in two different places. It
-                # may be confusing to have two different caches, but this is not
-                # trivial to change since each is needed for a different reason:
-                # - LinearOperator caching to `posterior.mvn` allows for reuse within
-                #  this function, which may be helpful if the same root decomposition
-                #  is produced by the calls to `self.base_sampler` and
-                #  `self._cache_root_decomposition`.
-                # - self._baseline_L allows a root decomposition to be persisted outside
-                #   this method.
-                baseline_samples = self.get_posterior_samples(posterior)
-            # We make a copy here because we will write an attribute `base_samples`
-            # to `self.base_sampler.base_samples`, and we don't want to mutate
-            # `self.sampler`.
-            self.base_sampler = deepcopy(self.sampler)
-            baseline_obj = self.objective(baseline_samples, X=X_baseline)
-            self.register_buffer("baseline_samples", baseline_samples)
-            self.register_buffer(
-                "baseline_obj_max_values", baseline_obj.max(dim=-1).values
+        else:
+            # Using MTMVN since we pass a single loc and covar for all `m` outputs.
+            new_mvn = MultitaskMultivariateNormal(
+                new_loc, to_linear_operator(new_cov), interleaved=False
             )
-            self._baseline_L = self._compute_root_decomposition(posterior=posterior)
+        return GPyTorchPosterior(distribution=new_mvn)
 
-    def _forward_cached(self, posterior: Posterior, X_full: Tensor, q: int) -> Tensor:
-        r"""Compute difference objective using cached root decomposition.
+
+class UnstandardizePosteriorTransform(PosteriorTransform):
+    r"""Posterior transform that unstandardizes the posterior.
+
+    TODO: remove this when MultiTask models support outcome transforms.
+
+    Example:
+        >>> unstd_transform = UnstandardizePosteriorTransform(Y_mean, Y_std)
+        >>> unstd_posterior = unstd_transform(posterior)
+    """
+
+    def __init__(self, Y_mean: Tensor, Y_std: Tensor) -> None:
+        r"""Initialize objective.
 
         Args:
-            posterior: The posterior.
-            X_full: A `batch_shape x n + q x d`-dim tensor of inputs
-            q: The batch size.
-
-        Returns:
-            A `sample_shape x batch_shape`-dim tensor containing the
-                difference in objective under each MC sample.
-        """
-        # handle one-to-many input transforms
-        n_w = posterior._extended_shape()[-2] // X_full.shape[-2]
-        q_in = q * n_w
-        self._set_sampler(q_in=q_in, posterior=posterior)
-        new_samples = self._get_f_X_samples(posterior=posterior, q_in=q_in)
-        new_obj = self.objective(new_samples, X=X_full[..., -q:, :])
-        new_obj_max_values = new_obj.max(dim=-1).values
-        n_sample_dims = len(self.base_sampler.sample_shape)
-        view_shape = torch.Size(
-            [
-                *self.baseline_obj_max_values.shape[:n_sample_dims],
-                *(1,) * (new_obj_max_values.ndim - self.baseline_obj_max_values.ndim),
-                *self.baseline_obj_max_values.shape[n_sample_dims:],
-            ]
-        )
-        return new_obj_max_values - self.baseline_obj_max_values.view(view_shape)
+            Y_mean: `m`-dim tensor of outcome means
+            Y_std: `m`-dim tensor of outcome standard deviations
 
-    @concatenate_pending_points
-    @t_batch_mode_transform()
-    def forward(self, X: Tensor) -> Tensor:
-        r"""Evaluate qNoisyExpectedImprovement on the candidate set `X`.
+        """
+        if Y_mean.ndim > 1 or Y_std.ndim > 1:
+            raise BotorchTensorDimensionError(
+                "Y_mean and Y_std must both be 1-dimensional, but got "
+                f"{Y_mean.ndim} and {Y_std.ndim}"
+            )
+        super().__init__()
+        self.outcome_transform = Standardize(m=Y_mean.shape[0]).to(Y_mean)
+        Y_std_unsqueezed = Y_std.unsqueeze(0)
+        self.outcome_transform.means = Y_mean.unsqueeze(0)
+        self.outcome_transform.stdvs = Y_std_unsqueezed
+        self.outcome_transform._stdvs_sq = Y_std_unsqueezed.pow(2)
+        self.outcome_transform._is_trained = torch.tensor(True)
+        self.outcome_transform.eval()
+
+    def evaluate(self, Y: Tensor) -> Tensor:
+        return self.outcome_transform.untransform(Y)[0]
+
+    def forward(self, posterior: GPyTorchPosterior) -> Tensor:
+        return self.outcome_transform.untransform_posterior(posterior)
+
+
+class MCAcquisitionObjective(Module, ABC):
+    r"""Abstract base class for MC-based objectives.
+
+    Args:
+        _verify_output_shape: If True and `X` is given, check that the q-batch
+            shape of the objectives agrees with that of X.
+        _is_mo: A boolean denoting whether the objectives are multi-output.
+
+    :meta private:
+    """
+
+    _verify_output_shape: bool = True
+    _is_mo: bool = False
+
+    @abstractmethod
+    def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
+        r"""Evaluate the objective on the samples.
 
         Args:
-            X: A `batch_shape x q x d`-dim Tensor of t-batches with `q` `d`-dim design
-                points each.
+            samples: A `sample_shape x batch_shape x q x m`-dim Tensors of
+                samples from a model posterior.
+            X: A `batch_shape x q x d`-dim tensor of inputs. Relevant only if
+                the objective depends on the inputs explicitly.
 
         Returns:
-            A `batch_shape'`-dim Tensor of Noisy Expected Improvement values at the
-            given design points `X`, where `batch_shape'` is the broadcasted batch shape
-            of model and input `X`.
+            Tensor: A `sample_shape x batch_shape x q`-dim Tensor of objective
+            values (assuming maximization).
+
+        This method is usually not called directly, but via the objectives.
+
+        Example:
+            >>> # `__call__` method:
+            >>> samples = sampler(posterior)
+            >>> outcome = mc_obj(samples)
         """
-        q = X.shape[-2]
-        X_full = torch.cat([match_batch_shape(self.X_baseline, X), X], dim=-2)
-        # TODO: Implement more efficient way to compute posterior over both training and
-        # test points in GPyTorch (https://github.com/cornellius-gp/gpytorch/issues/567)
-        posterior = self.model.posterior(
-            X_full, posterior_transform=self.posterior_transform
-        )
-        if self._cache_root:
-            diffs = self._forward_cached(posterior=posterior, X_full=X_full, q=q)
-        else:
-            samples = self.get_posterior_samples(posterior)
-            obj = self.objective(samples, X=X_full)
-            diffs = obj[..., -q:].max(dim=-1).values - obj[..., :-q].max(dim=-1).values
+        pass  # pragma: no cover
+
+    def __call__(
+        self, samples: Tensor, X: Optional[Tensor] = None, *args, **kwargs
+    ) -> Tensor:
+        output = super().__call__(samples=samples, X=X, *args, **kwargs)
+        # q-batch dimension is at -1 for single-output objectives and at
+        # -2 for multi-output objectives.
+        q_batch_idx = -2 if self._is_mo else -1
+        if (
+            X is not None
+            and self._verify_output_shape
+            and output.shape[q_batch_idx] != X.shape[-2]
+        ):
+            raise RuntimeError(
+                "The q-batch shape of the objective values does not agree with "
+                f"the q-batch shape of X. Got {output.shape[q_batch_idx]} and "
+                f"{X.shape[-2]}. This may happen if you used a one-to-many input "
+                "transform but forgot to use a corresponding objective."
+            )
+        return output
 
-        return diffs.clamp_min(0).mean(dim=0)
 
+class IdentityMCObjective(MCAcquisitionObjective):
+    r"""Trivial objective extracting the last dimension.
+
+    Example:
+        >>> identity_objective = IdentityMCObjective()
+        >>> samples = sampler(posterior)
+        >>> objective = identity_objective(samples)
+    """
+
+    def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
+        return samples.squeeze(-1)
 
-class qProbabilityOfImprovement(MCAcquisitionFunction):
-    r"""MC-based batch Probability of Improvement.
 
-    Estimates the probability of improvement over the current best observed
-    value by sampling from the joint posterior distribution of the q-batch.
-    MC-based estimates of a probability involves taking expectation of an
-    indicator function; to support auto-differntiation, the indicator is
-    replaced with a sigmoid function with temperature parameter `tau`.
+class LinearMCObjective(MCAcquisitionObjective):
+    r"""Linear objective constructed from a weight tensor.
 
-    `qPI(X) = P(max Y >= best_f), Y ~ f(X), X = (x_1,...,x_q)`
+    For input `samples` and `mc_obj = LinearMCObjective(weights)`, this produces
+    `mc_obj(samples) = sum_{i} weights[i] * samples[..., i]`
 
     Example:
-        >>> model = SingleTaskGP(train_X, train_Y)
-        >>> best_f = train_Y.max()[0]
-        >>> sampler = SobolQMCNormalSampler(1024)
-        >>> qPI = qProbabilityOfImprovement(model, best_f, sampler)
-        >>> qpi = qPI(test_X)
+        Example for a model with two outcomes:
+
+        >>> weights = torch.tensor([0.75, 0.25])
+        >>> linear_objective = LinearMCObjective(weights)
+        >>> samples = sampler(posterior)
+        >>> objective = linear_objective(samples)
     """
 
-    def __init__(
-        self,
-        model: Model,
-        best_f: Union[float, Tensor],
-        sampler: Optional[MCSampler] = None,
-        objective: Optional[MCAcquisitionObjective] = None,
-        posterior_transform: Optional[PosteriorTransform] = None,
-        X_pending: Optional[Tensor] = None,
-        tau: float = 1e-3,
-    ) -> None:
-        r"""q-Probability of Improvement.
+    def __init__(self, weights: Tensor) -> None:
+        r"""
+        Args:
+            weights: A one-dimensional tensor with `m` elements representing the
+                linear weights on the outputs.
+        """
+        super().__init__()
+        if weights.dim() != 1:
+            raise ValueError("weights must be a one-dimensional tensor.")
+        self.register_buffer("weights", weights)
+
+    def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
+        r"""Evaluate the linear objective on the samples.
+
+        Args:
+            samples: A `sample_shape x batch_shape x q x m`-dim tensors of
+                samples from a model posterior.
+            X: A `batch_shape x q x d`-dim tensor of inputs. Relevant only if
+                the objective depends on the inputs explicitly.
+
+        Returns:
+            A `sample_shape x batch_shape x q`-dim tensor of objective values.
+        """
+        if samples.shape[-1] != self.weights.shape[-1]:
+            raise RuntimeError("Output shape of samples not equal to that of weights")
+        return torch.einsum("...m, m", [samples, self.weights])
 
+
+class GenericMCObjective(MCAcquisitionObjective):
+    r"""Objective generated from a generic callable.
+
+    Allows to construct arbitrary MC-objective functions from a generic
+    callable. In order to be able to use gradient-based acquisition function
+    optimization it should be possible to backpropagate through the callable.
+
+    Example:
+        >>> generic_objective = GenericMCObjective(
+                lambda Y, X: torch.sqrt(Y).sum(dim=-1),
+            )
+        >>> samples = sampler(posterior)
+        >>> objective = generic_objective(samples)
+    """
+
+    def __init__(self, objective: Callable[[Tensor, Optional[Tensor]], Tensor]) -> None:
+        r"""
         Args:
-            model: A fitted model.
-            best_f: The best objective value observed so far (assumed noiseless). Can
-                be a `batch_shape`-shaped tensor, which in case of a batched model
-                specifies potentially different values for each element of the batch.
-            sampler: The sampler used to draw base samples. See `MCAcquisitionFunction`
-                more details.
-            objective: The MCAcquisitionObjective under which the samples are
-                evaluated. Defaults to `IdentityMCObjective()`.
-            posterior_transform: A PosteriorTransform (optional).
-            X_pending:  A `m x d`-dim Tensor of `m` design points that have
-                points that have been submitted for function evaluation
-                but have not yet been evaluated.  Concatenated into X upon
-                forward call.  Copied and set to have no gradient.
-            tau: The temperature parameter used in the sigmoid approximation
-                of the step function. Smaller values yield more accurate
-                approximations of the function, but result in gradients
-                estimates with higher variance.
-        """
-        super().__init__(
-            model=model,
-            sampler=sampler,
-            objective=objective,
-            posterior_transform=posterior_transform,
-            X_pending=X_pending,
-        )
-        self.register_buffer("best_f", torch.as_tensor(best_f, dtype=float))
-        self.register_buffer("tau", torch.as_tensor(tau, dtype=float))
+            objective: A callable `f(samples, X)` mapping a
+                `sample_shape x batch-shape x q x m`-dim Tensor `samples` and
+                an optional `batch-shape x q x d`-dim Tensor `X` to a
+                `sample_shape x batch-shape x q`-dim Tensor of objective values.
+        """
+        super().__init__()
+        if len(inspect.signature(objective).parameters) == 1:
+            warnings.warn(
+                "The `objective` callable of `GenericMCObjective` is expected to "
+                "take two arguments. Passing a callable that expects a single "
+                "argument will result in an error in future versions.",
+                DeprecationWarning,
+            )
 
-    @concatenate_pending_points
-    @t_batch_mode_transform()
-    def forward(self, X: Tensor) -> Tensor:
-        r"""Evaluate qProbabilityOfImprovement on the candidate set `X`.
+            def obj(samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
+                return objective(samples)
+
+            self.objective = obj
+        else:
+            self.objective = objective
+
+    def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
+        r"""Evaluate the objective on the samples.
 
         Args:
-            X: A `batch_shape x q x d`-dim Tensor of t-batches with `q` `d`-dim design
-                points each.
+            samples: A `sample_shape x batch_shape x q x m`-dim Tensors of
+                samples from a model posterior.
+            X: A `batch_shape x q x d`-dim tensor of inputs. Relevant only if
+                the objective depends on the inputs explicitly.
 
         Returns:
-            A `batch_shape'`-dim Tensor of Probability of Improvement values at the
-            given design points `X`, where `batch_shape'` is the broadcasted batch shape
-            of model and input `X`.
+            A `sample_shape x batch_shape x q`-dim Tensor of objective values.
         """
-        posterior = self.model.posterior(
-            X=X, posterior_transform=self.posterior_transform
-        )
-        samples = self.get_posterior_samples(posterior)
-        obj = self.objective(samples, X=X)  # `sample_shape x batch_shape x q`-dim
-        max_obj = obj.max(dim=-1)[0]  # `sample_shape x batch_shape`-dim
-        impr = max_obj - self.best_f.to(max_obj)
-        val = torch.sigmoid(impr / self.tau).mean(dim=0)
-        return val
+        return self.objective(samples, X=X)
+
 
+class ConstrainedMCObjective(GenericMCObjective):
+    r"""Feasibility-weighted objective.
 
-class qSimpleRegret(MCAcquisitionFunction):
-    r"""MC-based batch Simple Regret.
+    An Objective allowing to maximize some scalable objective on the model
+    outputs subject to a number of constraints. Constraint feasibilty is
+    approximated by a sigmoid function.
 
-    Samples from the joint posterior over the q-batch and computes the simple regret.
+        mc_acq(X) = (
+        (objective(X) + infeasible_cost) * \prod_i (1  - sigmoid(constraint_i(X)))
+        ) - infeasible_cost
 
-    `qSR(X) = E(max Y), Y ~ f(X), X = (x_1,...,x_q)`
+    See `botorch.utils.objective.apply_constraints` for details on the constraint
+    handling.
 
     Example:
-        >>> model = SingleTaskGP(train_X, train_Y)
-        >>> sampler = SobolQMCNormalSampler(1024)
-        >>> qSR = qSimpleRegret(model, sampler)
-        >>> qsr = qSR(test_X)
-    """
+        >>> bound = 0.0
+        >>> objective = lambda Y: Y[..., 0]
+        >>> # apply non-negativity constraint on f(x)[1]
+        >>> constraint = lambda Y: bound - Y[..., 1]
+        >>> constrained_objective = ConstrainedMCObjective(objective, [constraint])
+        >>> samples = sampler(posterior)
+        >>> objective = constrained_objective(samples)
 
-    @concatenate_pending_points
-    @t_batch_mode_transform()
-    def forward(self, X: Tensor) -> Tensor:
-        r"""Evaluate qSimpleRegret on the candidate set `X`.
+    TODO: Deprecate this as default way to handle constraints with MC acquisition
+    functions once we have data on how well SampleReducingMCAcquisitionFunction works.
+    """
 
+    def __init__(
+        self,
+        objective: Callable[[Tensor, Optional[Tensor]], Tensor],
+        constraints: List[Callable[[Tensor], Tensor]],
+        infeasible_cost: Union[Tensor, float] = 0.0,
+        eta: Union[Tensor, float] = 1e-3,
+    ) -> None:
+        r"""
         Args:
-            X: A `batch_shape x q x d`-dim Tensor of t-batches with `q` `d`-dim design
-                points each.
+            objective: A callable `f(samples, X)` mapping a
+                `sample_shape x batch-shape x q x m`-dim Tensor `samples` and
+                an optional `batch-shape x q x d`-dim Tensor `X` to a
+                `sample_shape x batch-shape x q`-dim Tensor of objective values.
+            constraints: A list of callables, each mapping a Tensor of dimension
+                `sample_shape x batch-shape x q x m` to a Tensor of dimension
+                `sample_shape x batch-shape x q`, where negative values imply
+                feasibility.
+            infeasible_cost: The cost of a design if all associated samples are
+                infeasible.
+            eta: The temperature parameter of the sigmoid function approximating
+                the constraint. Can be either a float or a 1-dim tensor. In case
+                of a float the same eta is used for every constraint in
+                constraints. In case of a tensor the length of the tensor must
+                match the number of provided constraints. The i-th constraint is
+                then estimated with the i-th eta value.
+        """
+        super().__init__(objective=objective)
+        self.constraints = constraints
+        if type(eta) is not Tensor:
+            eta = torch.full((len(constraints),), eta)
+        self.register_buffer("eta", eta)
+        self.register_buffer("infeasible_cost", torch.as_tensor(infeasible_cost))
+
+    def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
+        r"""Evaluate the feasibility-weighted objective on the samples.
+
+        Args:
+            samples: A `sample_shape x batch_shape x q x m`-dim Tensors of
+                samples from a model posterior.
+            X: A `batch_shape x q x d`-dim tensor of inputs. Relevant only if
+                the objective depends on the inputs explicitly.
 
         Returns:
-            A `batch_shape'`-dim Tensor of Simple Regret values at the given design
-            points `X`, where `batch_shape'` is the broadcasted batch shape of model
-            and input `X`.
+            A `sample_shape x batch_shape x q`-dim Tensor of objective values
+            weighted by feasibility (assuming maximization).
         """
-        posterior = self.model.posterior(
-            X=X, posterior_transform=self.posterior_transform
+        obj = super().forward(samples=samples)
+        return apply_constraints(
+            obj=obj,
+            constraints=self.constraints,
+            samples=samples,
+            infeasible_cost=self.infeasible_cost,
+            eta=self.eta,
         )
-        samples = self.get_posterior_samples(posterior)
-        obj = self.objective(samples, X=X)
-        val = obj.max(dim=-1)[0].mean(dim=0)
-        return val
-
 
-class qUpperConfidenceBound(MCAcquisitionFunction):
-    r"""MC-based batch Upper Confidence Bound.
 
-    Uses a reparameterization to extend UCB to qUCB for q > 1 (See Appendix A
-    of [Wilson2017reparam].)
+class LearnedObjective(MCAcquisitionObjective):
+    r"""Learned preference objective constructed from a preference model.
 
-    `qUCB = E(max(mu + |Y_tilde - mu|))`, where `Y_tilde ~ N(mu, beta pi/2 Sigma)`
-    and `f(X)` has distribution `N(mu, Sigma)`.
+    For input `samples`, it samples each individual sample again from the latent
+    preference posterior distribution using `pref_model` and return the posterior mean.
 
     Example:
-        >>> model = SingleTaskGP(train_X, train_Y)
-        >>> sampler = SobolQMCNormalSampler(1024)
-        >>> qUCB = qUpperConfidenceBound(model, 0.1, sampler)
-        >>> qucb = qUCB(test_X)
+        >>> train_X = torch.rand(2, 2)
+        >>> train_comps = torch.LongTensor([[0, 1]])
+        >>> pref_model = PairwiseGP(train_X, train_comps)
+        >>> learned_pref_obj = LearnedObjective(pref_model)
+        >>> samples = sampler(posterior)
+        >>> objective = learned_pref_obj(samples)
     """
 
     def __init__(
         self,
-        model: Model,
-        beta: float,
+        pref_model: Model,
         sampler: Optional[MCSampler] = None,
-        objective: Optional[MCAcquisitionObjective] = None,
-        posterior_transform: Optional[PosteriorTransform] = None,
-        X_pending: Optional[Tensor] = None,
-    ) -> None:
-        r"""q-Upper Confidence Bound.
-
+    ):
+        r"""
         Args:
-            model: A fitted model.
-            beta: Controls tradeoff between mean and standard deviation in UCB.
-            sampler: The sampler used to draw base samples. See `MCAcquisitionFunction`
-                more details.
-            objective: The MCAcquisitionObjective under which the samples are
-                evaluated. Defaults to `IdentityMCObjective()`.
-            posterior_transform: A PosteriorTransform (optional).
-            X_pending: A `batch_shape x m x d`-dim Tensor of `m` design points that have
-                points that have been submitted for function evaluation but have not yet
-                been evaluated. Concatenated into X upon forward call. Copied and set to
-                have no gradient.
-        """
-        super().__init__(
-            model=model,
-            sampler=sampler,
-            objective=objective,
-            posterior_transform=posterior_transform,
-            X_pending=X_pending,
-        )
-        self.beta_prime = math.sqrt(beta * math.pi / 2)
+            pref_model: A BoTorch model, which models the latent preference/utility
+                function. Given an input tensor of size
+                `sample_size x batch_shape x N x d`, its `posterior` method should
+                return a `Posterior` object with single outcome representing the
+                utility values of the input.
+            sampler: Sampler for the preference model to account for uncertainty in
+                preferece when calculating the objective; it's not the one used
+                in MC acquisition functions. If None,
+                it uses `IIDNormalSampler(sample_shape=torch.Size([1]))`.
+        """
+        super().__init__()
+        self.pref_model = pref_model
+        if isinstance(pref_model, DeterministicModel):
+            assert sampler is None
+            self.sampler = None
+        else:
+            if sampler is None:
+                self.sampler = IIDNormalSampler(sample_shape=torch.Size([1]))
+            else:
+                self.sampler = sampler
 
-    @concatenate_pending_points
-    @t_batch_mode_transform()
-    def forward(self, X: Tensor) -> Tensor:
-        r"""Evaluate qUpperConfidenceBound on the candidate set `X`.
+    def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
+        r"""Sample each element of samples.
 
         Args:
-            X: A `batch_sahpe x q x d`-dim Tensor of t-batches with `q` `d`-dim design
-                points each.
+            samples: A `sample_size x batch_shape x N x d`-dim Tensors of
+                samples from a model posterior.
 
         Returns:
-            A `batch_shape'`-dim Tensor of Upper Confidence Bound values at the given
-            design points `X`, where `batch_shape'` is the broadcasted batch shape of
-            model and input `X`.
+            A `(sample_size * num_samples) x batch_shape x N`-dim Tensor of
+            objective values sampled from utility posterior using `pref_model`.
         """
-        posterior = self.model.posterior(
-            X=X, posterior_transform=self.posterior_transform
-        )
-        samples = self.get_posterior_samples(posterior)
-        obj = self.objective(samples, X=X)
-        mean = obj.mean(dim=0)
-        ucb_samples = mean + self.beta_prime * (obj - mean).abs()
-        return ucb_samples.max(dim=-1)[0].mean(dim=0)
+        post = self.pref_model.posterior(samples)
+        if isinstance(self.pref_model, DeterministicModel):
+            # return preference posterior mean
+            return post.mean.squeeze(-1)
+        else:
+            # return preference posterior sample mean
+            samples = self.sampler(post).squeeze(-1)
+            return samples.reshape(-1, *samples.shape[2:])  # batch_shape x N
```

### Comparing `botorch-0.8.5/botorch/acquisition/multi_objective/__init__.py` & `botorch-0.9.1/botorch/acquisition/multi_objective/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 )
 from botorch.acquisition.multi_objective.multi_fidelity import MOMF
 from botorch.acquisition.multi_objective.objective import (
     AnalyticMultiOutputObjective,
     IdentityAnalyticMultiOutputObjective,
     IdentityMCMultiOutputObjective,
     MCMultiOutputObjective,
-    UnstandardizeAnalyticMultiOutputObjective,
     UnstandardizeMCMultiOutputObjective,
     WeightedMCMultiOutputObjective,
 )
 from botorch.acquisition.multi_objective.utils import (
     get_default_partitioning_alpha,
     prune_inferior_points_multi_objective,
 )
@@ -42,11 +41,10 @@
     "AnalyticMultiOutputObjective",
     "ExpectedHypervolumeImprovement",
     "IdentityAnalyticMultiOutputObjective",
     "IdentityMCMultiOutputObjective",
     "MCMultiOutputObjective",
     "MultiObjectiveAnalyticAcquisitionFunction",
     "MultiObjectiveMCAcquisitionFunction",
-    "UnstandardizeAnalyticMultiOutputObjective",
     "UnstandardizeMCMultiOutputObjective",
     "WeightedMCMultiOutputObjective",
 ]
```

### Comparing `botorch-0.8.5/botorch/acquisition/multi_objective/analytic.py` & `botorch-0.9.1/botorch/acquisition/multi_objective/analytic.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,27 +39,22 @@
 class MultiObjectiveAnalyticAcquisitionFunction(AcquisitionFunction):
     r"""Abstract base class for Multi-Objective batch acquisition functions."""
 
     def __init__(
         self,
         model: Model,
         posterior_transform: Optional[PosteriorTransform] = None,
-        **kwargs,
     ) -> None:
         r"""Constructor for the MultiObjectiveAnalyticAcquisitionFunction base class.
 
         Args:
             model: A fitted model.
             posterior_transform: A PosteriorTransform (optional).
         """
         super().__init__(model=model)
-        posterior_transform = self._deprecate_acqf_objective(
-            posterior_transform=posterior_transform,
-            objective=kwargs.get("objective"),
-        )
         if posterior_transform is None or isinstance(
             posterior_transform, PosteriorTransform
         ):
             self.posterior_transform = posterior_transform
         else:
             raise UnsupportedError(
                 "Only a posterior_transform of type PosteriorTransform is "
@@ -154,15 +149,15 @@
         self._cross_product_indices = torch.tensor(
             list(product(*[[0, 1] for _ in range(ref_point.shape[0])])),
             dtype=torch.long,
             device=ref_point.device,
         )
         self.normal = Normal(0, 1)
 
-    def psi(self, lower: Tensor, upper: Tensor, mu: Tensor, sigma: Tensor) -> None:
+    def psi(self, lower: Tensor, upper: Tensor, mu: Tensor, sigma: Tensor) -> Tensor:
         r"""Compute Psi function.
 
         For each cell i and outcome k:
 
             Psi(lower_{i,k}, upper_{i,k}, mu_k, sigma_k) = (
             sigma_k * PDF((upper_{i,k} - mu_k) / sigma_k) + (
             mu_k - lower_{i,k}
@@ -181,15 +176,15 @@
             A `batch_shape x num_cells x m`-dim tensor of values.
         """
         u = (upper - mu) / sigma
         return sigma * self.normal.log_prob(u).exp() + (mu - lower) * (
             1 - self.normal.cdf(u)
         )
 
-    def nu(self, lower: Tensor, upper: Tensor, mu: Tensor, sigma: Tensor) -> None:
+    def nu(self, lower: Tensor, upper: Tensor, mu: Tensor, sigma: Tensor) -> Tensor:
         r"""Compute Nu function.
 
         For each cell i and outcome k:
 
             nu(lower_{i,k}, upper_{i,k}, mu_k, sigma_k) = (
             upper_{i,k} - lower_{i,k}
             ) * (1 - CDF((upper_{i,k} - mu_k) / sigma_k))
```

### Comparing `botorch-0.8.5/botorch/acquisition/multi_objective/joint_entropy_search.py` & `botorch-0.9.1/botorch/acquisition/multi_objective/joint_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/acquisition/multi_objective/max_value_entropy_search.py` & `botorch-0.9.1/botorch/acquisition/multi_objective/max_value_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/acquisition/multi_objective/monte_carlo.py` & `botorch-0.9.1/botorch/acquisition/multi_objective/monte_carlo.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 from botorch.utils.multi_objective.box_decompositions.non_dominated import (
     FastNondominatedPartitioning,
     NondominatedPartitioning,
 )
 from botorch.utils.multi_objective.box_decompositions.utils import (
     _pad_batch_pareto_frontier,
 )
-from botorch.utils.objective import apply_constraints_nonnegative_soft
+from botorch.utils.objective import compute_smoothed_feasibility_indicator
 from botorch.utils.torch import BufferDict
 from botorch.utils.transforms import (
     concatenate_pending_points,
     is_fully_bayesian,
     match_batch_shape,
     t_batch_mode_transform,
 )
@@ -132,15 +132,15 @@
                 "sample q-batch shape being different than that of the inputs."
                 "Use a composite objective that applies feasibility weighting to"
                 "samples before calculating the risk measure."
             )
         self.add_module("objective", objective)
         self.constraints = constraints
         if constraints:
-            if type(eta) != Tensor:
+            if type(eta) is not Tensor:
                 eta = torch.full((len(constraints),), eta)
             self.register_buffer("eta", eta)
         self.X_pending = None
         if X_pending is not None:
             self.set_X_pending(X_pending)
 
     @abstractmethod
@@ -275,23 +275,17 @@
             improvement for each batch.
         """
         # Note that the objective may subset the outcomes (e.g. this will usually happen
         # if there are constraints present).
         obj = self.objective(samples, X=X)
         q = obj.shape[-2]
         if self.constraints is not None:
-            feas_weights = torch.ones(
-                obj.shape[:-1], device=obj.device, dtype=obj.dtype
-            )
-            feas_weights = apply_constraints_nonnegative_soft(
-                obj=feas_weights,
-                constraints=self.constraints,
-                samples=samples,
-                eta=self.eta,
-            )
+            feas_weights = compute_smoothed_feasibility_indicator(
+                constraints=self.constraints, samples=samples, eta=self.eta
+            )  # `sample_shape x batch-shape x q`
         self._cache_q_subset_indices(q_out=q)
         batch_shape = obj.shape[:-2]
         # this is n_samples x input_batch_shape x
         areas_per_segment = torch.zeros(
             *batch_shape,
             self.cell_lower_bounds.shape[-2],
             dtype=obj.dtype,
@@ -415,15 +409,16 @@
                 have points that have been submitted for function evaluation, but
                 have not yet been evaluated.
             eta: The temperature parameter for the sigmoid function used for the
                 differentiable approximation of the constraints. In case of a float the
                 same eta is used for every constraint in constraints. In case of a
                 tensor the length of the tensor must match the number of provided
                 constraints. The i-th constraint is then estimated with the i-th
-                eta value.
+                eta value. For more details, on this parameter, see the docs of
+                `compute_smoothed_feasibility_indicator`.
             prune_baseline: If True, remove points in `X_baseline` that are
                 highly unlikely to be the pareto optimal and better than the
                 reference point. This can significantly improve computation time and
                 is generally recommended. In order to customize pruning parameters,
                 instead manually call `prune_inferior_points_multi_objective` on
                 `X_baseline` before instantiating the acquisition function.
             alpha: The hyperparameter controlling the approximate non-dominated
@@ -438,14 +433,19 @@
             incremental_nehvi: A boolean indicating whether to compute the
                 incremental NEHVI from the `i`th point where `i=1, ..., q`
                 under sequential greedy optimization, or the full qNEHVI over
                 `q` points.
             cache_root: A boolean indicating whether to cache the root
                 decomposition over `X_baseline` and use low-rank updates.
         """
+        if len(ref_point) < 2:
+            raise ValueError(
+                "qNoisyExpectedHypervolumeImprovement supports m>=2 outcomes "
+                f"but ref_point has length {len(ref_point)}, which is smaller than 2."
+            )
         ref_point = torch.as_tensor(
             ref_point, dtype=X_baseline.dtype, device=X_baseline.device
         )
         super(qExpectedHypervolumeImprovement, self).__init__(
             model=model,
             sampler=sampler,
             objective=objective,
```

### Comparing `botorch-0.8.5/botorch/acquisition/multi_objective/multi_fidelity.py` & `botorch-0.9.1/botorch/acquisition/multi_objective/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/acquisition/multi_objective/multi_output_risk_measures.py` & `botorch-0.9.1/botorch/acquisition/multi_objective/multi_output_risk_measures.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/acquisition/multi_objective/objective.py` & `botorch-0.9.1/botorch/acquisition/multi_objective/objective.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,15 @@
 
 import warnings
 
 from abc import abstractmethod
 from typing import List, Optional
 
 import torch
-from botorch.acquisition.objective import (
-    AcquisitionObjective,
-    GenericMCObjective,
-    MCAcquisitionObjective,
-    UnstandardizePosteriorTransform,
-)
+from botorch.acquisition.objective import GenericMCObjective, MCAcquisitionObjective
 from botorch.exceptions.errors import BotorchError, BotorchTensorDimensionError
 from botorch.models.model import Model
 from botorch.posteriors import GPyTorchPosterior
 from botorch.utils import apply_constraints
 from botorch.utils.transforms import normalize_indices
 from torch import Tensor
 
@@ -258,54 +253,29 @@
         self.register_buffer("Y_std", Y_std)
 
     def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
         samples = super().forward(samples=samples)
         return samples * self.Y_std + self.Y_mean
 
 
-class AnalyticMultiOutputObjective(AcquisitionObjective):
+class AnalyticMultiOutputObjective(torch.nn.Module):
     r"""Abstract base class for multi-output analyic objectives.
 
     DEPRECATED - This will be removed in the next version.
 
     """
-    pass  # pragma: no cover
+
+    def __init__(self, *args, **kwargs) -> None:
+        """Initialize objective."""
+        warnings.warn("AnalyticMultiOutputObjective is deprecated.", DeprecationWarning)
+        super().__init__(*args, **kwargs)
 
 
 class IdentityAnalyticMultiOutputObjective(AnalyticMultiOutputObjective):
     """DEPRECATED - This will be removed in the next version."""
 
     def __init__(self):
         """Initialize objective."""
-        warnings.warn(
-            "IdentityAnalyticMultiOutputObjective is deprecated. "
-            "Use IdentityPosteriorTransform instead.",
-            DeprecationWarning,
-        )
         super().__init__()
 
     def forward(self, posterior: GPyTorchPosterior) -> GPyTorchPosterior:
         return posterior
-
-
-class UnstandardizeAnalyticMultiOutputObjective(
-    UnstandardizePosteriorTransform, AnalyticMultiOutputObjective
-):
-    r"""Objective that unstandardizes the posterior.
-
-    DEPRECATED - This will be removed in the next version.
-    """
-
-    def __init__(self, Y_mean: Tensor, Y_std: Tensor) -> None:
-        r"""Initialize objective.
-
-        Args:
-            Y_mean: `m`-dim tensor of outcome means
-            Y_std: `m`-dim tensor of outcome standard deviations
-
-        """
-        warnings.warn(
-            "UnstandardizeAnalyticMultiOutputObjective is deprecated. "
-            "Use UnstandardizePosteriorTransform instead.",
-            DeprecationWarning,
-        )
-        super().__init__(Y_mean=Y_mean, Y_std=Y_std)
```

### Comparing `botorch-0.8.5/botorch/acquisition/multi_objective/predictive_entropy_search.py` & `botorch-0.9.1/botorch/acquisition/multi_objective/predictive_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/acquisition/multi_objective/utils.py` & `botorch-0.9.1/botorch/acquisition/multi_objective/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/acquisition/multi_step_lookahead.py` & `botorch-0.9.1/botorch/acquisition/multi_step_lookahead.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,27 +111,20 @@
                 have been submitted for function evaluation but have not yet been
                 evaluated. Concatenated into `X` upon forward call. Copied and set to
                 have no gradient.
             collapse_fantasy_base_samples: If True, collapse_batch_dims of the Samplers
                 will be applied on fantasy batch dimensions as well, meaning that base
                 samples are the same in all subtrees starting from the same level.
         """
-        if not isinstance(objective, MCAcquisitionObjective):
-            # TODO: clean this up after removing AcquisitionObjective.
-            if posterior_transform is None:
-                posterior_transform = self._deprecate_acqf_objective(
-                    posterior_transform=posterior_transform,
-                    objective=objective,
-                )
-                objective = None
-            else:
-                raise RuntimeError(
-                    "Got both a non-MC objective (DEPRECATED) and a posterior "
-                    "transform. Use only a posterior transform instead."
-                )
+        if objective is not None and not isinstance(objective, MCAcquisitionObjective):
+            raise UnsupportedError(
+                "`qMultiStepLookahead` got a non-MC `objective`. This is not supported."
+                " Use `posterior_transform` and `objective=None` instead."
+            )
+
         super(MCAcquisitionFunction, self).__init__(model=model)
         self.batch_sizes = batch_sizes
         if not ((num_fantasies is None) ^ (samplers is None)):
             raise UnsupportedError(
                 "qMultiStepLookahead requires exactly one of `num_fantasies` or "
                 "`samplers` as arguments."
             )
@@ -152,15 +145,14 @@
         if inner_mc_samples is None:
             inner_mc_samples = [None] * (1 + len(num_fantasies))
         # TODO: Allow passing in inner samplers directly
         inner_samplers = _construct_inner_samplers(
             batch_sizes=batch_sizes,
             valfunc_cls=valfunc_cls,
             objective=objective,
-            posterior_transform=posterior_transform,
             inner_mc_samples=inner_mc_samples,
         )
         if valfunc_argfacs is None:
             valfunc_argfacs = [None] * (1 + len(batch_sizes))
 
         self.objective = objective
         self.posterior_transform = posterior_transform
@@ -508,34 +500,32 @@
 
 
 def _construct_inner_samplers(
     batch_sizes: List[int],
     valfunc_cls: List[Optional[Type[AcquisitionFunction]]],
     inner_mc_samples: List[Optional[int]],
     objective: Optional[MCAcquisitionObjective] = None,
-    posterior_transform: Optional[PosteriorTransform] = None,
 ) -> List[Optional[MCSampler]]:
     r"""Check validity of inputs and construct inner samplers.
 
     Helper function to be used internally for constructing inner samplers.
 
     Args:
         batch_sizes: A list `[q_1, ..., q_k]` containing the batch sizes for the
             `k` look-ahead steps.
         valfunc_cls: A list of `k + 1` acquisition function classes to be used as the
             (stage + terminal) value functions. Each element (except for the last one)
             can be `None`, in which case a zero stage value is assumed for the
             respective stage.
         inner_mc_samples: A list `[n_0, ..., n_k]` containing the number of MC
             samples to be used for evaluating the stage value function. Ignored if
-            the objective is `None` or a `ScalarizedObjective`.
+            the objective is `None`.
         objective: The objective under which the output is evaluated. If `None`, use
             the model output (requires a single-output model or a posterior transform).
             Otherwise the objective is MC-evaluated (using `inner_sampler`).
-        posterior_transform: A PosteriorTransform (optional).
 
     Returns:
         A list with `k + 1` elements that are either `MCSampler`s or `None.
     """
     inner_samplers = []
     for q, vfc, mcs in zip([None] + batch_sizes, valfunc_cls, inner_mc_samples):
         if vfc is None:
```

### Comparing `botorch-0.8.5/botorch/acquisition/objective.py` & `botorch-0.9.1/botorch/acquisition/logei.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,610 +1,521 @@
-#!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-r"""Objective Modules to be used with acquisition functions."""
+r"""
+Batch implementations of the LogEI family of improvements-based acquisition functions.
+"""
 
 from __future__ import annotations
 
-import inspect
-import warnings
-from abc import ABC, abstractmethod
-from typing import Callable, List, Optional, TYPE_CHECKING, Union
+from copy import deepcopy
+
+from functools import partial
+
+from typing import Any, Callable, List, Optional, Tuple, TypeVar, Union
 
 import torch
-from botorch.exceptions.errors import BotorchTensorDimensionError, UnsupportedError
+from botorch.acquisition.cached_cholesky import CachedCholeskyMCAcquisitionFunction
+from botorch.acquisition.monte_carlo import SampleReducingMCAcquisitionFunction
+from botorch.acquisition.objective import (
+    ConstrainedMCObjective,
+    MCAcquisitionObjective,
+    PosteriorTransform,
+)
+from botorch.acquisition.utils import (
+    compute_best_feasible_objective,
+    prune_inferior_points,
+)
+from botorch.exceptions.errors import BotorchError
 from botorch.models.model import Model
-from botorch.models.transforms.outcome import Standardize
-from botorch.posteriors.gpytorch import GPyTorchPosterior, scalarize_posterior
-from botorch.sampling import IIDNormalSampler, MCSampler
-from botorch.utils import apply_constraints
-from gpytorch.distributions import MultitaskMultivariateNormal, MultivariateNormal
-from linear_operator.operators.dense_linear_operator import to_linear_operator
+from botorch.sampling.base import MCSampler
+from botorch.utils.safe_math import (
+    fatmax,
+    log_fatplus,
+    log_softplus,
+    logmeanexp,
+    smooth_amax,
+)
+from botorch.utils.transforms import match_batch_shape
 from torch import Tensor
-from torch.nn import Module
-
-if TYPE_CHECKING:
-    from botorch.posteriors.posterior import Posterior  # pragma: no cover
-    from botorch.posteriors.posterior_list import PosteriorList  # pragma: no cover
 
+"""
+NOTE: On the default temperature parameters:
 
-class AcquisitionObjective(Module, ABC):
-    r"""Abstract base class for objectives.
+tau_relu: It is generally important to set `tau_relu` to be very small, in particular,
+smaller than the expected improvement value. Otherwise, the optimization can stagnate.
+By setting `tau_relu=1e-6` by default, stagnation is exceedingly unlikely to occur due
+to the smooth ReLU approximation for practical applications of BO.
+IDEA: We could consider shrinking `tau_relu` with the progression of the optimization.
+
+tau_max: This is only relevant for the batch (`q > 1`) case, and `tau_max=1e-2` is
+sufficient to get a good approximation to the maximum improvement in the batch of
+candidates. If `fat=False`, the smooth approximation to the maximum can saturate
+numerically. It is therefore recommended to use `fat=True` when optimizing batches
+of `q > 1` points.
+"""
+TAU_RELU = 1e-6
+TAU_MAX = 1e-2
+FloatOrTensor = TypeVar("FloatOrTensor", float, Tensor)
 
-    DEPRECATED - This will be removed in the next version.
-
-    :meta private:
-    """
-    ...
 
-
-class PosteriorTransform(Module, ABC):
+class LogImprovementMCAcquisitionFunction(SampleReducingMCAcquisitionFunction):
     r"""
-    Abstract base class for objectives that transform the posterior.
+    Abstract base class for Monte-Carlo-based batch LogEI acquisition functions.
 
     :meta private:
     """
 
-    @abstractmethod
-    def evaluate(self, Y: Tensor) -> Tensor:
-        r"""Evaluate the transform on a set of outcomes.
-
-        Args:
-            Y: A `batch_shape x q x m`-dim tensor of outcomes.
-
-        Returns:
-            A `batch_shape x q' [x m']`-dim tensor of transformed outcomes.
-        """
-        pass  # pragma: no cover
-
-    @abstractmethod
-    def forward(self, posterior) -> Posterior:
-        r"""Compute the transformed posterior.
-
-        Args:
-            posterior: The posterior to be transformed.
-
-        Returns:
-            The transformed posterior object.
-        """
-        pass  # pragma: no cover
-
-
-# import DeterministicModel after PosteriorTransform to avoid circular import
-from botorch.models.deterministic import DeterministicModel  # noqa
-
-
-class ScalarizedPosteriorTransform(PosteriorTransform):
-    r"""An affine posterior transform for scalarizing multi-output posteriors.
+    _log: bool = True
 
-    For a Gaussian posterior at a single point (`q=1`) with mean `mu` and
-    covariance matrix `Sigma`, this yields a single-output posterior with mean
-    `weights^T * mu` and variance `weights^T Sigma w`.
-
-    Example:
-        Example for a model with two outcomes:
-
-        >>> weights = torch.tensor([0.5, 0.25])
-        >>> posterior_transform = ScalarizedPosteriorTransform(weights)
-        >>> EI = ExpectedImprovement(
-        ... model, best_f=0.1, posterior_transform=posterior_transform
-        ... )
-    """
-
-    scalarize: bool = True
-
-    def __init__(self, weights: Tensor, offset: float = 0.0) -> None:
+    def __init__(
+        self,
+        model: Model,
+        sampler: Optional[MCSampler] = None,
+        objective: Optional[MCAcquisitionObjective] = None,
+        posterior_transform: Optional[PosteriorTransform] = None,
+        X_pending: Optional[Tensor] = None,
+        constraints: Optional[List[Callable[[Tensor], Tensor]]] = None,
+        eta: Union[Tensor, float] = 1e-3,
+        fat: bool = True,
+        tau_max: float = TAU_MAX,
+    ) -> None:
         r"""
         Args:
-            weights: A one-dimensional tensor with `m` elements representing the
-                linear weights on the outputs.
-            offset: An offset to be added to posterior mean.
-        """
-        if weights.dim() != 1:
-            raise ValueError("weights must be a one-dimensional tensor.")
-        super().__init__()
-        self.register_buffer("weights", weights)
-        self.offset = offset
-
-    def evaluate(self, Y: Tensor) -> Tensor:
-        r"""Evaluate the transform on a set of outcomes.
-
-        Args:
-            Y: A `batch_shape x q x m`-dim tensor of outcomes.
-
-        Returns:
-            A `batch_shape x q`-dim tensor of transformed outcomes.
-        """
-        return self.offset + Y @ self.weights
-
-    def forward(
-        self, posterior: Union[GPyTorchPosterior, PosteriorList]
-    ) -> GPyTorchPosterior:
-        r"""Compute the posterior of the affine transformation.
-
-        Args:
-            posterior: A posterior with the same number of outputs as the
-                elements in `self.weights`.
-
-        Returns:
-            A single-output posterior.
-        """
-        return scalarize_posterior(
-            posterior=posterior, weights=self.weights, offset=self.offset
+            model: A fitted model.
+            sampler: The sampler used to draw base samples. If not given,
+                a sampler is generated using `get_sampler`.
+                NOTE: For posteriors that do not support base samples,
+                a sampler compatible with intended use case must be provided.
+                See `ForkedRNGSampler` and `StochasticSampler` as examples.
+            objective: The MCAcquisitionObjective under which the samples are
+                evaluated. Defaults to `IdentityMCObjective()`.
+            posterior_transform: A PosteriorTransform (optional).
+            X_pending: A `batch_shape, m x d`-dim Tensor of `m` design points
+                that have points that have been submitted for function evaluation
+                but have not yet been evaluated.
+            constraints: A list of constraint callables which map a Tensor of posterior
+                samples of dimension `sample_shape x batch-shape x q x m`-dim to a
+                `sample_shape x batch-shape x q`-dim Tensor. The associated constraints
+                are satisfied if `constraint(samples) < 0`.
+            eta: Temperature parameter(s) governing the smoothness of the sigmoid
+                approximation to the constraint indicators. See the docs of
+                `compute_(log_)constraint_indicator` for more details on this parameter.
+            fat: Toggles the logarithmic / linear asymptotic behavior of the smooth
+                approximation to the ReLU.
+            tau_max: Temperature parameter controlling the sharpness of the
+                approximation to the `max` operator over the `q` candidate points.
+        """
+        if isinstance(objective, ConstrainedMCObjective):
+            raise BotorchError(
+                "Log-Improvement should not be used with `ConstrainedMCObjective`."
+                "Please pass the `constraints` directly to the constructor of the "
+                "acquisition function."
+            )
+        q_reduction = partial(fatmax if fat else smooth_amax, tau=tau_max)
+        super().__init__(
+            model=model,
+            sampler=sampler,
+            objective=objective,
+            posterior_transform=posterior_transform,
+            X_pending=X_pending,
+            sample_reduction=logmeanexp,
+            q_reduction=q_reduction,
+            constraints=constraints,
+            eta=eta,
+            fat=fat,
         )
+        self.tau_max = tau_max
 
 
-class ScalarizedObjective(ScalarizedPosteriorTransform, AcquisitionObjective):
-    """DEPRECATED - Use ScalarizedPosteriorTransform instead."""
-
-    def __init__(self, weights: Tensor, offset: float = 0.0) -> None:
-        r"""
-        Args:
-            weights: A one-dimensional tensor with `m` elements representing the
-                linear weights on the outputs.
-            offset: An offset to be added to posterior mean.
-        """
-        warnings.warn(
-            "ScalarizedObjective is deprecated and will be removed in the next "
-            "version. Use ScalarizedPosteriorTransform instead."
-        )
-        super().__init__(weights=weights, offset=offset)
+class qLogExpectedImprovement(LogImprovementMCAcquisitionFunction):
+    r"""MC-based batch Log Expected Improvement.
 
+    This computes qLogEI by
+    (1) sampling the joint posterior over q points,
+    (2) evaluating the smoothed log improvement over the current best for each sample,
+    (3) smoothly maximizing over q, and
+    (4) averaging over the samples in log space.
 
-class ExpectationPosteriorTransform(PosteriorTransform):
-    r"""Transform the `batch x (q * n_w) x m` posterior into a `batch x q x m`
-    posterior of the expectation. The expectation is calculated over each
-    consecutive `n_w` block of points in the posterior.
+    `qLogEI(X) ~ log(qEI(X)) = log(E(max(max Y - best_f, 0)))`,
 
-    This is intended for use with `InputPerturbation` or `AppendFeatures` for
-    optimizing the expectation over `n_w` points. This should not be used when
-    there are constraints present, since this does not take into account
-    the feasibility of the objectives.
+    where `Y ~ f(X)`, and `X = (x_1,...,x_q)`.
 
-    Note: This is different than `ScalarizedPosteriorTransform` in that
-    this operates over the q-batch dimension.
+    Example:
+        >>> model = SingleTaskGP(train_X, train_Y)
+        >>> best_f = train_Y.max()[0]
+        >>> sampler = SobolQMCNormalSampler(1024)
+        >>> qLogEI = qLogExpectedImprovement(model, best_f, sampler)
+        >>> qei = qLogEI(test_X)
     """
 
-    def __init__(self, n_w: int, weights: Optional[Tensor] = None) -> None:
-        r"""A posterior transform calculating the expectation over the q-batch
-        dimension.
-
-        Args:
-            n_w: The number of points in the q-batch of the posterior to compute
-                the expectation over. This corresponds to the size of the
-                `feature_set` of `AppendFeatures` or the size of the `perturbation_set`
-                of `InputPerturbation`.
-            weights: An optional `n_w x m`-dim tensor of weights. Can be used to
-                compute a weighted expectation. Weights are normalized before use.
-        """
-        super().__init__()
-        if weights is not None:
-            if weights.dim() != 2 or weights.shape[0] != n_w:
-                raise ValueError("`weights` must be a tensor of size `n_w x m`.")
-            if torch.any(weights < 0):
-                raise ValueError("`weights` must be non-negative.")
-        else:
-            weights = torch.ones(n_w, 1)
-        # Normalize the weights.
-        weights = weights / weights.sum(dim=0)
-        self.register_buffer("weights", weights)
-        self.n_w = n_w
-
-    def evaluate(self, Y: Tensor) -> Tensor:
-        r"""Evaluate the expectation of a set of outcomes.
+    def __init__(
+        self,
+        model: Model,
+        best_f: Union[float, Tensor],
+        sampler: Optional[MCSampler] = None,
+        objective: Optional[MCAcquisitionObjective] = None,
+        posterior_transform: Optional[PosteriorTransform] = None,
+        X_pending: Optional[Tensor] = None,
+        constraints: Optional[List[Callable[[Tensor], Tensor]]] = None,
+        eta: Union[Tensor, float] = 1e-3,
+        fat: bool = True,
+        tau_max: float = TAU_MAX,
+        tau_relu: float = TAU_RELU,
+    ) -> None:
+        r"""q-Log Expected Improvement.
 
         Args:
-            Y: A `batch_shape x (q * n_w) x m`-dim tensor of outcomes.
-
-        Returns:
-            A `batch_shape x q x m`-dim tensor of expectation outcomes.
-        """
-        batch_shape, m = Y.shape[:-2], Y.shape[-1]
-        weighted_Y = Y.view(*batch_shape, -1, self.n_w, m) * self.weights.to(Y)
-        return weighted_Y.sum(dim=-2)
+            model: A fitted model.
+            best_f: The best objective value observed so far (assumed noiseless). Can be
+                a `batch_shape`-shaped tensor, which in case of a batched model
+                specifies potentially different values for each element of the batch.
+            sampler: The sampler used to draw base samples. See `MCAcquisitionFunction`
+                more details.
+            objective: The MCAcquisitionObjective under which the samples are evaluated.
+                Defaults to `IdentityMCObjective()`.
+            posterior_transform: A PosteriorTransform (optional).
+            X_pending:  A `m x d`-dim Tensor of `m` design points that have been
+                submitted for function evaluation but have not yet been evaluated.
+                Concatenated into `X` upon forward call. Copied and set to have no
+                gradient.
+            constraints: A list of constraint callables which map a Tensor of posterior
+                samples of dimension `sample_shape x batch-shape x q x m`-dim to a
+                `sample_shape x batch-shape x q`-dim Tensor. The associated constraints
+                are satisfied if `constraint(samples) < 0`.
+            eta: Temperature parameter(s) governing the smoothness of the sigmoid
+                approximation to the constraint indicators. See the docs of
+                `compute_(log_)smoothed_constraint_indicator` for details.
+            fat: Toggles the logarithmic / linear asymptotic behavior of the smooth
+                approximation to the ReLU.
+            tau_max: Temperature parameter controlling the sharpness of the smooth
+                approximations to max.
+            tau_relu: Temperature parameter controlling the sharpness of the smooth
+                approximations to ReLU.
+        """
+        super().__init__(
+            model=model,
+            sampler=sampler,
+            objective=objective,
+            posterior_transform=posterior_transform,
+            X_pending=X_pending,
+            constraints=constraints,
+            eta=eta,
+            tau_max=check_tau(tau_max, name="tau_max"),
+            fat=fat,
+        )
+        self.register_buffer("best_f", torch.as_tensor(best_f))
+        self.tau_relu = check_tau(tau_relu, name="tau_relu")
 
-    def forward(self, posterior: GPyTorchPosterior) -> GPyTorchPosterior:
-        r"""Compute the posterior of the expectation.
+    def _sample_forward(self, obj: Tensor) -> Tensor:
+        r"""Evaluate qLogExpectedImprovement on the candidate set `X`.
 
         Args:
-            posterior: An `m`-outcome joint posterior over `q * n_w` points.
+            obj: `mc_shape x batch_shape x q`-dim Tensor of MC objective values.
 
         Returns:
-            An `m`-outcome joint posterior over `q` expectations.
+            A `mc_shape x batch_shape x q`-dim Tensor of expected improvement values.
         """
-        org_mvn = posterior.distribution
-        if getattr(org_mvn, "_interleaved", False):
-            raise UnsupportedError(
-                "`ExpectationPosteriorTransform` does not support "
-                "interleaved posteriors."
-            )
-        # Initialize the weight matrix of shape compatible with the mvn.
-        org_event_shape = org_mvn.event_shape
-        batch_shape = org_mvn.batch_shape
-        q = org_event_shape[0] // self.n_w
-        m = 1 if len(org_event_shape) == 1 else org_event_shape[-1]
-        tkwargs = {"device": org_mvn.loc.device, "dtype": org_mvn.loc.dtype}
-        weights = torch.zeros(q * m, q * self.n_w * m, **tkwargs)
-        # Make sure self.weights has the correct dtype/device and shape.
-        self.weights = self.weights.to(org_mvn.loc).expand(self.n_w, m)
-        # Fill in the non-zero entries of the weight matrix.
-        # We want each row to have non-zero weights for the corresponding
-        # `n_w` sized diagonal. The `m` outcomes are not interleaved.
-        for i in range(q * m):
-            weights[i, self.n_w * i : self.n_w * (i + 1)] = self.weights[:, i // q]
-        # Trasform the mean.
-        new_loc = (
-            (weights @ org_mvn.loc.unsqueeze(-1))
-            .view(*batch_shape, m, q)
-            .transpose(-1, -2)
+        li = _log_improvement(
+            Y=obj,
+            best_f=self.best_f,
+            tau=self.tau_relu,
+            fat=self._fat,
         )
-        # Transform the covariance matrix.
-        org_cov = (
-            org_mvn.lazy_covariance_matrix
-            if org_mvn.islazy
-            else org_mvn.covariance_matrix
-        )
-        new_cov = weights @ (org_cov @ weights.t())
-        if m == 1:
-            new_mvn = MultivariateNormal(
-                new_loc.squeeze(-1), to_linear_operator(new_cov)
-            )
-        else:
-            # Using MTMVN since we pass a single loc and covar for all `m` outputs.
-            new_mvn = MultitaskMultivariateNormal(
-                new_loc, to_linear_operator(new_cov), interleaved=False
-            )
-        return GPyTorchPosterior(distribution=new_mvn)
+        return li
 
 
-class UnstandardizePosteriorTransform(PosteriorTransform):
-    r"""Posterior transform that unstandardizes the posterior.
+class qLogNoisyExpectedImprovement(
+    LogImprovementMCAcquisitionFunction, CachedCholeskyMCAcquisitionFunction
+):
+    r"""MC-based batch Log Noisy Expected Improvement.
+
+    This function does not assume a `best_f` is known (which would require
+    noiseless observations). Instead, it uses samples from the joint posterior
+    over the `q` test points and previously observed points. A smooth approximation
+    to the canonical improvement over previously observed points is computed
+    for each sample and the logarithm of the average is returned.
 
-    TODO: remove this when MultiTask models support outcome transforms.
+    `qLogNEI(X) ~ log(qNEI(X)) = Log E(max(max Y - max Y_baseline, 0))`, where
+    `(Y, Y_baseline) ~ f((X, X_baseline)), X = (x_1,...,x_q)`
 
     Example:
-        >>> unstd_transform = UnstandardizePosteriorTransform(Y_mean, Y_std)
-        >>> unstd_posterior = unstd_transform(posterior)
+        >>> model = SingleTaskGP(train_X, train_Y)
+        >>> sampler = SobolQMCNormalSampler(1024)
+        >>> qLogNEI = qLogNoisyExpectedImprovement(model, train_X, sampler)
+        >>> acqval = qLogNEI(test_X)
     """
 
-    def __init__(self, Y_mean: Tensor, Y_std: Tensor) -> None:
-        r"""Initialize objective.
+    def __init__(
+        self,
+        model: Model,
+        X_baseline: Tensor,
+        sampler: Optional[MCSampler] = None,
+        objective: Optional[MCAcquisitionObjective] = None,
+        posterior_transform: Optional[PosteriorTransform] = None,
+        X_pending: Optional[Tensor] = None,
+        constraints: Optional[List[Callable[[Tensor], Tensor]]] = None,
+        eta: Union[Tensor, float] = 1e-3,
+        fat: bool = True,
+        prune_baseline: bool = False,
+        cache_root: bool = True,
+        tau_max: float = TAU_MAX,
+        tau_relu: float = TAU_RELU,
+        **kwargs: Any,
+    ) -> None:
+        r"""q-Noisy Expected Improvement.
 
         Args:
-            Y_mean: `m`-dim tensor of outcome means
-            Y_std: `m`-dim tensor of outcome standard deviations
-
-        """
-        if Y_mean.ndim > 1 or Y_std.ndim > 1:
-            raise BotorchTensorDimensionError(
-                "Y_mean and Y_std must both be 1-dimensional, but got "
-                f"{Y_mean.ndim} and {Y_std.ndim}"
-            )
-        super().__init__()
-        self.outcome_transform = Standardize(m=Y_mean.shape[0]).to(Y_mean)
-        Y_std_unsqueezed = Y_std.unsqueeze(0)
-        self.outcome_transform.means = Y_mean.unsqueeze(0)
-        self.outcome_transform.stdvs = Y_std_unsqueezed
-        self.outcome_transform._stdvs_sq = Y_std_unsqueezed.pow(2)
-        self.outcome_transform.eval()
-
-    def evaluate(self, Y: Tensor) -> Tensor:
-        return self.outcome_transform.untransform(Y)[0]
-
-    def forward(self, posterior: GPyTorchPosterior) -> Tensor:
-        return self.outcome_transform.untransform_posterior(posterior)
-
-
-class MCAcquisitionObjective(Module, ABC):
-    r"""Abstract base class for MC-based objectives.
-
-    Args:
-        _verify_output_shape: If True and `X` is given, check that the q-batch
-            shape of the objectives agrees with that of X.
-        _is_mo: A boolean denoting whether the objectives are multi-output.
-
-    :meta private:
-    """
-
-    _verify_output_shape: bool = True
-    _is_mo: bool = False
+            model: A fitted model.
+            X_baseline: A `batch_shape x r x d`-dim Tensor of `r` design points
+                that have already been observed. These points are considered as
+                the potential best design point.
+            sampler: The sampler used to draw base samples. See `MCAcquisitionFunction`
+                more details.
+            objective: The MCAcquisitionObjective under which the samples are
+                evaluated. Defaults to `IdentityMCObjective()`.
+            posterior_transform: A PosteriorTransform (optional).
+            X_pending: A `batch_shape x m x d`-dim Tensor of `m` design points
+                that have points that have been submitted for function evaluation
+                but have not yet been evaluated. Concatenated into `X` upon
+                forward call. Copied and set to have no gradient.
+            constraints: A list of constraint callables which map a Tensor of posterior
+                samples of dimension `sample_shape x batch-shape x q x m`-dim to a
+                `sample_shape x batch-shape x q`-dim Tensor. The associated constraints
+                are satisfied if `constraint(samples) < 0`.
+            eta: Temperature parameter(s) governing the smoothness of the sigmoid
+                approximation to the constraint indicators. See the docs of
+                `compute_(log_)smoothed_constraint_indicator` for details.
+            fat: Toggles the logarithmic / linear asymptotic behavior of the smooth
+                approximation to the ReLU.
+            prune_baseline: If True, remove points in `X_baseline` that are
+                highly unlikely to be the best point. This can significantly
+                improve performance and is generally recommended. In order to
+                customize pruning parameters, instead manually call
+                `botorch.acquisition.utils.prune_inferior_points` on `X_baseline`
+                before instantiating the acquisition function.
+            cache_root: A boolean indicating whether to cache the root
+                decomposition over `X_baseline` and use low-rank updates.
+            tau_max: Temperature parameter controlling the sharpness of the smooth
+                approximations to max.
+            tau_relu: Temperature parameter controlling the sharpness of the smooth
+                approximations to ReLU.
+            kwargs: Here for qNEI for compatibility.
+
+        TODO: similar to qNEHVI, when we are using sequential greedy candidate
+        selection, we could incorporate pending points X_baseline and compute
+        the incremental q(Log)NEI from the new point. This would greatly increase
+        efficiency for large batches.
+        """
+        # TODO: separate out baseline variables initialization and other functions
+        # in qNEI to avoid duplication of both code and work at runtime.
+        super().__init__(
+            model=model,
+            sampler=sampler,
+            objective=objective,
+            posterior_transform=posterior_transform,
+            X_pending=X_pending,
+            constraints=constraints,
+            eta=eta,
+            fat=fat,
+            tau_max=tau_max,
+        )
+        self.tau_relu = tau_relu
+        self._init_baseline(
+            model=model,
+            X_baseline=X_baseline,
+            sampler=sampler,
+            objective=objective,
+            posterior_transform=posterior_transform,
+            prune_baseline=prune_baseline,
+            cache_root=cache_root,
+            **kwargs,
+        )
 
-    @abstractmethod
-    def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
-        r"""Evaluate the objective on the samples.
+    def _sample_forward(self, obj: Tensor) -> Tensor:
+        r"""Evaluate qLogNoisyExpectedImprovement per sample on the candidate set `X`.
 
         Args:
-            samples: A `sample_shape x batch_shape x q x m`-dim Tensors of
-                samples from a model posterior.
-            X: A `batch_shape x q x d`-dim tensor of inputs. Relevant only if
-                the objective depends on the inputs explicitly.
+            obj: `mc_shape x batch_shape x q`-dim Tensor of MC objective values.
 
         Returns:
-            Tensor: A `sample_shape x batch_shape x q`-dim Tensor of objective
-            values (assuming maximization).
-
-        This method is usually not called directly, but via the objectives.
-
-        Example:
-            >>> # `__call__` method:
-            >>> samples = sampler(posterior)
-            >>> outcome = mc_obj(samples)
+            A `sample_shape x batch_shape x q`-dim Tensor of log noisy expected smoothed
+            improvement values.
         """
-        pass  # pragma: no cover
+        return _log_improvement(
+            Y=obj,
+            best_f=self.compute_best_f(obj),
+            tau=self.tau_relu,
+            fat=self._fat,
+        )
 
-    def __call__(
-        self, samples: Tensor, X: Optional[Tensor] = None, *args, **kwargs
-    ) -> Tensor:
-        output = super().__call__(samples=samples, X=X, *args, **kwargs)
-        # q-batch dimension is at -1 for single-output objectives and at
-        # -2 for multi-output objectives.
-        q_batch_idx = -2 if self._is_mo else -1
-        if (
-            X is not None
-            and self._verify_output_shape
-            and output.shape[q_batch_idx] != X.shape[-2]
-        ):
-            raise RuntimeError(
-                "The q-batch shape of the objective values does not agree with "
-                f"the q-batch shape of X. Got {output.shape[q_batch_idx]} and "
-                f"{X.shape[-2]}. This may happen if you used a one-to-many input "
-                "transform but forgot to use a corresponding objective."
+    def _init_baseline(
+        self,
+        model: Model,
+        X_baseline: Tensor,
+        sampler: Optional[MCSampler] = None,
+        objective: Optional[MCAcquisitionObjective] = None,
+        posterior_transform: Optional[PosteriorTransform] = None,
+        prune_baseline: bool = False,
+        cache_root: bool = True,
+        **kwargs: Any,
+    ) -> None:
+        # setup of CachedCholeskyMCAcquisitionFunction
+        self._setup(model=model, cache_root=cache_root)
+        if prune_baseline:
+            X_baseline = prune_inferior_points(
+                model=model,
+                X=X_baseline,
+                objective=objective,
+                posterior_transform=posterior_transform,
+                marginalize_dim=kwargs.get("marginalize_dim"),
             )
-        return output
-
-
-class IdentityMCObjective(MCAcquisitionObjective):
-    r"""Trivial objective extracting the last dimension.
-
-    Example:
-        >>> identity_objective = IdentityMCObjective()
-        >>> samples = sampler(posterior)
-        >>> objective = identity_objective(samples)
-    """
-
-    def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
-        return samples.squeeze(-1)
-
-
-class LinearMCObjective(MCAcquisitionObjective):
-    r"""Linear objective constructed from a weight tensor.
-
-    For input `samples` and `mc_obj = LinearMCObjective(weights)`, this produces
-    `mc_obj(samples) = sum_{i} weights[i] * samples[..., i]`
-
-    Example:
-        Example for a model with two outcomes:
-
-        >>> weights = torch.tensor([0.75, 0.25])
-        >>> linear_objective = LinearMCObjective(weights)
-        >>> samples = sampler(posterior)
-        >>> objective = linear_objective(samples)
-    """
-
-    def __init__(self, weights: Tensor) -> None:
-        r"""
-        Args:
-            weights: A one-dimensional tensor with `m` elements representing the
-                linear weights on the outputs.
-        """
-        super().__init__()
-        if weights.dim() != 1:
-            raise ValueError("weights must be a one-dimensional tensor.")
-        self.register_buffer("weights", weights)
+        self.register_buffer("X_baseline", X_baseline)
+        # registering buffers for _get_samples_and_objectives in the next `if` block
+        self.register_buffer("baseline_samples", None)
+        self.register_buffer("baseline_obj", None)
+        if self._cache_root:
+            self.q_in = -1
+            # set baseline samples
+            with torch.no_grad():  # this is _get_samples_and_objectives(X_baseline)
+                posterior = self.model.posterior(
+                    X_baseline, posterior_transform=self.posterior_transform
+                )
+                # Note: The root decomposition is cached in two different places. It
+                # may be confusing to have two different caches, but this is not
+                # trivial to change since each is needed for a different reason:
+                # - LinearOperator caching to `posterior.mvn` allows for reuse within
+                #   this function, which may be helpful if the same root decomposition
+                #   is produced by the calls to `self.base_sampler` and
+                #   `self._cache_root_decomposition`.
+                # - self._baseline_L allows a root decomposition to be persisted outside
+                #   this method.
+                self.baseline_samples = self.get_posterior_samples(posterior)
+                self.baseline_obj = self.objective(self.baseline_samples, X=X_baseline)
+
+            # We make a copy here because we will write an attribute `base_samples`
+            # to `self.base_sampler.base_samples`, and we don't want to mutate
+            # `self.sampler`.
+            self.base_sampler = deepcopy(self.sampler)
+            self.register_buffer(
+                "_baseline_best_f",
+                self._compute_best_feasible_objective(
+                    samples=self.baseline_samples, obj=self.baseline_obj
+                ),
+            )
+            self._baseline_L = self._compute_root_decomposition(posterior=posterior)
 
-    def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
-        r"""Evaluate the linear objective on the samples.
+    def compute_best_f(self, obj: Tensor) -> Tensor:
+        """Computes the best (feasible) noisy objective value.
 
         Args:
-            samples: A `sample_shape x batch_shape x q x m`-dim tensors of
-                samples from a model posterior.
-            X: A `batch_shape x q x d`-dim tensor of inputs. Relevant only if
-                the objective depends on the inputs explicitly.
+            obj: `sample_shape x batch_shape x q`-dim Tensor of objectives in forward.
 
         Returns:
-            A `sample_shape x batch_shape x q`-dim tensor of objective values.
+            A `sample_shape x batch_shape x 1`-dim Tensor of best feasible objectives.
         """
-        if samples.shape[-1] != self.weights.shape[-1]:
-            raise RuntimeError("Output shape of samples not equal to that of weights")
-        return torch.einsum("...m, m", [samples, self.weights])
-
-
-class GenericMCObjective(MCAcquisitionObjective):
-    r"""Objective generated from a generic callable.
-
-    Allows to construct arbitrary MC-objective functions from a generic
-    callable. In order to be able to use gradient-based acquisition function
-    optimization it should be possible to backpropagate through the callable.
-
-    Example:
-        >>> generic_objective = GenericMCObjective(
-                lambda Y, X: torch.sqrt(Y).sum(dim=-1),
-            )
-        >>> samples = sampler(posterior)
-        >>> objective = generic_objective(samples)
-    """
-
-    def __init__(self, objective: Callable[[Tensor, Optional[Tensor]], Tensor]) -> None:
-        r"""
-        Args:
-            objective: A callable `f(samples, X)` mapping a
-                `sample_shape x batch-shape x q x m`-dim Tensor `samples` and
-                an optional `batch-shape x q x d`-dim Tensor `X` to a
-                `sample_shape x batch-shape x q`-dim Tensor of objective values.
-        """
-        super().__init__()
-        if len(inspect.signature(objective).parameters) == 1:
-            warnings.warn(
-                "The `objective` callable of `GenericMCObjective` is expected to "
-                "take two arguments. Passing a callable that expects a single "
-                "argument will result in an error in future versions.",
-                DeprecationWarning,
-            )
-
-            def obj(samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
-                return objective(samples)
-
-            self.objective = obj
+        if self._cache_root:
+            val = self._baseline_best_f
         else:
-            self.objective = objective
+            val = self._compute_best_feasible_objective(
+                samples=self.baseline_samples, obj=self.baseline_obj
+            )
+        # ensuring shape, dtype, device compatibility with obj
+        n_sample_dims = len(self.sample_shape)
+        view_shape = torch.Size(
+            [
+                *val.shape[:n_sample_dims],  # sample dimensions
+                *(1,) * (obj.ndim - val.ndim),  # pad to match obj
+                *val.shape[n_sample_dims:],  # the rest
+            ]
+        )
+        return val.view(view_shape).to(obj)
 
-    def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
-        r"""Evaluate the feasibility-weigthed objective on the samples.
+    def _get_samples_and_objectives(self, X: Tensor) -> Tuple[Tensor, Tensor]:
+        r"""Compute samples at new points, using the cached root decomposition.
 
         Args:
-            samples: A `sample_shape x batch_shape x q x m`-dim Tensors of
-                samples from a model posterior.
-            X: A `batch_shape x q x d`-dim tensor of inputs. Relevant only if
-                the objective depends on the inputs explicitly.
+            X: A `batch_shape x q x d`-dim tensor of inputs.
 
         Returns:
-            A `sample_shape x batch_shape x q`-dim Tensor of objective values
-            weighted by feasibility (assuming maximization).
-        """
-        return self.objective(samples, X=X)
-
-
-class ConstrainedMCObjective(GenericMCObjective):
-    r"""Feasibility-weighted objective.
-
-    An Objective allowing to maximize some scalable objective on the model
-    outputs subject to a number of constraints. Constraint feasibilty is
-    approximated by a sigmoid function.
-
-        mc_acq(X) = (
-        (objective(X) + infeasible_cost) * \prod_i (1  - sigmoid(constraint_i(X)))
-        ) - infeasible_cost
-
-    See `botorch.utils.objective.apply_constraints` for details on the constraint
-    handling.
-
-    Example:
-        >>> bound = 0.0
-        >>> objective = lambda Y: Y[..., 0]
-        >>> # apply non-negativity constraint on f(x)[1]
-        >>> constraint = lambda Y: bound - Y[..., 1]
-        >>> constrained_objective = ConstrainedMCObjective(objective, [constraint])
-        >>> samples = sampler(posterior)
-        >>> objective = constrained_objective(samples)
-    """
-
-    def __init__(
-        self,
-        objective: Callable[[Tensor, Optional[Tensor]], Tensor],
-        constraints: List[Callable[[Tensor], Tensor]],
-        infeasible_cost: Union[Tensor, float] = 0.0,
-        eta: Union[Tensor, float] = 1e-3,
-    ) -> None:
-        r"""
-        Args:
-            objective: A callable `f(samples, X)` mapping a
-                `sample_shape x batch-shape x q x m`-dim Tensor `samples` and
-                an optional `batch-shape x q x d`-dim Tensor `X` to a
-                `sample_shape x batch-shape x q`-dim Tensor of objective values.
-            constraints: A list of callables, each mapping a Tensor of dimension
-                `sample_shape x batch-shape x q x m` to a Tensor of dimension
-                `sample_shape x batch-shape x q`, where negative values imply
-                feasibility.
-            infeasible_cost: The cost of a design if all associated samples are
-                infeasible.
-            eta: The temperature parameter of the sigmoid function approximating
-                the constraint. Can be either a float or a 1-dim tensor. In case
-                of a float the same eta is used for every constraint in
-                constraints. In case of a tensor the length of the tensor must
-                match the number of provided constraints. The i-th constraint is
-                then estimated with the i-th eta value.
+            A two-tuple `(samples, obj)`, where `samples` is a tensor of posterior
+            samples with shape `sample_shape x batch_shape x q x m`, and `obj` is a
+            tensor of MC objective values with shape `sample_shape x batch_shape x q`.
         """
-        super().__init__(objective=objective)
-        self.constraints = constraints
-        if type(eta) != Tensor:
-            eta = torch.full((len(constraints),), eta)
-        self.register_buffer("eta", eta)
-        self.register_buffer("infeasible_cost", torch.as_tensor(infeasible_cost))
-
-    def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
-        r"""Evaluate the feasibility-weighted objective on the samples.
-
-        Args:
-            samples: A `sample_shape x batch_shape x q x m`-dim Tensors of
-                samples from a model posterior.
-            X: A `batch_shape x q x d`-dim tensor of inputs. Relevant only if
-                the objective depends on the inputs explicitly.
+        n_baseline, q = self.X_baseline.shape[-2], X.shape[-2]
+        X_full = torch.cat([match_batch_shape(self.X_baseline, X), X], dim=-2)
+        # TODO: Implement more efficient way to compute posterior over both training and
+        # test points in GPyTorch (https://github.com/cornellius-gp/gpytorch/issues/567)
+        posterior = self.model.posterior(
+            X_full, posterior_transform=self.posterior_transform
+        )
+        if not self._cache_root:
+            samples_full = super().get_posterior_samples(posterior)
+            obj_full = self.objective(samples_full, X=X_full)
+            # assigning baseline buffers so `best_f` can be computed in _sample_forward
+            self.baseline_samples, samples = samples_full.split([n_baseline, q], dim=-2)
+            self.baseline_obj, obj = obj_full.split([n_baseline, q], dim=-1)
+            return samples, obj
+
+        # handle one-to-many input transforms
+        n_plus_q = X_full.shape[-2]
+        n_w = posterior._extended_shape()[-2] // n_plus_q
+        q_in = q * n_w
+        self._set_sampler(q_in=q_in, posterior=posterior)
+        samples = self._get_f_X_samples(posterior=posterior, q_in=q_in)
+        obj = self.objective(samples, X=X_full[..., -q:, :])
+        return samples, obj
 
-        Returns:
-            A `sample_shape x batch_shape x q`-dim Tensor of objective values
-            weighted by feasibility (assuming maximization).
-        """
-        obj = super().forward(samples=samples)
-        return apply_constraints(
-            obj=obj,
-            constraints=self.constraints,
+    def _compute_best_feasible_objective(self, samples: Tensor, obj: Tensor) -> Tensor:
+        return compute_best_feasible_objective(
             samples=samples,
-            infeasible_cost=self.infeasible_cost,
-            eta=self.eta,
+            obj=obj,
+            constraints=self._constraints,
+            model=self.model,
+            objective=self.objective,
+            posterior_transform=self.posterior_transform,
+            X_baseline=self.X_baseline,
         )
 
 
-class LearnedObjective(MCAcquisitionObjective):
-    r"""Learned preference objective constructed from a preference model.
+"""
+###################################### utils ##########################################
+"""
 
-    For input `samples`, it samples each individual sample again from the latent
-    preference posterior distribution using `pref_model` and return the posterior mean.
 
-    Example:
-        >>> train_X = torch.rand(2, 2)
-        >>> train_comps = torch.LongTensor([[0, 1]])
-        >>> pref_model = PairwiseGP(train_X, train_comps)
-        >>> learned_pref_obj = LearnedObjective(pref_model)
-        >>> samples = sampler(posterior)
-        >>> objective = learned_pref_obj(samples)
-    """
+def _log_improvement(
+    Y: Tensor,
+    best_f: Tensor,
+    tau: Union[float, Tensor],
+    fat: bool,
+) -> Tensor:
+    """Computes the logarithm of the softplus-smoothed improvement, i.e.
+    `log_softplus(Y - best_f, beta=(1 / tau))`.
+    Note that softplus is an approximation to the regular ReLU objective whose maximum
+    pointwise approximation error is linear with respect to tau as tau goes to zero.
 
-    def __init__(
-        self,
-        pref_model: Model,
-        sampler: Optional[MCSampler] = None,
-    ):
-        r"""
-        Args:
-            pref_model: A BoTorch model, which models the latent preference/utility
-                function. Given an input tensor of size
-                `sample_size x batch_shape x N x d`, its `posterior` method should
-                return a `Posterior` object with single outcome representing the
-                utility values of the input.
-            sampler: Sampler for the preference model to account for uncertainty in
-                preferece when calculating the objective; it's not the one used
-                in MC acquisition functions. If None,
-                it uses `IIDNormalSampler(sample_shape=torch.Size([1]))`.
-        """
-        super().__init__()
-        self.pref_model = pref_model
-        if isinstance(pref_model, DeterministicModel):
-            assert sampler is None
-            self.sampler = None
-        else:
-            if sampler is None:
-                self.sampler = IIDNormalSampler(sample_shape=torch.Size([1]))
-            else:
-                self.sampler = sampler
-
-    def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
-        r"""Sample each element of samples.
-
-        Args:
-            samples: A `sample_size x batch_shape x N x d`-dim Tensors of
-                samples from a model posterior.
-
-        Returns:
-            A `(sample_size * num_samples) x batch_shape x N`-dim Tensor of
-            objective values sampled from utility posterior using `pref_model`.
-        """
-        post = self.pref_model.posterior(samples)
-        if isinstance(self.pref_model, DeterministicModel):
-            # return preference posterior mean
-            return post.mean.squeeze(-1)
-        else:
-            # return preference posterior sample mean
-            samples = self.sampler(post).squeeze(-1)
-            return samples.reshape(-1, *samples.shape[2:])  # batch_shape x N
+    Args:
+        obj: `mc_samples x batch_shape x q`-dim Tensor of output samples.
+        best_f: Best previously observed objective value(s), broadcastable with `obj`.
+        tau: Temperature parameter for smooth approximation of ReLU.
+            as `tau -> 0`, maximum pointwise approximation error is linear w.r.t. `tau`.
+        fat: Toggles the logarithmic / linear asymptotic behavior of the
+            smooth approximation to ReLU.
+
+    Returns:
+        A `mc_samples x batch_shape x q`-dim Tensor of improvement values.
+    """
+    log_soft_clamp = log_fatplus if fat else log_softplus
+    Z = Y - best_f.to(Y)
+    return log_soft_clamp(Z, tau=tau)  # ~ ((Y - best_f) / Y_std).clamp(0)
+
+
+def check_tau(tau: FloatOrTensor, name: str) -> FloatOrTensor:
+    """Checks the validity of the tau arguments of the functions below, and returns
+    `tau` if it is valid."""
+    if isinstance(tau, Tensor) and tau.numel() != 1:
+        raise ValueError(name + f" is not a scalar: {tau.numel() = }.")
+    if not (tau > 0):
+        raise ValueError(name + f" is non-positive: {tau = }.")
+    return tau
```

### Comparing `botorch-0.8.5/botorch/acquisition/penalized.py` & `botorch-0.9.1/botorch/acquisition/penalized.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 r"""
 Modules to add regularization to acquisition functions.
 """
 
 from __future__ import annotations
 
 import math
-from typing import Callable, List, Optional
+from typing import Any, Callable, List, Optional
 
 import torch
 from botorch.acquisition.acquisition import AcquisitionFunction
 from botorch.acquisition.analytic import AnalyticAcquisitionFunction
 from botorch.acquisition.objective import GenericMCObjective
 from botorch.exceptions import UnsupportedError
 from torch import Tensor
@@ -135,14 +135,74 @@
 
         regularization_term = group_lasso_regularizer(
             X=X.squeeze(-2) - self.init_point, groups=self.groups
         )
         return regularization_term
 
 
+def narrow_gaussian(X: Tensor, a: Tensor) -> Tensor:
+    return torch.exp(-0.5 * (X / a) ** 2)
+
+
+def nnz_approx(X: Tensor, target_point: Tensor, a: Tensor) -> Tensor:
+    r"""Differentiable relaxation of ||X - target_point||_0
+
+    Args:
+        X: An `n x d` tensor of inputs.
+        target_point: A tensor of size `n` corresponding to the target point.
+        a: A scalar tensor that controls the differentiable relaxation.
+    """
+    d = X.shape[-1]
+    if d != target_point.shape[-1]:
+        raise ValueError("X and target_point have different shapes.")
+    return d - narrow_gaussian(X - target_point, a).sum(dim=-1, keepdim=True)
+
+
+class L0Approximation(torch.nn.Module):
+    r"""Differentiable relaxation of the L0 norm using a Gaussian basis function."""
+
+    def __init__(self, target_point: Tensor, a: float = 1.0, **tkwargs: Any) -> None:
+        r"""Initializing L0 penalty with differentiable relaxation.
+
+        Args:
+            target_point: A tensor corresponding to the target point.
+            a: A hyperparameter that controls the differentiable relaxation.
+        """
+        super().__init__()
+        self.target_point = target_point
+        # hyperparameter to control the differentiable relaxation in L0 norm function.
+        self.register_buffer("a", torch.tensor(a, **tkwargs))
+
+    def __call__(self, X: Tensor) -> Tensor:
+        return nnz_approx(X=X, target_point=self.target_point, a=self.a)
+
+
+class L0PenaltyApprox(L0Approximation):
+    r"""Differentiable relaxation of the L0 norm to be added to any arbitrary
+    acquisition function to construct a PenalizedAcquisitionFunction."""
+
+    def __init__(self, target_point: Tensor, a: float = 1.0, **tkwargs: Any) -> None:
+        r"""Initializing L0 penalty with differentiable relaxation.
+
+        Args:
+            target_point: A tensor corresponding to the target point.
+            a: A hyperparameter that controls the differentiable relaxation.
+        """
+        super().__init__(target_point=target_point, a=a, **tkwargs)
+
+    def __call__(self, X: Tensor) -> Tensor:
+        r"""
+        Args:
+            X: A "batch_shape x q x dim" representing the points to be evaluated.
+        Returns:
+            A tensor of size "batch_shape" representing the acqfn for each q-batch.
+        """
+        return super().__call__(X=X).squeeze(dim=-1).min(dim=-1).values
+
+
 class PenalizedAcquisitionFunction(AcquisitionFunction):
     r"""Single-outcome acquisition function regularized by the given penalty.
 
     The usage is similar to:
         raw_acqf = NoisyExpectedImprovement(...)
         penalty = GroupLassoPenalty(...)
         acqf = PenalizedAcquisitionFunction(raw_acqf, penalty)
@@ -256,30 +316,34 @@
     """
 
     def __init__(
         self,
         objective: Callable[[Tensor, Optional[Tensor]], Tensor],
         penalty_objective: torch.nn.Module,
         regularization_parameter: float,
+        expand_dim: Optional[int] = None,
     ) -> None:
         r"""Penalized MC objective.
 
         Args:
             objective: A callable `f(samples, X)` mapping a
                 `sample_shape x batch-shape x q x m`-dim Tensor `samples` and
                 an optional `batch-shape x q x d`-dim Tensor `X` to a
                 `sample_shape x batch-shape x q`-dim Tensor of objective values.
             penalty_objective: A torch.nn.Module `f(X)` that takes in a
                 `batch-shape x q x d`-dim Tensor `X` and outputs a
                 `1 x batch-shape x q`-dim Tensor of penalty objective values.
             regularization_parameter: weight of the penalty (regularization) term
+            expand_dim: dim to expand penalty_objective to match with objective when
+                fully bayesian model is used. If None, no expansion is performed.
         """
         super().__init__(objective=objective)
         self.penalty_objective = penalty_objective
         self.regularization_parameter = regularization_parameter
+        self.expand_dim = expand_dim
 
     def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
         r"""Evaluate the penalized objective on the samples.
 
         Args:
             samples: A `sample_shape x batch_shape x q x m`-dim Tensors of
                 samples from a model posterior.
@@ -288,8 +352,40 @@
 
         Returns:
             A `sample_shape x batch_shape x q`-dim Tensor of objective values
             with penalty added for each point.
         """
         obj = super().forward(samples=samples, X=X)
         penalty_obj = self.penalty_objective(X)
+        # when fully bayesian model is used, we pass unmarginalize_dim to match the
+        # shape between obj `sample_shape x batch-shape x mcmc_samples x q` and
+        # penalty_obj `1 x batch-shape x q`
+        if self.expand_dim is not None:
+            # reshape penalty_obj to match the dim
+            penalty_obj = penalty_obj.unsqueeze(self.expand_dim)
         return obj - self.regularization_parameter * penalty_obj
+
+
+class L0PenaltyApproxObjective(L0Approximation):
+    r"""Differentiable relaxation of the L0 norm penalty objective class.
+    An instance of this class can be added to any arbitrary objective to
+    construct a PenalizedMCObjective.
+    """
+
+    def __init__(self, target_point: Tensor, a: float = 1.0, **tkwargs: Any) -> None:
+        r"""Initializing L0 penalty with differentiable relaxation.
+
+        Args:
+            target_point: A tensor corresponding to the target point.
+            a: A hyperparameter that controls the differentiable relaxation.
+        """
+        super().__init__(target_point=target_point, a=a, **tkwargs)
+
+    def __call__(self, X: Tensor) -> Tensor:
+        r"""
+        Args:
+            X: A "batch_shape x q x dim" representing the points to be evaluated.
+        Returns:
+            A "1 x batch_shape x q" tensor representing the penalty for each point.
+            The first dimension corresponds to the dimension of MC samples.
+        """
+        return super().__call__(X=X).squeeze(dim=-1).unsqueeze(dim=0)
```

### Comparing `botorch-0.8.5/botorch/acquisition/predictive_entropy_search.py` & `botorch-0.9.1/botorch/acquisition/predictive_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/acquisition/proximal.py` & `botorch-0.9.1/botorch/acquisition/proximal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/acquisition/risk_measures.py` & `botorch-0.9.1/botorch/acquisition/risk_measures.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/acquisition/utils.py` & `botorch-0.9.1/botorch/acquisition/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from botorch.sampling.base import MCSampler
 from botorch.sampling.get_sampler import get_sampler
 from botorch.sampling.pathwise import draw_matheron_paths
 from botorch.utils.multi_objective.box_decompositions.non_dominated import (
     FastNondominatedPartitioning,
     NondominatedPartitioning,
 )
+from botorch.utils.objective import compute_feasibility_indicator
 from botorch.utils.sampling import optimize_posterior_samples
 from botorch.utils.transforms import is_fully_bayesian
 from torch import Tensor
 
 
 def get_acquisition_function(
     acquisition_function_name: str,
@@ -95,49 +96,96 @@
         "qNEHVI",
     ]:
         raise NotImplementedError(
             "PosteriorTransforms are not yet implemented for multi-objective "
             "acquisition functions."
         )
     # instantiate and return the requested acquisition function
-    if acquisition_function_name in ("qEI", "qPI"):
-        obj = objective(
-            model.posterior(X_observed, posterior_transform=posterior_transform).mean
+    if acquisition_function_name in ("qEI", "qLogEI", "qPI"):
+        # Since these are the non-noisy variants, use the posterior mean at the observed
+        # inputs directly to compute the best feasible value without sampling.
+        Y = model.posterior(X_observed, posterior_transform=posterior_transform).mean
+        obj = objective(samples=Y, X=X_observed)
+        best_f = compute_best_feasible_objective(
+            samples=Y,
+            obj=obj,
+            constraints=constraints,
+            model=model,
+            objective=objective,
+            posterior_transform=posterior_transform,
+            X_baseline=X_observed,
         )
-        best_f = obj.max(dim=-1).values
     if acquisition_function_name == "qEI":
         return monte_carlo.qExpectedImprovement(
             model=model,
             best_f=best_f,
             sampler=sampler,
             objective=objective,
             posterior_transform=posterior_transform,
             X_pending=X_pending,
+            constraints=constraints,
+            eta=eta,
+        )
+    if acquisition_function_name == "qLogEI":
+        # putting the import here to avoid circular imports
+        # ideally, the entire function should be moved out of this file,
+        # but since it is used for legacy code to be deprecated, we keep it here.
+        from botorch.acquisition.logei import qLogExpectedImprovement
+
+        return qLogExpectedImprovement(
+            model=model,
+            best_f=best_f,
+            sampler=sampler,
+            objective=objective,
+            posterior_transform=posterior_transform,
+            X_pending=X_pending,
+            constraints=constraints,
+            eta=eta,
         )
     elif acquisition_function_name == "qPI":
         return monte_carlo.qProbabilityOfImprovement(
             model=model,
             best_f=best_f,
             sampler=sampler,
             objective=objective,
             posterior_transform=posterior_transform,
             X_pending=X_pending,
             tau=kwargs.get("tau", 1e-3),
+            constraints=constraints,
+            eta=eta,
         )
     elif acquisition_function_name == "qNEI":
         return monte_carlo.qNoisyExpectedImprovement(
             model=model,
             X_baseline=X_observed,
             sampler=sampler,
             objective=objective,
             posterior_transform=posterior_transform,
             X_pending=X_pending,
             prune_baseline=kwargs.get("prune_baseline", True),
             marginalize_dim=kwargs.get("marginalize_dim"),
             cache_root=kwargs.get("cache_root", True),
+            constraints=constraints,
+            eta=eta,
+        )
+    elif acquisition_function_name == "qLogNEI":
+        from botorch.acquisition.logei import qLogNoisyExpectedImprovement
+
+        return qLogNoisyExpectedImprovement(
+            model=model,
+            X_baseline=X_observed,
+            sampler=sampler,
+            objective=objective,
+            posterior_transform=posterior_transform,
+            X_pending=X_pending,
+            prune_baseline=kwargs.get("prune_baseline", True),
+            marginalize_dim=kwargs.get("marginalize_dim"),
+            cache_root=kwargs.get("cache_root", True),
+            constraints=constraints,
+            eta=eta,
         )
     elif acquisition_function_name == "qSR":
         return monte_carlo.qSimpleRegret(
             model=model,
             sampler=sampler,
             objective=objective,
             posterior_transform=posterior_transform,
@@ -209,14 +257,121 @@
             cache_root=kwargs.get("cache_root", True),
         )
     raise NotImplementedError(
         f"Unknown acquisition function {acquisition_function_name}"
     )
 
 
+def compute_best_feasible_objective(
+    samples: Tensor,
+    obj: Tensor,
+    constraints: Optional[List[Callable[[Tensor], Tensor]]],
+    model: Optional[Model] = None,
+    objective: Optional[MCAcquisitionObjective] = None,
+    posterior_transform: Optional[PosteriorTransform] = None,
+    X_baseline: Optional[Tensor] = None,
+    infeasible_obj: Optional[Tensor] = None,
+) -> Tensor:
+    """Computes the largest `obj` value that is feasible under the `constraints`. If
+    `constraints` is None, returns the best unconstrained objective value.
+
+    When no feasible observations exist and `infeasible_obj` is not `None`, returns
+    `infeasible_obj` (potentially reshaped). When no feasible observations exist and
+    `infeasible_obj` is `None`, uses `model`, `objective`, `posterior_transform`, and
+    `X_baseline` to infer and return an `infeasible_obj` `M` s.t. `M < min_x f(x)`.
+
+    Args:
+        samples: `(sample_shape) x batch_shape x q x m`-dim posterior samples.
+        obj: A `(sample_shape) x batch_shape x q`-dim Tensor of MC objective values.
+        constraints: A list of constraint callables which map posterior samples to
+            a scalar. The associated constraint is considered satisfied if this
+            scalar is less than zero.
+        model: A Model, only required when there are no feasible observations.
+        objective: An MCAcquisitionObjective, only optionally used when there are no
+            feasible observations.
+        posterior_transform: A PosteriorTransform, only optionally used when there are
+            no feasible observations.
+        X_baseline: A `batch_shape x d`-dim Tensor of baseline points, only required
+            when there are no feasible observations.
+        infeasible_obj: A Tensor to be returned when no feasible points exist.
+
+    Returns:
+        A `(sample_shape) x batch_shape x 1`-dim Tensor of best feasible objectives.
+    """
+    if constraints is None:  # unconstrained case
+        # we don't need to differentiate through X_baseline for now, so taking
+        # the regular max over the n points to get best_f is fine
+        with torch.no_grad():
+            return obj.amax(dim=-1, keepdim=True)
+
+    is_feasible = compute_feasibility_indicator(
+        constraints=constraints, samples=samples
+    )  # sample_shape x batch_shape x q
+    if is_feasible.any():
+        obj = torch.where(is_feasible, obj, -torch.inf)
+        with torch.no_grad():
+            return obj.amax(dim=-1, keepdim=True)
+
+    elif infeasible_obj is not None:
+        return infeasible_obj.expand(*obj.shape[:-1], 1)
+
+    else:
+        if model is None:
+            raise ValueError(
+                "Must specify `model` when no feasible observation exists."
+            )
+        if X_baseline is None:
+            raise ValueError(
+                "Must specify `X_baseline` when no feasible observation exists."
+            )
+        return _estimate_objective_lower_bound(
+            model=model,
+            objective=objective,
+            posterior_transform=posterior_transform,
+            X=X_baseline,
+        ).expand(*obj.shape[:-1], 1)
+
+
+def _estimate_objective_lower_bound(
+    model: Model,
+    objective: Optional[MCAcquisitionObjective],
+    posterior_transform: Optional[PosteriorTransform],
+    X: Tensor,
+) -> Tensor:
+    """Estimates a lower bound on the objective values by evaluating the model at convex
+    combinations of `X`, returning the 6-sigma lower bound of the computed statistics.
+
+    Args:
+        model: A fitted model.
+        objective: An MCAcquisitionObjective with `m` outputs.
+        posterior_transform: A PosteriorTransform.
+        X: A `n x d`-dim Tensor of design points from which to draw convex combinations.
+
+    Returns:
+        A `m`-dimensional Tensor of lower bounds of the objectives.
+    """
+    convex_weights = torch.rand(
+        32,
+        X.shape[-2],
+        dtype=X.dtype,
+        device=X.device,
+    )
+    weights_sum = convex_weights.sum(dim=0, keepdim=True)
+    convex_weights = convex_weights / weights_sum
+    # infeasible cost M is such that -M < min_x f(x), thus
+    # 0 < min_x f(x) - (-M), so we should take -M as a lower
+    # bound on the best feasible objective
+    return -get_infeasible_cost(
+        X=convex_weights @ X,
+        model=model,
+        objective=objective,
+        posterior_transform=posterior_transform,
+    )
+
+
 def get_infeasible_cost(
     X: Tensor,
     model: Model,
     objective: Optional[Callable[[Tensor, Optional[Tensor]], Tensor]] = None,
     posterior_transform: Optional[PosteriorTransform] = None,
 ) -> Tensor:
     r"""Get infeasible cost for a model and objective.
```

### Comparing `botorch-0.8.5/botorch/cross_validation.py` & `botorch-0.9.1/botorch/cross_validation.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/exceptions/__init__.py` & `botorch-0.9.1/botorch/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/exceptions/errors.py` & `botorch-0.9.1/botorch/exceptions/errors.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/exceptions/warnings.py` & `botorch-0.9.1/botorch/exceptions/warnings.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/fit.py` & `botorch-0.9.1/botorch/fit.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/generation/__init__.py` & `botorch-0.9.1/botorch/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/generation/gen.py` & `botorch-0.9.1/botorch/generation/gen.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     _arrayify,
     make_scipy_bounds,
     make_scipy_linear_constraints,
     make_scipy_nonlinear_inequality_constraints,
     NLC_TOL,
 )
 from botorch.optim.stopping import ExpMAStoppingCriterion
-from botorch.optim.utils import _filter_kwargs, columnwise_clamp, fix_features
+from botorch.optim.utils import columnwise_clamp, fix_features
 from botorch.optim.utils.timeout import minimize_with_timeout
 from scipy.optimize import OptimizeResult
 from torch import Tensor
 from torch.optim import Optimizer
 
 logger = _get_logger()
 
@@ -110,46 +110,45 @@
     """
     options = options or {}
     options = {**options, "maxiter": options.get("maxiter", 2000)}
 
     # if there are fixed features we may optimize over a domain of lower dimension
     reduced_domain = False
     if fixed_features:
-        # TODO: We can support fixed features, see Max's comment on D33551393. We can
-        # consider adding this at a later point.
-        if nonlinear_inequality_constraints:
-            raise NotImplementedError(
-                "Fixed features are not supported when non-linear inequality "
-                "constraints are given."
-            )
-        # if there are no constraints things are straightforward
-        if not (inequality_constraints or equality_constraints):
+        # if there are no constraints, things are straightforward
+        if not (
+            inequality_constraints
+            or equality_constraints
+            or nonlinear_inequality_constraints
+        ):
             reduced_domain = True
         # if there are we need to make sure features are fixed to specific values
         else:
             reduced_domain = None not in fixed_features.values()
 
     if reduced_domain:
         _no_fixed_features = _remove_fixed_features_from_optimization(
             fixed_features=fixed_features,
             acquisition_function=acquisition_function,
             initial_conditions=initial_conditions,
             lower_bounds=lower_bounds,
             upper_bounds=upper_bounds,
             inequality_constraints=inequality_constraints,
             equality_constraints=equality_constraints,
+            nonlinear_inequality_constraints=nonlinear_inequality_constraints,
         )
         # call the routine with no fixed_features
         clamped_candidates, batch_acquisition = gen_candidates_scipy(
             initial_conditions=_no_fixed_features.initial_conditions,
             acquisition_function=_no_fixed_features.acquisition_function,
             lower_bounds=_no_fixed_features.lower_bounds,
             upper_bounds=_no_fixed_features.upper_bounds,
             inequality_constraints=_no_fixed_features.inequality_constraints,
             equality_constraints=_no_fixed_features.equality_constraints,
+            nonlinear_inequality_constraints=_no_fixed_features.nonlinear_inequality_constraints,  # noqa: E501
             options=options,
             fixed_features=None,
             timeout_sec=timeout_sec,
         )
         clamped_candidates = _no_fixed_features.acquisition_function._construct_X_full(
             clamped_candidates
         )
@@ -338,14 +337,15 @@
             fixed_features=fixed_features,
             acquisition_function=acquisition_function,
             initial_conditions=initial_conditions,
             lower_bounds=lower_bounds,
             upper_bounds=upper_bounds,
             inequality_constraints=None,
             equality_constraints=None,
+            nonlinear_inequality_constraints=None,
         )
 
         # call the routine with no fixed_features
         elapsed = time.monotonic() - start_time
         clamped_candidates, batch_acquisition = gen_candidates_torch(
             initial_conditions=subproblem.initial_conditions,
             acquisition_function=subproblem.acquisition_function,
@@ -363,17 +363,15 @@
         return clamped_candidates, batch_acquisition
     _clamp = partial(columnwise_clamp, lower=lower_bounds, upper=upper_bounds)
     clamped_candidates = _clamp(initial_conditions).requires_grad_(True)
     _optimizer = optimizer(params=[clamped_candidates], lr=options.get("lr", 0.025))
 
     i = 0
     stop = False
-    stopping_criterion = ExpMAStoppingCriterion(
-        **_filter_kwargs(ExpMAStoppingCriterion, **options)
-    )
+    stopping_criterion = ExpMAStoppingCriterion(**options)
     while not stop:
         i += 1
         with torch.no_grad():
             X = _clamp(clamped_candidates).requires_grad_(True)
 
         loss = -acquisition_function(X).sum()
         grad = torch.autograd.grad(loss, X)[0]
```

### Comparing `botorch-0.8.5/botorch/generation/sampling.py` & `botorch-0.9.1/botorch/generation/sampling.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 import torch
 from botorch.acquisition.acquisition import AcquisitionFunction
 from botorch.acquisition.objective import (
     IdentityMCObjective,
     MCAcquisitionObjective,
     PosteriorTransform,
-    ScalarizedPosteriorTransform,
 )
 from botorch.generation.utils import _flip_sub_unique
 from botorch.models.model import Model
 
 from botorch.models.model_list_gp_regression import ModelListGP
 from botorch.models.multitask import MultiTaskGP
 from botorch.utils.sampling import batched_multinomial
@@ -86,30 +85,15 @@
             objective: The MCAcquisitionObjective under which the samples are
                 evaluated. Defaults to `IdentityMCObjective()`.
             posterior_transform: An optional PosteriorTransform.
             replacement: If True, sample with replacement.
         """
         super().__init__()
         self.model = model
-        if objective is None:
-            objective = IdentityMCObjective()
-        elif not isinstance(objective, MCAcquisitionObjective):
-            # TODO: Clean up once ScalarizedObjective is removed.
-            if posterior_transform is not None:
-                raise RuntimeError(
-                    "A ScalarizedObjective (DEPRECATED) and a posterior transform "
-                    "are not supported at the same time. Use only a posterior "
-                    "transform instead."
-                )
-            else:
-                posterior_transform = ScalarizedPosteriorTransform(
-                    weights=objective.weights, offset=objective.offset
-                )
-                objective = IdentityMCObjective()
-        self.objective = objective
+        self.objective = IdentityMCObjective() if objective is None else objective
         self.posterior_transform = posterior_transform
         self.replacement = replacement
 
     def forward(
         self, X: Tensor, num_samples: int = 1, observation_noise: bool = False
     ) -> Tensor:
         r"""Sample from the model posterior.
```

### Comparing `botorch-0.8.5/botorch/generation/utils.py` & `botorch-0.9.1/botorch/generation/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import torch
 from botorch.acquisition import AcquisitionFunction, FixedFeatureAcquisitionFunction
-from botorch.optim.parameter_constraints import _generate_unfixed_lin_constraints
+from botorch.optim.parameter_constraints import (
+    _generate_unfixed_lin_constraints,
+    _generate_unfixed_nonlin_constraints,
+)
 from torch import Tensor
 
 
 def _flip_sub_unique(x: Tensor, k: int) -> Tensor:
     """Get the first k unique elements of a single-dimensional tensor, traversing the
     tensor from the back.
 
@@ -59,24 +62,26 @@
 
     acquisition_function: FixedFeatureAcquisitionFunction
     initial_conditions: Tensor
     lower_bounds: Optional[Union[float, Tensor]]
     upper_bounds: Optional[Union[float, Tensor]]
     inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]]
     equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]]
+    nonlinear_inequality_constraints: Optional[List[Callable[[Tensor], Tensor]]]
 
 
 def _remove_fixed_features_from_optimization(
     fixed_features: Dict[int, Optional[float]],
     acquisition_function: AcquisitionFunction,
     initial_conditions: Tensor,
     lower_bounds: Optional[Union[float, Tensor]],
     upper_bounds: Optional[Union[float, Tensor]],
     inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]],
     equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]],
+    nonlinear_inequality_constraints: Optional[List[Callable[[Tensor], Tensor]]],
 ) -> _NoFixedFeatures:
     """
     Given a set of non-empty fixed features, this function effectively reduces the
     dimensionality of the domain that the acquisition function is being optimized
     over by removing the set of fixed features. Consequently, this function returns a
     new `FixedFeatureAcquisitionFunction`, new constraints, and bounds defined over
     unfixed features.
@@ -94,14 +99,19 @@
         upper_bounds: Minimum values for each column of initial_conditions.
         inequality constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `sum_i (X[indices[i]] * coefficients[i]) >= rhs`.
         equality constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `sum_i (X[indices[i]] * coefficients[i]) = rhs`.
+        nonlinear_inequality_constraints: A list of callables with that represent
+            non-linear inequality constraints of the form `callable(x) >= 0`. Each
+            callable is expected to take a `(num_restarts) x q x d`-dim tensor as
+            an input and return a `(num_restarts) x q`-dim tensor with the
+            constraint values.
 
     Returns:
         _NoFixedFeatures dataclass object.
     """
     # sort the keys for consistency
     sorted_keys = sorted(fixed_features)
     sorted_values = []
@@ -136,15 +146,21 @@
     )
     equality_constraints = _generate_unfixed_lin_constraints(
         constraints=equality_constraints,
         fixed_features=fixed_features,
         dimension=d,
         eq=True,
     )
+    nonlinear_inequality_constraints = _generate_unfixed_nonlin_constraints(
+        constraints=nonlinear_inequality_constraints,
+        fixed_features=fixed_features,
+        dimension=d,
+    )
     return _NoFixedFeatures(
         acquisition_function=acquisition_function,
         initial_conditions=initial_conditions,
         lower_bounds=lower_bounds,
         upper_bounds=upper_bounds,
         inequality_constraints=inequality_constraints,
         equality_constraints=equality_constraints,
+        nonlinear_inequality_constraints=nonlinear_inequality_constraints,
     )
```

### Comparing `botorch-0.8.5/botorch/models/__init__.py` & `botorch-0.9.1/botorch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/approximate_gp.py` & `botorch-0.9.1/botorch/models/approximate_gp.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,49 +28,52 @@
 """
 
 from __future__ import annotations
 
 import copy
 import warnings
 
-from typing import Optional, Type, Union
+from typing import Optional, Type, TypeVar, Union
 
 import torch
 from botorch.models.gpytorch import GPyTorchModel
 from botorch.models.transforms.input import InputTransform
 from botorch.models.transforms.outcome import OutcomeTransform
 from botorch.models.utils import validate_input_scaling
+from botorch.models.utils.gpytorch_modules import (
+    get_gaussian_likelihood_with_gamma_prior,
+    get_matern_kernel_with_gamma_prior,
+)
 from botorch.models.utils.inducing_point_allocators import (
     GreedyVarianceReduction,
     InducingPointAllocator,
 )
 from botorch.posteriors.gpytorch import GPyTorchPosterior
-from gpytorch.constraints import GreaterThan
 from gpytorch.distributions import MultivariateNormal
-from gpytorch.kernels import Kernel, MaternKernel, ScaleKernel
+from gpytorch.kernels import Kernel
 from gpytorch.likelihoods import (
     GaussianLikelihood,
     Likelihood,
     MultitaskGaussianLikelihood,
 )
 from gpytorch.means import ConstantMean, Mean
 from gpytorch.models import ApproximateGP
-from gpytorch.priors import GammaPrior
 from gpytorch.utils.memoize import clear_cache_hook
 from gpytorch.variational import (
     _VariationalDistribution,
     _VariationalStrategy,
     CholeskyVariationalDistribution,
     IndependentMultitaskVariationalStrategy,
     VariationalStrategy,
 )
 from torch import Tensor
+from torch.nn import Module
 
 
-MIN_INFERRED_NOISE_LEVEL = 1e-4
+TApproxModel = TypeVar("TApproxModel", bound="ApproximateGPyTorchModel")
 
 
 class ApproximateGPyTorchModel(GPyTorchModel):
     r"""
     Botorch wrapper class for various (variational) approximate GP models in
     GPyTorch.
 
@@ -116,14 +119,27 @@
             self.likelihood = likelihood
         self._desired_num_outputs = num_outputs
 
     @property
     def num_outputs(self):
         return self._desired_num_outputs
 
+    def eval(self: TApproxModel) -> TApproxModel:
+        r"""Puts the model in `eval` mode."""
+        return Module.eval(self)
+
+    def train(self: TApproxModel, mode: bool = True) -> TApproxModel:
+        r"""Put the model in `train` mode.
+
+        Args:
+            mode: A boolean denoting whether to put in `train` or `eval` mode.
+                If `False`, model is put in `eval` mode.
+        """
+        return Module.train(self, mode=mode)
+
     def posterior(
         self, X, output_indices=None, observation_noise=False, *args, **kwargs
     ) -> GPyTorchPosterior:
         self.eval()  # make sure model is in eval mode
 
         # input transforms are applied at `posterior` in `eval` mode, and at
         # `model.forward()` at the training time
@@ -171,15 +187,15 @@
         inducing_points: Optional[Union[Tensor, int]] = None,
         inducing_point_allocator: Optional[InducingPointAllocator] = None,
     ) -> None:
         r"""
         Args:
             train_X: Training inputs (due to the ability of the SVGP to sub-sample
                 this does not have to be all of the training inputs).
-            train_Y: Training targets (optional).
+            train_Y: Not used.
             num_outputs: Number of output responses per input.
             covar_module: Kernel function. If omitted, uses a `MaternKernel`.
             mean_module: Mean of GP model. If omitted, uses a `ConstantMean`.
             variational_distribution: Type of variational distribution to use
                 (default: CholeskyVariationalDistribution), the properties of the
                 variational distribution will encourage scalability or ease of
                 optimization.
@@ -197,23 +213,17 @@
         input_batch_shape = train_X.shape[:-2]
         aug_batch_shape = copy.deepcopy(input_batch_shape)
         if num_outputs > 1:
             aug_batch_shape += torch.Size((num_outputs,))
         self._aug_batch_shape = aug_batch_shape
 
         if covar_module is None:
-            covar_module = ScaleKernel(
-                base_kernel=MaternKernel(
-                    nu=2.5,
-                    ard_num_dims=train_X.shape[-1],
-                    batch_shape=self._aug_batch_shape,
-                    lengthscale_prior=GammaPrior(3.0, 6.0),
-                ),
+            covar_module = get_matern_kernel_with_gamma_prior(
+                ard_num_dims=train_X.shape[-1],
                 batch_shape=self._aug_batch_shape,
-                outputscale_prior=GammaPrior(2.0, 0.15),
             ).to(train_X)
             self._subset_batch_dict = {
                 "mean_module.constant": -2,
                 "covar_module.raw_outputscale": -1,
                 "covar_module.base_kernel.raw_lengthscale": -3,
             }
 
@@ -364,24 +374,16 @@
         aug_batch_shape = copy.deepcopy(self._input_batch_shape)
         if num_outputs > 1:
             aug_batch_shape += torch.Size([num_outputs])
         self._aug_batch_shape = aug_batch_shape
 
         if likelihood is None:
             if num_outputs == 1:
-                noise_prior = GammaPrior(1.1, 0.05)
-                noise_prior_mode = (noise_prior.concentration - 1) / noise_prior.rate
-                likelihood = GaussianLikelihood(
-                    noise_prior=noise_prior,
-                    batch_shape=self._aug_batch_shape,
-                    noise_constraint=GreaterThan(
-                        MIN_INFERRED_NOISE_LEVEL,
-                        transform=None,
-                        initial_value=noise_prior_mode,
-                    ),
+                likelihood = get_gaussian_likelihood_with_gamma_prior(
+                    batch_shape=self._aug_batch_shape
                 )
             else:
                 likelihood = MultitaskGaussianLikelihood(num_tasks=num_outputs)
         else:
             self._is_custom_likelihood = True
 
         if learn_inducing_points and (inducing_point_allocator is not None):
@@ -396,15 +398,14 @@
         if inducing_point_allocator is None:
             self._inducing_point_allocator = GreedyVarianceReduction()
         else:
             self._inducing_point_allocator = inducing_point_allocator
 
         model = _SingleTaskVariationalGP(
             train_X=transformed_X,
-            train_Y=train_Y,
             num_outputs=num_outputs,
             learn_inducing_points=learn_inducing_points,
             covar_module=covar_module,
             mean_module=mean_module,
             variational_distribution=variational_distribution,
             variational_strategy=variational_strategy,
             inducing_points=inducing_points,
```

### Comparing `botorch-0.8.5/botorch/models/contextual.py` & `botorch-0.9.1/botorch/models/contextual.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,15 @@
     ) -> None:
         r"""
         Args:
             train_X: (n x d) X training data.
             train_Y: (n x 1) Y training data.
             train_Yvar: (n x 1) Noise variance of Y.
             decomposition: Keys are context names. Values are the indexes of
-                parameters belong to the context. The parameter indexes are in the
-                same order across contexts.
+                parameters belong to the context.
             cat_feature_dict: Keys are context names and values are list of categorical
                 features i.e. {"context_name" : [cat_0, ..., cat_k]}, where k is the
                 number of categorical variables. If None, we use context names in the
                 decomposition as the only categorical feature, i.e., k = 1.
             embs_feature_dict: Pre-trained continuous embedding features of each
                 context.
             embs_dim_list: Embedding dimension for each categorical variable. The length
```

### Comparing `botorch-0.8.5/botorch/models/contextual_multioutput.py` & `botorch-0.9.1/botorch/models/contextual_multioutput.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/converter.py` & `botorch-0.9.1/botorch/models/converter.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/cost.py` & `botorch-0.9.1/botorch/models/cost.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/deterministic.py` & `botorch-0.9.1/botorch/models/deterministic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/ensemble.py` & `botorch-0.9.1/botorch/models/ensemble.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/fully_bayesian.py` & `botorch-0.9.1/botorch/models/fully_bayesian.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 import math
 from abc import abstractmethod
 from typing import Any, Dict, List, Mapping, Optional, Tuple
 
 import pyro
 import torch
 from botorch.acquisition.objective import PosteriorTransform
-from botorch.models.gp_regression import MIN_INFERRED_NOISE_LEVEL
 from botorch.models.gpytorch import BatchedMultiOutputGPyTorchModel
 from botorch.models.transforms.input import InputTransform
 from botorch.models.transforms.outcome import OutcomeTransform
 from botorch.models.utils import validate_input_scaling
+from botorch.models.utils.gpytorch_modules import MIN_INFERRED_NOISE_LEVEL
 from botorch.posteriors.fully_bayesian import FullyBayesianPosterior, MCMC_DIM
 from gpytorch.constraints import GreaterThan
 from gpytorch.distributions.multivariate_normal import MultivariateNormal
 from gpytorch.kernels import MaternKernel, ScaleKernel
 from gpytorch.kernels.kernel import dist, Kernel
 from gpytorch.likelihoods.gaussian_likelihood import (
     FixedNoiseGaussianLikelihood,
@@ -60,19 +60,19 @@
 from torch import Tensor
 
 
 _sqrt5 = math.sqrt(5)
 
 
 def _handle_torch_linalg(exception: Exception) -> bool:
-    return type(exception) == torch.linalg.LinAlgError
+    return type(exception) is torch.linalg.LinAlgError
 
 
 def _handle_valerr_in_dist_init(exception: Exception) -> bool:
-    if not type(exception) == ValueError:
+    if type(exception) is not ValueError:
         return False
     return "satisfy the constraint PositiveDefinite()" in str(exception)
 
 
 register_exception_handler("torch_linalg", _handle_torch_linalg)
 register_exception_handler("valerr_in_dist_init", _handle_valerr_in_dist_init)
```

### Comparing `botorch-0.8.5/botorch/models/fully_bayesian_multitask.py` & `botorch-0.9.1/botorch/models/fully_bayesian_multitask.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 # LICENSE file in the root directory of this source tree.
 
 
 r"""Multi-task Gaussian Process Regression models with fully Bayesian inference.
 """
 
 
-from typing import Any, Dict, List, NoReturn, Optional, Tuple
+from typing import Any, Dict, List, Mapping, NoReturn, Optional, Tuple
 
 import pyro
 import torch
 from botorch.acquisition.objective import PosteriorTransform
 from botorch.models.fully_bayesian import (
     matern52_kernel,
     MIN_INFERRED_NOISE_LEVEL,
     PyroModel,
     reshape_and_detach,
     SaasPyroModel,
 )
-from botorch.models.multitask import FixedNoiseMultiTaskGP
+from botorch.models.multitask import MultiTaskGP
 from botorch.models.transforms.input import InputTransform
 from botorch.models.transforms.outcome import OutcomeTransform
 from botorch.posteriors.fully_bayesian import FullyBayesianPosterior, MCMC_DIM
 from botorch.utils.datasets import SupervisedDataset
 from gpytorch.distributions.multivariate_normal import MultivariateNormal
 from gpytorch.kernels import MaternKernel
 from gpytorch.kernels.kernel import Kernel
@@ -159,15 +159,15 @@
         latent_features = reshape_and_detach(
             target=latent_features,
             new_value=mcmc_samples["latent_features"],
         )
         return mean_module, covar_module, likelihood, task_covar_module, latent_features
 
 
-class SaasFullyBayesianMultiTaskGP(FixedNoiseMultiTaskGP):
+class SaasFullyBayesianMultiTaskGP(MultiTaskGP):
     r"""A fully Bayesian multi-task GP model with the SAAS prior.
 
     This model assumes that the inputs have been normalized to [0, 1]^d and that the
     output has been stratified standardized to have zero mean and unit variance for
     each task.The SAAS model [Eriksson2021saasbo]_ with a Matern-5/2 is used as data
     kernel by default.
 
@@ -205,16 +205,25 @@
 
         Args:
             train_X: Training inputs (n x (d + 1))
             train_Y: Training targets (n x 1)
             train_Yvar: Observed noise variance (n x 1). If None, we infer the noise.
                 Note that the inferred noise is common across all tasks.
             task_feature: The index of the task feature (`-d <= task_feature <= d`).
+            output_tasks: A list of task indices for which to compute model
+                outputs for. If omitted, return outputs for all task indices.
             rank: The num of learned task embeddings to be used in the task kernel.
                 If omitted, set it to be 1.
+            outcome_transform: An outcome transform that is applied to the
+                training data during instantiation and to the posterior during
+                inference (that is, the `Posterior` obtained by calling
+                `.posterior` on the model will be on the original scale).
+            input_transform: An input transform that is applied to the inputs `X`
+                in the model's forward pass.
+            pyro_model: Optional `PyroModel`, defaults to `MultitaskSaasPyroModel`.
         """
         if not (
             train_X.ndim == train_Y.ndim == 2
             and len(train_X) == len(train_Y)
             and train_Y.shape[-1] == 1
         ):
             raise ValueError(
@@ -232,25 +241,25 @@
             train_Y, train_Yvar = outcome_transform(train_Y, train_Yvar)
         if train_Yvar is not None:  # Clamp after transforming
             train_Yvar = train_Yvar.clamp(MIN_INFERRED_NOISE_LEVEL)
 
         super().__init__(
             train_X=train_X,
             train_Y=train_Y,
-            # Using train_Y as a dummy input here when train_Yvar is None.
-            train_Yvar=train_Yvar if train_Yvar is not None else train_Y,
+            train_Yvar=train_Yvar,
             task_feature=task_feature,
             output_tasks=output_tasks,
         )
         self.to(train_X)
 
         self.mean_module = None
         self.covar_module = None
         self.likelihood = None
         self.task_covar_module = None
+        self.register_buffer("latent_features", None)
         if pyro_model is None:
             pyro_model = MultitaskSaasPyroModel()
         pyro_model.set_inputs(
             train_X=transformed_X,
             train_Y=train_Y,
             train_Yvar=train_Yvar,
             task_feature=task_feature,
@@ -388,7 +397,53 @@
         inputs = super().construct_inputs(
             training_data=training_data, task_feature=task_feature, rank=rank, **kwargs
         )
         inputs.pop("task_covar_prior")
         if "train_Yvar" not in inputs:
             inputs["train_Yvar"] = None
         return inputs
+
+    def load_state_dict(self, state_dict: Mapping[str, Any], strict: bool = True):
+        r"""Custom logic for loading the state dict.
+
+        The standard approach of calling `load_state_dict` currently doesn't play well
+        with the `SaasFullyBayesianMultiTaskGP` since the `mean_module`, `covar_module`
+        and `likelihood` aren't initialized until the model has been fitted. The reason
+        for this is that we don't know the number of MCMC samples until NUTS is called.
+        Given the state dict, we can initialize a new model with some dummy samples and
+        then load the state dict into this model. This currently only works for a
+        `MultitaskSaasPyroModel` and supporting more Pyro models likely requires moving
+        the model construction logic into the Pyro model itself.
+
+        TODO: If this were to inherif from `SaasFullyBayesianSingleTaskGP`, we could
+        simplify this method and eliminate some others.
+        """
+        if not isinstance(self.pyro_model, MultitaskSaasPyroModel):
+            raise NotImplementedError(  # pragma: no cover
+                "load_state_dict only works for MultitaskSaasPyroModel"
+            )
+        raw_mean = state_dict["mean_module.raw_constant"]
+        num_mcmc_samples = len(raw_mean)
+        dim = self.pyro_model.train_X.shape[-1] - 1  # Removing 1 for the task feature.
+        task_rank = self.pyro_model.task_rank
+        tkwargs = {"device": raw_mean.device, "dtype": raw_mean.dtype}
+        # Load some dummy samples
+        mcmc_samples = {
+            "mean": torch.ones(num_mcmc_samples, **tkwargs),
+            "lengthscale": torch.ones(num_mcmc_samples, dim, **tkwargs),
+            "outputscale": torch.ones(num_mcmc_samples, **tkwargs),
+            "task_lengthscale": torch.ones(num_mcmc_samples, task_rank, **tkwargs),
+            "latent_features": torch.ones(
+                num_mcmc_samples, self._rank, task_rank, **tkwargs
+            ),
+        }
+        if self.pyro_model.train_Yvar is None:
+            mcmc_samples["noise"] = torch.ones(num_mcmc_samples, **tkwargs)
+        (
+            self.mean_module,
+            self.covar_module,
+            self.likelihood,
+            self.task_covar_module,
+            self.latent_features,
+        ) = self.pyro_model.load_mcmc_samples(mcmc_samples=mcmc_samples)
+        # Load the actual samples from the state dict
+        super().load_state_dict(state_dict=state_dict, strict=strict)
```

### Comparing `botorch-0.8.5/botorch/models/gp_regression.py` & `botorch-0.9.1/botorch/models/gp_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,39 +35,38 @@
 import torch
 from botorch import settings
 from botorch.models.gpytorch import BatchedMultiOutputGPyTorchModel
 from botorch.models.model import FantasizeMixin
 from botorch.models.transforms.input import InputTransform
 from botorch.models.transforms.outcome import Log, OutcomeTransform
 from botorch.models.utils import fantasize as fantasize_flag, validate_input_scaling
+from botorch.models.utils.gpytorch_modules import (
+    get_gaussian_likelihood_with_gamma_prior,
+    get_matern_kernel_with_gamma_prior,
+    MIN_INFERRED_NOISE_LEVEL,
+)
 from botorch.sampling.base import MCSampler
 from gpytorch.constraints.constraints import GreaterThan
 from gpytorch.distributions.multivariate_normal import MultivariateNormal
-from gpytorch.kernels.matern_kernel import MaternKernel
-from gpytorch.kernels.scale_kernel import ScaleKernel
 from gpytorch.likelihoods.gaussian_likelihood import (
     _GaussianLikelihoodBase,
     FixedNoiseGaussianLikelihood,
     GaussianLikelihood,
 )
 from gpytorch.likelihoods.likelihood import Likelihood
 from gpytorch.likelihoods.noise_models import HeteroskedasticNoise
 from gpytorch.means.constant_mean import ConstantMean
 from gpytorch.means.mean import Mean
 from gpytorch.mlls.noise_model_added_loss_term import NoiseModelAddedLossTerm
 from gpytorch.models.exact_gp import ExactGP
 from gpytorch.module import Module
 from gpytorch.priors.smoothed_box_prior import SmoothedBoxPrior
-from gpytorch.priors.torch_priors import GammaPrior
 from torch import Tensor
 
 
-MIN_INFERRED_NOISE_LEVEL = 1e-4
-
-
 class SingleTaskGP(BatchedMultiOutputGPyTorchModel, ExactGP, FantasizeMixin):
     r"""A single-task exact GP model.
 
     A single-task exact GP using relatively strong priors on the Kernel
     hyperparameters, which work best when covariates are normalized to the unit
     cube and outcomes are standardized (zero mean, unit variance).
 
@@ -123,43 +122,29 @@
         ignore_X_dims = getattr(self, "_ignore_X_dims_scaling_check", None)
         validate_input_scaling(
             train_X=transformed_X, train_Y=train_Y, ignore_X_dims=ignore_X_dims
         )
         self._set_dimensions(train_X=train_X, train_Y=train_Y)
         train_X, train_Y, _ = self._transform_tensor_args(X=train_X, Y=train_Y)
         if likelihood is None:
-            noise_prior = GammaPrior(1.1, 0.05)
-            noise_prior_mode = (noise_prior.concentration - 1) / noise_prior.rate
-            likelihood = GaussianLikelihood(
-                noise_prior=noise_prior,
-                batch_shape=self._aug_batch_shape,
-                noise_constraint=GreaterThan(
-                    MIN_INFERRED_NOISE_LEVEL,
-                    transform=None,
-                    initial_value=noise_prior_mode,
-                ),
+            likelihood = get_gaussian_likelihood_with_gamma_prior(
+                batch_shape=self._aug_batch_shape
             )
         else:
             self._is_custom_likelihood = True
         ExactGP.__init__(
             self, train_inputs=train_X, train_targets=train_Y, likelihood=likelihood
         )
         if mean_module is None:
             mean_module = ConstantMean(batch_shape=self._aug_batch_shape)
         self.mean_module = mean_module
         if covar_module is None:
-            covar_module = ScaleKernel(
-                MaternKernel(
-                    nu=2.5,
-                    ard_num_dims=transformed_X.shape[-1],
-                    batch_shape=self._aug_batch_shape,
-                    lengthscale_prior=GammaPrior(3.0, 6.0),
-                ),
+            covar_module = get_matern_kernel_with_gamma_prior(
+                ard_num_dims=transformed_X.shape[-1],
                 batch_shape=self._aug_batch_shape,
-                outputscale_prior=GammaPrior(2.0, 0.15),
             )
             self._subset_batch_dict = {
                 "likelihood.noise_covar.raw_noise": -2,
                 "mean_module.raw_constant": -1,
                 "covar_module.raw_outputscale": -1,
                 "covar_module.base_kernel.raw_lengthscale": -3,
             }
@@ -259,23 +244,17 @@
         ExactGP.__init__(
             self, train_inputs=train_X, train_targets=train_Y, likelihood=likelihood
         )
         if mean_module is None:
             mean_module = ConstantMean(batch_shape=self._aug_batch_shape)
         self.mean_module = mean_module
         if covar_module is None:
-            covar_module = ScaleKernel(
-                base_kernel=MaternKernel(
-                    nu=2.5,
-                    ard_num_dims=transformed_X.shape[-1],
-                    batch_shape=self._aug_batch_shape,
-                    lengthscale_prior=GammaPrior(3.0, 6.0),
-                ),
+            covar_module = get_matern_kernel_with_gamma_prior(
+                ard_num_dims=transformed_X.shape[-1],
                 batch_shape=self._aug_batch_shape,
-                outputscale_prior=GammaPrior(2.0, 0.15),
             )
             self._subset_batch_dict = {
                 "mean_module.raw_constant": -1,
                 "covar_module.raw_outputscale": -1,
                 "covar_module.base_kernel.raw_lengthscale": -3,
             }
         self.covar_module = covar_module
```

### Comparing `botorch-0.8.5/botorch/models/gp_regression_fidelity.py` & `botorch-0.9.1/botorch/models/gp_regression_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/gp_regression_mixed.py` & `botorch-0.9.1/botorch/models/gp_regression_mixed.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/gpytorch.py` & `botorch-0.9.1/botorch/models/gpytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from __future__ import annotations
 
 import itertools
 import warnings
 from abc import ABC
 from copy import deepcopy
-from typing import Any, Iterator, List, Optional, Tuple, TYPE_CHECKING, Union
+from typing import Any, List, Optional, Tuple, TYPE_CHECKING, Union
 
 import torch
 from botorch.acquisition.objective import PosteriorTransform
 from botorch.exceptions.errors import BotorchTensorDimensionError, InputDataError
 from botorch.exceptions.warnings import BotorchTensorDimensionWarning
 from botorch.models.model import Model, ModelList
 from botorch.models.utils import (
@@ -377,15 +377,18 @@
                     X=X, original_batch_shape=self._input_batch_shape
                 )
             mvn = self(X)
             if observation_noise is not False:
                 if torch.is_tensor(observation_noise):
                     # TODO: Validate noise shape
                     # make observation_noise `batch_shape x q x n`
-                    obs_noise = observation_noise.transpose(-1, -2)
+                    if self.num_outputs > 1:
+                        obs_noise = observation_noise.transpose(-1, -2)
+                    else:
+                        obs_noise = observation_noise.squeeze(-1)
                     mvn = self.likelihood(mvn, X, noise=obs_noise)
                 elif isinstance(self.likelihood, FixedNoiseGaussianLikelihood):
                     # Use the mean of the previous noise values (TODO: be smarter here).
                     noise = self.likelihood.noise.mean().expand(X.shape[:-1])
                     mvn = self.likelihood(mvn, X, noise=noise)
                 else:
                     mvn = self.likelihood(mvn, X)
@@ -523,15 +526,15 @@
             new_model.outcome_transform = subset_octf
         except AttributeError:
             pass
 
         return new_model
 
 
-class ModelListGPyTorchModel(GPyTorchModel, ModelList, ABC):
+class ModelListGPyTorchModel(ModelList, GPyTorchModel, ABC):
     r"""Abstract base class for models based on multi-output GPyTorch models.
 
     This is meant to be used with a gpytorch ModelList wrapper for independent
     evaluation of submodels.
 
     :meta private:
     """
@@ -606,82 +609,38 @@
 
         # Nonlinear transforms untransform to a `TransformedPosterior`,
         # which can't be made into a `GPyTorchPosterior`
         returns_untransformed = any(
             hasattr(mod, "outcome_transform") and (not mod.outcome_transform._is_linear)
             for mod in self.models
         )
-        if returns_untransformed:
-            return ModelList.posterior(
-                self,
-                X,
-                output_indices,
-                observation_noise,
-                posterior_transform,
-                **kwargs,
-            )
-
-        self.eval()  # make sure model is in eval mode
-        # input transforms are applied at `posterior` in `eval` mode, and at
-        # `model.forward()` at the training time
-        transformed_X = self.transform_inputs(X)
-        mvn_gen: Iterator
-        with gpt_posterior_settings():
-            # only compute what's necessary
-            if output_indices is not None:
-                mvns = [self.models[i](transformed_X[i]) for i in output_indices]
-                if observation_noise is not False:
-                    if isinstance(observation_noise, Tensor):
-                        lh_kwargs = [
-                            {"noise": observation_noise[..., i]}
-                            for i, lh in enumerate(self.likelihood.likelihoods)
-                        ]
-                    else:
-                        lh_kwargs = [
-                            {"noise": lh.noise.mean().expand(t_X.shape[:-1])}
-                            if isinstance(lh, FixedNoiseGaussianLikelihood)
-                            else {}
-                            for t_X, lh in zip(
-                                transformed_X, self.likelihood.likelihoods
-                            )
-                        ]
-                    mvns = [
-                        self.likelihood_i(i, mvn, transformed_X[i], **lkws)
-                        for i, mvn, lkws in zip(output_indices, mvns, lh_kwargs)
-                    ]
-                mvn_gen = zip(output_indices, mvns)
-            else:
-                mvns = self(*transformed_X)
-                if observation_noise is not False:
-                    mvnX = [(mvn, transformed_X[i]) for i, mvn in enumerate(mvns)]
-                    if torch.is_tensor(observation_noise):
-                        mvns = self.likelihood(*mvnX, noise=observation_noise)
-                    else:
-                        mvns = self.likelihood(*mvnX)
-                mvn_gen = enumerate(mvns)
-        # apply output transforms of individual models if present
-        mvns = []
-        for i, mvn in mvn_gen:
-            if hasattr(self.models[i], "outcome_transform"):
-                oct = self.models[i].outcome_transform
-                tf_mvn = oct.untransform_posterior(GPyTorchPosterior(mvn)).distribution
-            else:
-                tf_mvn = mvn
-            mvns.append(tf_mvn)
-        # return result as a GPyTorchPosteriors/FullyBayesianPosterior
-        mvn = (
-            mvns[0]
-            if len(mvns) == 1
-            else MultitaskMultivariateNormal.from_independent_mvns(mvns=mvns)
+        # NOTE: We're not passing in the posterior transform here. We'll apply it later.
+        posterior = ModelList.posterior(
+            self,
+            X=X,
+            output_indices=output_indices,
+            observation_noise=observation_noise,
+            **kwargs,
         )
-        if any(is_fully_bayesian(m) for m in self.models):
-            # mixing fully Bayesian and other GP models is currently not supported
-            posterior = FullyBayesianPosterior(distribution=mvn)
-        else:
-            posterior = GPyTorchPosterior(distribution=mvn)
+        if not returns_untransformed:
+            mvns = [p.distribution for p in posterior.posteriors]
+            # Combining MTMVNs into a single MTMVN is currently not supported.
+            if not any(isinstance(m, MultitaskMultivariateNormal) for m in mvns):
+                # Return the result as a GPyTorchPosterior/FullyBayesianPosterior.
+                mvn = (
+                    mvns[0]
+                    if len(mvns) == 1
+                    else MultitaskMultivariateNormal.from_independent_mvns(mvns=mvns)
+                )
+                if any(is_fully_bayesian(m) for m in self.models):
+                    # Mixing fully Bayesian and other GP models is currently
+                    # not supported.
+                    posterior = FullyBayesianPosterior(distribution=mvn)
+                else:
+                    posterior = GPyTorchPosterior(distribution=mvn)
         if posterior_transform is not None:
             return posterior_transform(posterior)
         return posterior
 
     def condition_on_observations(self, X: Tensor, Y: Tensor, **kwargs: Any) -> Model:
         raise NotImplementedError()
 
@@ -702,52 +661,78 @@
         observation_noise: Union[bool, Tensor] = False,
         posterior_transform: Optional[PosteriorTransform] = None,
         **kwargs: Any,
     ) -> Union[GPyTorchPosterior, TransformedPosterior]:
         r"""Computes the posterior over model outputs at the provided points.
 
         Args:
-            X: A `q x d` or `batch_shape x q x d` (batch mode) tensor, where `d` is the
-                dimension of the feature space (not including task indices) and
-                `q` is the number of points considered jointly.
-            output_indices: A list of indices, corresponding to the outputs over
-                which to compute the posterior (if the model is multi-output).
-                Can be used to speed up computation if only a subset of the
-                model's outputs are required for optimization. If omitted,
-                computes the posterior over all model outputs.
+            X: A tensor of shape `batch_shape x q x d` or `batch_shape x q x (d + 1)`,
+                where `d` is the dimension of the feature space (not including task
+                indices) and `q` is the number of points considered jointly. The `+ 1`
+                dimension is the optional task feature / index. If given, the model
+                produces the outputs for the given task indices. If omitted, the
+                model produces outputs for tasks in in `self._output_tasks` (specified
+                as `output_tasks` while constructing the model), which can overwritten
+                using `output_indices`.
+            output_indices: A list of indices, corresponding to the tasks over
+                which to compute the posterior. Only used if `X` does not include the
+                task feature. If omitted, defaults to `self._output_tasks`.
             observation_noise: If True, add observation noise from the respective
                 likelihoods. If a Tensor, specifies the observation noise levels
                 to add.
             posterior_transform: An optional PosteriorTransform.
 
         Returns:
             A `GPyTorchPosterior` object, representing `batch_shape` joint
-            distributions over `q` points and the outputs selected by
-            `output_indices`. Includes measurement noise if
-            `observation_noise` is specified.
-        """
-        if output_indices is None:
-            output_indices = self._output_tasks
-        num_outputs = len(output_indices)
-        if any(i not in self._output_tasks for i in output_indices):
-            raise ValueError("Too many output indices")
-        cls_name = self.__class__.__name__
-
-        # construct evaluation X
-        X_full = _make_X_full(X=X, output_indices=output_indices, tf=self._task_feature)
+            distributions over `q` points. If the task features are included in `X`,
+            the posterior will be single output. Otherwise, the posterior will be
+            single or multi output corresponding to the tasks included in
+            either the `output_indices` or `self._output_tasks`.
+        """
+        includes_task_feature = X.shape[-1] == self.num_non_task_features + 1
+        if includes_task_feature:
+            # Make sure all task feature values are valid.
+            task_features = X[..., self._task_feature].unique()
+            if not (
+                (task_features >= 0).all() and (task_features < self.num_tasks).all()
+            ):
+                raise ValueError(
+                    "Expected all task features in `X` to be between 0 and "
+                    f"self.num_tasks - 1. Got {task_features}."
+                )
+            if output_indices is not None:
+                raise ValueError(
+                    "`output_indices` must be None when `X` includes task features."
+                )
+            num_outputs = 1
+            X_full = X
+        else:
+            # Add the task features to construct the full X for evaluation.
+            if output_indices is None:
+                output_indices = self._output_tasks
+            num_outputs = len(output_indices)
+            if not all(0 <= i < self.num_tasks for i in output_indices):
+                raise ValueError(
+                    "Expected `output_indices` to be between 0 and self.num_tasks - 1. "
+                    f"Got {output_indices}."
+                )
+            X_full = _make_X_full(
+                X=X, output_indices=output_indices, tf=self._task_feature
+            )
 
         self.eval()  # make sure model is in eval mode
         # input transforms are applied at `posterior` in `eval` mode, and at
         # `model.forward()` at the training time
         X_full = self.transform_inputs(X_full)
         with gpt_posterior_settings():
             mvn = self(X_full)
             if observation_noise is not False:
                 raise NotImplementedError(
-                    f"Specifying observation noise is not yet supported by {cls_name}"
+                    "Specifying observation noise is not yet supported by "
+                    f"{self.__class__.__name__}."
                 )
         # If single-output, return the posterior of a single-output model
         if num_outputs == 1:
             posterior = GPyTorchPosterior(distribution=mvn)
         else:
             # Otherwise, make a MultitaskMultivariateNormal out of this
             mtmvn = MultitaskMultivariateNormal(
```

### Comparing `botorch-0.8.5/botorch/models/higher_order_gp.py` & `botorch-0.9.1/botorch/models/higher_order_gp.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 import torch
 from botorch.acquisition.objective import PosteriorTransform
 from botorch.models.gpytorch import BatchedMultiOutputGPyTorchModel
 from botorch.models.model import FantasizeMixin
 from botorch.models.transforms.input import InputTransform
 from botorch.models.transforms.outcome import OutcomeTransform, Standardize
 from botorch.models.utils import gpt_posterior_settings
+from botorch.models.utils.gpytorch_modules import (
+    get_gaussian_likelihood_with_gamma_prior,
+)
 from botorch.posteriors import (
     GPyTorchPosterior,
     HigherOrderGPPosterior,
     TransformedPosterior,
 )
-from gpytorch.constraints import GreaterThan
 from gpytorch.distributions import MultivariateNormal
 from gpytorch.kernels import Kernel, MaternKernel
-from gpytorch.likelihoods import GaussianLikelihood, Likelihood
+from gpytorch.likelihoods import Likelihood
 from gpytorch.models import ExactGP
 from gpytorch.priors.torch_priors import GammaPrior, MultivariateNormalPrior
 from gpytorch.settings import fast_pred_var, skip_posterior_variances
 from linear_operator.operators import (
     BatchRepeatLinearOperator,
     DiagLinearOperator,
     KroneckerProductLinearOperator,
@@ -45,17 +47,14 @@
     ZeroLinearOperator,
 )
 from linear_operator.settings import _fast_solves
 from torch import Tensor
 from torch.nn import ModuleList, Parameter, ParameterList
 
 
-MIN_INFERRED_NOISE_LEVEL = 1e-4
-
-
 class FlattenedStandardize(Standardize):
     r"""
     Standardize outcomes in a structured multi-output settings by reshaping the
     batched output dimensions to be a vector. Specifically, an output dimension
     of [a x b x c] will be squeezed to be a vector of [a * b * c].
     """
 
@@ -228,25 +227,16 @@
         self._aug_batch_shape = batch_shape
         self._num_dimensions = num_output_dims + 1
         self._num_outputs = train_Y.shape[0] if batch_shape else 1
         self.target_shape = train_Y.shape[-num_output_dims:]
         self._input_batch_shape = batch_shape
 
         if likelihood is None:
-
-            noise_prior = GammaPrior(1.1, 0.05)
-            noise_prior_mode = (noise_prior.concentration - 1) / noise_prior.rate
-            likelihood = GaussianLikelihood(
-                noise_prior=noise_prior,
-                batch_shape=self._aug_batch_shape,
-                noise_constraint=GreaterThan(
-                    MIN_INFERRED_NOISE_LEVEL,
-                    transform=None,
-                    initial_value=noise_prior_mode,
-                ),
+            likelihood = get_gaussian_likelihood_with_gamma_prior(
+                batch_shape=self._aug_batch_shape
             )
         else:
             self._is_custom_likelihood = True
 
         super().__init__(
             train_X,
             train_Y.view(*self._aug_batch_shape, -1),
```

### Comparing `botorch-0.8.5/botorch/models/kernels/__init__.py` & `botorch-0.9.1/botorch/models/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/kernels/categorical.py` & `botorch-0.9.1/botorch/models/kernels/categorical.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/kernels/contextual_lcea.py` & `botorch-0.9.1/botorch/models/kernels/contextual_lcea.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,19 +7,86 @@
 from typing import Any, Dict, List, Optional
 
 import torch
 from gpytorch.constraints import Positive
 from gpytorch.kernels.kernel import Kernel
 from gpytorch.kernels.matern_kernel import MaternKernel
 from gpytorch.priors.torch_priors import GammaPrior
-from linear_operator.operators.sum_linear_operator import SumLinearOperator
+from linear_operator.operators import DiagLinearOperator
+from linear_operator.operators.dense_linear_operator import DenseLinearOperator
 from torch import Tensor
 from torch.nn import ModuleList
 
 
+def get_order(indices: List[int]) -> List[int]:
+    r"""Get the order indices as integers ranging from 0 to the number of indices.
+
+    Args:
+        indices: A list of parameter indices.
+
+    Returns:
+        A list of integers ranging from 0 to the number of indices.
+    """
+    return [i % len(indices) for i in indices]
+
+
+def is_contiguous(indices: List[int]) -> bool:
+    r"""Check if the list of integers is contiguous.
+
+    Args:
+        indices: A list of parameter indices.
+    Returns:
+        A boolean indicating whether the indices are contiguous.
+    """
+    min_idx = min(indices)
+    return set(indices) == set(range(min_idx, min_idx + len(indices)))
+
+
+def get_permutation(decomposition: Dict[str, List[int]]) -> Optional[List[int]]:
+    """Construct permutation to reorder the parameters such that:
+
+    1) the parameters for each context are contiguous.
+    2) The parameters for each context are in the same order
+
+    Args:
+        decomposition: A dictionary mapping context names to a list of
+            parameters.
+    Returns:
+        A permutation to reorder the parameters for (1) and (2).
+        Returning `None` means that ordering specified in `decomposition`
+        satisfies (1) and (2).
+    """
+    permutation = None
+    if not all(
+        is_contiguous(indices=active_parameters)
+        for active_parameters in decomposition.values()
+    ):
+        permutation = _create_new_permutation(decomposition=decomposition)
+    else:
+        same_order = True
+        expected_order = get_order(indices=next(iter(decomposition.values())))
+        for active_parameters in decomposition.values():
+            order = get_order(indices=active_parameters)
+            if order != expected_order:
+                same_order = False
+                break
+        if not same_order:
+            permutation = _create_new_permutation(decomposition=decomposition)
+    return permutation
+
+
+def _create_new_permutation(decomposition: Dict[str, List[int]]) -> List[int]:
+    # make contiguous and ordered
+    permutation = []
+    for active_parameters in decomposition.values():
+        sorted_indices = sorted(active_parameters)
+        permutation.extend(sorted_indices)
+    return permutation
+
+
 class LCEAKernel(Kernel):
     r"""The Latent Context Embedding Additive (LCE-A) Kernel.
 
     This kernel is similar to the SACKernel, and is used when context breakdowns are
     unbserverable. It assumes the same additive structure and a spatial kernel shared
     across contexts. Rather than assuming independence, LCEAKernel models the
     correlation in the latent functions for each context through learning context
@@ -36,16 +103,15 @@
         embs_dim_list: Optional[List[int]] = None,
         context_weight_dict: Optional[Dict] = None,
         device: Optional[torch.device] = None,
     ) -> None:
         r"""
         Args:
             decomposition: Keys index context names. Values are the indexes of
-                parameters belong to the context. The parameter indexes are in the same
-                order across contexts.
+                parameters belong to the context.
             batch_shape: Batch shape as usual for gpytorch kernels. Model does not
                 support batch training. When batch_shape is non-empty, it is used for
                 loading hyper-parameter values generated from MCMC sampling.
             train_embedding: A boolean indictor of whether to learn context embeddings.
             cat_feature_dict: Keys are context names and values are list of categorical
                 features i.e. {"context_name" : [cat_0, ..., cat_k]}. k equals the
                 number of categorical variables. If None, uses context names in the
@@ -54,34 +120,33 @@
                 context.
             embs_dim_list: Embedding dimension for each categorical variable. The length
                 equals to num of categorical features k. If None, the embedding
                 dimension is set to 1 for each categorical variable.
             context_weight_dict: Known population weights of each context.
         """
         super().__init__(batch_shape=batch_shape)
-        self.decomposition = decomposition
         self.batch_shape = batch_shape
         self.train_embedding = train_embedding
         self._device = device
 
-        num_param = len(next(iter(decomposition.values())))
+        self.num_param = len(next(iter(decomposition.values())))
         self.context_list = list(decomposition.keys())
         self.num_contexts = len(self.context_list)
 
         # get parameter space decomposition
         for active_parameters in decomposition.values():
             # check number of parameters are same in each decomp
-            if len(active_parameters) != num_param:
+            if len(active_parameters) != self.num_param:
                 raise ValueError(
-                    "num of parameters needs to be same across all contexts"
+                    "The number of parameters needs to be same across all contexts."
                 )
-        self._indexers = {
-            context: torch.tensor(active_params, device=self.device)
-            for context, active_params in self.decomposition.items()
-        }
+        # reorder the parameter list based on decomposition such that
+        # parameters for each context are contiguous and in the same order for each
+        # context
+        self.permutation = get_permutation(decomposition=decomposition)
         # get context features and set emb dim
         self.context_cat_feature = None
         self.context_emb_feature = None
         self.n_embs = 0
         self.emb_weight_matrix_list = None
         self.emb_dims = None
         self._set_context_features(
@@ -98,15 +163,15 @@
             ard_num_dims=self.n_embs,
             batch_shape=batch_shape,
             lengthscale_prior=GammaPrior(3.0, 6.0),
         )
         # base kernel
         self.base_kernel = MaternKernel(
             nu=2.5,
-            ard_num_dims=num_param,
+            ard_num_dims=self.num_param,
             batch_shape=batch_shape,
             lengthscale_prior=GammaPrior(3.0, 6.0),
         )
         # outputscales for each context (note this is like sqrt of outputscale)
         self.context_weight = None
         if context_weight_dict is None:
             outputscale_list = torch.zeros(
@@ -299,51 +364,76 @@
                         *self.batch_shape + self.context_emb_feature.shape
                     ),
                 ],
                 dim=-1,
             )
         return embeddings
 
+    def train(self, mode: bool = True) -> None:
+        super().train(mode=mode)
+        if not mode:
+            self.register_buffer("_context_covar", self._eval_context_covar())
+
     def forward(
         self,
         x1: Tensor,
         x2: Tensor,
         diag: bool = False,
         last_dim_is_batch: bool = False,
         **params: Any,
     ) -> Tensor:
         """Iterate across each partition of parameter space and sum the
         covariance matrices together
         """
         # context covar matrix
-        context_covar = self._eval_context_covar()
-        # check input batch size if b x ns x n x d: expand context_covar to
-        # b x ns x num_context x num_context
-        if x1.dim() > context_covar.dim():
-            context_covar = context_covar.expand(*x1.shape[:1] + context_covar.shape)
-        covars = []
-        # TODO: speed computation of covariance matrix
-        for i in range(self.num_contexts):
-            for j in range(self.num_contexts):
-                context1 = self.context_list[i]
-                context2 = self.context_list[j]
-                active_params1 = self._indexers[context1]
-                active_params2 = self._indexers[context2]
-                covars.append(
-                    (
-                        context_covar.index_select(  # pyre-ignore
-                            -1, torch.tensor([j], device=self.device)
-                        ).index_select(
-                            -2, torch.tensor([i], device=self.device)
-                        )  # b x ns x 1 x 1
-                    )
-                    * self.base_kernel(
-                        x1=x1.index_select(-1, active_params1),
-                        x2=x2.index_select(-1, active_params2),
-                        diag=diag,
-                    )
-                )
+        context_covar = (
+            self._eval_context_covar() if self.training else self._context_covar
+        )
+        base_covar_perm = self._eval_base_covar_perm(x1, x2)
+        # expand context_covar to match base_covar_perm
+        if base_covar_perm.dim() > context_covar.dim():
+            context_covar = context_covar.expand(base_covar_perm.shape)
+        # then weight by the context kernel
+        # compute the base kernel on the d parameters
+        einsum_str = "...nnki, ...nnki -> ...n" if diag else "...ki, ...ki -> ..."
+        covar_dense = torch.einsum(einsum_str, context_covar, base_covar_perm)
         if diag:
-            res = sum(covars)
-        else:
-            res = SumLinearOperator(*covars)
-        return res
+            return DiagLinearOperator(covar_dense)
+        return DenseLinearOperator(covar_dense)
+
+    def _eval_base_covar_perm(self, x1: Tensor, x2: Tensor) -> Tensor:
+        """Computes the base covariance matrix on x1, x2, applying permutations and
+        reshaping the kernel matrix as required by `forward`.
+
+        NOTE: Using the notation n = num_observations, k = num_contexts, d = input_dim,
+        the input tensors have to have the following shapes.
+
+        Args:
+            x1: `batch_shape x n x (k*d)`-dim Tensor of kernel inputs.
+            x2: `batch_shape x n x (k*d)`-dim Tensor of kernel inputs.
+
+        Returns:
+            `batch_shape x n x n x k x k`-dim Tensor of base covariance values.
+        """
+        if self.permutation is not None:
+            x1 = x1[..., self.permutation]
+            x2 = x2[..., self.permutation]
+        # turn last two dimensions of n x (k*d) into (n*k) x d.
+        x1_exp = x1.reshape(*x1.shape[:-2], -1, self.num_param)
+        x2_exp = x2.reshape(*x2.shape[:-2], -1, self.num_param)
+        # batch shape x n*k x n*k
+        base_covar = self.base_kernel(x1_exp, x2_exp)
+        # batch shape x n x n x k x k
+        view_shape = x1.shape[:-2] + torch.Size(
+            [
+                x1.shape[-2],
+                self.num_contexts,
+                x2.shape[-2],
+                self.num_contexts,
+            ]
+        )
+        base_covar_perm = (
+            base_covar.to_dense()
+            .view(view_shape)
+            .permute(*list(range(x1.ndim - 2)), -4, -2, -3, -1)
+        )
+        return base_covar_perm
```

### Comparing `botorch-0.8.5/botorch/models/kernels/contextual_sac.py` & `botorch-0.9.1/botorch/models/kernels/contextual_sac.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/kernels/downsampling.py` & `botorch-0.9.1/botorch/models/kernels/downsampling.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/kernels/exponential_decay.py` & `botorch-0.9.1/botorch/models/kernels/exponential_decay.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/kernels/linear_truncated_fidelity.py` & `botorch-0.9.1/botorch/models/kernels/linear_truncated_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/likelihoods/pairwise.py` & `botorch-0.9.1/botorch/models/likelihoods/pairwise.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 from __future__ import annotations
 
 import math
 from abc import ABC, abstractmethod
 from typing import Any, Tuple
 
 import torch
+from botorch.utils.probability.utils import (
+    log_ndtr,
+    log_phi,
+    standard_normal_log_hazard,
+)
 from gpytorch.likelihoods import Likelihood
 from torch import Tensor
 from torch.distributions import Bernoulli
 
 
 class PairwiseLikelihood(Likelihood, ABC):
     """
@@ -116,24 +121,24 @@
         scaled_util = (utility / math.sqrt(2)).unsqueeze(-1)
         z = D.to(scaled_util) @ scaled_util
         z = z.clamp(-self._zlim, self._zlim).squeeze(-1)
         return z
 
     def _calc_z_derived(self, z: Tensor) -> Tuple[Tensor, Tensor, Tensor]:
         """Calculate auxiliary statistics derived from z, including log pdf,
-        log cdf, and the hazard function (pdf divided by cdf)"""
-        std_norm = torch.distributions.normal.Normal(
-            torch.zeros(1, dtype=z.dtype, device=z.device),
-            torch.ones(1, dtype=z.dtype, device=z.device),
-        )
-        z_logpdf = std_norm.log_prob(z)
-        z_cdf = std_norm.cdf(z)
-        z_logcdf = torch.log(z_cdf)
-        hazard = torch.exp(z_logpdf - z_logcdf)
-        return z_logpdf, z_logcdf, hazard
+        log cdf, and the hazard function (pdf divided by cdf)
+
+        Args:
+            z: A Tensor of arbitrary shape.
+
+        Returns:
+            Tensors with standard normal logpdf(z), logcdf(z), and hazard function
+            values evaluated at -z.
+        """
+        return log_phi(z), log_ndtr(z), standard_normal_log_hazard(-z).exp()
 
     def p(self, utility: Tensor, D: Tensor, log: bool = False) -> Tensor:
         z = self._calc_z(utility=utility, D=D)
         std_norm = torch.distributions.normal.Normal(
             torch.zeros(1, dtype=z.dtype, device=z.device),
             torch.ones(1, dtype=z.dtype, device=z.device),
         )
@@ -144,15 +149,14 @@
         # Original grad should be of dimension m x n, as in (6) from
         # [Chu2005preference]_. The sum over the m dimension of grad. of
         # negative log likelihood with respect to the utility
         z = self._calc_z(utility, D)
         _, _, h = self._calc_z_derived(z)
         h_factor = h / math.sqrt(2)
         grad = (h_factor.unsqueeze(-2) @ (-D)).squeeze(-2)
-
         return grad
 
     def negative_log_hessian_sum(self, utility: Tensor, D: Tensor) -> Tensor:
         # Original hess should be of dimension m x n x n, as in (7) from
         # [Chu2005preference]_ Sum over the first dimension and return a tensor of
         # shape n x n.
         # The sum over the m dimension of hessian of negative log likelihood
```

### Comparing `botorch-0.8.5/botorch/models/model.py` & `botorch-0.9.1/botorch/models/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,18 +28,20 @@
     TypeVar,
     Union,
 )
 
 import numpy as np
 import torch
 from botorch import settings
-from botorch.exceptions.errors import InputDataError
+from botorch.exceptions.errors import BotorchTensorDimensionError, InputDataError
+from botorch.logging import shape_to_str
 from botorch.models.utils.assorted import fantasize as fantasize_flag
 from botorch.posteriors import Posterior, PosteriorList
 from botorch.sampling.base import MCSampler
+from botorch.sampling.list_sampler import ListSampler
 from botorch.utils.datasets import BotorchDataset
 from botorch.utils.transforms import is_fully_bayesian
 from torch import Tensor
 from torch.nn import Module, ModuleDict, ModuleList
 
 if TYPE_CHECKING:
     from botorch.acquisition.objective import PosteriorTransform  # pragma: no cover
@@ -323,14 +325,27 @@
             sampler: The sampler used for sampling from the posterior at `X`.
             observation_noise: If True, include observation noise.
             kwargs: Will be passed to `model.condition_on_observations`
 
         Returns:
             The constructed fantasy model.
         """
+        # if the inputs are empty, expand the inputs
+        if X.shape[-2] == 0:
+            output_shape = (
+                sampler.sample_shape
+                + X.shape[:-2]
+                + self.batch_shape
+                + torch.Size([0, self.num_outputs])
+            )
+            return self.condition_on_observations(
+                X=self.transform_inputs(X),
+                Y=torch.empty(output_shape, dtype=X.dtype, device=X.device),
+                **kwargs,
+            )
         propagate_grads = kwargs.pop("propagate_grads", False)
         with fantasize_flag():
             with settings.propagate_grads(propagate_grads):
                 post_X = self.posterior(X, observation_noise=observation_noise)
             Y_fantasized = sampler(post_X)  # num_fantasies x batch_shape x n' x m
             return self.condition_on_observations(
                 X=self.transform_inputs(X), Y=Y_fantasized, **kwargs
@@ -364,15 +379,15 @@
 
     def _get_group_subset_indices(
         self, idcs: Optional[List[int]]
     ) -> Dict[int, List[int]]:
         r"""Convert global subset indices to indices for the individual models.
 
         Args:
-            idcs: A list of inidices to which the `ModelList` model is to be
+            idcs: A list of indices to which the `ModelList` model is to be
                 subset to.
 
         Returns:
             A dictionary mapping model indices to subset indices of the
                 respective model in the `ModelList`.
         """
         if idcs is None:
@@ -387,15 +402,15 @@
             group_indices[grp_idx].append(sub_idx)
         return group_indices
 
     def posterior(
         self,
         X: Tensor,
         output_indices: Optional[List[int]] = None,
-        observation_noise: bool = False,
+        observation_noise: Union[bool, Tensor] = False,
         posterior_transform: Optional[Callable[[PosteriorList], Posterior]] = None,
         **kwargs: Any,
     ) -> Posterior:
         r"""Computes the posterior over model outputs at the provided points.
 
         Note: The input transforms should be applied here using
             `self.transform_inputs(X)` after the `self.eval()` call and before
@@ -406,28 +421,41 @@
                 feature space, `q` is the number of points considered jointly,
                 and `b` is the batch dimension.
             output_indices: A list of indices, corresponding to the outputs over
                 which to compute the posterior (if the model is multi-output).
                 Can be used to speed up computation if only a subset of the
                 model's outputs are required for optimization. If omitted,
                 computes the posterior over all model outputs.
-            observation_noise: If True, add observation noise to the posterior.
+            observation_noise: If True, add the observation noise from the
+                respective likelihoods to the posterior. If a Tensor of shape
+                `(batch_shape) x q x m`, use it directly as the observation
+                noise (with `observation_noise[...,i]` added to the posterior
+                of the `i`-th model).
             posterior_transform: An optional PosteriorTransform.
 
         Returns:
             A `Posterior` object, representing a batch of `b` joint distributions
             over `q` points and `m` outputs each.
         """
         group_indices = self._get_group_subset_indices(idcs=output_indices)
-        posteriors = [
-            self.models[i].posterior(
-                X=X, output_indices=idcs, observation_noise=observation_noise
+        posteriors = []
+        for i, idcs in group_indices.items():
+            if isinstance(observation_noise, Tensor):
+                if idcs is None:
+                    start_idx = sum(m.num_outputs for m in self.models[:i])
+                    end_idx = start_idx + self.models[i].num_outputs
+                    idcs = list(range(start_idx, end_idx))
+                obs_noise = observation_noise[..., idcs]
+            else:
+                obs_noise = observation_noise
+            posteriors.append(
+                self.models[i].posterior(
+                    X=X, output_indices=idcs, observation_noise=obs_noise
+                )
             )
-            for i, idcs in group_indices.items()
-        ]
         posterior = PosteriorList(*posteriors)
         if posterior_transform is not None:
             posterior = posterior_transform(posterior)
         return posterior
 
     @property
     def batch_shape(self) -> torch.Size:
@@ -512,14 +540,80 @@
                     k.replace(f"models.{i}.", ""): v
                     for k, v in state_dict.items()
                     if k.startswith(f"models.{i}.")
                 }
                 m.load_state_dict(filtered_dict)
         super().load_state_dict(state_dict=state_dict, strict=strict)
 
+    def fantasize(
+        self,
+        X: Tensor,
+        sampler: MCSampler,
+        observation_noise: bool = True,
+        evaluation_mask: Optional[Tensor] = None,
+        **kwargs: Any,
+    ) -> Model:
+        r"""Construct a fantasy model.
+
+        Constructs a fantasy model in the following fashion:
+        (1) compute the model posterior at `X` (including observation noise if
+        `observation_noise=True`).
+        (2) sample from this posterior (using `sampler`) to generate "fake"
+        observations.
+        (3) condition the model on the new fake observations.
+
+        Args:
+            X: A `batch_shape x n' x d`-dim Tensor, where `d` is the dimension of
+                the feature space, `n'` is the number of points per batch, and
+                `batch_shape` is the batch shape (must be compatible with the
+                batch shape of the model).
+            sampler: The sampler used for sampling from the posterior at `X`. If
+                evaluation_mask is not None, this must be a `ListSampler`.
+            observation_noise: If True, include observation noise.
+            evaluation_mask: A `n' x m`-dim tensor of booleans indicating which
+                outputs should be fantasized for a given design. This uses the same
+                evaluation mask for all batches.
+
+        Returns:
+            The constructed fantasy model.
+        """
+        if evaluation_mask is not None:
+            if evaluation_mask.ndim != 2 or evaluation_mask.shape != torch.Size(
+                [X.shape[-2], self.num_outputs]
+            ):
+                raise BotorchTensorDimensionError(
+                    f"Expected evaluation_mask of shape `{X.shape[0]} "
+                    f"x {self.num_outputs}`, but got "
+                    f"{shape_to_str(evaluation_mask.shape)}."
+                )
+            if not isinstance(sampler, ListSampler):
+                raise ValueError("Decoupled fantasization requires a list of samplers.")
+
+        fant_models = []
+        X_i = X
+        for i in range(self.num_outputs):
+            # get the inputs to fantasize at for output i
+            if evaluation_mask is not None:
+                mask_i = evaluation_mask[:, i]
+                X_i = X[..., mask_i, :]
+                # TODO (T158701749): implement a QMC DecoupledSampler that draws all
+                # samples from a single Sobol sequence or consider requiring that the
+                # sampling is IID to ensure good coverage.
+                sampler_i = sampler.samplers[i]
+            else:
+                sampler_i = sampler
+            fant_model = self.models[i].fantasize(
+                X=X_i,
+                sampler=sampler_i,
+                observation_noise=observation_noise,
+                **kwargs,
+            )
+            fant_models.append(fant_model)
+        return self.__class__(*fant_models)
+
 
 class ModelDict(ModuleDict):
     r"""A lightweight container mapping model names to models."""
 
     def __init__(self, **models: Model) -> None:
         r"""Initialize a `ModelDict`.
```

### Comparing `botorch-0.8.5/botorch/models/model_list_gp_regression.py` & `botorch-0.9.1/botorch/models/model_list_gp_regression.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/multitask.py` & `botorch-0.9.1/botorch/models/multitask.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,51 +5,63 @@
 # LICENSE file in the root directory of this source tree.
 
 r"""
 Multi-Task GP models.
 
 References
 
+.. [Bonilla2007MTGP]
+    E. Bonilla, K. Chai and C. Williams. Multi-task Gaussian Process Prediction.
+    Advances in Neural Information Processing Systems 20, NeurIPS 2007.
+
+.. [Swersky2013MTBO]
+    K. Swersky, J. Snoek and R. Adams. Multi-Task Bayesian Optimization.
+    Advances in Neural Information Processing Systems 26, NeurIPS 2013.
+
 .. [Doucet2010sampl]
     A. Doucet. A Note on Efficient Conditional Simulation of Gaussian Distributions.
     http://www.stats.ox.ac.uk/~doucet/doucet_simulationconditionalgaussian.pdf,
     Apr 2010.
 
 .. [Maddox2021bohdo]
     W. Maddox, M. Balandat, A. Wilson, and E. Bakshy. Bayesian Optimization with
     High-Dimensional Outputs. https://arxiv.org/abs/2106.12997, Jun 2021.
 """
 
 from __future__ import annotations
 
 import math
+import warnings
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import torch
 from botorch.acquisition.objective import PosteriorTransform
-from botorch.models.gp_regression import MIN_INFERRED_NOISE_LEVEL
 from botorch.models.gpytorch import GPyTorchModel, MultiTaskGPyTorchModel
 from botorch.models.model import FantasizeMixin
 from botorch.models.transforms.input import InputTransform
 from botorch.models.transforms.outcome import OutcomeTransform
+from botorch.models.utils.gpytorch_modules import (
+    get_matern_kernel_with_gamma_prior,
+    MIN_INFERRED_NOISE_LEVEL,
+)
 from botorch.posteriors.multitask import MultitaskGPPosterior
 from botorch.utils.datasets import SupervisedDataset
 from gpytorch.constraints import GreaterThan
 from gpytorch.distributions.multitask_multivariate_normal import (
     MultitaskMultivariateNormal,
 )
 from gpytorch.distributions.multivariate_normal import MultivariateNormal
 from gpytorch.kernels.index_kernel import IndexKernel
 from gpytorch.kernels.matern_kernel import MaternKernel
 from gpytorch.kernels.multitask_kernel import MultitaskKernel
-from gpytorch.kernels.scale_kernel import ScaleKernel
 from gpytorch.likelihoods.gaussian_likelihood import (
     FixedNoiseGaussianLikelihood,
     GaussianLikelihood,
 )
+from gpytorch.likelihoods.likelihood import Likelihood
 from gpytorch.likelihoods.multitask_gaussian_likelihood import (
     MultitaskGaussianLikelihood,
 )
 from gpytorch.means import MultitaskMean
 from gpytorch.means.constant_mean import ConstantMean
 from gpytorch.models.exact_gp import ExactGP
 from gpytorch.module import Module
@@ -69,47 +81,63 @@
     RootLinearOperator,
     to_linear_operator,
 )
 from torch import Tensor
 
 
 class MultiTaskGP(ExactGP, MultiTaskGPyTorchModel, FantasizeMixin):
-    r"""Multi-Task GP model using an ICM kernel, inferring observation noise.
+    r"""Multi-Task exact GP model using an ICM (intrinsic co-regionalization model)
+    kernel. See [Bonilla2007MTGP]_ and [Swersky2013MTBO]_ for a reference on the
+    model and its use in Bayesian optimization.
+
 
-    Multi-task exact GP that uses a simple ICM kernel. Can be single-output or
-    multi-output. This model uses relatively strong priors on the base Kernel
-    hyperparameters, which work best when covariates are normalized to the unit
-    cube and outcomes are standardized (zero mean, unit variance).
-
-    This model infers the noise level. WARNING: It currently does not support
-    different noise levels for the different tasks. If you have known observation
-    noise, please use `FixedNoiseMultiTaskGP` instead.
+    The model can be single-output or multi-output, determined by the `output_tasks`.
+    This model uses relatively strong priors on the base Kernel hyperparameters, which
+    work best when covariates are normalized to the unit cube and outcomes are
+    standardized (zero mean, unit variance).
+
+    If the `train_Yvar` is None, this model infers the noise level. If you have
+    known observation noise, you can set `train_Yvar` to a tensor containing
+    the noise variance measurements. WARNING: This currently does not support
+    different noise levels for the different tasks.
     """
 
     def __init__(
         self,
         train_X: Tensor,
         train_Y: Tensor,
         task_feature: int,
+        train_Yvar: Optional[Tensor] = None,
+        mean_module: Optional[Module] = None,
         covar_module: Optional[Module] = None,
+        likelihood: Optional[Likelihood] = None,
         task_covar_prior: Optional[Prior] = None,
         output_tasks: Optional[List[int]] = None,
         rank: Optional[int] = None,
         input_transform: Optional[InputTransform] = None,
         outcome_transform: Optional[OutcomeTransform] = None,
     ) -> None:
-        r"""Multi-Task GP model using an ICM kernel, inferring observation noise.
+        r"""Multi-Task GP model using an ICM kernel.
 
         Args:
             train_X: A `n x (d + 1)` or `b x n x (d + 1)` (batch mode) tensor
                 of training data. One of the columns should contain the task
                 features (see `task_feature` argument).
             train_Y: A `n x 1` or `b x n x 1` (batch mode) tensor of training
                 observations.
             task_feature: The index of the task feature (`-d <= task_feature <= d`).
+            train_Yvar: An optional `n` or `b x n` (batch mode) tensor of observed
+                measurement noise. If None, we infer the noise.
+                Note that the inferred noise is common across all tasks.
+            mean_module: The mean function to be used. Defaults to `ConstantMean`.
+            covar_module: The module for computing the covariance matrix between
+                the non-task features. Defaults to `MaternKernel`.
+            likelihood: A likelihood. The default is selected based on `train_Yvar`.
+                If `train_Yvar` is None, a standard `GaussianLikelihood` with inferred
+                noise level is used. Otherwise, a FixedNoiseGaussianLikelihood is used.
             output_tasks: A list of task indices for which to compute model
                 outputs for. If omitted, return outputs for all task indices.
             rank: The rank to be used for the index kernel. If omitted, use a
                 full rank (i.e. number of tasks) kernel.
             task_covar_prior : A Prior on the task covariance matrix. Must operate
                 on p.s.d. matrices. A common prior for this is the `LKJ` prior.
             input_transform: An input transform that is applied in the model's
@@ -128,58 +156,58 @@
             >>> train_Y = torch.cat(f1(X1), f2(X2)).unsqueeze(-1)
             >>> model = MultiTaskGP(train_X, train_Y, task_feature=-1)
         """
         with torch.no_grad():
             transformed_X = self.transform_inputs(
                 X=train_X, input_transform=input_transform
             )
-        self._validate_tensor_args(X=transformed_X, Y=train_Y)
-        all_tasks, task_feature, d = self.get_all_tasks(
+        self._validate_tensor_args(X=transformed_X, Y=train_Y, Yvar=train_Yvar)
+        all_tasks, task_feature, self.num_non_task_features = self.get_all_tasks(
             transformed_X, task_feature, output_tasks
         )
+        self.num_tasks = len(all_tasks)
         if outcome_transform is not None:
-            train_Y, _ = outcome_transform(train_Y)
+            train_Y, train_Yvar = outcome_transform(Y=train_Y, Yvar=train_Yvar)
 
         # squeeze output dim
         train_Y = train_Y.squeeze(-1)
         if output_tasks is None:
             output_tasks = all_tasks
         else:
             if set(output_tasks) - set(all_tasks):
                 raise RuntimeError("All output tasks must be present in input data.")
         self._output_tasks = output_tasks
         self._num_outputs = len(output_tasks)
 
         # TODO (T41270962): Support task-specific noise levels in likelihood
-        likelihood = GaussianLikelihood(noise_prior=GammaPrior(1.1, 0.05))
+        if likelihood is None:
+            if train_Yvar is None:
+                likelihood = GaussianLikelihood(noise_prior=GammaPrior(1.1, 0.05))
+            else:
+                likelihood = FixedNoiseGaussianLikelihood(noise=train_Yvar.squeeze(-1))
 
         # construct indexer to be used in forward
         self._task_feature = task_feature
-        self._base_idxr = torch.arange(d)
+        self._base_idxr = torch.arange(self.num_non_task_features)
         self._base_idxr[task_feature:] += 1  # exclude task feature
 
         super().__init__(
             train_inputs=train_X, train_targets=train_Y, likelihood=likelihood
         )
-        self.mean_module = ConstantMean()
+        self.mean_module = mean_module or ConstantMean()
         if covar_module is None:
-            self.covar_module = ScaleKernel(
-                base_kernel=MaternKernel(
-                    nu=2.5, ard_num_dims=d, lengthscale_prior=GammaPrior(3.0, 6.0)
-                ),
-                outputscale_prior=GammaPrior(2.0, 0.15),
+            self.covar_module = get_matern_kernel_with_gamma_prior(
+                ard_num_dims=self.num_non_task_features
             )
         else:
             self.covar_module = covar_module
 
-        num_tasks = len(all_tasks)
-        self._rank = rank if rank is not None else num_tasks
-
+        self._rank = rank if rank is not None else self.num_tasks
         self.task_covar_module = IndexKernel(
-            num_tasks=num_tasks, rank=self._rank, prior=task_covar_prior
+            num_tasks=self.num_tasks, rank=self._rank, prior=task_covar_prior
         )
         if input_transform is not None:
             self.input_transform = input_transform
         if outcome_transform is not None:
             self.outcome_transform = outcome_transform
         self.to(train_X)
 
@@ -294,22 +322,15 @@
             "rank": rank,
         }
 
 
 class FixedNoiseMultiTaskGP(MultiTaskGP):
     r"""Multi-Task GP model using an ICM kernel, with known observation noise.
 
-    This is the fixed-noise version of `MultiTaskGP` -– that is,
-    `FixedNoiseMultiTaskGP` is to `MultiTaskGP` as `FixedNoiseGP` is to
-    `SingleTaskGP`. It can be single-output or
-    multi-output. This model uses relatively strong priors on the base Kernel
-    hyperparameters, which work best when covariates are normalized to the unit
-    cube and outcomes are standardized (zero mean, unit variance).
-
-    This model requires observation noise data (specified in `train_Yvar`).
+    DEPRECATED: Please use `MultiTaskGP` with `train_Yvar` instead.
     """
 
     def __init__(
         self,
         train_X: Tensor,
         train_Y: Tensor,
         train_Yvar: Tensor,
@@ -324,16 +345,16 @@
         r"""
         Args:
             train_X: A `n x (d + 1)` or `b x n x (d + 1)` (batch mode) tensor
                 of training data. One of the columns should contain the task
                 features (see `task_feature` argument).
             train_Y: A `n x 1` or `b x n x 1` (batch mode) tensor of training
                 observations.
-            train_Yvar: A `n` or `b x n` (batch mode) tensor of observation
-                noise standard errors.
+            train_Yvar: A `n` or `b x n` (batch mode) tensor of observed measurement
+                noise.
             task_feature: The index of the task feature (`-d <= task_feature <= d`).
             task_covar_prior : A Prior on the task covariance matrix. Must operate
                 on p.s.d. matrices. A common prior for this is the `LKJ` prior.
             output_tasks: A list of task indices for which to compute model
                 outputs for. If omitted, return outputs for all task indices.
             rank: The rank to be used for the index kernel. If omitted, use a
                 full rank (i.e. number of tasks) kernel.
@@ -350,41 +371,34 @@
             >>> train_X = torch.cat([
             >>>     torch.cat([X1, i1], -1), torch.cat([X2, i2], -1),
             >>> ], dim=0)
             >>> train_Y = torch.cat(f1(X1), f2(X2))
             >>> train_Yvar = 0.1 + 0.1 * torch.rand_like(train_Y)
             >>> model = FixedNoiseMultiTaskGP(train_X, train_Y, train_Yvar, -1)
         """
-        with torch.no_grad():
-            transformed_X = self.transform_inputs(
-                X=train_X, input_transform=input_transform
-            )
-        self._validate_tensor_args(X=transformed_X, Y=train_Y, Yvar=train_Yvar)
-
-        if outcome_transform is not None:
-            train_Y, train_Yvar = outcome_transform(train_Y, train_Yvar)
-
-        # We'll instatiate a MultiTaskGP and simply override the likelihood
+        warnings.warn(
+            "`FixedNoiseMultiTaskGP` has been deprecated and will be removed in a "
+            "future release. Please use the `MultiTaskGP` model instead. "
+            "When `train_Yvar` is specified, `MultiTaskGP` behaves the same "
+            "as the `FixedNoiseMultiTaskGP`.",
+            DeprecationWarning,
+        )
         super().__init__(
             train_X=train_X,
             train_Y=train_Y,
+            train_Yvar=train_Yvar,
             covar_module=covar_module,
             task_feature=task_feature,
             output_tasks=output_tasks,
             rank=rank,
             task_covar_prior=task_covar_prior,
             input_transform=input_transform,
-            outcome_transform=None,  # outcome_transform is applied already
+            outcome_transform=outcome_transform,
         )
 
-        if outcome_transform is not None:
-            self.outcome_transform = outcome_transform
-        self.likelihood = FixedNoiseGaussianLikelihood(noise=train_Yvar.squeeze(-1))
-        self.to(train_X)
-
 
 class KroneckerMultiTaskGP(ExactGP, GPyTorchModel, FantasizeMixin):
     """Multi-task GP with Kronecker structure, using an ICM kernel.
 
     This model assumes the "block design" case, i.e., it requires that all tasks
     are observed at all data points.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `botorch-0.8.5/botorch/models/pairwise_gp.py` & `botorch-0.9.1/botorch/models/pairwise_gp.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,21 +407,22 @@
         """
         prior_mean = self._prior_mean(datapoints)
 
         if ret_np:
             utility = torch.tensor(utility, dtype=self.datapoints.dtype)
             prior_mean = prior_mean.cpu()
 
+        # NOTE: During the optimization, it can occur that b, p, and g_ are NaNs, though
+        # in the cases that occured during testing, the optimization routine escaped and
+        # terminated successfully without NaNs in the result.
         b = self.likelihood.negative_log_gradient_sum(utility=utility, D=D)
-
         # g_ = covar_inv x (utility - pred_prior)
         p = (utility - prior_mean).unsqueeze(-1).to(covar_chol)
         g_ = torch.cholesky_solve(p, covar_chol).squeeze(-1)
         g = g_ + b
-
         if ret_np:
             return g.cpu().numpy()
         else:
             return g
 
     def _hess_posterior_f(
         self,
@@ -571,15 +572,15 @@
                         args=fsolve_args,
                         **kwargs,
                     )
 
             self._x0 = x.copy()  # save for warm-starting
             f = torch.tensor(x, dtype=datapoints.dtype, device=datapoints.device)
 
-        # To perform hyperparameter optimization, this need to be recalculated
+        # To perform hyperparameter optimization, this needs to be recalculated
         # when calling forward() in order to obtain correct gradients
         # self.likelihood_hess is updated here is for the rare case where we
         # do not want to call forward()
         self.likelihood_hess = self.likelihood.negative_log_hessian_sum(
             utility=f, D=self.D
         )
```

### Comparing `botorch-0.8.5/botorch/models/transforms/__init__.py` & `botorch-0.9.1/botorch/models/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/transforms/factory.py` & `botorch-0.9.1/botorch/models/transforms/factory.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/transforms/input.py` & `botorch-0.9.1/botorch/models/transforms/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             other: Another input transform.
 
         Returns:
             A boolean indicating if the other transform is equivalent.
         """
         other_state_dict = other.state_dict()
         return (
-            type(self) == type(other)
+            type(self) is type(other)
             and (self.transform_on_train == other.transform_on_train)
             and (self.transform_on_eval == other.transform_on_eval)
             and (self.transform_on_fantasize == other.transform_on_fantasize)
             and all(
                 torch.allclose(v, other_state_dict[k].to(v))
                 for k, v in self.state_dict().items()
             )
@@ -320,15 +320,15 @@
 
 class AffineInputTransform(ReversibleInputTransform, Module):
     def __init__(
         self,
         d: int,
         coefficient: Tensor,
         offset: Tensor,
-        indices: Optional[List[int]] = None,
+        indices: Optional[Union[List[int], Tensor]] = None,
         batch_shape: torch.Size = torch.Size(),  # noqa: B008
         transform_on_train: bool = True,
         transform_on_eval: bool = True,
         transform_on_fantasize: bool = True,
         reverse: bool = False,
     ) -> None:
         r"""Apply affine transformation to input:
@@ -338,15 +338,16 @@
         Args:
             d: The dimension of the input space.
             coefficient: Tensor of linear coefficients, shape must to be
                 broadcastable with `(batch_shape x n x d)`-dim input tensors.
             offset: Tensor of offset coefficients, shape must to be
                 broadcastable with `(batch_shape x n x d)`-dim input tensors.
             indices: The indices of the inputs to transform. If omitted,
-                take all dimensions of the inputs into account.
+                take all dimensions of the inputs into account. Either a list of ints
+                or a Tensor of type `torch.long`.
             batch_shape: The batch shape of the inputs (assuming input tensors
                 of shape `batch_shape x n x d`). If provided, perform individual
                 transformation per batch, otherwise uses a single transformation.
             transform_on_train: A boolean indicating whether to apply the
                 transform in train() mode. Default: True.
             transform_on_eval: A boolean indicating whether to apply the
                 transform in eval() mode. Default: True.
@@ -355,15 +356,17 @@
             reverse: A boolean indicating whether the forward pass should untransform
                 the inputs.
         """
         super().__init__()
         if (indices is not None) and (len(indices) == 0):
             raise ValueError("`indices` list is empty!")
         if (indices is not None) and (len(indices) > 0):
-            indices = torch.tensor(indices, dtype=torch.long)
+            indices = torch.as_tensor(
+                indices, dtype=torch.long, device=coefficient.device
+            )
             if len(indices) > d:
                 raise ValueError("Can provide at most `d` indices!")
             if (indices > d - 1).any():
                 raise ValueError("Elements of `indices` have to be smaller than `d`!")
             if len(indices.unique()) != len(indices):
                 raise ValueError("Elements of `indices` tensor must be unique!")
             self.register_buffer("indices", indices)
@@ -494,15 +497,15 @@
     in eval mode, calling `forward` simply applies the normalization using the
     current module state.
     """
 
     def __init__(
         self,
         d: int,
-        indices: Optional[List[int]] = None,
+        indices: Optional[Union[List[int], Tensor]] = None,
         bounds: Optional[Tensor] = None,
         batch_shape: torch.Size = torch.Size(),  # noqa: B008
         transform_on_train: bool = True,
         transform_on_eval: bool = True,
         transform_on_fantasize: bool = True,
         reverse: bool = False,
         min_range: float = 1e-8,
@@ -622,15 +625,15 @@
     (i.e. the mean/std normalizing constants). If in eval mode, calling `forward`
     simply applies the standardization using the current module state.
     """
 
     def __init__(
         self,
         d: int,
-        indices: Optional[List[int]] = None,
+        indices: Optional[Union[List[int], Tensor]] = None,
         batch_shape: torch.Size = torch.Size(),  # noqa: B008
         transform_on_train: bool = True,
         transform_on_eval: bool = True,
         transform_on_fantasize: bool = True,
         reverse: bool = False,
         min_std: float = 1e-8,
     ) -> None:
@@ -688,14 +691,21 @@
         )
         self._coefficient = coefficient.clamp_(min=self.min_std)
 
 
 class Round(InputTransform, Module):
     r"""A discretization transformation for discrete inputs.
 
+    If `approximate=False` (the default), uses PyTorch's `round`.
+
+    If `approximate=True`, a differentiable approximate rounding function is
+    used, with a temperature parameter of `tau`. This method is a piecewise
+    approximation of a rounding function where each piece is a hyperbolic
+    tangent function.
+
     For integers, this will typically be used in conjunction
     with normalization as follows:
 
     In eval() mode (i.e. after training), the inputs pass
     would typically be normalized to the unit cube (e.g. during candidate
     optimization). 1. These are unnormalized back to the raw input space.
     2. The integers are rounded. 3. All values are normalized to the unit
@@ -1533,13 +1543,13 @@
         Args:
             other: Another input transform.
 
         Returns:
             A boolean indicating if the other transform is equivalent.
         """
         return (
-            type(self) == type(other)
+            type(self) is type(other)
             and (self.transform_on_train == other.transform_on_train)
             and (self.transform_on_eval == other.transform_on_eval)
             and (self.transform_on_fantasize == other.transform_on_fantasize)
             and self.categorical_features == other.categorical_features
         )
```

### Comparing `botorch-0.8.5/botorch/models/transforms/outcome.py` & `botorch-0.9.1/botorch/models/transforms/outcome.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,19 @@
     International Conference on Artificial Intelligence and Statistics. PMLR, 2021,
     http://proceedings.mlr.press/v130/eriksson21a.html
 
 """
 
 from __future__ import annotations
 
+import warnings
+
 from abc import ABC, abstractmethod
 from collections import OrderedDict
-from typing import List, Optional, Tuple, Union
+from typing import Any, List, Mapping, Optional, Tuple, Union
 
 import torch
 from botorch.models.transforms.utils import (
     norm_to_lognorm_mean,
     norm_to_lognorm_variance,
 )
 from botorch.posteriors import GPyTorchPosterior, Posterior, TransformedPosterior
@@ -241,22 +243,36 @@
             outputs: Which of the outputs to standardize. If omitted, all
                 outputs will be standardized.
             batch_shape: The batch_shape of the training targets.
             min_stddv: The minimum standard deviation for which to perform
                 standardization (if lower, only de-mean the data).
         """
         super().__init__()
-        self.register_buffer("means", None)
-        self.register_buffer("stdvs", None)
-        self.register_buffer("_stdvs_sq", None)
+        self.register_buffer("means", torch.zeros(*batch_shape, 1, m))
+        self.register_buffer("stdvs", torch.ones(*batch_shape, 1, m))
+        self.register_buffer("_stdvs_sq", torch.ones(*batch_shape, 1, m))
+        self.register_buffer("_is_trained", torch.tensor(False))
         self._outputs = normalize_indices(outputs, d=m)
         self._m = m
         self._batch_shape = batch_shape
         self._min_stdv = min_stdv
 
+    def load_state_dict(
+        self, state_dict: Mapping[str, Any], strict: bool = True
+    ) -> None:
+        r"""Custom logic for loading the state dict."""
+        if "_is_trained" not in state_dict:
+            warnings.warn(
+                "Key '_is_trained' not found in state_dict. Setting to True. "
+                "In a future release, this will result in an error.",
+                DeprecationWarning,
+            )
+            state_dict = {**state_dict, "_is_trained": torch.tensor(True)}
+        super().load_state_dict(state_dict, strict=strict)
+
     def forward(
         self, Y: Tensor, Yvar: Optional[Tensor] = None
     ) -> Tuple[Tensor, Optional[Tensor]]:
         r"""Standardize outcomes.
 
         If the module is in train mode, this updates the module state (i.e. the
         mean/std normalizing constants). If the module is in eval mode, simply
@@ -291,14 +307,15 @@
             if self._outputs is not None:
                 unused = [i for i in range(self._m) if i not in self._outputs]
                 means[..., unused] = 0.0
                 stdvs[..., unused] = 1.0
             self.means = means
             self.stdvs = stdvs
             self._stdvs_sq = stdvs.pow(2)
+            self._is_trained = torch.tensor(True)
 
         Y_tf = (Y - self.means) / self.stdvs
         Yvar_tf = Yvar / self._stdvs_sq if Yvar is not None else None
         return Y_tf, Yvar_tf
 
     def subset_output(self, idcs: List[int]) -> OutcomeTransform:
         r"""Subset the transform along the output dimension.
@@ -321,18 +338,18 @@
             new_outputs = [i for i in self._outputs if i in nlzd_idcs]
         new_tf = self.__class__(
             m=new_m,
             outputs=new_outputs,
             batch_shape=self._batch_shape,
             min_stdv=self._min_stdv,
         )
-        if self.means is not None:
-            new_tf.means = self.means[..., nlzd_idcs]
-            new_tf.stdvs = self.stdvs[..., nlzd_idcs]
-            new_tf._stdvs_sq = self._stdvs_sq[..., nlzd_idcs]
+        new_tf.means = self.means[..., nlzd_idcs]
+        new_tf.stdvs = self.stdvs[..., nlzd_idcs]
+        new_tf._stdvs_sq = self._stdvs_sq[..., nlzd_idcs]
+        new_tf._is_trained = self._is_trained
         if not self.training:
             new_tf.eval()
         return new_tf
 
     def untransform(
         self, Y: Tensor, Yvar: Optional[Tensor] = None
     ) -> Tuple[Tensor, Optional[Tensor]]:
@@ -345,15 +362,15 @@
 
         Returns:
             A two-tuple with the un-standardized outcomes:
 
             - The un-standardized outcome observations.
             - The un-standardized observation noise (if applicable).
         """
-        if self.means is None:
+        if not self._is_trained:
             raise RuntimeError(
                 "`Standardize` transforms must be called on outcome data "
                 "(e.g. `transform(Y)`) before calling `untransform`, since "
                 "means and standard deviations need to be computed."
             )
 
         Y_utf = self.means + self.stdvs * Y
@@ -378,15 +395,15 @@
             `TransformedPosterior`.
         """
         if self._outputs is not None:
             raise NotImplementedError(
                 "Standardize does not yet support output selection for "
                 "untransform_posterior"
             )
-        if self.means is None:
+        if not self._is_trained:
             raise RuntimeError(
                 "`Standardize` transforms must be called on outcome data "
                 "(e.g. `transform(Y)`) before calling `untransform_posterior`, since "
                 "means and standard deviations need to be computed."
             )
         is_mtgp_posterior = False
         if type(posterior) is GPyTorchPosterior:
```

### Comparing `botorch-0.8.5/botorch/models/transforms/utils.py` & `botorch-0.9.1/botorch/models/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/utils/__init__.py` & `botorch-0.9.1/botorch/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/models/utils/assorted.py` & `botorch-0.9.1/botorch/models/utils/assorted.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,16 +189,16 @@
         atol_std: The tolerance for the std check.
         raise_on_fail: If True, raise an exception instead of a warning.
     """
     with torch.no_grad():
         Ymean, Ystd = torch.mean(Y, dim=-2), torch.std(Y, dim=-2)
         if torch.abs(Ymean).max() > atol_mean or torch.abs(Ystd - 1).max() > atol_std:
             msg = (
-                "Input data is not standardized. Please consider scaling the "
-                "input to zero mean and unit variance."
+                f"Input data is not standardized (mean = {Ymean}, std = {Ystd}). "
+                "Please consider scaling the input to zero mean and unit variance."
             )
             if raise_on_fail:
                 raise InputDataError(msg)
             warnings.warn(msg, InputDataWarning)
 
 
 def validate_input_scaling(
```

### Comparing `botorch-0.8.5/botorch/models/utils/inducing_point_allocators.py` & `botorch-0.9.1/botorch/models/utils/inducing_point_allocators.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Union
 
 import torch
+from botorch.exceptions.errors import UnsupportedError
 from botorch.models.model import Model
 
 from botorch.utils.probability.utils import ndtr as Phi, phi
 from gpytorch.module import Module
 from linear_operator.operators import LinearOperator
 from torch import Tensor
 
@@ -70,67 +71,86 @@
 
         Returns:
             A (\*batch_shape, m, d)-dim tensor of inducing point locations.
         """
         quality_function = self._get_quality_function()
         covar_module = covar_module.to(inputs.device)
 
-        train_train_kernel = covar_module(inputs).evaluate_kernel()
+        # We use 'no_grad' here because `inducing_points` are not
+        # auto-differentiable with respect to the kernel hyper-parameters,
+        # because `_pivoted_cholesky_init` does in-place operations.
+        with torch.no_grad():
+            # Evaluate lazily because this may only be needed to figure out what
+            # case we are in
+            possibly_lazy_kernel = covar_module(inputs)
+
+        base_case = possibly_lazy_kernel.ndimension() == 2
+        multi_task_case = (
+            possibly_lazy_kernel.ndimension() == 3 and len(input_batch_shape) == 0
+        )
+
+        if base_case or multi_task_case:
+            train_train_kernel = possibly_lazy_kernel.evaluate_kernel()
 
-        # base case
-        if train_train_kernel.ndimension() == 2:
+        if base_case:
             quality_scores = quality_function(inputs)
             inducing_points = _pivoted_cholesky_init(
                 train_inputs=inputs,
                 kernel_matrix=train_train_kernel,
                 max_length=num_inducing,
                 quality_scores=quality_scores,
             )
-        # multi-task case
-        elif train_train_kernel.ndimension() == 3 and len(input_batch_shape) == 0:
+            return inducing_points
+
+        if multi_task_case:
             input_element = inputs[0] if inputs.ndimension() == 3 else inputs
             kernel_element = train_train_kernel[0]
             quality_scores = quality_function(input_element)
             inducing_points = _pivoted_cholesky_init(
                 train_inputs=input_element,
                 kernel_matrix=kernel_element,
                 max_length=num_inducing,
                 quality_scores=quality_scores,
             )
+            return inducing_points
+
         # batched input cases
-        else:
-            batched_inputs = (
-                inputs.expand(*input_batch_shape, -1, -1)
-                if inputs.ndimension() == 2
-                else inputs
-            )
-            reshaped_inputs = batched_inputs.flatten(end_dim=-3)
-            inducing_points = []
-            for input_element in reshaped_inputs:
-                # the extra kernel evals are a little wasteful but make it
-                # easier to infer the task batch size
+        batched_inputs = (
+            inputs.expand(*input_batch_shape, -1, -1)
+            if inputs.ndimension() == 2
+            else inputs
+        )
+        reshaped_inputs = batched_inputs.flatten(end_dim=-3)
+        inducing_points = []
+        for input_element in reshaped_inputs:
+            # the extra kernel evals are a little wasteful but make it
+            # easier to infer the task batch size
+            # We use 'no_grad' here because `inducing_points` are not
+            # auto-differentiable with respect to the kernel hyper-parameters,
+            # because `_pivoted_cholesky_init` does in-place operations.
+            with torch.no_grad():
                 kernel_element = covar_module(input_element).evaluate_kernel()
-                # handle extra task batch dimension
-                kernel_element = (
-                    kernel_element[0]
-                    if kernel_element.ndimension() == 3
-                    else kernel_element
-                )
-                quality_scores = quality_function(input_element)
-                inducing_points.append(
-                    _pivoted_cholesky_init(
-                        train_inputs=input_element,
-                        kernel_matrix=kernel_element,
-                        max_length=num_inducing,
-                        quality_scores=quality_scores,
-                    )
+            # handle extra task batch dimension
+            kernel_element = (
+                kernel_element[0]
+                if kernel_element.ndimension() == 3
+                else kernel_element
+            )
+            quality_scores = quality_function(input_element)
+            inducing_points.append(
+                _pivoted_cholesky_init(
+                    train_inputs=input_element,
+                    kernel_matrix=kernel_element,
+                    max_length=num_inducing,
+                    quality_scores=quality_scores,
                 )
-            inducing_points = torch.stack(inducing_points).view(
-                *input_batch_shape, num_inducing, -1
             )
+        inducing_points = torch.stack(inducing_points).view(
+            *input_batch_shape, num_inducing, -1
+        )
 
         return inducing_points
 
 
 class QualityFunction(ABC):
     """A function that scores inputs with respect
     to a specific criterion."""
@@ -300,23 +320,28 @@
     # todo test for shape of quality function
 
     if quality_scores.shape[0] != train_inputs.shape[0]:
         raise ValueError(
             "_pivoted_cholesky_init requires a quality score for each of train_inputs"
         )
 
+    if kernel_matrix.requires_grad:
+        raise UnsupportedError(
+            "`_pivoted_cholesky_init` does not support using a `kernel_matrix` "
+            "with `requires_grad=True`."
+        )
+
     item_size = kernel_matrix.shape[-2]
     cis = torch.zeros(
         (max_length, item_size), device=kernel_matrix.device, dtype=kernel_matrix.dtype
     )
     di2s = kernel_matrix.diagonal()
     scores = di2s * torch.square(quality_scores)
-    selected_items = []
     selected_item = torch.argmax(scores)
-    selected_items.append(selected_item)
+    selected_items = [selected_item]
 
     while len(selected_items) < max_length:
         k = len(selected_items) - 1
         ci_optimal = cis[:k, selected_item]
         di_optimal = torch.sqrt(di2s[selected_item])
         elements = kernel_matrix[..., selected_item, :]
         eis = (elements - torch.matmul(ci_optimal, cis[:k, :])) / di_optimal
```

### Comparing `botorch-0.8.5/botorch/models/utils/parse_training_data.py` & `botorch-0.9.1/botorch/models/utils/parse_training_data.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/optim/__init__.py` & `botorch-0.9.1/botorch/optim/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,24 +11,32 @@
 )
 from botorch.optim.core import (
     OptimizationResult,
     OptimizationStatus,
     scipy_minimize,
     torch_minimize,
 )
+from botorch.optim.homotopy import (
+    FixedHomotopySchedule,
+    Homotopy,
+    HomotopyParameter,
+    LinearHomotopySchedule,
+    LogLinearHomotopySchedule,
+)
 from botorch.optim.initializers import initialize_q_batch, initialize_q_batch_nonneg
 from botorch.optim.numpy_converter import module_to_array, set_params_with_array
 from botorch.optim.optimize import (
     gen_batch_initial_conditions,
     optimize_acqf,
     optimize_acqf_cyclic,
     optimize_acqf_discrete,
     optimize_acqf_discrete_local_search,
     optimize_acqf_mixed,
 )
+from botorch.optim.optimize_homotopy import optimize_acqf_homotopy
 from botorch.optim.stopping import ExpMAStoppingCriterion
 
 
 __all__ = [
     "ForwardBackwardClosure",
     "get_loss_closure",
     "get_loss_closure_with_grads",
@@ -38,13 +46,19 @@
     "OptimizationResult",
     "OptimizationStatus",
     "optimize_acqf",
     "optimize_acqf_cyclic",
     "optimize_acqf_discrete",
     "optimize_acqf_discrete_local_search",
     "optimize_acqf_mixed",
+    "optimize_acqf_homotopy",
     "module_to_array",
     "scipy_minimize",
     "set_params_with_array",
     "torch_minimize",
     "ExpMAStoppingCriterion",
+    "FixedHomotopySchedule",
+    "Homotopy",
+    "HomotopyParameter",
+    "LinearHomotopySchedule",
+    "LogLinearHomotopySchedule",
 ]
```

### Comparing `botorch-0.8.5/botorch/optim/closures/__init__.py` & `botorch-0.9.1/botorch/optim/closures/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/optim/closures/core.py` & `botorch-0.9.1/botorch/optim/closures/core.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/optim/closures/model_closures.py` & `botorch-0.9.1/botorch/optim/closures/model_closures.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/optim/core.py` & `botorch-0.9.1/botorch/optim/core.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/optim/fit.py` & `botorch-0.9.1/botorch/optim/fit.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/optim/initializers.py` & `botorch-0.9.1/botorch/optim/initializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,18 +185,18 @@
         n: Number of q-batches to sample.
         q: Number of samples per q-batch
         bounds: A `2 x d` tensor of lower and upper bounds for each column of `X`.
         n_burnin: The number of burn-in samples for the Markov chain sampler.
             thinning: The amount of thinning (number of steps to take between
             returning samples).
         seed: The random seed.
-        inequality constraints: A list of tuples (indices, coefficients, rhs),
+        inequality_constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`.
-        equality constraints: A list of tuples (indices, coefficients, rhs),
+        equality_constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
 
     Returns:
         A `n x q x d`-dim tensor of samples.
     """
```

### Comparing `botorch-0.8.5/botorch/optim/numpy_converter.py` & `botorch-0.9.1/botorch/optim/numpy_converter.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/optim/optimize.py` & `botorch-0.9.1/botorch/optim/optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 Methods for optimizing acquisition functions.
 """
 
 from __future__ import annotations
 
 import dataclasses
 
-import time
 import warnings
 
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import torch
 from botorch.acquisition.acquisition import (
     AcquisitionFunction,
@@ -210,58 +209,56 @@
         raise NotImplementedError(
             "sequential optimization currently not supported for one-shot "
             "acquisition functions. Must have `sequential=False`."
         )
 
 
 def _optimize_acqf_sequential_q(
-    opt_inputs: OptimizeAcqfInputs, timeout_sec: Optional[float], start_time: float
+    opt_inputs: OptimizeAcqfInputs,
 ) -> Tuple[Tensor, Tensor]:
     """
     Helper function for `optimize_acqf` when sequential=True and q > 1.
     """
     _validate_sequential_inputs(opt_inputs)
-    if timeout_sec is not None:
-        # When using sequential optimization, we allocate the total timeout
-        # evenly across the individual acquisition optimizations.
-        timeout_sec = (timeout_sec - start_time) / opt_inputs.q
-
+    # When using sequential optimization, we allocate the total timeout
+    # evenly across the individual acquisition optimizations.
+    timeout_sec = (
+        opt_inputs.timeout_sec / opt_inputs.q
+        if opt_inputs.timeout_sec is not None
+        else None
+    )
     candidate_list, acq_value_list = [], []
     base_X_pending = opt_inputs.acq_function.X_pending
 
     new_inputs = dataclasses.replace(
         opt_inputs,
         q=1,
         batch_initial_conditions=None,
         return_best_only=True,
         sequential=False,
         timeout_sec=timeout_sec,
     )
     for i in range(opt_inputs.q):
 
-        candidate, acq_value = _optimize_acqf_batch(
-            new_inputs, start_time=start_time, timeout_sec=timeout_sec
-        )
+        candidate, acq_value = _optimize_acqf_batch(new_inputs)
 
         candidate_list.append(candidate)
         acq_value_list.append(acq_value)
         candidates = torch.cat(candidate_list, dim=-2)
         new_inputs.acq_function.set_X_pending(
             torch.cat([base_X_pending, candidates], dim=-2)
             if base_X_pending is not None
             else candidates
         )
         logger.info(f"Generated sequential candidate {i+1} of {opt_inputs.q}")
     opt_inputs.acq_function.set_X_pending(base_X_pending)
     return candidates, torch.stack(acq_value_list)
 
 
-def _optimize_acqf_batch(
-    opt_inputs: OptimizeAcqfInputs, start_time: float, timeout_sec: Optional[float]
-) -> Tuple[Tensor, Tensor]:
+def _optimize_acqf_batch(opt_inputs: OptimizeAcqfInputs) -> Tuple[Tensor, Tensor]:
     options = opt_inputs.options or {}
 
     initial_conditions_provided = opt_inputs.batch_initial_conditions is not None
 
     if initial_conditions_provided:
         batch_initial_conditions = opt_inputs.batch_initial_conditions
     else:
@@ -281,52 +278,45 @@
 
     batch_limit: int = options.get(
         "batch_limit",
         opt_inputs.num_restarts
         if not opt_inputs.nonlinear_inequality_constraints
         else 1,
     )
-    has_parameter_constraints = (
-        opt_inputs.inequality_constraints is not None
-        or opt_inputs.equality_constraints is not None
-        or opt_inputs.nonlinear_inequality_constraints is not None
-    )
 
-    def _optimize_batch_candidates(
-        timeout_sec: Optional[float],
-    ) -> Tuple[Tensor, Tensor, List[Warning]]:
+    def _optimize_batch_candidates() -> Tuple[Tensor, Tensor, List[Warning]]:
         batch_candidates_list: List[Tensor] = []
         batch_acq_values_list: List[Tensor] = []
         batched_ics = batch_initial_conditions.split(batch_limit)
         opt_warnings = []
-        if timeout_sec is not None:
-            timeout_sec = (timeout_sec - start_time) / len(batched_ics)
+        timeout_sec = (
+            opt_inputs.timeout_sec / len(batched_ics)
+            if opt_inputs.timeout_sec is not None
+            else None
+        )
 
         bounds = opt_inputs.bounds
         gen_kwargs: Dict[str, Any] = {
             "lower_bounds": None if bounds[0].isinf().all() else bounds[0],
             "upper_bounds": None if bounds[1].isinf().all() else bounds[1],
             "options": {k: v for k, v in options.items() if k not in INIT_OPTION_KEYS},
             "fixed_features": opt_inputs.fixed_features,
             "timeout_sec": timeout_sec,
         }
 
-        if has_parameter_constraints:
-            # only add parameter constraints to gen_kwargs if they are specified
-            # to avoid unnecessary warnings in _filter_kwargs
-            gen_kwargs.update(
-                {
-                    "inequality_constraints": opt_inputs.inequality_constraints,
-                    "equality_constraints": opt_inputs.equality_constraints,
-                    # the line is too long
-                    "nonlinear_inequality_constraints": (
-                        opt_inputs.nonlinear_inequality_constraints
-                    ),
-                }
-            )
+        # only add parameter constraints to gen_kwargs if they are specified
+        # to avoid unnecessary warnings in _filter_kwargs
+        for constraint_name in [
+            "inequality_constraints",
+            "equality_constraints",
+            "nonlinear_inequality_constraints",
+        ]:
+            if (constraint := getattr(opt_inputs, constraint_name)) is not None:
+                gen_kwargs[constraint_name] = constraint
+
         filtered_gen_kwargs = _filter_kwargs(opt_inputs.gen_candidates, **gen_kwargs)
 
         for i, batched_ics_ in enumerate(batched_ics):
             # optimize using random restart optimization
             with warnings.catch_warnings(record=True) as ws:
                 warnings.simplefilter("always", category=OptimizationWarning)
                 (
@@ -344,15 +334,15 @@
         has_scalars = batch_acq_values_list[0].ndim == 0
         if has_scalars:
             batch_acq_values = torch.stack(batch_acq_values_list)
         else:
             batch_acq_values = torch.cat(batch_acq_values_list).flatten()
         return batch_candidates, batch_acq_values, opt_warnings
 
-    batch_candidates, batch_acq_values, ws = _optimize_batch_candidates(timeout_sec)
+    batch_candidates, batch_acq_values, ws = _optimize_batch_candidates()
 
     optimization_warning_raised = any(
         (issubclass(w.category, OptimizationWarning) for w in ws)
     )
     if optimization_warning_raised and opt_inputs.retry_on_optimization_warning:
         first_warn_msg = (
             "Optimization failed in `gen_candidates_scipy` with the following "
@@ -378,30 +368,34 @@
                 fixed_features=opt_inputs.fixed_features,
                 options=options,
                 inequality_constraints=opt_inputs.inequality_constraints,
                 equality_constraints=opt_inputs.equality_constraints,
                 **opt_inputs.ic_gen_kwargs,
             )
 
-            batch_candidates, batch_acq_values, ws = _optimize_batch_candidates(
-                timeout_sec
-            )
+            batch_candidates, batch_acq_values, ws = _optimize_batch_candidates()
 
             optimization_warning_raised = any(
                 (issubclass(w.category, OptimizationWarning) for w in ws)
             )
             if optimization_warning_raised:
                 warnings.warn(
                     "Optimization failed on the second try, after generating a "
                     "new set of initial conditions.",
                     RuntimeWarning,
                 )
 
     if opt_inputs.post_processing_func is not None:
         batch_candidates = opt_inputs.post_processing_func(batch_candidates)
+        with torch.no_grad():
+            acq_values_list = [
+                opt_inputs.acq_function(cand)
+                for cand in batch_candidates.split(batch_limit, dim=0)
+            ]
+            batch_acq_values = torch.cat(acq_values_list, dim=0)
 
     if opt_inputs.return_best_only:
         best = torch.argmax(batch_acq_values.view(-1), dim=0)
         batch_candidates = batch_candidates[best]
         batch_acq_values = batch_acq_values[best]
 
     if not opt_inputs.full_tree:
@@ -446,18 +440,27 @@
         num_restarts: The number of starting points for multistart acquisition
             function optimization.
         raw_samples: The number of samples for initialization. This is required
             if `batch_initial_conditions` is not specified.
         options: Options for candidate generation.
         inequality_constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
-            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`
+            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`. `indices` and
+            `coefficients` should be torch tensors. See the docstring of
+            `make_scipy_linear_constraints` for an example. When q=1, or when
+            applying the same constraint to each candidate in the batch,
+            `indices` should be a 1-d tensor. For inter-point constraints,
+            `indices` must be a 2-d Tensor, where in each row `indices[i] =
+            (k_i, l_i)` the first index `k_i` corresponds to the `k_i`-th
+            element of the `q`-batch and the second index `l_i` corresponds to
+            the `l_i`-th feature of that element.
         equality_constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an equality constraint of the form
-            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`
+            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`. See the docstring of
+            `make_scipy_linear_constraints` for an example.
         nonlinear_inequality_constraints: A list of callables with that represent
             non-linear inequality constraints of the form `callable(x) >= 0`. Each
             callable is expected to take a `(num_restarts) x q x d`-dim tensor as an
             input and return a `(num_restarts) x q`-dim tensor with the constraint
             values. The constraints will later be passed to SLSQP. You need to pass in
             `batch_initial_conditions` in this case. Using non-linear inequality
             constraints also requires that `batch_limit` is set to 1, which will be
@@ -554,29 +557,20 @@
         return _optimize_acqf_all_features_fixed(
             bounds=opt_inputs.bounds,
             fixed_features=opt_inputs.fixed_features,
             q=opt_inputs.q,
             acq_function=opt_inputs.acq_function,
         )
 
-    start_time: float = time.monotonic()
-    timeout_sec = opt_inputs.timeout_sec
-
     # Perform sequential optimization via successive conditioning on pending points
     if opt_inputs.sequential and opt_inputs.q > 1:
-        return _optimize_acqf_sequential_q(
-            opt_inputs=opt_inputs,
-            timeout_sec=timeout_sec,
-            start_time=start_time,
-        )
+        return _optimize_acqf_sequential_q(opt_inputs=opt_inputs)
 
     # Batch optimization (including the case q=1)
-    return _optimize_acqf_batch(
-        opt_inputs=opt_inputs, start_time=start_time, timeout_sec=timeout_sec
-    )
+    return _optimize_acqf_batch(opt_inputs=opt_inputs)
 
 
 def optimize_acqf_cyclic(
     acq_function: AcquisitionFunction,
     bounds: Tensor,
     q: int,
     num_restarts: int,
```

### Comparing `botorch-0.8.5/botorch/optim/parameter_constraints.py` & `botorch-0.9.1/botorch/optim/parameter_constraints.py`

 * *Files 3% similar despite different names*

```diff
@@ -308,21 +308,59 @@
                     eval_lin_constraint, flat_idxr=idxr, coeffs=coeffs, rhs=float(rhs)
                 )
                 jac = partial(lin_constraint_jac, flat_idxr=idxr, coeffs=coeffs, n=n)
                 constraints.append({"type": ctype, "fun": fun, "jac": jac})
     return constraints
 
 
+def _generate_unfixed_nonlin_constraints(
+    constraints: Optional[List[Callable[[Tensor], Tensor]]],
+    fixed_features: Dict[int, float],
+    dimension: int,
+) -> Optional[List[Callable[[Tensor], Tensor]]]:
+    """Given a dictionary of fixed features, returns a list of callables for
+    nonlinear inequality constraints expecting only a tensor with the non-fixed
+    features as input.
+    """
+    if not constraints:
+        return constraints
+
+    selector = []
+    idx_X, idx_f = 0, dimension - len(fixed_features)
+    for i in range(dimension):
+        if i in fixed_features.keys():
+            selector.append(idx_f)
+            idx_f += 1
+        else:
+            selector.append(idx_X)
+            idx_X += 1
+
+    values = torch.tensor(list(fixed_features.values()), dtype=torch.double)
+
+    def _wrap_nonlin_constraint(
+        constraint: Callable[[Tensor], Tensor]
+    ) -> Callable[[Tensor], Tensor]:
+        def new_nonlin_constraint(X: Tensor) -> Tensor:
+            ivalues = values.to(X).expand(*X.shape[:-1], len(fixed_features))
+            X_perm = torch.cat([X, ivalues], dim=-1)
+            return constraint(X_perm[..., selector])
+
+        return new_nonlin_constraint
+
+    return [
+        _wrap_nonlin_constraint(constraint=constraint) for constraint in constraints
+    ]
+
+
 def _generate_unfixed_lin_constraints(
     constraints: Optional[List[Tuple[Tensor, Tensor, float]]],
     fixed_features: Dict[int, float],
     dimension: int,
     eq: bool,
 ) -> Optional[List[Tuple[Tensor, Tensor, float]]]:
-
     # If constraints is None or an empty list, then return itself
     if not constraints:
         return constraints
 
     # replace_index generates the new indices for the unfixed dimensions
     # after eliminating the fixed dimensions.
     # Example: dimension = 5, ff.keys() = [1, 3], replace_index = {0: 0, 2: 1, 4: 2}
```

### Comparing `botorch-0.8.5/botorch/optim/stopping.py` & `botorch-0.9.1/botorch/optim/stopping.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
-import typing  # noqa F401
 from abc import ABC, abstractmethod
 
 import torch
 from torch import Tensor
 
 
 class StoppingCriterion(ABC):
```

### Comparing `botorch-0.8.5/botorch/optim/utils/__init__.py` & `botorch-0.9.1/botorch/optim/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/optim/utils/acquisition_utils.py` & `botorch-0.9.1/botorch/optim/utils/acquisition_utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/optim/utils/common.py` & `botorch-0.9.1/botorch/optim/utils/common.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/optim/utils/model_utils.py` & `botorch-0.9.1/botorch/optim/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/optim/utils/numpy_utils.py` & `botorch-0.9.1/botorch/optim/utils/numpy_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # LICENSE file in the root directory of this source tree.
 
 r"""Utilities for interfacing Numpy and Torch."""
 
 from __future__ import annotations
 
 from itertools import tee
-from math import prod
 from typing import Callable, Dict, Iterator, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from botorch.utils.types import NoneType
 from numpy import ndarray
 from torch import Tensor
@@ -147,22 +146,27 @@
         parameters: A dictionary of parameters.
         bounds: A dictionary of (optional) lower and upper bounds.
 
     Returns:
         An ndarray of bounds.
     """
     inf = float("inf")
-    out = None
+    full_size = sum(param.numel() for param in parameters.values())
+    out = np.full((full_size, 2), (-inf, inf))
     index = 0
     for name, param in parameters.items():
-        size = prod(param.shape)
+        size = param.numel()
         if name in bounds:
             lower, upper = bounds[name]
-            lower = -inf if lower is None else float(lower)
-            upper = inf if upper is None else float(upper)
-            if lower != -inf or upper != inf:
-                if out is None:
-                    full_size = sum(prod(param.shape) for param in parameters.values())
-                    out = np.full((full_size, 2), (-inf, inf))
-                out[index : index + size] = (lower, upper)
+            lower = -inf if lower is None else lower
+            upper = inf if upper is None else upper
+            if isinstance(lower, Tensor):
+                lower = lower.cpu()
+            if isinstance(upper, Tensor):
+                upper = upper.cpu()
+            out[index : index + size, 0] = lower
+            out[index : index + size, 1] = upper
         index = index + size
+    # If all bounds are +/- inf, return None.
+    if np.isinf(out).all():
+        out = None
     return out
```

### Comparing `botorch-0.8.5/botorch/optim/utils/timeout.py` & `botorch-0.9.1/botorch/optim/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/posteriors/__init__.py` & `botorch-0.9.1/botorch/posteriors/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/posteriors/base_samples.py` & `botorch-0.9.1/botorch/posteriors/base_samples.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/posteriors/deterministic.py` & `botorch-0.9.1/botorch/posteriors/deterministic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/posteriors/ensemble.py` & `botorch-0.9.1/botorch/posteriors/ensemble.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/posteriors/fully_bayesian.py` & `botorch-0.9.1/botorch/posteriors/fully_bayesian.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+from __future__ import annotations
 
-from functools import lru_cache
 from typing import Callable, Optional, Tuple
 
 import torch
 from botorch.posteriors.gpytorch import GPyTorchPosterior
 from gpytorch.distributions import MultivariateNormal
 from torch import Tensor
 
@@ -50,14 +50,38 @@
         f_center = f(center)
         # Check convergence
         if (f_center - target).abs().max() <= tol:
             return center
     return center
 
 
+def _quantile(posterior: FullyBayesianPosterior, value: Tensor) -> Tensor:
+    r"""Compute the posterior quantiles for the mixture of models."""
+    if value.numel() > 1:
+        return torch.stack(
+            [_quantile(posterior=posterior, value=v) for v in value], dim=0
+        )
+    if value <= 0 or value >= 1:
+        raise ValueError("value is expected to be in the range (0, 1).")
+    dist = torch.distributions.Normal(
+        loc=posterior.mean, scale=posterior.variance.sqrt()
+    )
+    if posterior.mean.shape[MCMC_DIM] == 1:  # Analytical solution
+        return dist.icdf(value).squeeze(MCMC_DIM)
+    icdf_val = dist.icdf(value)
+    low = icdf_val.min(dim=MCMC_DIM).values - TOL
+    high = icdf_val.max(dim=MCMC_DIM).values + TOL
+    bounds = torch.cat((low.unsqueeze(0), high.unsqueeze(0)), dim=0)
+    return batched_bisect(
+        f=lambda x: dist.cdf(x.unsqueeze(MCMC_DIM)).mean(dim=MCMC_DIM),
+        target=value.item(),
+        bounds=bounds,
+    )
+
+
 class FullyBayesianPosterior(GPyTorchPosterior):
     r"""A posterior for a fully Bayesian model.
 
     The MCMC batch dimension that corresponds to the models in the mixture is located
     at `MCMC_DIM` (defined at the top of this file). Note that while each MCMC sample
     corresponds to a Gaussian posterior, the fully Bayesian posterior is rather a
     mixture of Gaussian distributions.
@@ -78,38 +102,14 @@
             if self._is_mt
             else distribution.variance.unsqueeze(-1)
         )
 
         self._mixture_mean: Optional[Tensor] = None
         self._mixture_variance: Optional[Tensor] = None
 
-        # using lru_cache on methods can cause memory leaks. See flake8 B019
-        # So we define a function here instead, to be called by self.quantile
-        @lru_cache
-        def _quantile(value: Tensor) -> Tensor:
-            r"""Compute the posterior quantiles for the mixture of models."""
-            if value.numel() > 1:
-                return torch.stack([self.quantile(v) for v in value], dim=0)
-            if value <= 0 or value >= 1:
-                raise ValueError("value is expected to be in the range (0, 1).")
-            dist = torch.distributions.Normal(loc=self.mean, scale=self.variance.sqrt())
-            if self.mean.shape[MCMC_DIM] == 1:  # Analytical solution
-                return dist.icdf(value).squeeze(MCMC_DIM)
-            icdf_val = dist.icdf(value)
-            low = icdf_val.min(dim=MCMC_DIM).values - TOL
-            high = icdf_val.max(dim=MCMC_DIM).values + TOL
-            bounds = torch.cat((low.unsqueeze(0), high.unsqueeze(0)), dim=0)
-            return batched_bisect(
-                f=lambda x: dist.cdf(x.unsqueeze(MCMC_DIM)).mean(dim=MCMC_DIM),
-                target=value.item(),
-                bounds=bounds,
-            )
-
-        self._quantile = _quantile
-
     @property
     def mixture_mean(self) -> Tensor:
         r"""The posterior mean for the mixture of models."""
         if self._mixture_mean is None:
             self._mixture_mean = self._mean.mean(dim=MCMC_DIM)
         return self._mixture_mean
 
@@ -122,15 +122,15 @@
             t2 = self._mean.pow(2).sum(dim=MCMC_DIM) / num_mcmc_samples
             t3 = -(self._mean.sum(dim=MCMC_DIM) / num_mcmc_samples).pow(2)
             self._mixture_variance = t1 + t2 + t3
         return self._mixture_variance
 
     def quantile(self, value: Tensor) -> Tensor:
         r"""Compute the posterior quantiles for the mixture of models."""
-        return self._quantile(value)
+        return _quantile(posterior=self, value=value)
 
     @property
     def batch_range(self) -> Tuple[int, int]:
         r"""The t-batch range.
 
         This is used in samplers to identify the t-batch component of the
         `base_sample_shape`. The base samples are expanded over the t-batches to
```

### Comparing `botorch-0.8.5/botorch/posteriors/gpytorch.py` & `botorch-0.9.1/botorch/posteriors/gpytorch.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/posteriors/higher_order.py` & `botorch-0.9.1/botorch/posteriors/higher_order.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/posteriors/multitask.py` & `botorch-0.9.1/botorch/posteriors/multitask.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/posteriors/posterior.py` & `botorch-0.9.1/botorch/posteriors/posterior.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/posteriors/posterior_list.py` & `botorch-0.9.1/botorch/posteriors/posterior_list.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/posteriors/torch.py` & `botorch-0.9.1/botorch/posteriors/torch.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/posteriors/transformed.py` & `botorch-0.9.1/botorch/posteriors/transformed.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/__init__.py` & `botorch-0.9.1/botorch/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/base.py` & `botorch-0.9.1/botorch/sampling/base.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/deterministic.py` & `botorch-0.9.1/botorch/sampling/deterministic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/get_sampler.py` & `botorch-0.9.1/botorch/sampling/get_sampler.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/index_sampler.py` & `botorch-0.9.1/botorch/sampling/index_sampler.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/list_sampler.py` & `botorch-0.9.1/botorch/sampling/list_sampler.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/normal.py` & `botorch-0.9.1/botorch/sampling/normal.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             self.to(dtype=posterior.dtype)
 
 
 class SobolQMCNormalSampler(NormalMCSampler):
     r"""Sampler for quasi-MC N(0,1) base samples using Sobol sequences.
 
     Example:
-        >>> sampler = SobolQMCNormalSampler(1024, seed=1234)
+        >>> sampler = SobolQMCNormalSampler(torch.Size([1024]), seed=1234)
         >>> posterior = model.posterior(test_X)
         >>> samples = sampler(posterior)
     """
 
     def _construct_base_samples(self, posterior: Posterior) -> None:
         r"""Generate quasi-random Normal base samples (if necessary).
```

### Comparing `botorch-0.8.5/botorch/sampling/pairwise_samplers.py` & `botorch-0.9.1/botorch/sampling/pairwise_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/pathwise/__init__.py` & `botorch-0.9.1/botorch/sampling/pathwise/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/pathwise/features/__init__.py` & `botorch-0.9.1/botorch/sampling/pathwise/features/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/pathwise/features/generators.py` & `botorch-0.9.1/botorch/sampling/pathwise/features/generators.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/pathwise/features/maps.py` & `botorch-0.9.1/botorch/sampling/pathwise/features/maps.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,14 +105,16 @@
             weight: A tensor of weights used to linearly combine the module's inputs.
             bias: A tensor of biases to be added to the linearly combined inputs.
             input_transform: An optional input transform for the module.
             output_transform: An optional output transform for the module.
         """
         super().__init__()
         self.kernel = kernel
+        self.register_buffer("weight", weight)
+        self.register_buffer("bias", bias)
         self.weight = weight
         self.bias = bias
         self.input_transform = input_transform
         self.output_transform = output_transform
 
     def forward(self, x: Tensor) -> Tensor:
         out = x @ self.weight.transpose(-2, -1)
```

### Comparing `botorch-0.8.5/botorch/sampling/pathwise/paths.py` & `botorch-0.9.1/botorch/sampling/pathwise/paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,16 @@
             weight: A tensor of weights used to combine input features.
             bias_module: An optional module used to define additive offsets.
             input_transform: An optional input transform for the module.
             output_transform: An optional output transform for the module.
         """
         super().__init__()
         self.feature_map = feature_map
+        if not isinstance(weight, Parameter):
+            self.register_buffer("weight", weight)
         self.weight = weight
         self.bias_module = bias_module
         self.input_transform = input_transform
         self.output_transform = output_transform
 
     def forward(self, x: Tensor, **kwargs) -> Tensor:
         feat = self.feature_map(x, **kwargs)
```

### Comparing `botorch-0.8.5/botorch/sampling/pathwise/posterior_samplers.py` & `botorch-0.9.1/botorch/sampling/pathwise/posterior_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/pathwise/prior_samplers.py` & `botorch-0.9.1/botorch/sampling/pathwise/prior_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/pathwise/update_strategies.py` & `botorch-0.9.1/botorch/sampling/pathwise/update_strategies.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/pathwise/utils.py` & `botorch-0.9.1/botorch/sampling/pathwise/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/qmc.py` & `botorch-0.9.1/botorch/sampling/qmc.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/sampling/stochastic_samplers.py` & `botorch-0.9.1/botorch/sampling/stochastic_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/settings.py` & `botorch-0.9.1/botorch/settings.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/test_functions/__init__.py` & `botorch-0.9.1/botorch/test_functions/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,21 +50,25 @@
     EggHolder,
     Griewank,
     Hartmann,
     HolderTable,
     Levy,
     Michalewicz,
     Powell,
+    PressureVessel,
     Rastrigin,
     Rosenbrock,
     Shekel,
     SixHumpCamel,
+    SpeedReducer,
     StyblinskiTang,
     SyntheticTestFunction,
+    TensionCompressionString,
     ThreeHumpCamel,
+    WeldedBeamSO,
 )
 
 
 __all__ = [
     "Ackley",
     "AugmentedBranin",
     "AugmentedHartmann",
@@ -95,24 +99,28 @@
     "HolderTable",
     "Levy",
     "Michalewicz",
     "MW7",
     "OSY",
     "Penicillin",
     "Powell",
+    "PressureVessel",
     "Rastrigin",
     "Rosenbrock",
     "Shekel",
     "SixHumpCamel",
+    "SpeedReducer",
     "SRN",
     "StyblinskiTang",
     "SyntheticTestFunction",
+    "TensionCompressionString",
     "ThreeHumpCamel",
     "ToyRobust",
     "VehicleSafety",
     "WeldedBeam",
+    "WeldedBeamSO",
     "ZDT1",
     "ZDT2",
     "ZDT3",
     "MOMFBraninCurrin",
     "MOMFPark",
 ]
```

### Comparing `botorch-0.8.5/botorch/test_functions/base.py` & `botorch-0.9.1/botorch/test_functions/base.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/test_functions/multi_fidelity.py` & `botorch-0.9.1/botorch/test_functions/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/test_functions/multi_objective.py` & `botorch-0.9.1/botorch/test_functions/multi_objective.py`

 * *Files 3% similar despite different names*

```diff
@@ -1440,15 +1440,18 @@
         c1 = 225.0 - ((X**2) ** 2).sum(dim=-1)
         c2 = -10.0 - X[..., 0] + 3 * X[..., 1]
         return torch.stack([c1, c2], dim=-1)
 
 
 class WeldedBeam(MultiObjectiveTestProblem, ConstrainedBaseTestProblem):
     r"""
-    The Welded Beam test problem.
+    The Welded Beam multi-objective test problem. Similar to `WeldedBeamSO` in
+    `botorch.test_function.synthetic`, but with an additional output, somewhat
+    modified constraints, and a different domain.
+
     Implementation from
     https://github.com/msu-coinlab/pymoo/blob/master/pymoo/problems/multi/welded_beam.py
     Note that this implementation assumes minimization, so please choose negate=True.
     """
 
     dim = 4
     num_constraints = 4
@@ -1458,39 +1461,48 @@
         (0.1, 10.0),
         (0.1, 10.0),
         (0.125, 5.0),
     ]
     _ref_point = [40, 0.015]
 
     def evaluate_true(self, X: Tensor) -> Tensor:
-        f1 = 1.10471 * X[..., 0] ** 2 * X[..., 1] + 0.04811 * X[..., 2] * X[..., 3] * (
-            14.0 + X[..., 1]
-        )
-        f2 = 2.1952 / (X[..., 3] * X[..., 2] ** 3)
+        # We could do the following, but the constraints are using somewhat
+        # different numbers (see below).
+        # f1 = WeldedBeam.evaluate_true(self, X)
+        x1, x2, x3, x4 = X.unbind(-1)
+        f1 = 1.10471 * (x1**2) * x2 + 0.04811 * x3 * x4 * (14.0 + x2)
+        f2 = 2.1952 / (x4 * x3**3)
         return torch.stack([f1, f2], dim=-1)
 
     def evaluate_slack_true(self, X: Tensor) -> Tensor:
-        P = 6000
-        L = 14
-        t_max = 13600
-        s_max = 30000
-
-        R = torch.sqrt(0.25 * (X[..., 1] ** 2 + (X[..., 0] + X[..., 2]) ** 2))
-        M = P * (L + X[..., 1] / 2)
-        J = (
-            2
-            * math.sqrt(0.5)
-            * X[..., 0]
-            * X[..., 1]
-            * (X[..., 1] ** 2 / 12 + 0.25 * (X[..., 0] + X[..., 2]) ** 2)
-        )
-        t1 = P / (math.sqrt(2) * X[..., 0] * X[..., 1])
+        x1, x2, x3, x4 = X.unbind(-1)
+        P = 6000.0
+        L = 14.0
+        t_max = 13600.0
+        s_max = 30000.0
+
+        # Ideally, we could just do the following, but the numbers in the
+        # single-outcome WeldedBeam are different (see below)
+        # g1_, g2_, g3_, _, _, g6_ = WeldedBeam.evaluate_slack_true(self, X)
+        # g1 = g1_ / t_max
+        # g2 = g2_ / s_max
+        # g3 = 1 / (5 - 0.125) * g3_
+        # g4 = 1 / P * g6_
+
+        R = torch.sqrt(0.25 * (x2**2 + (x1 + x3) ** 2))
+        M = P * (L + x2 / 2)
+        # This `J` is different than the one in [CoelloCoello2002constraint]_
+        # by a factor of 2 (sqrt(2) instead of sqrt(0.5))
+        J = 2 * math.sqrt(0.5) * x1 * x2 * (x2**2 / 12 + 0.25 * (x1 + x3) ** 2)
+        t1 = P / (math.sqrt(2) * x1 * x2)
         t2 = M * R / J
-        t = torch.sqrt(t1**2 + t2**2 + t1 * t2 * X[..., 1] / R)
-        s = 6 * P * L / (X[..., 3] * X[..., 2] ** 2)
-        P_c = 64746.022 * (1 - 0.0282346 * X[..., 2]) * X[..., 2] * X[..., 3] ** 3
-
-        g1 = (1 / t_max) * (t - t_max)
-        g2 = (1 / s_max) * (s - s_max)
-        g3 = (1 / (5 - 0.125)) * (X[..., 0] - X[..., 3])
-        g4 = (1 / P) * (P - P_c)
-        return -torch.stack([g1, g2, g3, g4], dim=-1)
+        t = torch.sqrt(t1**2 + t1 * t2 * x2 / R + t2**2)
+        s = 6 * P * L / (x4 * x3**2)
+        # These numbers are also different from [CoelloCoello2002constraint]_
+        P_c = 64746.022 * (1 - 0.0282346 * x3) * x3 * x4**3
+
+        g1 = (t - t_max) / t_max
+        g2 = (s - s_max) / s_max
+        g3 = 1 / (5 - 0.125) * (x1 - x4)
+        g4 = (P - P_c) / P
+
+        return torch.stack([g1, g2, g3, g4], dim=-1)
```

### Comparing `botorch-0.8.5/botorch/test_functions/multi_objective_multi_fidelity.py` & `botorch-0.9.1/botorch/test_functions/multi_objective_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/test_functions/sensitivity_analysis.py` & `botorch-0.9.1/botorch/test_functions/sensitivity_analysis.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/__init__.py` & `botorch-0.9.1/botorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/constants.py` & `botorch-0.9.1/botorch/utils/constants.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/containers.py` & `botorch-0.9.1/botorch/utils/containers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/context_managers.py` & `botorch-0.9.1/botorch/utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/datasets.py` & `botorch-0.9.1/botorch/utils/datasets.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,36 +33,37 @@
 
 
 class SupervisedDatasetMeta(type):
     def __call__(cls, *args: Any, **kwargs: Any):
         r"""Converts Tensor-valued fields to DenseContainer under the assumption
         that said fields house collections of feature vectors."""
         hints = get_type_hints(cls)
-        f_iter = filter(lambda f: f.init, fields(cls))
+        fields_iter = (item for item in fields(cls) if item.init is not None)
         f_dict = {}
-        for obj, f in chain(
-            zip(args, f_iter), ((kwargs.pop(f.name, MISSING), f) for f in f_iter)
+        for value, field in chain(
+            zip(args, fields_iter),
+            ((kwargs.pop(field.name, MISSING), field) for field in fields_iter),
         ):
-            if obj is MISSING:
-                if f.default is not MISSING:
-                    obj = f.default
-                elif f.default_factory is not MISSING:
-                    obj = f.default_factory()
+            if value is MISSING:
+                if field.default is not MISSING:
+                    value = field.default
+                elif field.default_factory is not MISSING:
+                    value = field.default_factory()
                 else:
-                    raise RuntimeError(f"Missing required field `{f.name}`.")
+                    raise RuntimeError(f"Missing required field `{field.name}`.")
 
-            if issubclass(hints[f.name], BotorchContainer):
-                if isinstance(obj, Tensor):
-                    obj = DenseContainer(obj, event_shape=obj.shape[-1:])
-                elif not isinstance(obj, BotorchContainer):
+            if issubclass(hints[field.name], BotorchContainer):
+                if isinstance(value, Tensor):
+                    value = DenseContainer(value, event_shape=value.shape[-1:])
+                elif not isinstance(value, BotorchContainer):
                     raise TypeError(
-                        f"Expected <BotorchContainer | Tensor> for field `{f.name}` "
-                        f"but was {type(obj)}."
+                        "Expected <BotorchContainer | Tensor> for field "
+                        f"`{field.name}` but was {type(value)}."
                     )
-            f_dict[f.name] = obj
+            f_dict[field.name] = value
 
         return super().__call__(**f_dict, **kwargs)
 
 
 @dataclass
 class SupervisedDataset(BotorchDataset, metaclass=SupervisedDatasetMeta):
     r"""Base class for datasets consisting of labelled pairs `(x, y)`.
```

### Comparing `botorch-0.8.5/botorch/utils/dispatcher.py` & `botorch-0.9.1/botorch/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/feasible_volume.py` & `botorch-0.9.1/botorch/utils/feasible_volume.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/gp_sampling.py` & `botorch-0.9.1/botorch/utils/gp_sampling.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/low_rank.py` & `botorch-0.9.1/botorch/utils/low_rank.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/multi_objective/__init__.py` & `botorch-0.9.1/botorch/utils/multi_objective/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/__init__.py` & `botorch-0.9.1/botorch/utils/multi_objective/box_decompositions/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/box_decomposition.py` & `botorch-0.9.1/botorch/utils/multi_objective/box_decompositions/box_decomposition.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
             sort: A boolean indicating whether to sort the Pareto frontier.
             Y: A `(batch_shape) x n x m`-dim tensor of outcomes.
         """
         super().__init__()
         self._neg_ref_point = -ref_point
         self.sort = torch.tensor(sort, dtype=torch.bool)
         self.num_outcomes = ref_point.shape[-1]
+        self.register_buffer("hypercell_bounds", None)
 
         if Y is not None:
             if Y.isnan().any():
                 raise ValueError(
                     "NaN inputs are not supported. Got Y with "
                     f"{Y.isnan().sum()} NaN values."
                 )
```

### Comparing `botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py` & `botorch-0.9.1/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/dominated.py` & `botorch-0.9.1/botorch/utils/multi_objective/box_decompositions/dominated.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def _get_partitioning(self) -> None:
         r"""Get the bounds of each hypercell in the decomposition."""
         minimization_cell_bounds = get_partition_bounds(
             Z=self._Z, U=self._U, ref_point=self._neg_ref_point.view(-1)
         )
         cell_bounds = -minimization_cell_bounds.flip(0)
-        self.register_buffer("hypercell_bounds", cell_bounds)
+        self.hypercell_bounds = cell_bounds
 
     def _compute_hypervolume_if_y_has_data(self) -> Tensor:
         r"""Compute hypervolume that is dominated by the Pareto Frontier.
 
         Returns:
             A `(batch_shape)`-dim tensor containing the hypervolume dominated by
                 each Pareto frontier.
```

### Comparing `botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/non_dominated.py` & `botorch-0.9.1/botorch/utils/multi_objective/box_decompositions/non_dominated.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/multi_objective/box_decompositions/utils.py` & `botorch-0.9.1/botorch/utils/multi_objective/box_decompositions/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/multi_objective/hypervolume.py` & `botorch-0.9.1/botorch/utils/multi_objective/hypervolume.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/multi_objective/pareto.py` & `botorch-0.9.1/botorch/utils/multi_objective/pareto.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/multi_objective/scalarization.py` & `botorch-0.9.1/botorch/utils/multi_objective/scalarization.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/objective.py` & `botorch-0.9.1/botorch/utils/objective.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 
 r"""
 Helpers for handling objectives.
 """
 
 from __future__ import annotations
 
+import warnings
+
 from typing import Callable, List, Optional, Union
 
 import torch
+from botorch.utils.safe_math import log_fatmoid, logexpit
 from torch import Tensor
 
 
 def get_objective_weights_transform(
     weights: Optional[Tensor],
 ) -> Callable[[Tensor, Optional[Tensor]], Tensor]:
     r"""Create a linear objective callable from a set of weights.
@@ -83,30 +86,93 @@
             constraint in constraints. In case of a tensor the length of the tensor
             must match the number of provided constraints. The i-th constraint is
             then estimated with the i-th eta value.
 
     Returns:
         A `n_samples x b x q (x m')`-dim tensor of feasibility-weighted objectives.
     """
-    if type(eta) != Tensor:
+    w = compute_smoothed_feasibility_indicator(
+        constraints=constraints, samples=samples, eta=eta
+    )
+    if obj.dim() == samples.dim():
+        w = w.unsqueeze(-1)  # Need to unsqueeze to accommodate the outcome dimension.
+    return obj.clamp_min(0).mul(w)  # Enforce non-negativity of obj, apply constraints.
+
+
+def compute_feasibility_indicator(
+    constraints: Optional[List[Callable[[Tensor], Tensor]]],
+    samples: Tensor,
+) -> Tensor:
+    r"""Computes the feasibility of a list of constraints given posterior samples.
+
+    Args:
+        constraints: A list of callables, each mapping a batch_shape x q x m`-dim Tensor
+            to a `batch_shape x q`-dim Tensor, where negative values imply feasibility.
+        samples: A batch_shape x q x m`-dim Tensor of posterior samples.
+
+    Returns:
+        A `batch_shape x q`-dim tensor of Boolean feasibility values.
+    """
+    ind = torch.ones(samples.shape[:-1], dtype=torch.bool, device=samples.device)
+    if constraints is not None:
+        for constraint in constraints:
+            ind = ind.logical_and(constraint(samples) < 0)
+    return ind
+
+
+def compute_smoothed_feasibility_indicator(
+    constraints: List[Callable[[Tensor], Tensor]],
+    samples: Tensor,
+    eta: Union[Tensor, float],
+    log: bool = False,
+    fat: bool = False,
+) -> Tensor:
+    r"""Computes the smoothed feasibility indicator of a list of constraints.
+
+    Given posterior samples, using a sigmoid to smoothly approximate the feasibility
+    indicator of each individual constraint to ensure differentiability and high
+    gradient signal. The `fat` and `log` options improve the numerical behavior of
+    the smooth approximation.
+
+    NOTE: *Negative* constraint values are associated with feasibility.
+
+    Args:
+        constraints: A list of callables, each mapping a Tensor of size `b x q x m`
+            to a Tensor of size `b x q`, where negative values imply feasibility.
+            This callable must support broadcasting. Only relevant for multi-
+            output models (`m` > 1).
+        samples: A `n_samples x b x q x m` Tensor of samples drawn from the posterior.
+        eta: The temperature parameter for the sigmoid function. Can be either a float
+            or a 1-dim tensor. In case of a float the same eta is used for every
+            constraint in constraints. In case of a tensor the length of the tensor
+            must match the number of provided constraints. The i-th constraint is
+            then estimated with the i-th eta value.
+        log: Toggles the computation of the log-feasibility indicator.
+        fat: Toggles the computation of the fat-tailed feasibility indicator.
+
+    Returns:
+        A `n_samples x b x q`-dim tensor of feasibility indicator values.
+    """
+    if type(eta) is not Tensor:
         eta = torch.full((len(constraints),), eta)
     if len(eta) != len(constraints):
         raise ValueError(
             "Number of provided constraints and number of provided etas do not match."
         )
-    obj = obj.clamp_min(0)  # Enforce non-negativity with constraints
+    if not (eta > 0).all():
+        raise ValueError("eta must be positive.")
+    is_feasible = torch.zeros_like(samples[..., 0])
+    log_sigmoid = log_fatmoid if fat else logexpit
     for constraint, e in zip(constraints, eta):
-        constraint_eval = soft_eval_constraint(constraint(samples), eta=e)
-        if obj.dim() == samples.dim():
-            # Need to unsqueeze to accommodate the outcome dimension.
-            constraint_eval = constraint_eval.unsqueeze(-1)
-        obj = obj.mul(constraint_eval)
-    return obj
+        is_feasible = is_feasible + log_sigmoid(-constraint(samples) / e)
 
+    return is_feasible if log else is_feasible.exp()
 
+
+# TODO: deprecate this function
 def soft_eval_constraint(lhs: Tensor, eta: float = 1e-3) -> Tensor:
     r"""Element-wise evaluation of a constraint in a 'soft' fashion
 
     `value(x) = 1 / (1 + exp(x / eta))`
 
     Args:
         lhs: The left hand side of the constraint `lhs <= 0`.
@@ -114,16 +180,21 @@
             decreases, this approximates the Heaviside step function.
 
     Returns:
         Element-wise 'soft' feasibility indicator of the same shape as `lhs`.
         For each element `x`, `value(x) -> 0` as `x` becomes positive, and
         `value(x) -> 1` as x becomes negative.
     """
+    warnings.warn(
+        "`soft_eval_constraint` is deprecated. Please consider `torch.utils.sigmoid` "
+        + "with its `fat` and `log` options to compute feasibility indicators.",
+        DeprecationWarning,
+    )
     if eta <= 0:
-        raise ValueError("eta must be positive")
+        raise ValueError("eta must be positive.")
     return torch.sigmoid(-lhs / eta)
 
 
 def apply_constraints(
     obj: Tensor,
     constraints: List[Callable[[Tensor], Tensor]],
     samples: Tensor,
@@ -154,10 +225,13 @@
 
     Returns:
         A `n_samples x b x q (x m')`-dim tensor of feasibility-weighted objectives.
     """
     # obj has dimensions n_samples x b x q (x m')
     obj = obj.add(infeasible_cost)  # now it is nonnegative
     obj = apply_constraints_nonnegative_soft(
-        obj=obj, constraints=constraints, samples=samples, eta=eta
+        obj=obj,
+        constraints=constraints,
+        samples=samples,
+        eta=eta,
     )
     return obj.add(-infeasible_cost)
```

### Comparing `botorch-0.8.5/botorch/utils/probability/__init__.py` & `botorch-0.9.1/botorch/utils/probability/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/probability/bvn.py` & `botorch-0.9.1/botorch/utils/probability/bvn.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/probability/lin_ess.py` & `botorch-0.9.1/botorch/utils/probability/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,305 +1,327 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-r"""Linear Elliptical Slice Sampler.
+from __future__ import annotations
 
-References
+import math
 
-.. [Gessner2020]
-    A. Gessner, O. Kanjilal, and P. Hennig. Integrals over gaussians under
-    linear domain constraints. AISTATS 2020.
+from functools import lru_cache
+from math import pi
+from numbers import Number
+from typing import Any, Callable, Iterable, Iterator, Optional, Tuple, Union
 
+import torch
+from botorch.utils.safe_math import logdiffexp
+from numpy.polynomial.legendre import leggauss as numpy_leggauss
+from torch import BoolTensor, LongTensor, Tensor
+
+CaseNd = Tuple[Callable[[], BoolTensor], Callable[[BoolTensor], Tensor]]
+
+_log_2 = math.log(2)
+_sqrt_pi = math.sqrt(pi)
+_inv_sqrt_pi = 1 / _sqrt_pi
+_inv_sqrt_2pi = 1 / math.sqrt(2 * pi)
+_inv_sqrt_2 = 1 / math.sqrt(2)
+_neg_inv_sqrt_2 = -_inv_sqrt_2
+_log_sqrt_2pi = math.log(2 * pi) / 2
+STANDARDIZED_RANGE: Tuple[float, float] = (-1e6, 1e6)
+_log_two_inv_sqrt_2pi = _log_2 - _log_sqrt_2pi  # = log(2 / sqrt(2 * pi))
+
+
+def case_dispatcher(
+    out: Tensor,
+    cases: Iterable[CaseNd] = (),
+    default: Callable[[BoolTensor], Tensor] = None,
+) -> Tensor:
+    r"""Basic implementation of a tensorized switching case statement.
+
+    Args:
+        out: Tensor to which case outcomes are written.
+        cases: Iterable of function pairs (pred, func), where `mask=pred()` specifies
+            whether `func` is applicable for each entry in `out`. Note that cases are
+            resolved first-come, first-serve.
+        default: Optional `func` to which all unclaimed entries of `out` are dispatched.
+    """
+    active = None
+    for closure, func in cases:
+        pred = closure()
+        if not pred.any():
+            continue
 
-This implementation is based (with multiple changes / optimiations) on
-the following implementations based on the algorithm in [Gessner2020]_:
-https://github.com/alpiges/LinConGauss
-https://github.com/wjmaddox/pytorch_ess
-"""
+        mask = pred if (active is None) else pred & active
+        if not mask.any():
+            continue
 
-from __future__ import annotations
+        if mask.all():  # where possible, use Ellipsis to avoid indexing
+            out[...] = func(...)
+            return out
 
-import math
-from typing import Optional, Tuple
+        out[mask] = func(mask)
+        if active is None:
+            active = ~mask
+        else:
+            active[mask] = False
 
-import torch
-from botorch.utils.sampling import PolytopeSampler
-from torch import Tensor
+        if not active.any():
+            break
 
-_twopi = 2.0 * math.pi
-_delta_theta = 1.0e-6 * _twopi
+    if default is not None:
+        if active is None:
+            out[...] = default(...)
+        elif active.any():
+            out[active] = default(active)
 
+    return out
 
-class LinearEllipticalSliceSampler(PolytopeSampler):
-    r"""Linear Elliptical Slice Sampler.
 
-    TODOs:
-    - clean up docstrings
-    - optimize computations (if possible)
+@lru_cache(maxsize=None)
+def get_constants(
+    values: Union[Number, Iterator[Number]],
+    device: Optional[torch.device] = None,
+    dtype: Optional[torch.dtype] = None,
+) -> Union[Tensor, Tuple[Tensor, ...]]:
+    r"""Returns scalar-valued Tensors containing each of the given constants.
+    Used to expedite tensor operations involving scalar arithmetic. Note that
+    the returned Tensors should not be modified in-place."""
+    if isinstance(values, Number):
+        return torch.full((), values, dtype=dtype, device=device)
 
-    Maybe TODOs:
-    - Support degenerate domains (with zero volume)?
-    - Add batch support ?
-    """
+    return tuple(torch.full((), val, dtype=dtype, device=device) for val in values)
+
+
+def get_constants_like(
+    values: Union[Number, Iterator[Number]],
+    ref: Tensor,
+) -> Union[Tensor, Iterator[Tensor]]:
+    return get_constants(values, device=ref.device, dtype=ref.dtype)
+
+
+def gen_positional_indices(
+    shape: torch.Size,
+    dim: int,
+    device: Optional[torch.device] = None,
+) -> Iterator[torch.LongTensor]:
+    ndim = len(shape)
+    _dim = ndim + dim if dim < 0 else dim
+    if _dim >= ndim or _dim < 0:
+        raise ValueError(f"dim={dim} invalid for shape {shape}.")
+
+    cumsize = shape[_dim + 1 :].numel()
+    for i, s in enumerate(reversed(shape[: _dim + 1])):
+        yield torch.arange(0, s * cumsize, cumsize, device=device)[(...,) + i * (None,)]
+        cumsize *= s
+
+
+def build_positional_indices(
+    shape: torch.Size,
+    dim: int,
+    device: Optional[torch.device] = None,
+) -> LongTensor:
+    return sum(gen_positional_indices(shape=shape, dim=dim, device=device))
+
+
+@lru_cache(maxsize=None)
+def leggauss(deg: int, **tkwargs: Any) -> Tuple[Tensor, Tensor]:
+    x, w = numpy_leggauss(deg)
+    return torch.as_tensor(x, **tkwargs), torch.as_tensor(w, **tkwargs)
+
+
+def ndtr(x: Tensor) -> Tensor:
+    r"""Standard normal CDF."""
+    half, neg_inv_sqrt_2 = get_constants_like((0.5, _neg_inv_sqrt_2), x)
+    return half * torch.erfc(neg_inv_sqrt_2 * x)
+
+
+def phi(x: Tensor) -> Tensor:
+    r"""Standard normal PDF."""
+    inv_sqrt_2pi, neg_half = get_constants_like((_inv_sqrt_2pi, -0.5), x)
+    return inv_sqrt_2pi * (neg_half * x.square()).exp()
+
+
+def log_phi(x: Tensor) -> Tensor:
+    r"""Logarithm of standard normal pdf"""
+    log_sqrt_2pi, neg_half = get_constants_like((_log_sqrt_2pi, -0.5), x)
+    return neg_half * x.square() - log_sqrt_2pi
 
-    def __init__(
-        self,
-        inequality_constraints: Optional[Tuple[Tensor, Tensor]] = None,
-        bounds: Optional[Tensor] = None,
-        interior_point: Optional[Tensor] = None,
-        mean: Optional[Tensor] = None,
-        covariance_matrix: Optional[Tensor] = None,
-        covariance_root: Optional[Tensor] = None,
-    ) -> None:
-        r"""Initialize LinearEllipticalSliceSampler.
-
-        Args:
-            inequality_constraints: Tensors `(A, b)` describing inequality constraints
-                 `A @ x <= b`, where `A` is an `n_ineq_con x d`-dim Tensor and `b` is
-                 an `n_ineq_con x 1`-dim Tensor, with `n_ineq_con` the number of
-                 inequalities and `d` the dimension of the sample space. If omitted,
-                 must provide `bounds` instead.
-            bounds: A `2 x d`-dim tensor of box bounds. If omitted, must provide
-                `inequality_constraints` instead.
-            interior_point: A `d x 1`-dim Tensor presenting a point in the (relative)
-                interior of the polytope. If omitted, an interior point is determined
-                automatically by solving a Linear Program. Note: It is crucial that
-                the point lie in the interior of the feasible set (rather than on the
-                boundary), otherwise the sampler will produce invalid samples.
-            mean: The `d x 1`-dim mean of the MVN distribution (if omitted, use zero).
-            covariance_matrix: The `d x d`-dim covariance matrix of the MVN
-                distribution (if omitted, use the identity).
-            covariance_root: A `d x k`-dim root of the covariance matrix such that
-                covariance_root @ covariance_root.T = covariance_matrix.
-
-        This sampler samples from a multivariante Normal `N(mean, covariance_matrix)`
-        subject to linear domain constraints `A x <= b` (intersected with box bounds,
-        if provided).
-        """
-        super().__init__(
-            inequality_constraints=inequality_constraints,
-            # TODO: Support equality constraints?
-            interior_point=interior_point,
-            bounds=bounds,
+
+def log_ndtr(x: Tensor) -> Tensor:
+    """Implementation of log_ndtr that remedies problems of torch.special's version
+    for large negative x, where the torch implementation yields Inf or NaN gradients.
+
+    Args:
+        x: An input tensor with dtype torch.float32 or torch.float64.
+
+    Returns:
+        A tensor of values of the same type and shape as x containing log(ndtr(x)).
+    """
+    if not (x.dtype == torch.float32 or x.dtype == torch.float64):
+        raise TypeError(
+            f"log_Phi only supports torch.float32 and torch.float64 "
+            f"dtypes, but received {x.dtype = }."
         )
-        tkwargs = {"device": self.x0.device, "dtype": self.x0.dtype}
-        self._mean = mean
-        if covariance_matrix is not None:
-            if covariance_root is not None:
-                raise ValueError(
-                    "Provide either covariance_matrix or covariance_root, not both."
-                )
-            try:
-                covariance_root = torch.linalg.cholesky(covariance_matrix)
-            except RuntimeError as e:
-                raise_e = e
-                if "positive-definite" in str(raise_e):
-                    raise_e = ValueError(
-                        "Covariance matrix is not positive definite. "
-                        "Currently only non-degenerate distributions are supported."
-                    )
-                raise raise_e
-        self._covariance_root = covariance_root
-        self._x = self.x0.clone()  # state of the sampler ("current point")
-        # We will need the following repeatedly, let's allocate them once
-        self._zero = torch.zeros(1, **tkwargs)
-        self._nan = torch.tensor(float("nan"), **tkwargs)
-        self._full_angular_range = torch.tensor([0.0, _twopi], **tkwargs)
-
-    def draw(self, n: int = 1) -> Tuple[Tensor, Tensor]:
-        r"""Draw samples.
-
-        Args:
-            n: The number of samples.
-
-        Returns:
-            A `n x d`-dim tensor of `n` samples.
-        """
-        # TODO: Do we need to do any thinnning or warm-up here?
-        samples = torch.cat([self.step() for _ in range(n)], dim=-1)
-        return samples.transpose(-1, -2)
-
-    def step(self) -> Tensor:
-        r"""Take a step, return the new sample, update the internal state.
-
-        Returns:
-            A `d x 1`-dim sample from the domain.
-        """
-        nu = self._sample_base_rv()
-        theta = self._draw_angle(nu=nu)
-        self._x = self._get_cart_coords(nu=nu, theta=theta)
-        return self._x
-
-    def _sample_base_rv(self) -> Tensor:
-        r"""Sample a base random variable from N(mean, covariance_matrix).
-
-        Returns:
-            A `d x 1`-dim sample from the domain
-        """
-        nu = torch.randn_like(self._x)
-        if self._covariance_root is not None:
-            nu = self._covariance_root @ nu
-        if self._mean is not None:
-            nu = self._mean + nu
-        return nu
-
-    def _draw_angle(self, nu: Tensor) -> Tensor:
-        r"""Draw the rotation angle.
-
-        Args:
-            nu: A `d x 1`-dim tensor (the "new" direction, drawn from N(0, I)).
-
-        Returns:
-            A
-        """
-        rot_angle, rot_slices = self._find_rotated_intersections(nu)
-        rot_lengths = rot_slices[:, 1] - rot_slices[:, 0]
-        cum_lengths = torch.cumsum(rot_lengths, dim=0)
-        cum_lengths = torch.cat((self._zero, cum_lengths), dim=0)
-        rnd_angle = cum_lengths[-1] * torch.rand(
-            1, device=cum_lengths.device, dtype=cum_lengths.dtype
+    neg_inv_sqrt_2, log_2 = get_constants_like((_neg_inv_sqrt_2, _log_2), x)
+    return log_erfc(neg_inv_sqrt_2 * x) - log_2
+
+
+def log_erfc(x: Tensor) -> Tensor:
+    """Computes the logarithm of the complementary error function in a numerically
+    stable manner. The GitHub issue https://github.com/pytorch/pytorch/issues/31945
+    tracks progress toward moving this feature into PyTorch in C++.
+
+    Args:
+        x: An input tensor with dtype torch.float32 or torch.float64.
+
+    Returns:
+        A tensor of values of the same type and shape as x containing log(erfc(x)).
+    """
+    if not (x.dtype == torch.float32 or x.dtype == torch.float64):
+        raise TypeError(
+            f"log_erfc only supports torch.float32 and torch.float64 "
+            f"dtypes, but received {x.dtype = }."
         )
-        idx = torch.searchsorted(cum_lengths, rnd_angle) - 1
-        return rot_slices[idx, 0] + rnd_angle - cum_lengths[idx] + rot_angle
+    is_pos = x > 0
+    x_pos = x.masked_fill(~is_pos, 0)
+    x_neg = x.masked_fill(is_pos, 0)
+    return torch.where(
+        is_pos,
+        torch.log(torch.special.erfcx(x_pos)) - x_pos.square(),
+        torch.log(torch.special.erfc(x_neg)),
+    )
+
+
+def log_erfcx(x: Tensor) -> Tensor:
+    """Computes the logarithm of the complementary scaled error function in a
+    numerically stable manner. The GitHub issue tracks progress toward moving this
+    feature into PyTorch in C++: https://github.com/pytorch/pytorch/issues/31945.
+
+    Args:
+        x: An input tensor with dtype torch.float32 or torch.float64.
+
+    Returns:
+        A tensor of values of the same type and shape as x containing log(erfcx(x)).
+    """
+    is_pos = x > 0
+    x_pos = x.masked_fill(~is_pos, 0)
+    x_neg = x.masked_fill(is_pos, 0)
+    return torch.where(
+        is_pos,
+        torch.special.erfcx(x_pos).log(),
+        torch.special.erfc(x_neg).log() + x.square(),
+    )
+
+
+def standard_normal_log_hazard(x: Tensor) -> Tensor:
+    """Computes the logarithm of the hazard function of the standard normal
+    distribution, i.e. `log(phi(x) / Phi(-x))`.
+
+    Args:
+        x: A tensor of any shape, with either float32 or float64 dtypes.
+
+    Returns:
+        A Tensor of the same shape `x`, containing the values of the logarithm of the
+        hazard function evaluated at `x`.
+    """
+    # NOTE: using _inv_sqrt_2 instead of _neg_inv_sqrt_2 means we are computing Phi(-x).
+    a, b = get_constants_like((_log_two_inv_sqrt_2pi, _inv_sqrt_2), x)
+    return a - log_erfcx(b * x)
+
+
+def log_prob_normal_in(a: Tensor, b: Tensor) -> Tensor:
+    r"""Computes the probability that a standard normal random variable takes a value
+    in \[a, b\], i.e. log(Phi(b) - Phi(a)), where Phi is the standard normal CDF.
+    Returns accurate values and permits numerically stable backward passes for inputs
+    in [-1e100, 1e100] for double precision and [-1e20, 1e20] for single precision.
+    In contrast, a naive approach is not numerically accurate beyond [-10, 10].
+
+    Args:
+        a: Tensor of lower integration bounds of the Gaussian probability measure.
+        b: Tensor of upper integration bounds of the Gaussian probability measure.
+
+    Returns:
+        Tensor of the log probabilities.
+    """
+    if not (a < b).all():
+        raise ValueError("Received input tensors a, b for which not all a < b.")
+    # if abs(b) > abs(a), we use Phi(b) - Phi(a) = Phi(-a) - Phi(-b), since the
+    # right tail converges to 0 from below, leading to digit cancellation issues, while
+    # the left tail of log_ndtr is well behaved and results in large negative numbers
+    rev_cond = b.abs() > a.abs()  # condition for reversal of inputs
+    if rev_cond.any():
+        c = torch.where(rev_cond, -b, a)
+        b = torch.where(rev_cond, -a, b)
+        a = c  # after we updated b, can assign c to a
+    return logdiffexp(log_a=log_ndtr(a), log_b=log_ndtr(b))
+
+
+def swap_along_dim_(
+    values: Tensor,
+    i: Union[int, LongTensor],
+    j: Union[int, LongTensor],
+    dim: int,
+    buffer: Optional[Tensor] = None,
+) -> Tensor:
+    r"""Swaps Tensor slices in-place along dimension `dim`.
+
+    When passed as Tensors, `i` (and `j`) should be `dim`-dimensional tensors
+    with the same shape as `values.shape[:dim]`. The xception to this rule occurs
+    when `dim=0`, in which case `i` (and `j`) should be (at most) one-dimensional
+    when passed as a Tensor.
+
+    Args:
+        values: Tensor whose values are to be swapped.
+        i: Indices for slices along dimension `dim`.
+        j: Indices for slices along dimension `dim`.
+        dim: The dimension of `values` along which to swap slices.
+        buffer: Optional buffer used internally to store copied values.
+
+    Returns:
+        The original `values` tensor.
+    """
+    dim = values.ndim + dim if dim < 0 else dim
+    if dim and (
+        (isinstance(i, Tensor) and i.ndim) or (isinstance(j, Tensor) and j.ndim)
+    ):
+        # Handle n-dimensional batches of heterogeneous swaps via linear indexing
+        if isinstance(i, Tensor) and i.shape != values.shape[:dim]:
+            raise ValueError("Batch shapes of `i` and `values` do not match.")
 
-    def _get_cart_coords(self, nu: Tensor, theta: Tensor) -> Tensor:
-        r"""Determine location on ellipsoid in cartesian coordinates.
+        if isinstance(j, Tensor) and j.shape != values.shape[:dim]:
+            raise ValueError("Batch shapes of `j` and `values` do not match.")
 
-        Args:
-            nu: A `d x 1`-dim tensor (the "new" direction, drawn from N(0, I)).
-            theta: A `k`-dim tensor of angles.
-
-        Returns:
-            A `d x k`-dim tensor of samples from the domain in cartesian coordinates.
-        """
-        return self._x * torch.cos(theta) + nu * torch.sin(theta)
-
-    def _find_rotated_intersections(self, nu: Tensor) -> Tuple[Tensor, Tensor]:
-        r"""Finds rotated intersections.
-
-        Rotates the intersections by the rotation angle and makes sure that all
-        angles lie in [0, 2*pi].
-
-        Args:
-            nu: A `d x 1`-dim tensor (the "new" direction, drawn from N(0, I)).
-
-        Returns:
-            A two-tuple containing rotation angle (scalar) and a
-            `num_active / 2 x 2`-dim tensor of shifted angles.
-        """
-        slices = self._find_active_intersections(nu)
-        rot_angle = slices[0]
-        slices = slices - rot_angle
-        slices = torch.where(slices < 0, slices + _twopi, slices)
-        return rot_angle, slices.reshape(-1, 2)
-
-    def _find_active_intersections(self, nu: Tensor) -> Tensor:
-        """
-        Find angles of those intersections that are at the boundary of the integration
-        domain by adding and subtracting a small angle and evaluating on the ellipse
-        to see if we are on the boundary of the integration domain.
-
-        Args:
-            nu: A `d x 1`-dim tensor (the "new" direction, drawn from N(0, I)).
-
-        Returns:
-            A `num_active`-dim tensor containing the angles of active intersection in
-            increasing order so that activation happens in positive direction. If a
-            slice crosses `theta=0`, the first angle is appended at the end of the
-            tensor. Every element of the returned tensor defines a slice for elliptical
-            slice sampling.
-        """
-        theta = self._find_intersection_angles(nu)
-        active_directions = self._index_active(
-            nu=nu, theta=theta, delta_theta=_delta_theta
+        pidx = build_positional_indices(
+            shape=values.shape[: dim + 1], dim=-2, device=values.device
         )
-        theta_active = theta[active_directions.nonzero()]
-        delta_theta = _delta_theta
-        while theta_active.numel() % 2 == 1:
-            # Almost tangential ellipses, reduce delta_theta
-            delta_theta /= 10
-            active_directions = self._index_active(
-                theta=theta, nu=nu, delta_theta=delta_theta
-            )
-            theta_active = theta[active_directions.nonzero()]
-
-        if theta_active.numel() == 0:
-            theta_active = self._full_angular_range
-            # TODO: What about `self.ellipse_in_domain = False` in the original code ??
-        elif active_directions[active_directions.nonzero()][0] == -1:
-            theta_active = torch.cat((theta_active[1:], theta_active[:1]))
-
-        return theta_active.view(-1)
-
-    def _find_intersection_angles(self, nu: Tensor) -> Tensor:
-        """Compute all of the up to 2*n_ineq_con intersections of the ellipse
-        and the linear constraints.
-
-        For background, see equation (2) in
-        http://proceedings.mlr.press/v108/gessner20a/gessner20a.pdf
-
-        Args:
-            nu: A `d x 1`-dim tensor (the "new" direction, drawn from N(0, I)).
-
-        Returns:
-            An `M`-dim tensor, where `M <= 2 * n_ineq_con` (with `M = n_ineq_con`
-            if all intermediate computations yield finite numbers).
-        """
-        # Compared to the implementation in https://github.com/alpiges/LinConGauss
-        # we need to flip the sign of A b/c the original algorithm considers
-        # A @ x + b >= 0 feasible, whereas we consider A @ x - b <= 0 feasible.
-        g1 = -self.A @ self._x
-        g2 = -self.A @ nu
-        r = torch.sqrt(g1**2 + g2**2)
-        phi = 2 * torch.atan(g2 / (r + g1)).squeeze()
-
-        arg = -(self.b / r).squeeze()
-        # Write NaNs if there is no intersection
-        arg = torch.where(torch.absolute(arg) <= 1, arg, self._nan)
-
-        # Two solutions per linear constraint, shape of theta: (n_ineq_con, 2)
-        acos_arg = torch.arccos(arg)
-        theta = torch.stack((phi + acos_arg, phi - acos_arg), dim=-1)
-        theta = theta[torch.isfinite(theta)]  # shape: `n_ineq_con - num_not_finite`
-        theta = torch.where(theta < 0, theta + _twopi, theta)  # [0, 2*pi]
-
-        return torch.sort(theta).values
-
-    def _index_active(
-        self, nu: Tensor, theta: Tensor, delta_theta: float = _delta_theta
-    ) -> Tensor:
-        r"""Determine active indices.
-
-        Args:
-            nu: A `d x 1`-dim tensor (the "new" direction, drawn from N(0, I)).
-            theta: An `M`-dim tensor of intersection angles.
-            delta_theta: A small perturbation to be used for determining whether
-                intersections are at the boundary of the integration domain.
-
-        Returns:
-            An `M`-dim tensor with elements taking on values in {-1, 0, 1}.
-            A non-zero value indicates whether the associated intersection angle
-            is an active constraint. For active constraints, the sign indicates
-            the direction of the relevant domain (i.e. +1 (-1) means that
-            increasing (decreasing) the angle renders the sample feasible).
-        """
-        samples_pos = self._get_cart_coords(nu=nu, theta=theta + delta_theta)
-        samples_neg = self._get_cart_coords(nu=nu, theta=theta - delta_theta)
-        pos_diffs = self._is_feasible(samples_pos)
-        neg_diffs = self._is_feasible(samples_neg)
-        # We don't use bit-wise XOR here since we need the signs of the directions
-        return pos_diffs.to(nu) - neg_diffs.to(nu)
-
-    def _is_feasible(self, points: Tensor) -> Tensor:
-        r"""
-
-        Args:
-            points: A `M x d`-dim tensor of points.
-
-        Returns:
-            An `M`-dim binary tensor where `True` indicates that the associated
-            point is feasible.
-        """
-        return (self.A @ points <= self.b).all(dim=0)
+
+        swap_along_dim_(
+            values.view(-1, *values.shape[dim + 1 :]),
+            i=(pidx + i).view(-1),
+            j=(pidx + j).view(-1),
+            dim=0,
+            buffer=buffer,
+        )
+
+    else:
+        # Base cases: homogeneous swaps and 1-dimenensional heterogeneous swaps
+        if isinstance(i, Tensor) and i.ndim > 1:
+            raise ValueError("Tensor `i` must be at most 1-dimensional when `dim=0`.")
+
+        if isinstance(j, Tensor) and j.ndim > 1:
+            raise ValueError("Tensor `j` must be at most 1-dimensional when `dim=0`.")
+
+        if dim:
+            ctx = tuple(slice(None) for _ in range(dim))
+            i = ctx + (i,)
+            j = ctx + (j,)
+
+        if buffer is None:
+            buffer = values[i].clone()
+        else:
+            buffer.copy_(values[i])
+
+        values[i] = values[j]
+        values[j] = buffer
+
+    return values
```

### Comparing `botorch-0.8.5/botorch/utils/probability/linalg.py` & `botorch-0.9.1/botorch/utils/probability/linalg.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         if self.step != other.step:
             raise ValueError("Cannot conncatenate decompositions at different steps.")
 
         fields = {}
         for name in ("tril", "perm", "diag"):
             a = getattr(self, name)
             b = getattr(other, name)
-            if type(a) != type(b):
+            if type(a) is not type(b):
                 raise NotImplementedError(f"Types of field {name} do not match.")
 
             if a is not None:
                 fields[name] = torch.concat((a, b), dim=dim)
 
         return type(self)(step=self.step, **fields)
```

### Comparing `botorch-0.8.5/botorch/utils/probability/mvnxpb.py` & `botorch-0.9.1/botorch/utils/probability/mvnxpb.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,26 +172,28 @@
             else:  # pivot using order specified by precomputed pivoted Cholesky step
                 mask = self.perm[..., i:] == piv_chol.perm[..., i : i + 1]
                 pivot = i + torch.nonzero(mask, as_tuple=True)[-1]
 
             if pivot is not None and torch.any(pivot > i):
                 self.pivot_(pivot=pivot)
 
-            # Initialize `i`-th plug-in value as univariate conditional expectation
+            # Compute whitened bounds conditional on preceding plug-ins
             Lii = L[..., i, i].clone()
             if should_update_chol:
-                Lii = Lii.clip(min=0).sqrt()
+                Lii = Lii.clip(min=0).sqrt()  # conditional stddev
             inv_Lii = Lii.reciprocal()
-            if i == 0:
-                lb, ub = bounds[..., i, :].clone().unbind(dim=-1)
-            else:
-                db = (L[..., i, :i].clone() * y[..., :i].clone()).sum(-1, keepdim=True)
-                lb, ub = (bounds[..., i, :].clone() - db).unbind(dim=-1)
+            bounds_i = bounds[..., i, :].clone()
+            if i != 0:
+                bounds_i = bounds_i - torch.sum(
+                    L[..., i, :i].clone() * y[..., :i].clone(), dim=-1, keepdim=True
+                )
+            lb, ub = (inv_Lii.unsqueeze(-1) * bounds_i).unbind(dim=-1)
 
-            Phi_i = Phi(inv_Lii * ub) - Phi(inv_Lii * lb)
+            # Initialize `i`-th plug-in value as univariate conditional expectation
+            Phi_i = Phi(ub) - Phi(lb)
             small = Phi_i <= i * eps
             y[..., i] = case_dispatcher(  # used to select next pivot
                 out=(phi(lb) - phi(ub)) / Phi_i,
                 cases=(  # fallback cases for enhanced numerical stability
                     (lambda: small & (lb < -9), lambda m: ub[m]),
                     (lambda: small & (lb > 9), lambda m: lb[m]),
                     (lambda: small, lambda m: 0.5 * (lb[m] + ub[m])),
@@ -220,15 +222,15 @@
                 blk_corr = Lhh * Lih * istds.prod(-1)
                 blk_prob = bvn(blk_corr, *blk_lower, *blk_upper)
                 zh, zi = bvnmom(blk_corr, *blk_lower, *blk_upper, p=blk_prob)
 
                 # Replace 1D expectations with 2D ones `L[blk, blk]^{-1} y[..., blk]`
                 mask = blk_prob > zero
                 y[..., h] = torch.where(mask, zh, zero)
-                y[..., i] = torch.where(mask, (std_i * zi - Lih * zh) / Lii, zero)
+                y[..., i] = torch.where(mask, inv_Lii * (std_i * zi - Lih * zh), zero)
 
                 # Update running approximation to log probability
                 self.log_prob = self.log_prob + safe_log(blk_prob)
 
             self.step += 1
             if should_update_chol:
                 piv_chol.update_(eps=eps)
@@ -296,15 +298,15 @@
 
         state_dict = self.asdict()
         for key, _other in other.asdict().items():
             _self = state_dict.get(key)
             if _self is None and _other is None:
                 continue
 
-            if type(_self) != type(_other):
+            if type(_self) is not type(_other):
                 raise TypeError(
                     f"Concatenation failed: `self.{key}` has type {type(_self)}, "
                     f"but `other.{key}` is of type {type(_self)}."
                 )
 
             if isinstance(_self, PivotedCholesky):
                 state_dict[key] = _self.concat(_other, dim=dim)
```

### Comparing `botorch-0.8.5/botorch/utils/probability/truncated_multivariate_normal.py` & `botorch-0.9.1/botorch/utils/probability/truncated_multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/probability/unified_skew_normal.py` & `botorch-0.9.1/botorch/utils/probability/unified_skew_normal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/rounding.py` & `botorch-0.9.1/botorch/utils/rounding.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/sampling.py` & `botorch-0.9.1/botorch/utils/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -789,54 +789,31 @@
         n_burnin: The number of burn-in samples for the Markov chain sampler.
 
     Returns:
         A `n x d`-dim tensor of samples.
     """
     # create tensors representing linear inequality constraints
     # of the form Ax >= b.
-    # TODO: remove this error handling functionality in a few releases.
-    # Context: BoTorch inadvertently supported indices with unusual dtypes.
-    # This is now not supported.
-    index_dtype_error = (
-        "Normalizing {var_name} failed. Check that the first "
-        "element of {var_name} is the correct dtype following "
-        "the previous IndexError."
-    )
     if inequality_constraints:
         # normalize_linear_constraints is called to solve this issue:
         # https://github.com/pytorch/botorch/issues/1225
-        try:
-            # non-standard dtypes used to be supported for indices in constraints;
-            # this is no longer true
-            constraints = normalize_linear_constraints(bounds, inequality_constraints)
-        except IndexError as e:
-            msg = index_dtype_error.format(var_name="`inequality_constraints`")
-            raise ValueError(msg) from e
+        constraints = normalize_linear_constraints(bounds, inequality_constraints)
 
         A, b = sparse_to_dense_constraints(
             d=bounds.shape[-1],
             constraints=constraints,
         )
         # Note the inequality constraints are of the form Ax >= b,
         # but PolytopeSampler expects inequality constraints of the
         # form Ax <= b, so we multiply by -1 below.
         dense_inequality_constraints = -A, -b
     else:
         dense_inequality_constraints = None
     if equality_constraints:
-        try:
-            # non-standard dtypes used to be supported for indices in constraints;
-            # this is no longer true
-            constraints = normalize_linear_constraints(bounds, equality_constraints)
-        except IndexError as e:
-            msg = index_dtype_error.format(var_name="`equality_constraints`")
-            raise ValueError(msg) from e
-
-        # normalize_linear_constraints is called to solve this issue:
-        # https://github.com/pytorch/botorch/issues/1225
+        constraints = normalize_linear_constraints(bounds, equality_constraints)
         dense_equality_constraints = sparse_to_dense_constraints(
             d=bounds.shape[-1], constraints=constraints
         )
     else:
         dense_equality_constraints = None
     normalized_bounds = torch.zeros_like(bounds)
     normalized_bounds[1, :] = 1.0
```

### Comparing `botorch-0.8.5/botorch/utils/testing.py` & `botorch-0.9.1/botorch/utils/testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 import math
 import warnings
+from abc import abstractproperty
 from collections import OrderedDict
 from typing import Any, List, Optional, Tuple, Union
 from unittest import TestCase
 
 import torch
 from botorch import settings
 from botorch.acquisition.objective import PosteriorTransform
@@ -89,18 +90,15 @@
             other,
             rtol=rtol,
             atol=atol,
             equal_nan=equal_nan,
         )
 
 
-class BaseTestProblemBaseTestCase:
-
-    functions: List[BaseTestProblem]
-
+class BaseTestProblemTestCaseMixIn:
     def test_forward(self):
         for dtype in (torch.float, torch.double):
             for batch_shape in (torch.Size(), torch.Size([2]), torch.Size([2, 3])):
                 for f in self.functions:
                     f.to(device=self.device, dtype=dtype)
                     X = torch.rand(*batch_shape, f.dim, device=self.device, dtype=dtype)
                     X = f.bounds[0] + X * (f.bounds[1] - f.bounds[0])
@@ -109,16 +107,22 @@
                     self.assertEqual(res.dtype, dtype)
                     self.assertEqual(res.device.type, self.device.type)
                     tail_shape = torch.Size(
                         [f.num_objectives] if f.num_objectives > 1 else []
                     )
                     self.assertEqual(res.shape, batch_shape + tail_shape)
 
+    @abstractproperty
+    def functions(self) -> List[BaseTestProblem]:
+        # The functions that should be tested. Typically defined as a class
+        # attribute on the test case subclassing this class.
+        pass  # pragma: no cover
+
 
-class SyntheticTestFunctionBaseTestCase(BaseTestProblemBaseTestCase):
+class SyntheticTestFunctionTestCaseMixin:
     def test_optimal_value(self):
         for dtype in (torch.float, torch.double):
             for f in self.functions:
                 f.to(device=self.device, dtype=dtype)
                 try:
                     optval = f.optimal_value
                     optval_exp = -f._optimal_value if f.negate else f._optimal_value
@@ -139,14 +143,60 @@
                 res_exp = torch.full_like(res, f.optimal_value)
                 self.assertAllClose(res, res_exp, atol=1e-3, rtol=1e-3)
                 if f._check_grad_at_opt:
                     grad = torch.autograd.grad([*res], Xopt)[0]
                     self.assertLess(grad.abs().max().item(), 1e-3)
 
 
+class MultiObjectiveTestProblemTestCaseMixin:
+    def test_attributes(self):
+        for f in self.functions:
+            self.assertTrue(hasattr(f, "dim"))
+            self.assertTrue(hasattr(f, "num_objectives"))
+            self.assertEqual(f.bounds.shape, torch.Size([2, f.dim]))
+
+    def test_max_hv(self):
+        for dtype in (torch.float, torch.double):
+            for f in self.functions:
+                f.to(device=self.device, dtype=dtype)
+                if not hasattr(f, "_max_hv"):
+                    with self.assertRaises(NotImplementedError):
+                        f.max_hv
+                else:
+                    self.assertEqual(f.max_hv, f._max_hv)
+
+    def test_ref_point(self):
+        for dtype in (torch.float, torch.double):
+            for f in self.functions:
+                f.to(dtype=dtype, device=self.device)
+                self.assertTrue(
+                    torch.allclose(
+                        f.ref_point,
+                        torch.tensor(f._ref_point, dtype=dtype, device=self.device),
+                    )
+                )
+
+
+class ConstrainedTestProblemTestCaseMixin:
+    def test_num_constraints(self):
+        for f in self.functions:
+            self.assertTrue(hasattr(f, "num_constraints"))
+
+    def test_evaluate_slack_true(self):
+        for dtype in (torch.float, torch.double):
+            for f in self.functions:
+                f.to(device=self.device, dtype=dtype)
+                X = unnormalize(
+                    torch.rand(1, f.dim, device=self.device, dtype=dtype),
+                    bounds=f.bounds,
+                )
+                slack = f.evaluate_slack_true(X)
+                self.assertEqual(slack.shape, torch.Size([1, f.num_constraints]))
+
+
 class MockPosterior(Posterior):
     r"""Mock object that implements dummy methods and feeds through specified outputs"""
 
     def __init__(
         self, mean=None, variance=None, samples=None, base_shape=None, batch_range=None
     ) -> None:
         r"""
@@ -366,53 +416,59 @@
             covar = AddedDiagLinearOperator(covar, DiagLinearOperator(flat_diag))
         else:
             covar = covar + torch.diag_embed(flat_diag)
         mtmvn = MultitaskMultivariateNormal(mean, covar, interleaved=interleaved)
     return GPyTorchPosterior(mtmvn)
 
 
-class MultiObjectiveTestProblemBaseTestCase(BaseTestProblemBaseTestCase):
-    def test_attributes(self):
-        for f in self.functions:
-            self.assertTrue(hasattr(f, "dim"))
-            self.assertTrue(hasattr(f, "num_objectives"))
-            self.assertEqual(f.bounds.shape, torch.Size([2, f.dim]))
-
-    def test_max_hv(self):
-        for dtype in (torch.float, torch.double):
-            for f in self.functions:
-                f.to(device=self.device, dtype=dtype)
-                if not hasattr(f, "_max_hv"):
-                    with self.assertRaises(NotImplementedError):
-                        f.max_hv
-                else:
-                    self.assertEqual(f.max_hv, f._max_hv)
-
-    def test_ref_point(self):
-        for dtype in (torch.float, torch.double):
-            for f in self.functions:
-                f.to(dtype=dtype, device=self.device)
-                self.assertTrue(
-                    torch.allclose(
-                        f.ref_point,
-                        torch.tensor(f._ref_point, dtype=dtype, device=self.device),
-                    )
-                )
+def _get_max_violation_of_bounds(samples: torch.Tensor, bounds: torch.Tensor) -> float:
+    """
+    The maximum value by which samples lie outside bounds.
 
+    A negative value indicates that all samples lie within bounds.
 
-class ConstrainedMultiObjectiveTestProblemBaseTestCase(
-    MultiObjectiveTestProblemBaseTestCase
-):
-    def test_num_constraints(self):
-        for f in self.functions:
-            self.assertTrue(hasattr(f, "num_constraints"))
+    Args:
+        samples: An `n x q x d` - dimension tensor, as might be returned from
+            `sample_q_batches_from_polytope`.
+        bounds: A `2 x d` tensor of lower and upper bounds for each column.
+    """
+    n, q, d = samples.shape
+    samples = samples.reshape((n * q, d))
+    lower = samples.min(0).values
+    upper = samples.max(0).values
+    lower_dist = (bounds[0, :] - lower).max().item()
+    upper_dist = (upper - bounds[1, :]).max().item()
+    return max(lower_dist, upper_dist)
+
+
+def _get_max_violation_of_constraints(
+    samples: torch.Tensor,
+    constraints: Optional[List[Tuple[Tensor, Tensor, float]]],
+    equality: bool,
+) -> float:
+    r"""
+    Amount by which equality constraints are not obeyed.
 
-    def test_evaluate_slack_true(self):
-        for dtype in (torch.float, torch.double):
-            for f in self.functions:
-                f.to(device=self.device, dtype=dtype)
-                X = unnormalize(
-                    torch.rand(1, f.dim, device=self.device, dtype=dtype),
-                    bounds=f.bounds,
-                )
-                slack = f.evaluate_slack_true(X)
-                self.assertEqual(slack.shape, torch.Size([1, f.num_constraints]))
+    Args:
+        samples: An `n x q x d` - dimension tensor, as might be returned from
+            `sample_q_batches_from_polytope`.
+        constraints: A list of tuples (indices, coefficients, rhs),
+            with each tuple encoding an inequality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`, or `>=` if
+            `equality` is False.
+        equality: Whether these are equality constraints (not inequality).
+    """
+    n, q, d = samples.shape
+    max_error = 0
+    if constraints is not None:
+        for (ind, coef, rhs) in constraints:
+            if ind.ndim == 1:
+                constr = samples[:, :, ind] @ coef
+            else:
+                constr = samples[:, ind[:, 0], ind[:, 1]] @ coef
+
+            if equality:
+                error = (constr - rhs).abs().max()
+            else:
+                error = (rhs - constr).max()
+            max_error = max(max_error, error)
+    return max_error
```

### Comparing `botorch-0.8.5/botorch/utils/torch.py` & `botorch-0.9.1/botorch/utils/torch.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch/utils/transforms.py` & `botorch-0.9.1/botorch/utils/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,40 +190,30 @@
     Args:
         model: A BoTorch model (may be a `ModelList` or `ModelListGP`)
         d: The dimension of the tensor to index.
 
     Returns:
         True if at least one model is a `SaasFullyBayesianSingleTaskGP`
     """
-    from botorch.models import ModelList, ModelListGP
+    from botorch.models import ModelList
     from botorch.models.fully_bayesian import SaasFullyBayesianSingleTaskGP
     from botorch.models.fully_bayesian_multitask import SaasFullyBayesianMultiTaskGP
 
-    full_bayesian_model_cls = [
+    full_bayesian_model_cls = (
         SaasFullyBayesianSingleTaskGP,
         SaasFullyBayesianMultiTaskGP,
-    ]
+    )
 
-    if any(
-        isinstance(model, m_cls) or getattr(model, "is_fully_bayesian", False)
-        for m_cls in full_bayesian_model_cls
+    if isinstance(model, full_bayesian_model_cls) or getattr(
+        model, "is_fully_bayesian", False
     ):
         return True
     elif isinstance(model, ModelList):
         for m in model.models:
-            if any(
-                isinstance(m, m_cls) or getattr(model, "is_fully_bayesian", False)
-                for m_cls in full_bayesian_model_cls
-            ):
-                return True
-            elif isinstance(m, ModelListGP) and any(
-                isinstance(m_sub, m_cls)
-                for m_sub in m.models
-                for m_cls in full_bayesian_model_cls
-            ):
+            if is_fully_bayesian(m):
                 return True
     return False
 
 
 def t_batch_mode_transform(
     expected_q: Optional[int] = None,
     assert_output_shape: bool = True,
```

### Comparing `botorch-0.8.5/botorch/utils/types.py` & `botorch-0.9.1/botorch/utils/types.py`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch.egg-info/PKG-INFO` & `botorch-0.9.1/botorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: botorch
-Version: 0.8.5
+Version: 0.9.1
 Summary: Bayesian Optimization in PyTorch
 Home-page: https://botorch.org
 Author: Meta Platforms, Inc.
 License: MIT
 Project-URL: Documentation, https://botorch.org
 Project-URL: Source, https://github.com/pytorch/botorch
 Project-URL: conda, https://anaconda.org/pytorch/botorch
 Keywords: Bayesian optimization,PyTorch
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: tutorials
 License-File: LICENSE
 
 <a href="https://botorch.org">
@@ -75,18 +75,18 @@
 We recommend that end-users who are not actively doing research on Bayesian
 Optimization simply use Ax.
 
 
 ## Installation
 
 **Installation Requirements**
-- Python >= 3.8
-- PyTorch >= 1.12
-- gpytorch == 1.10
-- linear_operator == 0.4.0
+- Python >= 3.9
+- PyTorch >= 1.13.1
+- gpytorch == 1.11
+- linear_operator == 0.5.1
 - pyro-ppl >= 1.8.4
 - scipy
 - multiple-dispatch
 
 ### Prerequisite only for MacOS users with Intel processors:
 Before installing BoTorch, we recommend first manually installing PyTorch, a required dependency of
 BoTorch. Installing it according to the [PyTorch installation instructions](https://pytorch.org/get-started/locally/)
@@ -173,15 +173,17 @@
 1. Fit a Gaussian Process model to data
   ```python
   import torch
   from botorch.models import SingleTaskGP
   from botorch.fit import fit_gpytorch_mll
   from gpytorch.mlls import ExactMarginalLogLikelihood
 
-  train_X = torch.rand(10, 2)
+  # Double precision is highly recommended for GPs.
+  # See https://github.com/pytorch/botorch/discussions/1444
+  train_X = torch.rand(10, 2, dtype=torch.double)
   Y = 1 - (train_X - 0.5).norm(dim=-1, keepdim=True)  # explicit output dimension
   Y += 0.1 * torch.rand_like(Y)
   train_Y = (Y - Y.mean()) / Y.std()
 
   gp = SingleTaskGP(train_X, train_Y)
   mll = ExactMarginalLogLikelihood(gp.likelihood, gp)
   fit_gpytorch_mll(mll)
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: botorch Version: 0.8.5 Summary: Bayesian
+Metadata-Version: 2.1 Name: botorch Version: 0.9.1 Summary: Bayesian
 Optimization in PyTorch Home-page: https://botorch.org Author: Meta Platforms,
 Inc. License: MIT Project-URL: Documentation, https://botorch.org Project-URL:
 Source, https://github.com/pytorch/botorch Project-URL: conda, https://
 anaconda.org/pytorch/botorch Keywords: Bayesian optimization,PyTorch
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Developers Requires-Python:
->=3.8 Description-Content-Type: text/markdown Provides-Extra: dev Provides-
+>=3.9 Description-Content-Type: text/markdown Provides-Extra: dev Provides-
 Extra: test Provides-Extra: tutorials License-File: LICENSE [BoTorch_Logo]
 ===============================================================================
 [![Support Ukraine](https://img.shields.io/badge/Support-Ukraine-
 FFD500?style=flat&labelColor=005BBB)](https://opensource.fb.com/support-
 ukraine) [![Lint](https://github.com/pytorch/botorch/workflows/Lint/badge.svg)]
 (https://github.com/pytorch/botorch/actions?query=workflow%3ALint) [![Test]
 (https://github.com/pytorch/botorch/workflows/Test/badge.svg)](https://
@@ -43,16 +43,16 @@
 researchers and sophisticated practitioners in Bayesian Optimization and AI. We
 recommend using BoTorch as a low-level API for implementing new algorithms for
 [Ax](https://ax.dev). Ax has been designed to be an easy-to-use platform for
 end-users, which at the same time is flexible enough for Bayesian Optimization
 researchers to plug into for handling of feature transformations, (meta-)data
 management, storage, etc. We recommend that end-users who are not actively
 doing research on Bayesian Optimization simply use Ax. ## Installation
-**Installation Requirements** - Python >= 3.8 - PyTorch >= 1.12 - gpytorch ==
-1.10 - linear_operator == 0.4.0 - pyro-ppl >= 1.8.4 - scipy - multiple-dispatch
+**Installation Requirements** - Python >= 3.9 - PyTorch >= 1.13.1 - gpytorch ==
+1.11 - linear_operator == 0.5.1 - pyro-ppl >= 1.8.4 - scipy - multiple-dispatch
 ### Prerequisite only for MacOS users with Intel processors: Before installing
 BoTorch, we recommend first manually installing PyTorch, a required dependency
 of BoTorch. Installing it according to the [PyTorch installation instructions]
 (https://pytorch.org/get-started/locally/) ensures that it is properly linked
 against MKL, a library that optimizes mathematical computation for Intel
 processors. This will result in up to an order-of-magnitude speed-up for
 Bayesian optimization, as at the moment, installing PyTorch from pip does not
@@ -98,30 +98,32 @@
 notebooks. * You can also install either the dev or tutorials dependencies
 without installing both, e.g. by changing the last command to `pip install -
 e ".[dev]"`. ## Getting Started Here's a quick run down of the main components
 of a Bayesian optimization loop. For more details see our [Documentation]
 (https://botorch.org/docs/introduction) and the [Tutorials](https://
 botorch.org/tutorials). 1. Fit a Gaussian Process model to data ```python
 import torch from botorch.models import SingleTaskGP from botorch.fit import
-fit_gpytorch_mll from gpytorch.mlls import ExactMarginalLogLikelihood train_X =
-torch.rand(10, 2) Y = 1 - (train_X - 0.5).norm(dim=-1, keepdim=True) # explicit
-output dimension Y += 0.1 * torch.rand_like(Y) train_Y = (Y - Y.mean()) / Y.std
-() gp = SingleTaskGP(train_X, train_Y) mll = ExactMarginalLogLikelihood
-(gp.likelihood, gp) fit_gpytorch_mll(mll) ``` 2. Construct an acquisition
-function ```python from botorch.acquisition import UpperConfidenceBound UCB =
-UpperConfidenceBound(gp, beta=0.1) ``` 3. Optimize the acquisition function
-```python from botorch.optim import optimize_acqf bounds = torch.stack(
-[torch.zeros(2), torch.ones(2)]) candidate, acq_value = optimize_acqf( UCB,
-bounds=bounds, q=1, num_restarts=5, raw_samples=20, ) ``` ## Citing BoTorch If
-you use BoTorch, please cite the following paper: > [M. Balandat, B. Karrer, D.
-R. Jiang, S. Daulton, B. Letham, A. G. Wilson, and E. Bakshy. BoTorch: A
-Framework for Efficient Monte-Carlo Bayesian Optimization. Advances in Neural
-Information Processing Systems 33, 2020.](https://arxiv.org/abs/1910.06403) ```
-@inproceedings{balandat2020botorch, title={{BoTorch: A Framework for Efficient
-Monte-Carlo Bayesian Optimization}}, author={Balandat, Maximilian and Karrer,
-Brian and Jiang, Daniel R. and Daulton, Samuel and Letham, Benjamin and Wilson,
-Andrew Gordon and Bakshy, Eytan}, booktitle = {Advances in Neural Information
+fit_gpytorch_mll from gpytorch.mlls import ExactMarginalLogLikelihood # Double
+precision is highly recommended for GPs. # See https://github.com/pytorch/
+botorch/discussions/1444 train_X = torch.rand(10, 2, dtype=torch.double) Y = 1
+- (train_X - 0.5).norm(dim=-1, keepdim=True) # explicit output dimension Y +=
+0.1 * torch.rand_like(Y) train_Y = (Y - Y.mean()) / Y.std() gp = SingleTaskGP
+(train_X, train_Y) mll = ExactMarginalLogLikelihood(gp.likelihood, gp)
+fit_gpytorch_mll(mll) ``` 2. Construct an acquisition function ```python from
+botorch.acquisition import UpperConfidenceBound UCB = UpperConfidenceBound(gp,
+beta=0.1) ``` 3. Optimize the acquisition function ```python from botorch.optim
+import optimize_acqf bounds = torch.stack([torch.zeros(2), torch.ones(2)])
+candidate, acq_value = optimize_acqf( UCB, bounds=bounds, q=1, num_restarts=5,
+raw_samples=20, ) ``` ## Citing BoTorch If you use BoTorch, please cite the
+following paper: > [M. Balandat, B. Karrer, D. R. Jiang, S. Daulton, B. Letham,
+A. G. Wilson, and E. Bakshy. BoTorch: A Framework for Efficient Monte-Carlo
+Bayesian Optimization. Advances in Neural Information Processing Systems 33,
+2020.](https://arxiv.org/abs/1910.06403) ``` @inproceedings
+{balandat2020botorch, title={{BoTorch: A Framework for Efficient Monte-Carlo
+Bayesian Optimization}}, author={Balandat, Maximilian and Karrer, Brian and
+Jiang, Daniel R. and Daulton, Samuel and Letham, Benjamin and Wilson, Andrew
+Gordon and Bakshy, Eytan}, booktitle = {Advances in Neural Information
 Processing Systems 33}, year={2020}, url = {http://arxiv.org/abs/1910.06403} }
 ``` See [here](https://botorch.org/docs/papers) for an incomplete selection of
 peer-reviewed papers that build off of BoTorch. ## Contributing See the
 [CONTRIBUTING](CONTRIBUTING.md) file for how to help out. ## License BoTorch is
 MIT licensed, as found in the [LICENSE](LICENSE) file.
```

### Comparing `botorch-0.8.5/botorch.egg-info/SOURCES.txt` & `botorch-0.9.1/botorch.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -42,25 +42,28 @@
 botorch.egg-info/top_level.txt
 botorch/acquisition/__init__.py
 botorch/acquisition/acquisition.py
 botorch/acquisition/active_learning.py
 botorch/acquisition/analytic.py
 botorch/acquisition/cached_cholesky.py
 botorch/acquisition/cost_aware.py
+botorch/acquisition/decoupled.py
 botorch/acquisition/fixed_feature.py
 botorch/acquisition/input_constructors.py
 botorch/acquisition/joint_entropy_search.py
 botorch/acquisition/knowledge_gradient.py
+botorch/acquisition/logei.py
 botorch/acquisition/max_value_entropy_search.py
 botorch/acquisition/monte_carlo.py
 botorch/acquisition/multi_step_lookahead.py
 botorch/acquisition/objective.py
 botorch/acquisition/penalized.py
 botorch/acquisition/predictive_entropy_search.py
 botorch/acquisition/preference.py
+botorch/acquisition/prior_guided.py
 botorch/acquisition/proximal.py
 botorch/acquisition/risk_measures.py
 botorch/acquisition/utils.py
 botorch/acquisition/multi_objective/__init__.py
 botorch/acquisition/multi_objective/analytic.py
 botorch/acquisition/multi_objective/joint_entropy_search.py
 botorch/acquisition/multi_objective/max_value_entropy_search.py
@@ -99,31 +102,35 @@
 botorch/models/kernels/__init__.py
 botorch/models/kernels/categorical.py
 botorch/models/kernels/contextual_lcea.py
 botorch/models/kernels/contextual_sac.py
 botorch/models/kernels/downsampling.py
 botorch/models/kernels/exponential_decay.py
 botorch/models/kernels/linear_truncated_fidelity.py
+botorch/models/kernels/orthogonal_additive_kernel.py
 botorch/models/likelihoods/__init__.py
 botorch/models/likelihoods/pairwise.py
 botorch/models/transforms/__init__.py
 botorch/models/transforms/factory.py
 botorch/models/transforms/input.py
 botorch/models/transforms/outcome.py
 botorch/models/transforms/utils.py
 botorch/models/utils/__init__.py
 botorch/models/utils/assorted.py
+botorch/models/utils/gpytorch_modules.py
 botorch/models/utils/inducing_point_allocators.py
 botorch/models/utils/parse_training_data.py
 botorch/optim/__init__.py
 botorch/optim/core.py
 botorch/optim/fit.py
+botorch/optim/homotopy.py
 botorch/optim/initializers.py
 botorch/optim/numpy_converter.py
 botorch/optim/optimize.py
+botorch/optim/optimize_homotopy.py
 botorch/optim/parameter_constraints.py
 botorch/optim/stopping.py
 botorch/optim/closures/__init__.py
 botorch/optim/closures/core.py
 botorch/optim/closures/model_closures.py
 botorch/optim/utils/__init__.py
 botorch/optim/utils/acquisition_utils.py
@@ -165,14 +172,15 @@
 botorch/test_functions/__init__.py
 botorch/test_functions/base.py
 botorch/test_functions/multi_fidelity.py
 botorch/test_functions/multi_objective.py
 botorch/test_functions/multi_objective_multi_fidelity.py
 botorch/test_functions/sensitivity_analysis.py
 botorch/test_functions/synthetic.py
+botorch/test_functions/utils.py
 botorch/utils/__init__.py
 botorch/utils/constants.py
 botorch/utils/constraints.py
 botorch/utils/containers.py
 botorch/utils/context_managers.py
 botorch/utils/datasets.py
 botorch/utils/dispatcher.py
```

### Comparing `botorch-0.8.5/botorch_logo_lockup.png` & `botorch-0.9.1/botorch_logo_lockup.png`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/botorch_logo_lockup.svg` & `botorch-0.9.1/botorch_logo_lockup.svg`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/notebooks/tutorials_performance_tracking.ipynb` & `botorch-0.9.1/notebooks/tutorials_performance_tracking.ipynb`

 * *Files identical despite different names*

### Comparing `botorch-0.8.5/setup.py` & `botorch-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 
 from setuptools import find_packages, setup
 
 # Minimum required python version
 REQUIRED_MAJOR = 3
-REQUIRED_MINOR = 8
+REQUIRED_MINOR = 9
 
 # Requirements for testing, formatting, and tutorials
 TEST_REQUIRES = ["pytest", "pytest-cov"]
 FMT_REQUIRES = ["flake8", "ufmt", "flake8-docstrings"]
 TUTORIALS_REQUIRES = [
     "ax-platform",
     "cma",
@@ -92,15 +92,15 @@
         "License :: OSI Approved :: MIT License",
         "Topic :: Scientific/Engineering",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     packages=find_packages(exclude=["test", "test.*"]),
     install_requires=install_requires,
     extras_require={
         "dev": DEV_REQUIRES,
         "test": TEST_REQUIRES,
         "tutorials": TUTORIALS_REQUIRES,
     },
```

