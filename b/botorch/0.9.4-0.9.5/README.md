# Comparing `tmp/botorch-0.9.4.tar.gz` & `tmp/botorch-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botorch-0.9.4.tar", last modified: Mon Nov  6 23:45:41 2023, max compression
+gzip compressed data, was "botorch-0.9.5.tar", last modified: Sat Dec  9 02:30:23 2023, max compression
```

## Comparing `botorch-0.9.4.tar` & `botorch-0.9.5.tar`

### file list

```diff
@@ -1,247 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.156253 botorch-0.9.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.108250 botorch-0.9.4/.conda/
--rwxr-xr-x   0 runner    (1001) docker     (127)      436 2023-11-06 23:42:27.000000 botorch-0.9.4/.conda/build_conda.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-11-06 23:42:27.000000 botorch-0.9.4/.conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.108250 botorch-0.9.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.108250 botorch-0.9.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      951 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.112250 botorch-0.9.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/workflows/deploy_on_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/workflows/nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/workflows/reusable_tutorials.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/workflows/reusable_website.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/workflows/test_stable.yml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/workflows/tutorials_smoke_test_on_pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-11-06 23:42:27.000000 botorch-0.9.4/.github/workflows/tutorials_smoke_test_on_push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2023-11-06 23:42:27.000000 botorch-0.9.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    56614 2023-11-06 23:42:27.000000 botorch-0.9.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2023-11-06 23:42:27.000000 botorch-0.9.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2023-11-06 23:42:27.000000 botorch-0.9.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-11-06 23:42:27.000000 botorch-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-11-06 23:42:27.000000 botorch-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2023-11-06 23:45:41.156253 botorch-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9159 2023-11-06 23:42:27.000000 botorch-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.116250 botorch-0.9.4/botorch/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.120251 botorch-0.9.4/botorch/acquisition/
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/active_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)    49880 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/analytic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/cached_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/cost_aware.py
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/decoupled.py
--rw-r--r--   0 runner    (1001) docker     (127)     9439 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/fixed_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    55026 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/input_constructors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14981 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/joint_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    26176 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/knowledge_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)    23074 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/logei.py
--rw-r--r--   0 runner    (1001) docker     (127)    42589 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/max_value_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    36641 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/monte_carlo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.120251 botorch-0.9.4/botorch/acquisition/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/multi_objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/multi_objective/analytic.py
--rw-r--r--   0 runner    (1001) docker     (127)    31296 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/multi_objective/joint_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/multi_objective/logei.py
--rw-r--r--   0 runner    (1001) docker     (127)    15942 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/multi_objective/max_value_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    22146 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/multi_objective/monte_carlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6613 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/multi_objective/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)    34672 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/multi_objective/multi_output_risk_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)    10923 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/multi_objective/objective.py
--rw-r--r--   0 runner    (1001) docker     (127)    48822 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/multi_objective/predictive_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    15090 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/multi_objective/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29264 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/multi_step_lookahead.py
--rw-r--r--   0 runner    (1001) docker     (127)    23537 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/objective.py
--rw-r--r--   0 runner    (1001) docker     (127)    14862 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/penalized.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/predictive_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/preference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/prior_guided.py
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/proximal.py
--rw-r--r--   0 runner    (1001) docker     (127)    12052 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/risk_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)    18007 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/acquisition/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/cross_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.120251 botorch-0.9.4/botorch/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/exceptions/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/exceptions/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16563 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.120251 botorch-0.9.4/botorch/generation/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20101 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/generation/gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    15080 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/generation/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/generation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.124251 botorch-0.9.4/botorch/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19333 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/approximate_gp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/contextual.py
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/contextual_multioutput.py
--rw-r--r--   0 runner    (1001) docker     (127)    17891 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     7548 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    22032 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (127)    18178 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/fully_bayesian_multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)    14894 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    13680 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/gp_regression_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/gp_regression_mixed.py
--rw-r--r--   0 runner    (1001) docker     (127)    35444 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/gpytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    24087 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/higher_order_gp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.128251 botorch-0.9.4/botorch/models/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/kernels/categorical.py
--rw-r--r--   0 runner    (1001) docker     (127)    17647 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/kernels/contextual_lcea.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/kernels/contextual_sac.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/kernels/downsampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/kernels/exponential_decay.py
--rw-r--r--   0 runner    (1001) docker     (127)    10226 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/kernels/linear_truncated_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)    12106 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/kernels/orthogonal_additive_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.128251 botorch-0.9.4/botorch/models/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/likelihoods/pairwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    28254 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/model_list_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)    34167 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)    49300 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/pairwise_gp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.128251 botorch-0.9.4/botorch/models/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/transforms/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    63902 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/transforms/input.py
--rw-r--r--   0 runner    (1001) docker     (127)    31087 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/transforms/outcome.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/transforms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.128251 botorch-0.9.4/botorch/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13896 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/utils/assorted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/utils/gpytorch_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    12753 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/utils/inducing_point_allocators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/models/utils/parse_training_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.128251 botorch-0.9.4/botorch/optim/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.128251 botorch-0.9.4/botorch/optim/closures/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/closures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7789 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/closures/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/closures/model_closures.py
--rw-r--r--   0 runner    (1001) docker     (127)     9132 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/homotopy.py
--rw-r--r--   0 runner    (1001) docker     (127)    43569 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    56264 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/optimize_homotopy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19687 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/parameter_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/stopping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.132251 botorch-0.9.4/botorch/optim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/utils/acquisition_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/optim/utils/timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.132251 botorch-0.9.4/botorch/posteriors/
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/posteriors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/posteriors/base_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/posteriors/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/posteriors/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/posteriors/fully_bayesian.py
--rw-r--r--   0 runner    (1001) docker     (127)    14995 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/posteriors/gpytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11379 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/posteriors/higher_order.py
--rw-r--r--   0 runner    (1001) docker     (127)    12403 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/posteriors/multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/posteriors/posterior.py
--rw-r--r--   0 runner    (1001) docker     (127)     7217 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/posteriors/posterior_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/posteriors/torch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/posteriors/transformed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.140252 botorch-0.9.4/botorch/sampling/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/get_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/index_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/list_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/pairwise_samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.140252 botorch-0.9.4/botorch/sampling/pathwise/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/pathwise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.144252 botorch-0.9.4/botorch/sampling/pathwise/features/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/pathwise/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/pathwise/features/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/pathwise/features/maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/pathwise/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/pathwise/posterior_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/pathwise/prior_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/pathwise/update_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)    10536 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/pathwise/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/qmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/sampling/stochastic_samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.144252 botorch-0.9.4/botorch/test_functions/
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/test_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/test_functions/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/test_functions/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)    49438 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/test_functions/multi_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/test_functions/multi_objective_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/test_functions/sensitivity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    34011 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/test_functions/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/test_functions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.148252 botorch-0.9.4/botorch/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/context_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24942 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/feasible_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    20040 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/gp_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/low_rank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.148252 botorch-0.9.4/botorch/utils/multi_objective/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/multi_objective/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.148252 botorch-0.9.4/botorch/utils/multi_objective/box_decompositions/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/multi_objective/box_decompositions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13382 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/multi_objective/box_decompositions/box_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/multi_objective/box_decompositions/dominated.py
--rw-r--r--   0 runner    (1001) docker     (127)    18402 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/multi_objective/box_decompositions/non_dominated.py
--rw-r--r--   0 runner    (1001) docker     (127)    12735 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/multi_objective/box_decompositions/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33719 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/multi_objective/hypervolume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/multi_objective/pareto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/multi_objective/scalarization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/objective.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.148252 botorch-0.9.4/botorch/utils/probability/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/probability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/probability/bvn.py
--rw-r--r--   0 runner    (1001) docker     (127)    22921 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/probability/lin_ess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/probability/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    16553 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/probability/mvnxpb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/probability/truncated_multivariate_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)    10727 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/probability/unified_skew_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11385 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/probability/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/rounding.py
--rw-r--r--   0 runner    (1001) docker     (127)    18143 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/safe_math.py
--rw-r--r--   0 runner    (1001) docker     (127)    35598 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)    17329 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12370 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-06 23:45:40.000000 botorch-0.9.4/botorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.116250 botorch-0.9.4/botorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2023-11-06 23:45:40.000000 botorch-0.9.4/botorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2023-11-06 23:45:41.000000 botorch-0.9.4/botorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 23:45:40.000000 botorch-0.9.4/botorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-11-06 23:45:40.000000 botorch-0.9.4/botorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-06 23:45:40.000000 botorch-0.9.4/botorch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    79395 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch_logo_lockup.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    63261 2023-11-06 23:42:27.000000 botorch-0.9.4/botorch_logo_lockup.svg
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-11-06 23:42:27.000000 botorch-0.9.4/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 23:45:41.152253 botorch-0.9.4/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2023-11-06 23:42:27.000000 botorch-0.9.4/notebooks/tutorials_performance_tracking.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-11-06 23:42:27.000000 botorch-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-11-06 23:42:27.000000 botorch-0.9.4/requirements-fmt.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-11-06 23:42:27.000000 botorch-0.9.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-11-06 23:45:41.156253 botorch-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2023-11-06 23:42:27.000000 botorch-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.591698 botorch-0.9.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.551698 botorch-0.9.5/.conda/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      436 2023-12-09 02:28:27.000000 botorch-0.9.5/.conda/build_conda.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-12-09 02:28:27.000000 botorch-0.9.5/.conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.551698 botorch-0.9.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.551698 botorch-0.9.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.551698 botorch-0.9.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/workflows/deploy_on_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/workflows/nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/workflows/reusable_tutorials.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/workflows/reusable_website.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/workflows/test_stable.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/workflows/tutorials_smoke_test_on_pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2023-12-09 02:28:27.000000 botorch-0.9.5/.github/workflows/tutorials_smoke_test_on_push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2023-12-09 02:28:27.000000 botorch-0.9.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    58387 2023-12-09 02:28:27.000000 botorch-0.9.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2023-12-09 02:28:27.000000 botorch-0.9.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2023-12-09 02:28:27.000000 botorch-0.9.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-12-09 02:28:27.000000 botorch-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-09 02:28:27.000000 botorch-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10982 2023-12-09 02:30:23.591698 botorch-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2023-12-09 02:28:27.000000 botorch-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.555698 botorch-0.9.5/botorch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.559698 botorch-0.9.5/botorch/acquisition/
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49881 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/cached_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/cost_aware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/decoupled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9439 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/fixed_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57306 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/input_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14981 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/joint_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26175 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/knowledge_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23074 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/logei.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42592 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/max_value_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39503 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/monte_carlo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.563698 botorch-0.9.5/botorch/acquisition/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/multi_objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/multi_objective/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25595 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/multi_objective/hypervolume_knowledge_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31296 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/multi_objective/joint_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22260 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/multi_objective/logei.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15942 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/multi_objective/max_value_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22135 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/multi_objective/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6613 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/multi_objective/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34674 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/multi_objective/multi_output_risk_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/multi_objective/objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48821 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/multi_objective/predictive_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15078 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/multi_objective/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29268 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/multi_step_lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24419 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14861 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/penalized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/predictive_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/prior_guided.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/proximal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12052 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/risk_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21048 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/acquisition/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/cross_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.563698 botorch-0.9.5/botorch/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/exceptions/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/exceptions/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16563 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.563698 botorch-0.9.5/botorch/generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21360 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/generation/gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15080 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/generation/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/generation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.567698 botorch-0.9.5/botorch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19333 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/approximate_gp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/contextual_multioutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17891 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7548 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22111 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18370 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/fully_bayesian_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13680 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/gp_regression_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/gp_regression_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35956 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/gpytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24087 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/higher_order_gp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.567698 botorch-0.9.5/botorch/models/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/kernels/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17647 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/kernels/contextual_lcea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/kernels/contextual_sac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/kernels/downsampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/kernels/exponential_decay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10226 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/kernels/linear_truncated_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12106 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/kernels/orthogonal_additive_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.567698 botorch-0.9.5/botorch/models/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/likelihoods/pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28754 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/model_list_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34230 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49300 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/pairwise_gp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.571698 botorch-0.9.5/botorch/models/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/transforms/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64166 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/transforms/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31087 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/transforms/outcome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/transforms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.571698 botorch-0.9.5/botorch/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13961 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/utils/assorted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/utils/gpytorch_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12753 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/utils/inducing_point_allocators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/models/utils/parse_training_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.571698 botorch-0.9.5/botorch/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.571698 botorch-0.9.5/botorch/optim/closures/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/closures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/closures/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/closures/model_closures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7463 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/homotopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53672 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58328 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/optimize_homotopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24289 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/parameter_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/stopping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.575698 botorch-0.9.5/botorch/optim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/utils/acquisition_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/optim/utils/timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.575698 botorch-0.9.5/botorch/posteriors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/posteriors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/posteriors/base_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/posteriors/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/posteriors/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/posteriors/fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14995 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/posteriors/gpytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11379 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/posteriors/higher_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12403 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/posteriors/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/posteriors/posterior.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/posteriors/posterior_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/posteriors/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/posteriors/transformed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.579698 botorch-0.9.5/botorch/sampling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/get_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/index_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/list_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/pairwise_samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.579698 botorch-0.9.5/botorch/sampling/pathwise/
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/pathwise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.579698 botorch-0.9.5/botorch/sampling/pathwise/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/pathwise/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/pathwise/features/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/pathwise/features/maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/pathwise/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/pathwise/posterior_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/pathwise/prior_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/pathwise/update_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/pathwise/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/qmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/sampling/stochastic_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.579698 botorch-0.9.5/botorch/test_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/test_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/test_functions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/test_functions/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49615 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/test_functions/multi_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/test_functions/multi_objective_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/test_functions/sensitivity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38180 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/test_functions/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/test_functions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.583698 botorch-0.9.5/botorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/context_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25552 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/feasible_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20012 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/gp_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/low_rank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.583698 botorch-0.9.5/botorch/utils/multi_objective/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/multi_objective/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.587698 botorch-0.9.5/botorch/utils/multi_objective/box_decompositions/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/multi_objective/box_decompositions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13382 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/multi_objective/box_decompositions/box_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/multi_objective/box_decompositions/dominated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18402 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/multi_objective/box_decompositions/non_dominated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12735 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/multi_objective/box_decompositions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33719 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/multi_objective/hypervolume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/multi_objective/pareto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/multi_objective/scalarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/objective.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.587698 botorch-0.9.5/botorch/utils/probability/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/probability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/probability/bvn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22921 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/probability/lin_ess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/probability/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16553 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/probability/mvnxpb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/probability/truncated_multivariate_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10727 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/probability/unified_skew_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11385 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/probability/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/rounding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18143 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/safe_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35598 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17329 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12322 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-09 02:30:23.000000 botorch-0.9.5/botorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.587698 botorch-0.9.5/botorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10982 2023-12-09 02:30:23.000000 botorch-0.9.5/botorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2023-12-09 02:30:23.000000 botorch-0.9.5/botorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 02:30:23.000000 botorch-0.9.5/botorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2023-12-09 02:30:23.000000 botorch-0.9.5/botorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-09 02:30:23.000000 botorch-0.9.5/botorch.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    79395 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch_logo_lockup.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    63261 2023-12-09 02:28:27.000000 botorch-0.9.5/botorch_logo_lockup.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-09 02:28:27.000000 botorch-0.9.5/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 02:30:23.587698 botorch-0.9.5/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2023-12-09 02:28:27.000000 botorch-0.9.5/notebooks/tutorials_performance_tracking.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-09 02:28:27.000000 botorch-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-09 02:28:27.000000 botorch-0.9.5/requirements-fmt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-09 02:28:27.000000 botorch-0.9.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2023-12-09 02:30:23.591698 botorch-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2023-12-09 02:28:27.000000 botorch-0.9.5/setup.py
```

### Comparing `botorch-0.9.4/.conda/meta.yaml` & `botorch-0.9.5/.conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/.github/ISSUE_TEMPLATE/bug_report.md` & `botorch-0.9.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/.github/ISSUE_TEMPLATE/feature_request.md` & `botorch-0.9.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/.github/ISSUE_TEMPLATE.md` & `botorch-0.9.5/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/.github/PULL_REQUEST_TEMPLATE.md` & `botorch-0.9.5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/.github/workflows/deploy_on_release.yml` & `botorch-0.9.5/.github/workflows/deploy_on_release.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/.github/workflows/docs.yml` & `botorch-0.9.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/.github/workflows/lint.yml` & `botorch-0.9.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/.github/workflows/nightly.yml` & `botorch-0.9.5/.github/workflows/nightly.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/.github/workflows/reusable_tutorials.yml` & `botorch-0.9.5/.github/workflows/reusable_tutorials.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/.github/workflows/reusable_website.yml` & `botorch-0.9.5/.github/workflows/reusable_website.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/.github/workflows/test.yml` & `botorch-0.9.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/.github/workflows/test_stable.yml` & `botorch-0.9.5/.github/workflows/test_stable.yml`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/.gitignore` & `botorch-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/CHANGELOG.md` & `botorch-0.9.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,37 @@
 # Changelog
 
 The release log for BoTorch.
 
+## [0.9.5] -- Dec 8, 2023
+
+#### New features
+
+Hypervolume Knowledge Gradient (HVKG):
+* Add `qHypervolumeKnowledgeGradient`, which seeks to maximize the difference in hypervolume of the hypervolume-maximizing set of a fixed size after conditioning the unknown observation(s) that would be received if X were evaluated (#1950, #1982, #2101).
+* Add tutorial on decoupled Multi-Objective Bayesian Optimization (MOBO) with HVKG (#2094).
+
+Other new features:
+* Add `MultiOutputFixedCostModel`, which is useful for decoupled scenarios where the objectives have different costs (#2093).
+* Enable `q > 1` in acquisition function optimization when nonlinear constraints are present (#1793).
+* Support different noise levels for different outputs in test functions (#2136).
+
+#### Bug fixes
+* Fix fantasization with a `FixedNoiseGaussianLikelihood` when `noise` is known and `X` is empty (#2090).
+* Make `LearnedObjective` compatible with constraints in acquisition functions regardless of `sample_shape` (#2111).
+* Make input constructors for `qExpectedImprovement`, `qLogExpectedImprovement`, and `qProbabilityOfImprovement` compatible with `LearnedObjective` regardless of `sample_shape` (#2115).
+* Fix handling of constraints in `qSimpleRegret` (#2141).
+
+#### Other changes
+* Increase default sample size for `LearnedObjective` (#2095).
+* Allow passing in `X` with or without fidelity dimensions in `project_to_target_fidelity` (#2102).
+* Use full-rank task covariance matrix by default in SAAS MTGP (#2104).
+* Rename `FullyBayesianPosterior` to `GaussianMixturePosterior`; add `_is_ensemble` and `_is_fully_bayesian` attributes to `Model` (#2108).
+* Various improvements to tutorials including speedups, improved explanations, and compatibility with newer versions of libraries.
+
 
 ## [0.9.4] - Nov 6, 2023
 
 #### Compatibility
 * Re-establish compatibility with PyTorch 1.13.1 (#2083).
```

### Comparing `botorch-0.9.4/CODE_OF_CONDUCT.md` & `botorch-0.9.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/CONTRIBUTING.md` & `botorch-0.9.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/LICENSE` & `botorch-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/PKG-INFO` & `botorch-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botorch
-Version: 0.9.4
+Version: 0.9.5
 Summary: Bayesian Optimization in PyTorch
 Home-page: https://botorch.org
 Author: Meta Platforms, Inc.
 License: MIT
 Project-URL: Documentation, https://botorch.org
 Project-URL: Source, https://github.com/pytorch/botorch
 Project-URL: conda, https://anaconda.org/pytorch/botorch
@@ -28,15 +28,15 @@
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: ufmt; extra == "dev"
 Requires-Dist: flake8-docstrings; extra == "dev"
 Requires-Dist: black==22.3.0; extra == "dev"
 Requires-Dist: usort==1.0.2; extra == "dev"
-Requires-Dist: sphinx<=7.1.2; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: tutorials
 Requires-Dist: ax-platform; extra == "tutorials"
 Requires-Dist: cma; extra == "tutorials"
 Requires-Dist: jupyter; extra == "tutorials"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botorch Version: 0.9.4 Summary: Bayesian
+Metadata-Version: 2.1 Name: botorch Version: 0.9.5 Summary: Bayesian
 Optimization in PyTorch Home-page: https://botorch.org Author: Meta Platforms,
 Inc. License: MIT Project-URL: Documentation, https://botorch.org Project-URL:
 Source, https://github.com/pytorch/botorch Project-URL: conda, https://
 anaconda.org/pytorch/botorch Keywords: Bayesian optimization,PyTorch
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering Classifier: Intended Audience ::
@@ -10,23 +10,23 @@
 >=3.9 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: multipledispatch Requires-Dist: scipy Requires-Dist: torch>=1.13.1
 Requires-Dist: pyro-ppl>=1.8.4 Requires-Dist: gpytorch==1.11 Requires-Dist:
 linear_operator==0.5.1 Provides-Extra: dev Requires-Dist: pytest; extra ==
 "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: flake8; extra ==
 "dev" Requires-Dist: ufmt; extra == "dev" Requires-Dist: flake8-docstrings;
 extra == "dev" Requires-Dist: black==22.3.0; extra == "dev" Requires-Dist:
-usort==1.0.2; extra == "dev" Requires-Dist: sphinx<=7.1.2; extra == "dev"
-Provides-Extra: test Requires-Dist: pytest; extra == "test" Requires-Dist:
-pytest-cov; extra == "test" Provides-Extra: tutorials Requires-Dist: ax-
-platform; extra == "tutorials" Requires-Dist: cma; extra == "tutorials"
-Requires-Dist: jupyter; extra == "tutorials" Requires-Dist: kaleido; extra ==
-"tutorials" Requires-Dist: matplotlib; extra == "tutorials" Requires-Dist:
-memory_profiler; extra == "tutorials" Requires-Dist: papermill; extra ==
-"tutorials" Requires-Dist: pykeops; extra == "tutorials" Requires-Dist:
-torchvision; extra == "tutorials" _[_B_o_T_o_r_c_h_ _L_o_g_o_]
+usort==1.0.2; extra == "dev" Requires-Dist: sphinx; extra == "dev" Provides-
+Extra: test Requires-Dist: pytest; extra == "test" Requires-Dist: pytest-cov;
+extra == "test" Provides-Extra: tutorials Requires-Dist: ax-platform; extra ==
+"tutorials" Requires-Dist: cma; extra == "tutorials" Requires-Dist: jupyter;
+extra == "tutorials" Requires-Dist: kaleido; extra == "tutorials" Requires-
+Dist: matplotlib; extra == "tutorials" Requires-Dist: memory_profiler; extra ==
+"tutorials" Requires-Dist: papermill; extra == "tutorials" Requires-Dist:
+pykeops; extra == "tutorials" Requires-Dist: torchvision; extra == "tutorials"
+_[_B_o_T_o_r_c_h_ _L_o_g_o_]
 ===============================================================================
 [![Support Ukraine](https://img.shields.io/badge/Support-Ukraine-
 FFD500?style=flat&labelColor=005BBB)](https://opensource.fb.com/support-
 ukraine) [![Lint](https://github.com/pytorch/botorch/workflows/Lint/badge.svg)]
 (https://github.com/pytorch/botorch/actions?query=workflow%3ALint) [![Test]
 (https://github.com/pytorch/botorch/workflows/Test/badge.svg)](https://
 github.com/pytorch/botorch/actions?query=workflow%3ATest) [![Docs](https://
```

### Comparing `botorch-0.9.4/README.md` & `botorch-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/__init__.py` & `botorch-0.9.5/botorch/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,17 +26,19 @@
     gen_candidates_torch,
     get_best_candidates,
 )
 from botorch.logging import logger
 from botorch.utils import manual_seed
 
 try:
-    from botorch.version import version as __version__
+    # Marking this as a manual import to avoid autodeps complaints
+    # due to imports from non-existent file.
+    from botorch.version import version as __version__  # @manual
 except Exception:  # pragma: no cover
-    __version__ = "Unknown"  # pragma: no cover
+    __version__ = "Unknown"
 
 logger.info(
     "Turning off `fast_computations` in linear operator and increasing "
     "`max_cholesky_size` and `max_eager_kernel_size` to 4096, and "
     "`cholesky_max_tries` to 6. The approximate computations available in "
     "GPyTorch aim to speed up GP training and inference in large data "
     "regime but they are generally not robust enough to be used in a BO-loop. "
```

### Comparing `botorch-0.9.4/botorch/acquisition/__init__.py` & `botorch-0.9.5/botorch/acquisition/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/acquisition/acquisition.py` & `botorch-0.9.5/botorch/acquisition/acquisition.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     Abstract base class for acquisition functions using one-shot optimization
 
     :meta private:
     """
 
     @abstractmethod
     def get_augmented_q_batch_size(self, q: int) -> int:
-        r"""Get augmented q batch size for one-shot optimziation.
+        r"""Get augmented q batch size for one-shot optimization.
 
         Args:
             q: The number of candidates to consider jointly.
 
         Returns:
             The augmented size for one-shot optimization (including variables
             parameterizing the fantasy solutions).
```

### Comparing `botorch-0.9.4/botorch/acquisition/active_learning.py` & `botorch-0.9.5/botorch/acquisition/active_learning.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             # We use q=1 here b/c ScalarizedObjective currently does not fully exploit
             # LinearOperator operations and thus may be slow / overly memory-hungry.
             # TODO (T52818288): Properly use LinearOperators in scalarize_posterior
             mc_points = self.mc_points.view(-1, *bdims, 1, X.size(-1))
         else:
             # While we only need marginal variances, we can evaluate for q>1
             # b/c for GPyTorch models lazy evaluation can make this quite a bit
-            # faster than evaluting in t-batch mode with q-batch size of 1
+            # faster than evaluating in t-batch mode with q-batch size of 1
             mc_points = self.mc_points.view(*bdims, -1, X.size(-1))
 
         # evaluate the posterior at the grid points
         with settings.propagate_grads(True):
             posterior = fantasy_model.posterior(
                 mc_points, posterior_transform=self.posterior_transform
             )
```

### Comparing `botorch-0.9.4/botorch/acquisition/analytic.py` & `botorch-0.9.5/botorch/acquisition/analytic.py`

 * *Files 0% similar despite different names*

```diff
@@ -982,15 +982,15 @@
     log_ei_upper = _ei_helper(u_upper).log()
 
     # When u <= bound, we need to be more careful and rearrange the EI formula as
     # log(phi(u)) + log(1 - exp(w)), where w = log(abs(u) * Phi(u) / phi(u)).
     # To this end, a second branch is necessary, depending on whether or not u is
     # smaller than approximately the negative inverse square root of the machine
     # precision. Below this point, numerical issues in computing log(1 - exp(w)) occur
-    # as w approches zero from below, even though the relative contribution to log_ei
+    # as w approaches zero from below, even though the relative contribution to log_ei
     # vanishes in machine precision at that point.
     neg_inv_sqrt_eps = -1e6 if u.dtype == torch.float64 else -1e3
 
     # mask u for to avoid NaNs in gradients in first and second branch
     u_lower = u.masked_fill(u > bound, bound)
     u_eps = u_lower.masked_fill(u < neg_inv_sqrt_eps, neg_inv_sqrt_eps)
     # compute the logarithm of abs(u) * Phi(u) / phi(u) for moderately large negative u
```

### Comparing `botorch-0.9.4/botorch/acquisition/cached_cholesky.py` & `botorch-0.9.5/botorch/acquisition/cached_cholesky.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 r"""
 Abstract class for acquisition functions leveraging a cached Cholesky
-decomposition of the posterior covaiance over f(X_baseline).
+decomposition of the posterior covariance over f(X_baseline).
 """
 from __future__ import annotations
 
 import warnings
 from typing import Optional
 
 import torch
@@ -103,17 +103,17 @@
         @cached decorator, this function is doing a lot implicitly:
 
         1) Check if a root decomposition has already been cached to `lazy_covar`.
           Note that it will not have been if `posterior.mvn` is a
           `MultitaskMultivariateNormal`, since we construct `lazy_covar` in that
           case.
         2) If the root decomposition has not been found in the cache, compute it.
-        3) Write it to the cache of `lazy_covar`. Note that this will become inacessible
-          if `posterior.mvn` is a `MultitaskMultivariateNormal`, since in that case
-          `lazy_covar`'s scope is only this function.
+        3) Write it to the cache of `lazy_covar`. Note that this will become
+          inaccessible if `posterior.mvn` is a `MultitaskMultivariateNormal`,
+          since in that case `lazy_covar`'s scope is only this function.
 
         Args:
             posterior: The posterior over f(X_baseline).
         """
         if isinstance(posterior.distribution, MultitaskMultivariateNormal):
             lazy_covar = extract_batch_covar(posterior.distribution)
         else:
```

### Comparing `botorch-0.9.4/botorch/acquisition/cost_aware.py` & `botorch-0.9.5/botorch/acquisition/cost_aware.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     def __init__(
         self,
         cost_model: Union[DeterministicModel, GPyTorchModel],
         use_mean: bool = True,
         cost_objective: Optional[MCAcquisitionObjective] = None,
         min_cost: float = 1e-2,
     ) -> None:
-        r"""Cost-aware utility that weights increase in utiltiy by inverse cost.
+        r"""Cost-aware utility that weights increase in utility by inverse cost.
 
         Args:
             cost_model: A model of the cost of evaluating a candidate
                 set `X`, where `X` are the same features as in the model for the
                 acquisition function this is to be used with. If no cost_objective
                 is specified, the outputs are required to be non-negative.
             use_mean: If True, use the posterior mean, otherwise use posterior
@@ -118,15 +118,15 @@
                 un-transform predictions/samples of a cost model fit on the
                 log-transformed cost (often done to ensure non-negativity). If the
                 cost model is multi-output, then by default this will sum the cost
                 across outputs.
             min_cost: A value used to clamp the cost samples so that they are not
                 too close to zero, which may cause numerical issues.
         Returns:
-            The inverse-cost-weighted utiltiy.
+            The inverse-cost-weighted utility.
         """
         super().__init__()
         if cost_objective is None:
             if cost_model.num_outputs == 1:
                 cost_objective = IdentityMCObjective()
             else:
                 # sum over outputs
@@ -162,18 +162,18 @@
             A `num_fantasies x batch_shape`-dim Tensor of cost-weighted utilities.
         """
         if not self._use_mean and sampler is None:
             raise RuntimeError("Must provide `sampler` if `use_mean=False`")
         if X_evaluation_mask is not None:
             # TODO: support different evaluation masks for each X. This requires
             # either passing evaluation_mask to `cost_model.posterior`
-            # or assuming that evalauting `cost_model.posterior(X)` on all
+            # or assuming that evaluating `cost_model.posterior(X)` on all
             # `q` points and then only selecting the costs for relevant points
             # does not change the cost function for each point. This would not be
-            # true for instance if the incremental cost of evalauting an additional
+            # true for instance if the incremental cost of evaluating an additional
             # point decreased as the number of points increased.
             if not all(
                 torch.equal(X_evaluation_mask[0], X_evaluation_mask[i])
                 for i in range(1, X_evaluation_mask.shape[0])
             ):
                 raise NotImplementedError(
                     "Currently, all candidates must be evaluated on the same outputs."
```

### Comparing `botorch-0.9.4/botorch/acquisition/decoupled.py` & `botorch-0.9.5/botorch/acquisition/decoupled.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/acquisition/factory.py` & `botorch-0.9.5/botorch/acquisition/factory.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/acquisition/fixed_feature.py` & `botorch-0.9.5/botorch/acquisition/fixed_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 r"""
-A wrapper around AquisitionFunctions to fix certain features for optimization.
+A wrapper around AcquisitionFunctions to fix certain features for optimization.
 This is useful e.g. for performing contextual optimization.
 """
 
 from __future__ import annotations
 
 from numbers import Number
 from typing import List, Optional, Sequence, Union
@@ -46,15 +46,15 @@
         return hasattr(value, "device") and value.device == torch.device("cuda")
 
     any_cuda = any(_is_cuda(value) for value in values)
     return torch.device("cuda") if any_cuda else torch.device("cpu")
 
 
 class FixedFeatureAcquisitionFunction(AcquisitionFunction):
-    """A wrapper around AquisitionFunctions to fix a subset of features.
+    """A wrapper around AcquisitionFunctions to fix a subset of features.
 
     Example:
         >>> model = SingleTaskGP(train_X, train_Y)  # d = 5
         >>> qEI = qExpectedImprovement(model, best_f=0.0)
         >>> columns = [2, 4]
         >>> values = X[..., columns]
         >>> qEI_FF = FixedFeatureAcquisitionFunction(qEI, 5, columns, values)
```

### Comparing `botorch-0.9.4/botorch/acquisition/input_constructors.py` & `botorch-0.9.5/botorch/acquisition/input_constructors.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,23 +77,25 @@
 from botorch.acquisition.multi_objective.objective import (
     AnalyticMultiOutputObjective,
     IdentityAnalyticMultiOutputObjective,
     IdentityMCMultiOutputObjective,
 )
 from botorch.acquisition.multi_objective.utils import get_default_partitioning_alpha
 from botorch.acquisition.objective import (
+    ConstrainedMCObjective,
     IdentityMCObjective,
     MCAcquisitionObjective,
     PosteriorTransform,
 )
 from botorch.acquisition.preference import AnalyticExpectedUtilityOfBestOption
 from botorch.acquisition.risk_measures import RiskMeasureMCObjective
 from botorch.acquisition.utils import (
     compute_best_feasible_objective,
     expand_trace_observations,
+    get_infeasible_cost,
     get_optimal_samples,
     project_to_target_fidelity,
 )
 from botorch.exceptions.errors import UnsupportedError
 from botorch.models.cost import AffineFidelityCostModel
 from botorch.models.deterministic import FixedSingleSampleModel
 from botorch.models.gpytorch import GPyTorchModel
@@ -177,15 +179,15 @@
     field = getattr(dataset, fieldname)
     return transform(field) if transform else field
 
 
 def get_acqf_input_constructor(
     acqf_cls: Type[AcquisitionFunction],
 ) -> Callable[..., Dict[str, Any]]:
-    r"""Get acqusition function input constructor from registry.
+    r"""Get acquisition function input constructor from registry.
 
     Args:
         acqf_cls: The AcquisitionFunction class (not instance) for which
             to retrieve the input constructor.
 
     Returns:
         The input constructor associated with `acqf_cls`.
@@ -429,31 +431,51 @@
 @acqf_input_constructor(qSimpleRegret)
 def construct_inputs_qSimpleRegret(
     model: Model,
     objective: Optional[MCAcquisitionObjective] = None,
     posterior_transform: Optional[PosteriorTransform] = None,
     X_pending: Optional[Tensor] = None,
     sampler: Optional[MCSampler] = None,
+    constraints: Optional[List[Callable[[Tensor], Tensor]]] = None,
+    X_baseline: Optional[Tensor] = None,
 ) -> Dict[str, Any]:
     r"""Construct kwargs for qSimpleRegret.
 
     Args:
         model: The model to be used in the acquisition function.
         objective: The objective to be used in the acquisition function.
         posterior_transform: The posterior transform to be used in the
             acquisition function.
         X_pending: A `batch_shape, m x d`-dim Tensor of `m` design points
             that have points that have been submitted for function evaluation
             but have not yet been evaluated.
         sampler: The sampler used to draw base samples. If omitted, uses
             the acquisition functions's default sampler.
+        constraints: A list of constraint callables which map a Tensor of posterior
+            samples of dimension `sample_shape x batch-shape x q x m`-dim to a
+            `sample_shape x batch-shape x q`-dim Tensor. The associated constraints
+            are considered satisfied if the output is less than zero.
+        X_baseline: A `batch_shape x r x d`-dim Tensor of `r` design points
+            that have already been observed. These points are considered as
+            the potential best design point. If omitted, checks that all
+            training_data have the same input features and take the first `X`.
 
     Returns:
         A dict mapping kwarg names of the constructor to values.
     """
+    if constraints is not None:
+        if X_baseline is None:
+            raise ValueError("Constraints require an X_baseline.")
+        objective = ConstrainedMCObjective(
+            objective=objective,
+            constraints=constraints,
+            infeasible_cost=get_infeasible_cost(
+                X=X_baseline, model=model, objective=objective
+            ),
+        )
     return {
         "model": model,
         "objective": objective,
         "posterior_transform": posterior_transform,
         "X_pending": X_pending,
         "sampler": sampler,
     }
@@ -856,15 +878,15 @@
 
     alpha = (
         get_default_partitioning_alpha(num_objectives=num_objectives)
         if alpha is None
         else alpha
     )
     # This selects the objectives (a subset of the outcomes) and set each
-    # objective threhsold to have the proper optimization direction.
+    # objective threshold to have the proper optimization direction.
     if objective is None:
         objective = IdentityAnalyticMultiOutputObjective()
     if isinstance(objective, RiskMeasureMCObjective):
         pre_obj = objective.preprocessing_function
     else:
         pre_obj = objective
     ref_point = pre_obj(objective_thresholds)
@@ -917,15 +939,15 @@
     )
 
     # compute posterior mean (for ref point computation ref pareto frontier)
     with torch.no_grad():
         Y_pmean = model.posterior(X).mean
     # For HV-based acquisition functions we pass the constraint transform directly
     if constraints is not None:
-        # Adjust `Y_pmean` to contrain feasible points only.
+        # Adjust `Y_pmean` to contain feasible points only.
         feas = torch.stack([c(Y_pmean) <= 0 for c in constraints], dim=-1).all(dim=-1)
         Y_pmean = Y_pmean[feas]
 
     if objective is None:
         objective = IdentityMCMultiOutputObjective()
 
     ehvi_kwargs = construct_inputs_EHVI(
@@ -978,15 +1000,15 @@
         X_baseline = _get_dataset_field(
             training_data,
             fieldname="X",
             first_only=True,
             assert_shared=True,
         )
     # This selects the objectives (a subset of the outcomes) and set each
-    # objective threhsold to have the proper optimization direction.
+    # objective threshold to have the proper optimization direction.
     if objective is None:
         objective = IdentityMCMultiOutputObjective()
 
     if constraints is not None:
         if isinstance(objective, RiskMeasureMCObjective):
             raise UnsupportedError(
                 "Outcome constraints are not supported with risk measures. "
@@ -1317,14 +1339,32 @@
 def get_best_f_mc(
     training_data: MaybeDict[SupervisedDataset],
     objective: Optional[MCAcquisitionObjective] = None,
     posterior_transform: Optional[PosteriorTransform] = None,
     constraints: Optional[List[Callable[[Tensor], Tensor]]] = None,
     model: Optional[Model] = None,
 ) -> Tensor:
+    """
+    Computes the maximum value of the objective over the training data.
+
+    Args:
+        training_data: Has fields Y, which is evaluated by `objective`, and X,
+            which is used as `X_baseline`. `Y` is of shape
+            `batch_shape x q x m`.
+        objective: The objective under which to evaluate the training data. If
+            omitted, uses `IdentityMCObjective`.
+        posterior_transform: An optional PosteriorTransform to apply to `Y`
+            before computing the objective.
+        constraints: For assessing feasibility.
+        model: Used by `compute_best_feasible_objective` when there are no
+            feasible observations.
+
+    Returns:
+        A Tensor of shape `batch_shape`.
+    """
     if isinstance(training_data, dict) and not _field_is_shared(
         training_data, fieldname="X"
     ):
         raise NotImplementedError("Currently only block designs are supported.")
 
     X_baseline = _get_dataset_field(
         training_data,
@@ -1333,41 +1373,49 @@
         first_only=True,
     )
 
     Y = _get_dataset_field(
         training_data,
         fieldname="Y",
         join_rule=lambda field_tensors: torch.cat(field_tensors, dim=-1),
-    )  # batch_shape x n x d
+    )  # batch_shape x q x m
 
     if posterior_transform is not None:
         # retain the original tensor dimension since objective expects explicit
         # output dimension.
         Y_dim = Y.dim()
         Y = posterior_transform.evaluate(Y)
         if Y.dim() < Y_dim:
             Y = Y.unsqueeze(-1)
     if objective is None:
         if Y.shape[-1] > 1:
             raise UnsupportedError(
                 "Acquisition functions require an objective when "
-                "used with multi-output models (execpt for multi-objective"
+                "used with multi-output models (except for multi-objective"
                 "acquisition functions)."
             )
         objective = IdentityMCObjective()
-    obj = objective(Y, X=X_baseline)  # batch_shape x n
+    # `Y` is of shape `(batch_shape) x q x m`; `MCAcquisitionObjective`s expect
+    # inputs `sample_shape x (batch_shape) x q x m`.
+    # For most objectives, `obj` will have shape `1 x (batch_shape) x q`, but
+    # with a `LearnedObjective` it can be `num_samples x (batch_shape) x q`.
+    obj = objective(Y.unsqueeze(0), X=X_baseline)
+    if obj.shape[0] > 1:
+        obj = obj.mean(dim=0)
+    else:
+        obj = obj.squeeze(0)
     return compute_best_feasible_objective(
         samples=Y,
         obj=obj,
         constraints=constraints,
         model=model,
         objective=objective,
         posterior_transform=posterior_transform,
         X_baseline=X_baseline,
-    )
+    ).squeeze()
 
 
 def optimize_objective(
     model: Model,
     bounds: Tensor,
     q: int,
     objective: Optional[MCAcquisitionObjective] = None,
@@ -1440,18 +1488,18 @@
     if linear_constraints is None:
         inequality_constraints = None
     else:
         A, b = linear_constraints
         inequality_constraints = []
         k, d = A.shape
         for i in range(k):
-            indicies = A[i, :].nonzero(as_tuple=False).squeeze()
-            coefficients = -A[i, indicies]
+            indices = A[i, :].nonzero(as_tuple=False).squeeze()
+            coefficients = -A[i, indices]
             rhs = -b[i, 0]
-            inequality_constraints.append((indicies, coefficients, rhs))
+            inequality_constraints.append((indices, coefficients, rhs))
 
     return optimize_acqf(
         acq_function=acq_function,
         bounds=free_feature_bounds,
         q=q,
         num_restarts=optimizer_options.get("num_restarts", 60),
         raw_samples=optimizer_options.get("raw_samples", 1024),
```

### Comparing `botorch-0.9.4/botorch/acquisition/joint_entropy_search.py` & `botorch-0.9.5/botorch/acquisition/joint_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/acquisition/knowledge_gradient.py` & `botorch-0.9.5/botorch/acquisition/knowledge_gradient.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
 
                 `X_fantasies = X[..., -num_fantasies:, :]`
                 `X_fantasies.shape = b x num_fantasies x d`
 
                 `X_actual = X[..., :-num_fantasies, :]`
                 `X_actual.shape = b x q x d`
 
-                In addition, `X` may be augmented with fidelity parameteres as
+                In addition, `X` may be augmented with fidelity parameters as
                 part of thee `d`-dimension. Projecting fidelities to the target
                 fidelity is handled by `project`.
 
         Returns:
             A Tensor of shape `b`. For t-batch b, the q-KG value of the design
                 `X_actual[b]` is averaged across the fantasy models, where
                 `X_fantasies[b, i]` is chosen as the final selection for the
```

### Comparing `botorch-0.9.4/botorch/acquisition/logei.py` & `botorch-0.9.5/botorch/acquisition/logei.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/acquisition/max_value_entropy_search.py` & `botorch-0.9.5/botorch/acquisition/max_value_entropy_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
     @abstractmethod
     def _sample_max_values(
         self, num_samples: int, X_pending: Optional[Tensor] = None
     ) -> Tensor:
         r"""Draw samples from the posterior over maximum values.
 
-        These samples are used to compute Monte Carlo approximations of expecations
+        These samples are used to compute Monte Carlo approximations of expectations
         over the posterior over the function maximum.
 
         Args:
             num_samples: The number of samples to draw.
             X_pending: A `m x d`-dim Tensor of `m` design points that have been
                 submitted for function evaluation but have not yet been evaluated.
 
@@ -253,15 +253,15 @@
         )
 
     def _sample_max_values(
         self, num_samples: int, X_pending: Optional[Tensor] = None
     ) -> Tensor:
         r"""Draw samples from the posterior over maximum values on a discrete set.
 
-        These samples are used to compute Monte Carlo approximations of expecations
+        These samples are used to compute Monte Carlo approximations of expectations
         over the posterior over the function maximum.
 
         Args:
             num_samples: The number of samples to draw.
             X_pending: A `m x d`-dim Tensor of `m` design points that have been
                 submitted for function evaluation but have not yet been evaluated.
 
@@ -592,36 +592,36 @@
         check_no_nans(ratio)
 
         # prepare squared correlation between current and target fidelity
         rhos_squared = torch.pow(covar_mM.squeeze(-1), 2) / (variance_m * variance_M)
         # batch_shape x 1
         check_no_nans(rhos_squared)
 
-        # calculate quality contribution to the GIBBON acqusition function
+        # calculate quality contribution to the GIBBON acquisition function
         inner_term = 1 - rhos_squared * ratio * (normalized_mvs + ratio)
         acq = -0.5 * inner_term.clamp_min(CLAMP_LB).log()
         # average over posterior max samples
         acq = acq.mean(dim=1).unsqueeze(0)
 
         if self.X_pending is None:
-            # for q=1, no replusion term required
+            # for q=1, no repulsion term required
             return acq
 
         # for q>1 GIBBON requires repulsion terms r_i, where
         # r_i = log |C_i| for the predictive
         # correlation matricies C_i between each candidate point in X and
         # the m current batch elements in X_pending.
 
         # Each predictive covariance matrix can be expressed as
         # V_i = [[v_i, A_i], [A_i,B]] for a shared m x m tensor B.
-        # So we can efficientely calculate |V_i| using the formula for
+        # So we can efficiently calculate |V_i| using the formula for
         # determinant of block matricies, i.e.
         # |V_i| = (v_i - A_i^T * B^{-1} * A_i) * |B|
         # As the |B| term does not depend on X and we later take its log,
-        # it provides only a translation of the acqusition function surface
+        # it provides only a translation of the acquisition function surface
         # and can thus be ignored.
 
         if self.posterior_transform is not None:
             raise UnsupportedError(
                 "qLowerBoundMaxValueEntropy does not support PosteriorTransforms"
                 "when X_pending is not None."
             )
```

### Comparing `botorch-0.9.4/botorch/acquisition/monte_carlo.py` & `botorch-0.9.5/botorch/acquisition/monte_carlo.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     IdentityMCObjective,
     MCAcquisitionObjective,
     PosteriorTransform,
 )
 from botorch.acquisition.utils import (
     compute_best_feasible_objective,
     prune_inferior_points,
+    repeat_to_match_aug_dim,
 )
 from botorch.exceptions.errors import UnsupportedError
 from botorch.models.model import Model
 from botorch.sampling.base import MCSampler
 from botorch.utils.objective import compute_smoothed_feasibility_indicator
 from botorch.utils.transforms import (
     concatenate_pending_points,
@@ -115,15 +116,16 @@
             samples with shape `sample_shape x batch_shape x q x m`, and `obj` is a
             tensor of MC objective values with shape `sample_shape x batch_shape x q`.
         """
         posterior = self.model.posterior(
             X=X, posterior_transform=self.posterior_transform
         )
         samples = self.get_posterior_samples(posterior)
-        return samples, self.objective(samples=samples, X=X)
+        obj = self.objective(samples=samples, X=X)
+        return samples, obj
 
     @abstractmethod
     def forward(self, X: Tensor) -> Tensor:
         r"""Takes in a `batch_shape x q x d` X Tensor of t-batches with `q` `d`-dim
         design points each, and returns a Tensor with shape `batch_shape'`, where
         `batch_shape'` is the broadcasted batch shape of model and input `X`. Should
         utilize the result of `set_X_pending` as needed to account for pending function
@@ -279,14 +281,15 @@
             X: A `batch_shape x q x d` Tensor of t-batches with `q` `d`-dim
                 design points each.
 
         Returns:
             A Tensor with shape `sample_sample x batch_shape x q`.
         """
         samples, obj = self._get_samples_and_objectives(X)
+        samples = repeat_to_match_aug_dim(target_tensor=samples, reference_tensor=obj)
         acqval = self._sample_forward(obj)  # `sample_sample x batch_shape x q`
         return self._apply_constraints(acqval=acqval, samples=samples)
 
     @abstractmethod
     def _sample_forward(self, obj: Tensor) -> Tensor:
         """Evaluates the acquisition utility per MC sample based on objective value obj.
         Should utilize the result of `set_X_pending` as needed to account for pending
@@ -597,23 +600,23 @@
         if not self._cache_root:
             samples_full = super().get_posterior_samples(posterior)
             samples = samples_full[..., -q:, :]
             obj_full = self.objective(samples_full, X=X_full)
             # assigning baseline buffers so `best_f` can be computed in _sample_forward
             self.baseline_obj, obj = obj_full[..., :-q], obj_full[..., -q:]
             self.baseline_samples = samples_full[..., :-q, :]
-            return samples, obj
+        else:
+            # handle one-to-many input transforms
+            n_plus_q = X_full.shape[-2]
+            n_w = posterior._extended_shape()[-2] // n_plus_q
+            q_in = q * n_w
+            self._set_sampler(q_in=q_in, posterior=posterior)
+            samples = self._get_f_X_samples(posterior=posterior, q_in=q_in)
+            obj = self.objective(samples, X=X_full[..., -q:, :])
 
-        # handle one-to-many input transforms
-        n_plus_q = X_full.shape[-2]
-        n_w = posterior._extended_shape()[-2] // n_plus_q
-        q_in = q * n_w
-        self._set_sampler(q_in=q_in, posterior=posterior)
-        samples = self._get_f_X_samples(posterior=posterior, q_in=q_in)
-        obj = self.objective(samples, X=X_full[..., -q:, :])
         return samples, obj
 
     def _compute_best_feasible_objective(self, samples: Tensor, obj: Tensor) -> Tensor:
         r"""Computes best feasible objective value from samples.
 
         Args:
             samples: `sample_shape x batch_shape x q x m`-dim posterior samples.
@@ -635,15 +638,15 @@
 
 class qProbabilityOfImprovement(SampleReducingMCAcquisitionFunction):
     r"""MC-based batch Probability of Improvement.
 
     Estimates the probability of improvement over the current best observed
     value by sampling from the joint posterior distribution of the q-batch.
     MC-based estimates of a probability involves taking expectation of an
-    indicator function; to support auto-differntiation, the indicator is
+    indicator function; to support auto-differentiation, the indicator is
     replaced with a sigmoid function with temperature parameter `tau`.
 
     `qPI(X) = P(max Y >= best_f), Y ~ f(X), X = (x_1,...,x_q)`
 
     Example:
         >>> model = SingleTaskGP(train_X, train_Y)
         >>> best_f = train_Y.max()[0]
@@ -722,21 +725,62 @@
 class qSimpleRegret(SampleReducingMCAcquisitionFunction):
     r"""MC-based batch Simple Regret.
 
     Samples from the joint posterior over the q-batch and computes the simple regret.
 
     `qSR(X) = E(max Y), Y ~ f(X), X = (x_1,...,x_q)`
 
+    Constraints should be provided as a `ConstrainedMCObjective`.
+    Passing `constraints` as an argument is not supported. This is because
+    `SampleReducingMCAcquisitionFunction` computes the acquisition values on the sample
+    level and then weights the sample-level acquisition values by a soft feasibility
+    indicator. Hence, it expects non-log acquisition function values to be
+    non-negative. `qSimpleRegret` acquisition values can be negative, so we instead use
+    a `ConstrainedMCObjective` which applies constraints to the objectives (e.g. before
+    computing the acquisition function) and shifts negative objective values using
+    by an infeasible cost to ensure non-negativity (before applying constraints and
+    shifting them back).
+
     Example:
         >>> model = SingleTaskGP(train_X, train_Y)
         >>> sampler = SobolQMCNormalSampler(1024)
         >>> qSR = qSimpleRegret(model, sampler)
         >>> qsr = qSR(test_X)
     """
 
+    def __init__(
+        self,
+        model: Model,
+        sampler: Optional[MCSampler] = None,
+        objective: Optional[MCAcquisitionObjective] = None,
+        posterior_transform: Optional[PosteriorTransform] = None,
+        X_pending: Optional[Tensor] = None,
+    ) -> None:
+        r"""q-Simple Regret.
+
+        Args:
+            model: A fitted model.
+            sampler: The sampler used to draw base samples. See `MCAcquisitionFunction`
+                more details.
+            objective: The MCAcquisitionObjective under which the samples are
+                evaluated. Defaults to `IdentityMCObjective()`.
+            posterior_transform: A PosteriorTransform (optional).
+            X_pending:  A `m x d`-dim Tensor of `m` design points that have
+                points that have been submitted for function evaluation
+                but have not yet been evaluated.  Concatenated into X upon
+                forward call.  Copied and set to have no gradient.
+        """
+        super().__init__(
+            model=model,
+            sampler=sampler,
+            objective=objective,
+            posterior_transform=posterior_transform,
+            X_pending=X_pending,
+        )
+
     def _sample_forward(self, obj: Tensor) -> Tensor:
         r"""Evaluate qSimpleRegret per sample on the candidate set `X`.
 
         Args:
             obj: A `sample_shape x batch_shape x q`-dim Tensor of MC objective values.
 
         Returns:
@@ -750,14 +794,25 @@
 
     Uses a reparameterization to extend UCB to qUCB for q > 1 (See Appendix A
     of [Wilson2017reparam].)
 
     `qUCB = E(max(mu + |Y_tilde - mu|))`, where `Y_tilde ~ N(mu, beta pi/2 Sigma)`
     and `f(X)` has distribution `N(mu, Sigma)`.
 
+    Constraints should be provided as a `ConstrainedMCObjective`.
+    Passing `constraints` as an argument is not supported. This is because
+    `SampleReducingMCAcquisitionFunction` computes the acquisition values on the sample
+    level and then weights the sample-level acquisition values by a soft feasibility
+    indicator. Hence, it expects non-log acquisition function values to be
+    non-negative. `qSimpleRegret` acquisition values can be negative, so we instead use
+    a `ConstrainedMCObjective` which applies constraints to the objectives (e.g. before
+    computing the acquisition function) and shifts negative objective values using
+    by an infeasible cost to ensure non-negativity (before applying constraints and
+    shifting them back).
+
     Example:
         >>> model = SingleTaskGP(train_X, train_Y)
         >>> sampler = SobolQMCNormalSampler(1024)
         >>> qUCB = qUpperConfidenceBound(model, 0.1, sampler)
         >>> qucb = qUCB(test_X)
     """
```

### Comparing `botorch-0.9.4/botorch/acquisition/multi_objective/__init__.py` & `botorch-0.9.5/botorch/acquisition/multi_objective/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from botorch.acquisition.multi_objective.analytic import (
     ExpectedHypervolumeImprovement,
     MultiObjectiveAnalyticAcquisitionFunction,
 )
+from botorch.acquisition.multi_objective.hypervolume_knowledge_gradient import (
+    qHypervolumeKnowledgeGradient,
+    qMultiFidelityHypervolumeKnowledgeGradient,
+)
 from botorch.acquisition.multi_objective.max_value_entropy_search import (
     qMultiObjectiveMaxValueEntropy,
 )
 from botorch.acquisition.multi_objective.monte_carlo import (
     MultiObjectiveMCAcquisitionFunction,
     qExpectedHypervolumeImprovement,
     qNoisyExpectedHypervolumeImprovement,
@@ -31,14 +35,16 @@
 )
 
 
 __all__ = [
     "get_default_partitioning_alpha",
     "prune_inferior_points_multi_objective",
     "qExpectedHypervolumeImprovement",
+    "qHypervolumeKnowledgeGradient",
+    "qMultiFidelityHypervolumeKnowledgeGradient",
     "qNoisyExpectedHypervolumeImprovement",
     "MOMF",
     "qMultiObjectiveMaxValueEntropy",
     "AnalyticMultiOutputObjective",
     "ExpectedHypervolumeImprovement",
     "IdentityAnalyticMultiOutputObjective",
     "IdentityMCMultiOutputObjective",
```

### Comparing `botorch-0.9.4/botorch/acquisition/multi_objective/analytic.py` & `botorch-0.9.5/botorch/acquisition/multi_objective/analytic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/acquisition/multi_objective/joint_entropy_search.py` & `botorch-0.9.5/botorch/acquisition/multi_objective/joint_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/acquisition/multi_objective/logei.py` & `botorch-0.9.5/botorch/acquisition/multi_objective/logei.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     logmeanexp,
     logplusexp,
     logsumexp,
     smooth_amin,
 )
 from botorch.utils.transforms import (
     concatenate_pending_points,
-    is_fully_bayesian,
+    is_ensemble,
     match_batch_shape,
     t_batch_mode_transform,
 )
 from torch import Tensor
 
 
 class qLogExpectedHypervolumeImprovement(
@@ -91,15 +91,15 @@
             sampler: The sampler used to draw base samples. If not given,
                 a sampler is generated using `get_sampler`.
             objective: The MCMultiOutputObjective under which the samples are evaluated.
                 Defaults to `IdentityMultiOutputObjective()`.
             constraints: A list of callables, each mapping a Tensor of dimension
                 `sample_shape x batch-shape x q x m` to a Tensor of dimension
                 `sample_shape x batch-shape x q`, where negative values imply
-                feasibility. The acqusition function will compute expected feasible
+                feasibility. The acquisition function will compute expected feasible
                 hypervolume.
             X_pending: A `batch_shape x m x d`-dim Tensor of `m` design points that have
                 points that have been submitted for function evaluation but have not yet
                 been evaluated. Concatenated into `X` upon forward call. Copied and set
                 to have no gradient.
             eta: The temperature parameter for the sigmoid function used for the
                 differentiable approximation of the constraints. In case of a float the
@@ -266,15 +266,15 @@
         # 9) sum over segments (n_cells-dim) and average over MC samples
         return logmeanexp(logsumexp(log_areas_per_segment, dim=-1), dim=0)
 
     def _log_improvement(
         self, obj_subsets: Tensor, view_shape: Union[Tuple, torch.Size]
     ) -> Tensor:
         # smooth out the clamp and take the log (previous step 3)
-        # substract cell lower bounds, clamp min at zero, but first
+        # subtract cell lower bounds, clamp min at zero, but first
         # make obj_subsets broadcastable with cell bounds:
         # mc_samples x batch_shape x (num_cells = 1) x q_choose_i x i x m
         obj_subsets = obj_subsets.unsqueeze(-4)
         # making cell bounds broadcastable with obj_subsets:
         # (mc_samples = 1) x (batch_shape = 1) x num_cells x 1 x (i = 1) x m
         cell_lower_bounds = self.cell_lower_bounds.view(view_shape).unsqueeze(-3)
         Z = obj_subsets - cell_lower_bounds
@@ -370,15 +370,15 @@
                 Note: a pareto front is created for each mc sample, which can be
                 computationally intensive for `m` > 2.
             objective: The MCMultiOutputObjective under which the samples are
                 evaluated. Defaults to `IdentityMultiOutputObjective()`.
             constraints: A list of callables, each mapping a Tensor of dimension
                 `sample_shape x batch-shape x q x m` to a Tensor of dimension
                 `sample_shape x batch-shape x q`, where negative values imply
-                feasibility. The acqusition function will compute expected feasible
+                feasibility. The acquisition function will compute expected feasible
                 hypervolume.
             X_pending: A `batch_shape x m x d`-dim Tensor of `m` design points that
                 have points that have been submitted for function evaluation, but
                 have not yet been evaluated.
             eta: The temperature parameter for the sigmoid function used for the
                 differentiable approximation of the constraints. In case of a float the
                 same `eta` is used for every constraint in constraints. In case of a
@@ -450,17 +450,17 @@
         # generally pre-computed and cached before the `forward` call, see the docs of
         # `cache_pending` for details.
         # TODO: Improve the efficiency by not re-computing the X_baseline-X_baseline
         # covariance matrix, but only the covariance of
         # 1) X and X, and
         # 2) X and X_baseline.
         posterior = self.model.posterior(X_full)
-        # Account for possible one-to-many transform and the MCMC batch dimension in
-        # `SaasFullyBayesianSingleTaskGP`
-        event_shape_lag = 1 if is_fully_bayesian(self.model) else 2
+        # Account for possible one-to-many transform and the model batch dimensions in
+        # ensemble models.
+        event_shape_lag = 1 if is_ensemble(self.model) else 2
         n_w = (
             posterior._extended_shape()[X_full.dim() - event_shape_lag]
             // X_full.shape[-2]
         )
         q_in = X.shape[-2] * n_w
         self._set_sampler(q_in=q_in, posterior=posterior)
         samples = self._get_f_X_samples(posterior=posterior, q_in=q_in)
```

### Comparing `botorch-0.9.4/botorch/acquisition/multi_objective/max_value_entropy_search.py` & `botorch-0.9.5/botorch/acquisition/multi_objective/max_value_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/acquisition/multi_objective/monte_carlo.py` & `botorch-0.9.5/botorch/acquisition/multi_objective/monte_carlo.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 from botorch.utils.multi_objective.hypervolume import (
     NoisyExpectedHypervolumeMixin,
     SubsetIndexCachingMixin,
 )
 from botorch.utils.objective import compute_smoothed_feasibility_indicator
 from botorch.utils.transforms import (
     concatenate_pending_points,
-    is_fully_bayesian,
+    is_ensemble,
     match_batch_shape,
     t_batch_mode_transform,
 )
 from torch import Tensor
 
 
 class MultiObjectiveMCAcquisitionFunction(AcquisitionFunction, MCSamplerMixin, ABC):
@@ -180,15 +180,15 @@
             sampler: The sampler used to draw base samples. If not given,
                 a sampler is generated using `get_sampler`.
             objective: The MCMultiOutputObjective under which the samples are evaluated.
                 Defaults to `IdentityMCMultiOutputObjective()`.
             constraints: A list of callables, each mapping a Tensor of dimension
                 `sample_shape x batch-shape x q x m` to a Tensor of dimension
                 `sample_shape x batch-shape x q`, where negative values imply
-                feasibility. The acqusition function will compute expected feasible
+                feasibility. The acquisition function will compute expected feasible
                 hypervolume.
             X_pending: A `batch_shape x m x d`-dim Tensor of `m` design points that have
                 points that have been submitted for function evaluation but have not yet
                 been evaluated. Concatenated into `X` upon forward call. Copied and set
                 to have no gradient.
             eta: The temperature parameter for the sigmoid function used for the
                 differentiable approximation of the constraints. In case of a float the
@@ -287,15 +287,15 @@
             # take the minimum in each subset
             overlap_vertices = obj_subsets.min(dim=-2).values
             # add batch-dim to compute area for each segment (pseudo-pareto-vertex)
             # this tensor is mc_samples x batch_shape x num_cells x q_choose_i x m
             overlap_vertices = torch.min(
                 overlap_vertices.unsqueeze(-3), self.cell_upper_bounds.view(view_shape)
             )
-            # substract cell lower bounds, clamp min at zero
+            # subtract cell lower bounds, clamp min at zero
             lengths_i = (
                 overlap_vertices - self.cell_lower_bounds.view(view_shape)
             ).clamp_min(0.0)
             # take product over hyperrectangle side lengths to compute area
             # sum over all subsets of size i
             areas_i = lengths_i.prod(dim=-1)
             # if constraints are present, apply a differentiable approximation of
@@ -366,15 +366,15 @@
                 Note: a pareto front is created for each mc sample, which can be
                 computationally intensive for `m` > 2.
             objective: The MCMultiOutputObjective under which the samples are
                 evaluated. Defaults to `IdentityMCMultiOutputObjective()`.
             constraints: A list of callables, each mapping a Tensor of dimension
                 `sample_shape x batch-shape x q x m` to a Tensor of dimension
                 `sample_shape x batch-shape x q`, where negative values imply
-                feasibility. The acqusition function will compute expected feasible
+                feasibility. The acquisition function will compute expected feasible
                 hypervolume.
             X_pending: A `batch_shape x m x d`-dim Tensor of `m` design points that
                 have points that have been submitted for function evaluation, but
                 have not yet been evaluated.
             eta: The temperature parameter for the sigmoid function used for the
                 differentiable approximation of the constraints. In case of a float the
                 same `eta` is used for every constraint in constraints. In case of a
@@ -449,15 +449,15 @@
         # TODO: Improve the efficiency by not re-computing the X_baseline-X_baseline
         # covariance matrix, but only the covariance of
         # 1) X and X, and
         # 2) X and X_baseline.
         posterior = self.model.posterior(X_full)
         # Account for possible one-to-many transform and the MCMC batch dimension in
         # `SaasFullyBayesianSingleTaskGP`
-        event_shape_lag = 1 if is_fully_bayesian(self.model) else 2
+        event_shape_lag = 1 if is_ensemble(self.model) else 2
         n_w = (
             posterior._extended_shape()[X_full.dim() - event_shape_lag]
             // X_full.shape[-2]
         )
         q_in = X.shape[-2] * n_w
         self._set_sampler(q_in=q_in, posterior=posterior)
         samples = self._get_f_X_samples(posterior=posterior, q_in=q_in)
```

### Comparing `botorch-0.9.4/botorch/acquisition/multi_objective/multi_fidelity.py` & `botorch-0.9.5/botorch/acquisition/multi_objective/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/acquisition/multi_objective/multi_output_risk_measures.py` & `botorch-0.9.5/botorch/acquisition/multi_objective/multi_output_risk_measures.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,15 +495,15 @@
                 mvar_set = self.get_mvar_set_cpu(prepared_samples)
             else:
                 mvar_set = self.get_mvar_set_gpu(prepared_samples)
         if samples.requires_grad:
             # TODO: Investigate differentiability of MVaR.
             warnings.warn(
                 "Got `samples` that requires grad, but computing MVaR involves "
-                "non-differentable operations and the results will not be "
+                "non-differentiable operations and the results will not be "
                 "differentiable. This may lead to errors down the line!",
                 RuntimeWarning,
             )
         # Set the `pad_size` to either `self.n_w` or the size of the largest MVaR set.
         pad_size = self.n_w if self.pad_to_n_w else max([_.shape[0] for _ in mvar_set])
         padded_mvar_list = []
         for mvar_ in mvar_set:
@@ -632,15 +632,15 @@
             raise UnsupportedError("Negative weights are not supported in MARS.")
         if chebyshev_weights.dim() != 1:
             raise UnsupportedError("Batched weights are not supported in MARS.")
         self.register_buffer("_chebyshev_weights", chebyshev_weights)
 
     @property
     def baseline_Y(self) -> Optional[Tensor]:
-        r"""Baseline outcomes used indetermining the normalization bounds."""
+        r"""Baseline outcomes used in determining the normalization bounds."""
         return self._baseline_Y
 
     @baseline_Y.setter
     def baseline_Y(self, baseline_Y: Optional[Tensor]) -> None:
         r"""Update the baseline outcomes.
 
         Invalidates the cached Chebyshev objective.
```

### Comparing `botorch-0.9.4/botorch/acquisition/multi_objective/objective.py` & `botorch-0.9.5/botorch/acquisition/multi_objective/objective.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
 
     def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
         samples = super().forward(samples=samples)
         return samples * self.Y_std + self.Y_mean
 
 
 class AnalyticMultiOutputObjective(torch.nn.Module):
-    r"""Abstract base class for multi-output analyic objectives.
+    r"""Abstract base class for multi-output analytic objectives.
 
     DEPRECATED - This will be removed in the next version.
 
     """
 
     def __init__(self, *args, **kwargs) -> None:
         """Initialize objective."""
```

### Comparing `botorch-0.9.4/botorch/acquisition/multi_objective/predictive_entropy_search.py` & `botorch-0.9.5/botorch/acquisition/multi_objective/predictive_entropy_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         (c) When the convergence threshold is set too small.
 
 
         Problem (a) occurs because we have to compute the variable:
         `alpha = (mean(x_n) - mean(x_p)) / std(x_n - x_p)`, which becomes very
         large when `x_n` is better than `x_p` with high-probability. This leads to a
-        log(0) error when we compute `log(1 - cdf(alpha))`. We have pre-emptively
+        log(0) error when we compute `log(1 - cdf(alpha))`. We have preemptively
         clamped some values depending on `1`alpha` in order to mitigate this.
 
         Problem (b) occurs because we have to compute matrix inverses for the
         two-dimensional marginals (x_n, x_p). To address this we manually add jitter
         to the diagonal of the covariance matrix i.e. `ep_jitter` when training and
         `test_jitter` when testing. The default choice is not always appropriate
         because the same jitter is used for the inversion of the covariance
```

### Comparing `botorch-0.9.4/botorch/acquisition/multi_objective/utils.py` & `botorch-0.9.5/botorch/acquisition/multi_objective/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 )
 from botorch.utils.multi_objective.box_decompositions.dominated import (
     DominatedPartitioning,
 )
 from botorch.utils.multi_objective.pareto import is_non_dominated
 from botorch.utils.objective import compute_feasibility_indicator
 from botorch.utils.sampling import draw_sobol_samples
-from botorch.utils.transforms import is_fully_bayesian
+from botorch.utils.transforms import is_ensemble
 from torch import Tensor
 
 
 def get_default_partitioning_alpha(num_objectives: int) -> float:
     r"""Determines an approximation level based on the number of objectives.
 
     If `alpha` is 0, FastNondominatedPartitioning should be used. Otherwise,
@@ -106,15 +106,15 @@
         A `n' x d` with subset of points in `X`, where
 
             n' = min(N_nz, ceil(max_frac * n))
 
         with `N_nz` the number of points in `X` that have non-zero (empirical,
         under `num_samples` samples) probability of being pareto optimal.
     """
-    if marginalize_dim is None and is_fully_bayesian(model):
+    if marginalize_dim is None and is_ensemble(model):
         # TODO: Properly deal with marginalizing fully Bayesian models
         marginalize_dim = MCMC_DIM
 
     if X.ndim > 2:
         # TODO: support batched inputs (req. dealing with ragged tensors)
         raise UnsupportedError(
             "Batched inputs `X` are currently unsupported by "
```

### Comparing `botorch-0.9.4/botorch/acquisition/multi_step_lookahead.py` & `botorch-0.9.5/botorch/acquisition/multi_step_lookahead.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 r"""
-A general implementation of multi-step look-ahead acquistion function with configurable
+A general implementation of multi-step look-ahead acquisition function with configurable
 value functions. See [Jiang2020multistep]_.
 
 .. [Jiang2020multistep]
     S. Jiang, D. R. Jiang, M. Balandat, B. Karrer, J. Gardner, and R. Garnett.
     Efficient Nonmyopic Bayesian Optimization via One-Shot Multi-Step Trees.
     In Advances in Neural Information Processing Systems 33, 2020.
 
@@ -210,21 +210,21 @@
             batch_shape: The batch shape of the input tensor `X`.
         """
         tbatch_dim_start = -2 - len(batch_shape)
         for s in self.samplers:
             s.batch_range_override = (tbatch_dim_start, -2)
 
     def get_augmented_q_batch_size(self, q: int) -> int:
-        r"""Get augmented q batch size for one-shot optimzation.
+        r"""Get augmented q batch size for one-shot optimization.
 
         Args:
             q: The number of candidates to consider jointly.
 
         Returns:
-            The augmented size for one-shot optimzation (including variables
+            The augmented size for one-shot optimization (including variables
             parameterizing the fantasy solutions): `q_0 + f_1 q_1 + f_2 f_1 q_2 + ...`
         """
         return q + self._num_auxiliary
 
     def get_split_shapes(self, X: Tensor) -> Tuple[Size, List[Size], List[int]]:
         r"""Get the split shapes from X.
 
@@ -545,15 +545,15 @@
             if q is not None and q > 1:
                 raise UnsupportedError(
                     "Only batch sizes of q=1 are supported for analytic value "
                     "functions."
                 )
             if q is not None and mcs is not None:
                 warnings.warn(
-                    "inner_mc_samples is ignored for analytic acquistion functions",
+                    "inner_mc_samples is ignored for analytic acquisition functions",
                     BotorchWarning,
                 )
             inner_samplers.append(None)
         else:
             inner_sampler = SobolQMCNormalSampler(
                 sample_shape=torch.Size([32 if mcs is None else mcs])
             )
```

### Comparing `botorch-0.9.4/botorch/acquisition/objective.py` & `botorch-0.9.5/botorch/acquisition/objective.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 from torch import Tensor
 from torch.nn import Module
 
 if TYPE_CHECKING:
     from botorch.posteriors.posterior import Posterior  # pragma: no cover
     from botorch.posteriors.posterior_list import PosteriorList  # pragma: no cover
 
+DEFAULT_NUM_PREF_SAMPLES = 16
+
 
 class PosteriorTransform(Module, ABC):
     r"""
     Abstract base class for objectives that transform the posterior.
 
     :meta private:
     """
@@ -550,54 +552,66 @@
         sample_shape: Optional[torch.Size] = None,
         seed: Optional[int] = None,
     ):
         r"""
         Args:
             pref_model: A BoTorch model, which models the latent preference/utility
                 function. Given an input tensor of size
-                `sample_size x batch_shape x N x d`, its `posterior` method should
+                `sample_size x batch_shape x q x d`, its `posterior` method should
                 return a `Posterior` object with single outcome representing the
                 utility values of the input.
-            sampler: Sampler for the preference model to account for uncertainty in
-                preferece when calculating the objective; it's not the one used
-                in MC acquisition functions. If None,
-                it uses `IIDNormalSampler(sample_shape=torch.Size([1]))`.
+            sample_shape: Determines the number of preference-model samples drawn
+                *per outcome-model sample* when the `LearnedObjective` is called.
+                Note that this is an additional layer of sampling relative to what
+                is needed when evaluating most MC acquisition functions in order to
+                account for uncertainty in the preference model. If `None`, it will
+                default to `torch.Size([16])`, so that 16 samples will be drawn
+                from the preference model at each outcome sample. This number is
+                relatively high because sampling from the preference model is general
+                cheap relative to generating the outcome model posterior.
         """
         super().__init__()
         self.pref_model = pref_model
         if isinstance(pref_model, DeterministicModel):
             assert sample_shape is None
             self.sampler = None
         else:
             if sample_shape is None:
-                sample_shape = torch.Size([1])
+                sample_shape = torch.Size([DEFAULT_NUM_PREF_SAMPLES])
+            # using an IIDNormalSampler instead of a SobolQMCNormalSampler by default
+            # because SobolQMCNormalSampler can support up to 21201 total samples and
+            # becomes noticeably slower than uniform sampling when the sample size is
+            # large.
             self.sampler = IIDNormalSampler(sample_shape=sample_shape, seed=seed)
             self.sampler.batch_range_override = (1, -1)
 
     def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
         r"""Sample each element of samples.
 
         Args:
-            samples: A `sample_size x batch_shape x N x d`-dim Tensors of
+            samples: A `sample_size x batch_shape x q x d`-dim Tensors of
                 samples from a model posterior.
 
         Returns:
-            A `(sample_size * num_samples) x batch_shape x N`-dim Tensor of
+            A `(sample_size * num_samples) x batch_shape x q`-dim Tensor of
             objective values sampled from utility posterior using `pref_model`.
         """
         if samples.dtype != torch.float64 and any(
             d == torch.float64 for d in self.pref_model.dtypes_of_buffers
         ):
             warnings.warn(
                 LEARNED_OBJECTIVE_PREF_MODEL_MIXED_DTYPE_WARN,
                 InputDataWarning,
                 stacklevel=2,
             )
             samples = samples.to(torch.float64)
 
+        if samples.ndim < 3:
+            raise ValueError("samples should have at least 3 dimensions.")
+
         posterior = self.pref_model.posterior(samples)
         if isinstance(self.pref_model, DeterministicModel):
             # return preference posterior mean
             return posterior.mean.squeeze(-1)
         else:
             # return preference posterior augmented samples
             samples = self.sampler(posterior).squeeze(-1)
```

### Comparing `botorch-0.9.4/botorch/acquisition/penalized.py` & `botorch-0.9.5/botorch/acquisition/penalized.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         """
         return torch.linalg.norm((X - self.init_point), ord=1, dim=-1).unsqueeze(dim=0)
 
 
 class PenalizedMCObjective(GenericMCObjective):
     r"""Penalized MC objective.
 
-    Allows to construct a penaltized MC-objective by adding a penalty term to
+    Allows to construct a penalized MC-objective by adding a penalty term to
     the original objective.
 
         mc_acq(X) = objective(X) + penalty_objective(X)
 
     Note: PenalizedMCObjective allows adding penalty at the MCObjective level,
     different from the AcquisitionFunction level in PenalizedAcquisitionFunction.
```

### Comparing `botorch-0.9.4/botorch/acquisition/predictive_entropy_search.py` & `botorch-0.9.5/botorch/acquisition/predictive_entropy_search.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/acquisition/preference.py` & `botorch-0.9.5/botorch/acquisition/preference.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from torch import Tensor
 from torch.distributions import Bernoulli, Normal
 
 SIGMA_JITTER = 1e-8
 
 
 class AnalyticExpectedUtilityOfBestOption(AnalyticAcquisitionFunction):
-    r"""Analytic Prefential Expected Utility of Best Options, i.e., Analytical EUBO"""
+    r"""Analytic Preferential Expected Utility of Best Options, i.e., Analytical EUBO"""
 
     def __init__(
         self,
         pref_model: Model,
         outcome_model: Optional[DeterministicModel] = None,
         previous_winner: Optional[Tensor] = None,
     ) -> None:
```

### Comparing `botorch-0.9.4/botorch/acquisition/prior_guided.py` & `botorch-0.9.5/botorch/acquisition/prior_guided.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/acquisition/proximal.py` & `botorch-0.9.5/botorch/acquisition/proximal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/acquisition/risk_measures.py` & `botorch-0.9.5/botorch/acquisition/risk_measures.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/acquisition/utils.py` & `botorch-0.9.5/botorch/acquisition/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,32 +15,82 @@
 
 import torch
 from botorch.acquisition.objective import (
     IdentityMCObjective,
     MCAcquisitionObjective,
     PosteriorTransform,
 )
-from botorch.exceptions.errors import DeprecationError, UnsupportedError
+from botorch.exceptions.errors import (
+    BotorchTensorDimensionError,
+    DeprecationError,
+    UnsupportedError,
+)
 from botorch.models.fully_bayesian import MCMC_DIM
 from botorch.models.model import Model
 from botorch.sampling.base import MCSampler
 from botorch.sampling.get_sampler import get_sampler
 from botorch.sampling.pathwise import draw_matheron_paths
 from botorch.utils.objective import compute_feasibility_indicator
 from botorch.utils.sampling import optimize_posterior_samples
-from botorch.utils.transforms import is_fully_bayesian, normalize_indices
+from botorch.utils.transforms import is_ensemble, normalize_indices
 from torch import Tensor
 
 
 def get_acquisition_function(*args, **kwargs) -> None:
     raise DeprecationError(
         "`get_acquisition_function` has been moved to `botorch.acquisition.factory`."
     )
 
 
+def repeat_to_match_aug_dim(target_tensor: Tensor, reference_tensor: Tensor) -> Tensor:
+    """Repeat target_tensor until it has the same first dimension as reference_tensor
+    This works regardless of the batch shapes and q.
+    This is useful as we sometimes modify sample shapes such as in LearnedObjective.
+
+    Args:
+        target_tensor: A `sample_size x batch_shape x q x m`-dim Tensor
+        reference_tensor: A `(augmented_sample * sample_size) x batch_shape x q`-dim
+            Tensor. `augmented_sample` could be 1.
+
+    Returns:
+        The content of `target_tensor` potentially repeated so that its first dimension
+        matches that of `reference_tensor`.
+        The shape will be `(augmented_sample * sample_size) x batch_shape x q x m`.
+
+    Examples:
+        >>> import torch
+        >>> target_tensor = torch.arange(3).repeat(2, 1).T
+        >>> target_tensor
+        tensor([[0, 0],
+                [1, 1],
+                [2, 2]])
+        >>> repeat_to_match_aug_dim(target_tensor, torch.zeros(6))
+        tensor([[0, 0],
+                [1, 1],
+                [2, 2],
+                [0, 0],
+                [1, 1],
+                [2, 2]])
+    """
+    augmented_sample_num, remainder = divmod(
+        reference_tensor.shape[0], target_tensor.shape[0]
+    )
+    if remainder != 0:
+        raise ValueError(
+            "The first dimension of reference_tensor must "
+            "be a multiple of target_tensor's."
+        )
+
+    # using repeat here as obj might be constructed as
+    # obj.reshape(-1, *samples.shape[2:]) where the first 2 dimensions are
+    # of shape `augmented_samples x sample_shape`.
+    repeat_size = (augmented_sample_num,) + (1,) * (target_tensor.ndim - 1)
+    return target_tensor.repeat(*repeat_size)
+
+
 def compute_best_feasible_objective(
     samples: Tensor,
     obj: Tensor,
     constraints: Optional[List[Callable[[Tensor], Tensor]]],
     model: Optional[Model] = None,
     objective: Optional[MCAcquisitionObjective] = None,
     posterior_transform: Optional[PosteriorTransform] = None,
@@ -101,14 +151,17 @@
         infeasible_value = _estimate_objective_lower_bound(
             model=model,
             objective=objective,
             posterior_transform=posterior_transform,
             X=X_baseline,
         ).item()
 
+    is_feasible = repeat_to_match_aug_dim(
+        target_tensor=is_feasible, reference_tensor=obj
+    )
     obj = torch.where(is_feasible, obj, infeasible_value)
     with torch.no_grad():
         return obj.amax(dim=-1, keepdim=True)
 
 
 def _estimate_objective_lower_bound(
     model: Model,
@@ -233,15 +286,15 @@
         A `n' x d` with subset of points in `X`, where
 
             n' = min(N_nz, ceil(max_frac * n))
 
         with `N_nz` the number of points in `X` that have non-zero (empirical,
         under `num_samples` samples) probability of being the best point.
     """
-    if marginalize_dim is None and is_fully_bayesian(model):
+    if marginalize_dim is None and is_ensemble(model):
         # TODO: Properly deal with marginalizing fully Bayesian models
         marginalize_dim = MCMC_DIM
 
     if X.ndim > 2:
         # TODO: support batched inputs (req. dealing with ragged tensors)
         raise UnsupportedError(
             "Batched inputs `X` are currently unsupported by prune_inferior_points"
@@ -291,45 +344,73 @@
         counts, order_idcs = torch.sort(counts, descending=True)
         idcs = order_idcs[:max_points]
 
     return X[idcs]
 
 
 def project_to_target_fidelity(
-    X: Tensor, target_fidelities: Optional[Dict[int, float]] = None
+    X: Tensor,
+    target_fidelities: Optional[Dict[int, float]] = None,
+    d: Optional[int] = None,
 ) -> Tensor:
     r"""Project `X` onto the target set of fidelities.
 
     This function assumes that the set of feasible fidelities is a box, so
     projecting here just means setting each fidelity parameter to its target
-    value.
+    value. If X does not contain the fidelity dimensions, this will insert
+    them and set them to their target values.
 
     Args:
-        X: A `batch_shape x q x d`-dim Tensor of with `q` `d`-dim design points
-            for each t-batch.
+        X: A `batch_shape x q x (d or d-d_f)`-dim Tensor of with `q` `d` or
+            `d-d_f`-dim design points for each t-batch, where d_f is the
+            number of fidelity dimensions. If the argument `d` is not provided,
+            `X` must include the fidelity dimensions and have a trailing`X` must
+            include the fidelity dimensions and have a trailing
         target_fidelities: A dictionary mapping a subset of columns of `X` (the
             fidelity parameters) to their respective target fidelity value. If
             omitted, assumes that the last column of X is the fidelity parameter
             with a target value of 1.0.
+        d: The total dimension `d`.
 
     Return:
         A `batch_shape x q x d`-dim Tensor `X_proj` with fidelity parameters
             projected to the provided fidelity values.
     """
     if target_fidelities is None:
         target_fidelities = {-1: 1.0}
-    d = X.size(-1)
+    if d is None:
+        # assume X contains the fidelity dimensions
+        d = X.shape[-1]
     # normalize to positive indices
     tfs = {k if k >= 0 else d + k: v for k, v in target_fidelities.items()}
     ones = torch.ones(*X.shape[:-1], device=X.device, dtype=X.dtype)
-    # here we're looping through the feature dimension of X - this could be
-    # slow for large `d`, we should optimize this for that case
-    X_proj = torch.stack(
-        [X[..., i] if i not in tfs else tfs[i] * ones for i in range(d)], dim=-1
-    )
+    if X.shape[-1] == d:
+        # X contains fidelity dimensions
+        # here we're looping through the feature dimension of X - this could be
+        # slow for large `d`, we should optimize this for that case
+        X_proj = torch.stack(
+            [X[..., i] if i not in tfs else tfs[i] * ones for i in range(d)], dim=-1
+        )
+    elif X.shape[-1] == d - len(target_fidelities):
+        # need to insert fidelity dimensions
+        cols = []
+        X_idx = 0
+        for i in range(d):
+            if i not in tfs:
+                cols.append(X[..., X_idx])
+                X_idx += 1
+            else:
+                cols.append(tfs[i] * ones)
+        X_proj = torch.stack(cols, dim=-1)
+    else:
+        raise BotorchTensorDimensionError(
+            "X must have a last dimension with size `d` or `d-d_f`,"
+            f" but got {X.shape[-1]}."
+        )
+
     return X_proj
 
 
 def expand_trace_observations(
     X: Tensor, fidelity_dims: Optional[List[int]] = None, num_trace_obs: int = 0
 ) -> Tensor:
     r"""Expand `X` with trace observations.
```

### Comparing `botorch-0.9.4/botorch/cross_validation.py` & `botorch-0.9.5/botorch/cross_validation.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/exceptions/__init__.py` & `botorch-0.9.5/botorch/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/exceptions/errors.py` & `botorch-0.9.5/botorch/exceptions/errors.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/exceptions/warnings.py` & `botorch-0.9.5/botorch/exceptions/warnings.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/fit.py` & `botorch-0.9.5/botorch/fit.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/generation/__init__.py` & `botorch-0.9.5/botorch/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/generation/gen.py` & `botorch-0.9.5/botorch/generation/gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,22 +15,25 @@
 from functools import partial
 from typing import Any, Callable, Dict, List, NoReturn, Optional, Tuple, Type, Union
 
 import numpy as np
 import torch
 from botorch.acquisition import AcquisitionFunction
 from botorch.exceptions.warnings import OptimizationWarning
-from botorch.generation.utils import _remove_fixed_features_from_optimization
+from botorch.generation.utils import (
+    _convert_nonlinear_inequality_constraints,
+    _remove_fixed_features_from_optimization,
+)
 from botorch.logging import _get_logger
 from botorch.optim.parameter_constraints import (
     _arrayify,
     make_scipy_bounds,
     make_scipy_linear_constraints,
     make_scipy_nonlinear_inequality_constraints,
-    NLC_TOL,
+    nonlinear_constraint_is_feasible,
 )
 from botorch.optim.stopping import ExpMAStoppingCriterion
 from botorch.optim.utils import columnwise_clamp, fix_features
 from botorch.optim.utils.timeout import minimize_with_timeout
 from scipy.optimize import OptimizeResult
 from torch import Tensor
 from torch.optim import Optimizer
@@ -43,15 +46,15 @@
 def gen_candidates_scipy(
     initial_conditions: Tensor,
     acquisition_function: AcquisitionFunction,
     lower_bounds: Optional[Union[float, Tensor]] = None,
     upper_bounds: Optional[Union[float, Tensor]] = None,
     inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
     equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
-    nonlinear_inequality_constraints: Optional[List[Callable]] = None,
+    nonlinear_inequality_constraints: Optional[List[Tuple[Callable, bool]]] = None,
     options: Optional[Dict[str, Any]] = None,
     fixed_features: Optional[Dict[int, Optional[float]]] = None,
     timeout_sec: Optional[float] = None,
 ) -> Tuple[Tensor, Tensor]:
     r"""Generate a set of candidates using `scipy.optimize.minimize`.
 
     Optimizes an acquisition function starting from a set of initial candidates
@@ -65,19 +68,26 @@
         upper_bounds: Maximum values for each column of initial_conditions.
         inequality constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`.
         equality constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
-        nonlinear_inequality_constraints: A list of callables with that represent
-            non-linear inequality constraints of the form `callable(x) >= 0`. Each
-            callable is expected to take a `(num_restarts) x q x d`-dim tensor as
-            an input and return a `(num_restarts) x q`-dim tensor with the
-            constraint values. The constraints will later be passed to SLSQP.
+        nonlinear_inequality_constraints: A list of tuples representing the nonlinear
+            inequality constraints. The first element in the tuple is a callable
+            representing a constraint of the form `callable(x) >= 0`. In case of an
+            intra-point constraint, `callable()`takes in an one-dimensional tensor of
+            shape `d` and returns a scalar. In case of an inter-point constraint,
+            `callable()` takes a two dimensional tensor of shape `q x d` and again
+            returns a scalar. The second element is a boolean, indicating if it is an
+            intra-point or inter-point constraint (`True` for intra-point. `False` for
+            inter-point). For more information on intra-point vs inter-point
+            constraints, see the docstring of the `inequality_constraints` argument to
+            `optimize_acqf()`. The constraints will later be passed to the scipy
+            solver.
         options: Options used to control the optimization including "method"
             and "maxiter". Select method for `scipy.minimize` using the
             "method" key. By default uses L-BFGS-B for box-constrained problems
             and SLSQP if inequality or equality constraints are present. If
             `with_grad=False`, then we use a two-point finite difference estimate
             of the gradient.
         fixed_features: This is a dictionary of feature indices to values, where
@@ -121,14 +131,24 @@
             or nonlinear_inequality_constraints
         ):
             reduced_domain = True
         # if there are we need to make sure features are fixed to specific values
         else:
             reduced_domain = None not in fixed_features.values()
 
+    if nonlinear_inequality_constraints:
+        if not isinstance(nonlinear_inequality_constraints, list):
+            raise ValueError(
+                "`nonlinear_inequality_constraints` must be a list of tuples, "
+                f"got {type(nonlinear_inequality_constraints)}."
+            )
+        nonlinear_inequality_constraints = _convert_nonlinear_inequality_constraints(
+            nonlinear_inequality_constraints
+        )
+
     if reduced_domain:
         _no_fixed_features = _remove_fixed_features_from_optimization(
             fixed_features=fixed_features,
             acquisition_function=acquisition_function,
             initial_conditions=initial_conditions,
             lower_bounds=lower_bounds,
             upper_bounds=upper_bounds,
@@ -218,14 +238,15 @@
                 "`batch_limit` must be 1 when non-linear inequality constraints "
                 "are given."
             )
         constraints += make_scipy_nonlinear_inequality_constraints(
             nonlinear_inequality_constraints=nonlinear_inequality_constraints,
             f_np_wrapper=f_np_wrapper,
             x0=x0,
+            shapeX=shapeX,
         )
     x0 = _arrayify(x0)
 
     def f(x):
         return -acquisition_function(x)
 
     res = minimize_with_timeout(
@@ -250,22 +271,25 @@
         X=torch.from_numpy(res.x).to(initial_conditions).reshape(shapeX),
         fixed_features=fixed_features,
     )
 
     # SLSQP sometimes fails in the line search or may just fail to find a feasible
     # candidate in which case we just return the starting point. This happens rarely,
     # so it shouldn't be an issue given enough restarts.
-    if nonlinear_inequality_constraints and any(
-        nlc(candidates.view(-1)) < NLC_TOL for nlc in nonlinear_inequality_constraints
-    ):
-        candidates = torch.from_numpy(x0).to(candidates).reshape(shapeX)
-        warnings.warn(
-            "SLSQP failed to converge to a solution the satisfies the non-linear "
-            "constraints. Returning the feasible starting point."
-        )
+    if nonlinear_inequality_constraints:
+        for con, is_intrapoint in nonlinear_inequality_constraints:
+            if not nonlinear_constraint_is_feasible(
+                con, is_intrapoint=is_intrapoint, x=candidates
+            ):
+                candidates = torch.from_numpy(x0).to(candidates).reshape(shapeX)
+                warnings.warn(
+                    "SLSQP failed to converge to a solution the satisfies the "
+                    "non-linear constraints. Returning the feasible starting point."
+                )
+                break
 
     clamped_candidates = columnwise_clamp(
         X=candidates, lower=lower_bounds, upper=upper_bounds, raise_on_violation=True
     )
     with torch.no_grad():
         batch_acquisition = acquisition_function(clamped_candidates)
```

### Comparing `botorch-0.9.4/botorch/generation/sampling.py` & `botorch-0.9.5/botorch/generation/sampling.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/generation/utils.py` & `botorch-0.9.5/botorch/generation/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,55 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
+import warnings
 from dataclasses import dataclass
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import torch
+
 from botorch.acquisition import AcquisitionFunction, FixedFeatureAcquisitionFunction
 from botorch.optim.parameter_constraints import (
     _generate_unfixed_lin_constraints,
     _generate_unfixed_nonlin_constraints,
 )
 from torch import Tensor
 
 
+def _convert_nonlinear_inequality_constraints(
+    nonlinear_inequality_constraints: List[Union[Callable, Tuple[Callable, bool]]]
+) -> List[Tuple[Callable, bool]]:
+    """Convert legacy defintions of nonlinear inequality constraints into the new
+    format. Assumes intra-point constraints.
+    """
+    nlcs = []
+    legacy = False
+    # return nonlinear_inequality_constraints
+    for nlc in nonlinear_inequality_constraints:
+        if callable(nlc):
+            # old style --> convert
+            nlcs.append((nlc, True))
+            legacy = True
+        else:
+            nlcs.append(nlc)
+    if legacy:
+        warnings.warn(
+            "The `nonlinear_inequality_constraints` argument is expected "
+            "take a list of tuples. Passing a list of callables "
+            "will result in an error in future versions.",
+            DeprecationWarning,
+        )
+
+    return nlcs
+
+
 def _flip_sub_unique(x: Tensor, k: int) -> Tensor:
     """Get the first k unique elements of a single-dimensional tensor, traversing the
     tensor from the back.
 
     Args:
         x: A single-dimensional tensor
         k: the number of elements to return
```

### Comparing `botorch-0.9.4/botorch/logging.py` & `botorch-0.9.5/botorch/logging.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/__init__.py` & `botorch-0.9.5/botorch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/approximate_gp.py` & `botorch-0.9.5/botorch/models/approximate_gp.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/contextual.py` & `botorch-0.9.5/botorch/models/contextual.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/contextual_multioutput.py` & `botorch-0.9.5/botorch/models/contextual_multioutput.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/converter.py` & `botorch-0.9.5/botorch/models/converter.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/deterministic.py` & `botorch-0.9.5/botorch/models/deterministic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/ensemble.py` & `botorch-0.9.5/botorch/models/ensemble.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/fully_bayesian.py` & `botorch-0.9.5/botorch/models/fully_bayesian.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 import torch
 from botorch.acquisition.objective import PosteriorTransform
 from botorch.models.gpytorch import BatchedMultiOutputGPyTorchModel
 from botorch.models.transforms.input import InputTransform
 from botorch.models.transforms.outcome import OutcomeTransform
 from botorch.models.utils import validate_input_scaling
 from botorch.models.utils.gpytorch_modules import MIN_INFERRED_NOISE_LEVEL
-from botorch.posteriors.fully_bayesian import FullyBayesianPosterior, MCMC_DIM
+from botorch.posteriors.fully_bayesian import GaussianMixturePosterior, MCMC_DIM
 from gpytorch.constraints import GreaterThan
 from gpytorch.distributions.multivariate_normal import MultivariateNormal
 from gpytorch.kernels import MaternKernel, ScaleKernel
 from gpytorch.kernels.kernel import dist, Kernel
 from gpytorch.likelihoods.gaussian_likelihood import (
     FixedNoiseGaussianLikelihood,
     GaussianLikelihood,
@@ -323,14 +323,17 @@
 
     Example:
         >>> saas_gp = SaasFullyBayesianSingleTaskGP(train_X, train_Y)
         >>> fit_fully_bayesian_model_nuts(saas_gp)
         >>> posterior = saas_gp.posterior(test_X)
     """
 
+    _is_fully_bayesian = True
+    _is_ensemble = True
+
     def __init__(
         self,
         train_X: Tensor,
         train_Y: Tensor,
         train_Yvar: Optional[Tensor] = None,
         outcome_transform: Optional[OutcomeTransform] = None,
         input_transform: Optional[InputTransform] = None,
@@ -504,15 +507,15 @@
     def posterior(
         self,
         X: Tensor,
         output_indices: Optional[List[int]] = None,
         observation_noise: bool = False,
         posterior_transform: Optional[PosteriorTransform] = None,
         **kwargs: Any,
-    ) -> FullyBayesianPosterior:
+    ) -> GaussianMixturePosterior:
         r"""Computes the posterior over model outputs at the provided points.
 
         Args:
             X: A `(batch_shape) x q x d`-dim Tensor, where `d` is the dimension
                 of the feature space and `q` is the number of points considered
                 jointly.
             output_indices: A list of indices, corresponding to the outputs over
@@ -522,19 +525,20 @@
                 computes the posterior over all model outputs.
             observation_noise: If True, add the observation noise from the
                 likelihood to the posterior. If a Tensor, use it directly as the
                 observation noise (must be of shape `(batch_shape) x q x m`).
             posterior_transform: An optional PosteriorTransform.
 
         Returns:
-            A `FullyBayesianPosterior` object. Includes observation noise if specified.
+            A `GaussianMixturePosterior` object. Includes observation noise
+                if specified.
         """
         self._check_if_fitted()
         posterior = super().posterior(
             X=X,
             output_indices=output_indices,
             observation_noise=observation_noise,
             posterior_transform=posterior_transform,
             **kwargs,
         )
-        posterior = FullyBayesianPosterior(distribution=posterior.distribution)
+        posterior = GaussianMixturePosterior(distribution=posterior.distribution)
         return posterior
```

### Comparing `botorch-0.9.4/botorch/models/fully_bayesian_multitask.py` & `botorch-0.9.5/botorch/models/fully_bayesian_multitask.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 # LICENSE file in the root directory of this source tree.
 
 
 r"""Multi-task Gaussian Process Regression models with fully Bayesian inference.
 """
 
 
-from typing import Any, Dict, List, Mapping, NoReturn, Optional, Tuple
+from typing import Any, Dict, List, Mapping, NoReturn, Optional, Tuple, Union
 
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
 from botorch.models.multitask import MultiTaskGP
 from botorch.models.transforms.input import InputTransform
 from botorch.models.transforms.outcome import OutcomeTransform
-from botorch.posteriors.fully_bayesian import FullyBayesianPosterior, MCMC_DIM
-from botorch.utils.datasets import SupervisedDataset
+from botorch.posteriors.fully_bayesian import GaussianMixturePosterior, MCMC_DIM
+from botorch.utils.datasets import MultiTaskDataset, SupervisedDataset
 from gpytorch.distributions.multivariate_normal import MultivariateNormal
 from gpytorch.kernels import MaternKernel
 from gpytorch.kernels.kernel import Kernel
 from gpytorch.likelihoods.likelihood import Likelihood
 from gpytorch.means.mean import Mean
 from torch import Tensor
 from torch.nn.parameter import Parameter
@@ -56,22 +56,22 @@
         Args:
             train_X: Training inputs (n x (d + 1))
             train_Y: Training targets (n x 1)
             train_Yvar: Observed noise variance (n x 1). If None, we infer the noise.
                 Note that the inferred noise is common across all tasks.
             task_feature: The index of the task feature (`-d <= task_feature <= d`).
             task_rank: The num of learned task embeddings to be used in the task kernel.
-                If omitted, set it to be 1.
+                If omitted, use a full rank (i.e. number of tasks) kernel.
         """
         super().set_inputs(train_X, train_Y, train_Yvar)
         # obtain a list of task indicies
         all_tasks = train_X[:, task_feature].unique().to(dtype=torch.long).tolist()
         self.task_feature = task_feature
         self.num_tasks = len(all_tasks)
-        self.task_rank = task_rank or 1
+        self.task_rank = task_rank or self.num_tasks
         # assume there is one column for task feature
         self.ard_num_dims = self.train_X.shape[-1] - 1
 
     def sample(self) -> None:
         r"""Sample from the SAAS model.
 
         This samples the mean, noise variance, outputscale, and lengthscales according
@@ -185,20 +185,23 @@
         >>> mtsaas_gp = SaasFullyBayesianMultiTaskGP(
         >>>     train_X, train_Y, train_Yvar, task_feature=-1,
         >>> )
         >>> fit_fully_bayesian_model_nuts(mtsaas_gp)
         >>> posterior = mtsaas_gp.posterior(test_X)
     """
 
+    _is_fully_bayesian = True
+    _is_ensemble = True
+
     def __init__(
         self,
         train_X: Tensor,
         train_Y: Tensor,
-        train_Yvar: Optional[Tensor],
         task_feature: int,
+        train_Yvar: Optional[Tensor] = None,
         output_tasks: Optional[List[int]] = None,
         rank: Optional[int] = None,
         outcome_transform: Optional[OutcomeTransform] = None,
         input_transform: Optional[InputTransform] = None,
         pyro_model: Optional[PyroModel] = None,
     ) -> None:
         r"""Initialize the fully Bayesian multi-task GP model.
@@ -208,15 +211,15 @@
             train_Y: Training targets (n x 1)
             train_Yvar: Observed noise variance (n x 1). If None, we infer the noise.
                 Note that the inferred noise is common across all tasks.
             task_feature: The index of the task feature (`-d <= task_feature <= d`).
             output_tasks: A list of task indices for which to compute model
                 outputs for. If omitted, return outputs for all task indices.
             rank: The num of learned task embeddings to be used in the task kernel.
-                If omitted, set it to be 1.
+                If omitted, use a full rank (i.e. number of tasks) kernel.
             outcome_transform: An outcome transform that is applied to the
                 training data during instantiation and to the posterior during
                 inference (that is, the `Posterior` obtained by calling
                 `.posterior` on the model will be on the original scale).
             input_transform: An input transform that is applied to the inputs `X`
                 in the model's forward pass.
             pyro_model: Optional `PyroModel`, defaults to `MultitaskSaasPyroModel`.
@@ -244,14 +247,15 @@
 
         super().__init__(
             train_X=train_X,
             train_Y=train_Y,
             train_Yvar=train_Yvar,
             task_feature=task_feature,
             output_tasks=output_tasks,
+            rank=rank,
         )
         self.to(train_X)
 
         self.mean_module = None
         self.covar_module = None
         self.likelihood = None
         self.task_covar_module = None
@@ -259,15 +263,15 @@
         if pyro_model is None:
             pyro_model = MultitaskSaasPyroModel()
         pyro_model.set_inputs(
             train_X=transformed_X,
             train_Y=train_Y,
             train_Yvar=train_Yvar,
             task_feature=task_feature,
-            task_rank=rank,
+            task_rank=self._rank,
         )
         self.pyro_model = pyro_model
         if outcome_transform is not None:
             self.outcome_transform = outcome_transform
         if input_transform is not None:
             self.input_transform = input_transform
 
@@ -330,29 +334,30 @@
     def posterior(
         self,
         X: Tensor,
         output_indices: Optional[List[int]] = None,
         observation_noise: bool = False,
         posterior_transform: Optional[PosteriorTransform] = None,
         **kwargs: Any,
-    ) -> FullyBayesianPosterior:
+    ) -> GaussianMixturePosterior:
         r"""Computes the posterior over model outputs at the provided points.
 
         Returns:
-            A `FullyBayesianPosterior` object. Includes observation noise if specified.
+            A `GaussianMixturePosterior` object. Includes observation noise
+                if specified.
         """
         self._check_if_fitted()
         posterior = super().posterior(
             X=X,
             output_indices=output_indices,
             observation_noise=observation_noise,
             posterior_transform=posterior_transform,
             **kwargs,
         )
-        posterior = FullyBayesianPosterior(distribution=posterior.distribution)
+        posterior = GaussianMixturePosterior(distribution=posterior.distribution)
         return posterior
 
     def forward(self, X: Tensor) -> MultivariateNormal:
         self._check_if_fitted()
         X = X.unsqueeze(MCMC_DIM)
 
         x_basic, task_idcs = self._split_inputs(X)
@@ -377,23 +382,23 @@
         covar_i = self.task_covar_module(latent_features)
         covar = covar_x.mul(covar_i)
         return MultivariateNormal(mean_x, covar)
 
     @classmethod
     def construct_inputs(
         cls,
-        training_data: Dict[str, SupervisedDataset],
+        training_data: Union[SupervisedDataset, MultiTaskDataset],
         task_feature: int,
         rank: Optional[int] = None,
         **kwargs: Any,
     ) -> Dict[str, Any]:
-        r"""Construct `Model` keyword arguments from dictionary of `SupervisedDataset`.
+        r"""Construct `Model` keyword arguments from a dataset and other args.
 
         Args:
-            training_data: Dictionary of `SupervisedDataset`.
+            training_data: A `SupervisedDataset` or a `MultiTaskDataset`.
             task_feature: Column index of embedded task indicator features. For details,
                 see `parse_training_data`.
             rank: The rank of the cross-task covariance matrix.
         """
         inputs = super().construct_inputs(
             training_data=training_data, task_feature=task_feature, rank=rank, **kwargs
         )
@@ -420,24 +425,23 @@
         if not isinstance(self.pyro_model, MultitaskSaasPyroModel):
             raise NotImplementedError(  # pragma: no cover
                 "load_state_dict only works for MultitaskSaasPyroModel"
             )
         raw_mean = state_dict["mean_module.raw_constant"]
         num_mcmc_samples = len(raw_mean)
         dim = self.pyro_model.train_X.shape[-1] - 1  # Removing 1 for the task feature.
-        task_rank = self.pyro_model.task_rank
         tkwargs = {"device": raw_mean.device, "dtype": raw_mean.dtype}
         # Load some dummy samples
         mcmc_samples = {
             "mean": torch.ones(num_mcmc_samples, **tkwargs),
             "lengthscale": torch.ones(num_mcmc_samples, dim, **tkwargs),
             "outputscale": torch.ones(num_mcmc_samples, **tkwargs),
-            "task_lengthscale": torch.ones(num_mcmc_samples, task_rank, **tkwargs),
+            "task_lengthscale": torch.ones(num_mcmc_samples, self._rank, **tkwargs),
             "latent_features": torch.ones(
-                num_mcmc_samples, self._rank, task_rank, **tkwargs
+                num_mcmc_samples, self.num_tasks, self._rank, **tkwargs
             ),
         }
         if self.pyro_model.train_Yvar is None:
             mcmc_samples["noise"] = torch.ones(num_mcmc_samples, **tkwargs)
         (
             self.mean_module,
             self.covar_module,
```

### Comparing `botorch-0.9.4/botorch/models/gp_regression.py` & `botorch-0.9.5/botorch/models/gp_regression.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/gp_regression_fidelity.py` & `botorch-0.9.5/botorch/models/gp_regression_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/gp_regression_mixed.py` & `botorch-0.9.5/botorch/models/gp_regression_mixed.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/gpytorch.py` & `botorch-0.9.5/botorch/models/gpytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 from botorch.models.utils import (
     _make_X_full,
     add_output_dim,
     gpt_posterior_settings,
     mod_batch_shape,
     multioutput_to_batch_mode_transform,
 )
-from botorch.posteriors.fully_bayesian import FullyBayesianPosterior
+from botorch.posteriors.fully_bayesian import GaussianMixturePosterior
 from botorch.posteriors.gpytorch import GPyTorchPosterior
-from botorch.utils.transforms import is_fully_bayesian
+from botorch.utils.transforms import is_ensemble
 from gpytorch.distributions import MultitaskMultivariateNormal, MultivariateNormal
 from gpytorch.likelihoods.gaussian_likelihood import FixedNoiseGaussianLikelihood
 from torch import Tensor
 
 if TYPE_CHECKING:
     from botorch.posteriors.posterior_list import PosteriorList  # pragma: no cover
     from botorch.posteriors.transformed import TransformedPosterior  # pragma: no cover
@@ -170,14 +170,17 @@
             specified.
         """
         self.eval()  # make sure model is in eval mode
         # input transforms are applied at `posterior` in `eval` mode, and at
         # `model.forward()` at the training time
         X = self.transform_inputs(X)
         with gpt_posterior_settings():
+            # NOTE: BoTorch's GPyTorchModels also inherit from GPyTorch's ExactGP, thus
+            # self(X) calls GPyTorch's ExactGP's __call__, which computes the posterior,
+            # rather than e.g. SingleTaskGP's forward, which computes the prior.
             mvn = self(X)
             if observation_noise is not False:
                 if isinstance(observation_noise, torch.Tensor):
                     # TODO: Make sure observation noise is transformed correctly
                     self._validate_tensor_args(X=X, Y=observation_noise)
                     if observation_noise.size(-1) == 1:
                         observation_noise = observation_noise.squeeze(-1)
@@ -370,14 +373,17 @@
         X = self.transform_inputs(X)
         with gpt_posterior_settings():
             # insert a dimension for the output dimension
             if self._num_outputs > 1:
                 X, output_dim_idx = add_output_dim(
                     X=X, original_batch_shape=self._input_batch_shape
                 )
+            # NOTE: BoTorch's GPyTorchModels also inherit from GPyTorch's ExactGP, thus
+            # self(X) calls GPyTorch's ExactGP's __call__, which computes the posterior,
+            # rather than e.g. SingleTaskGP's forward, which computes the prior.
             mvn = self(X)
             if observation_noise is not False:
                 if self._num_outputs > 1:
                     noise_shape = X.shape[:-3] + torch.Size(
                         [self._num_outputs, X.shape[-2]]
                     )
                 else:
@@ -609,15 +615,15 @@
                 of the `i`-th model).
             posterior_transform: An optional PosteriorTransform.
 
         Returns:
             - If no `posterior_transform` is provided and the component models have no
                 `outcome_transform`, or if the component models only use linear outcome
                 transforms like `Standardize` (i.e. not `Log`), returns a
-                `GPyTorchPosterior` or `FullyBayesianPosterior` object,
+                `GPyTorchPosterior` or `GaussianMixturePosterior` object,
                 representing `batch_shape` joint distributions over `q` points
                 and the outputs selected by `output_indices` each. Includes
                 measurement noise if `observation_noise` is specified.
             - If no `posterior_transform` is provided and component models have
                 nonlinear transforms like `Log`, returns a `PosteriorList` with
                 sub-posteriors of type `TransformedPosterior`
             - If `posterior_transform` is provided, that posterior transform will be
@@ -640,24 +646,24 @@
             observation_noise=observation_noise,
             **kwargs,
         )
         if not returns_untransformed:
             mvns = [p.distribution for p in posterior.posteriors]
             # Combining MTMVNs into a single MTMVN is currently not supported.
             if not any(isinstance(m, MultitaskMultivariateNormal) for m in mvns):
-                # Return the result as a GPyTorchPosterior/FullyBayesianPosterior.
+                # Return the result as a GPyTorchPosterior/GaussianMixturePosterior.
                 mvn = (
                     mvns[0]
                     if len(mvns) == 1
                     else MultitaskMultivariateNormal.from_independent_mvns(mvns=mvns)
                 )
-                if any(is_fully_bayesian(m) for m in self.models):
+                if any(is_ensemble(m) for m in self.models):
                     # Mixing fully Bayesian and other GP models is currently
                     # not supported.
-                    posterior = FullyBayesianPosterior(distribution=mvn)
+                    posterior = GaussianMixturePosterior(distribution=mvn)
                 else:
                     posterior = GPyTorchPosterior(distribution=mvn)
         if posterior_transform is not None:
             return posterior_transform(posterior)
         return posterior
 
     def condition_on_observations(self, X: Tensor, Y: Tensor, **kwargs: Any) -> Model:
```

### Comparing `botorch-0.9.4/botorch/models/higher_order_gp.py` & `botorch-0.9.5/botorch/models/higher_order_gp.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/kernels/__init__.py` & `botorch-0.9.5/botorch/models/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/kernels/categorical.py` & `botorch-0.9.5/botorch/models/kernels/categorical.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/kernels/contextual_lcea.py` & `botorch-0.9.5/botorch/models/kernels/contextual_lcea.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/kernels/contextual_sac.py` & `botorch-0.9.5/botorch/models/kernels/contextual_sac.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/kernels/downsampling.py` & `botorch-0.9.5/botorch/models/kernels/downsampling.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/kernels/exponential_decay.py` & `botorch-0.9.5/botorch/models/kernels/exponential_decay.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/kernels/linear_truncated_fidelity.py` & `botorch-0.9.5/botorch/models/kernels/linear_truncated_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/kernels/orthogonal_additive_kernel.py` & `botorch-0.9.5/botorch/models/kernels/orthogonal_additive_kernel.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/likelihoods/pairwise.py` & `botorch-0.9.5/botorch/models/likelihoods/pairwise.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/model.py` & `botorch-0.9.5/botorch/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from copy import deepcopy
 from typing import (
     Any,
     Callable,
     Dict,
-    Hashable,
     List,
     Mapping,
     Optional,
     Set,
     TYPE_CHECKING,
     TypeVar,
     Union,
@@ -67,25 +66,31 @@
     `documentation <https://pytorch.org/tutorials/beginner/examples_nn/polynomial_module.html>`_
     on custom NN Modules.
 
     `Module` provides several pieces of useful functionality: A `Model`'s attributes of
     `Tensor` or `Module` type are automatically registered so they can be moved and/or
     cast with the `to` method, automatically differentiated, and used with CUDA.
 
-    Args:
+    Attributes:
         _has_transformed_inputs: A boolean denoting whether `train_inputs` are currently
             stored as transformed or not.
         _original_train_inputs: A Tensor storing the original train inputs for use in
             `_revert_to_original_inputs`. Note that this is necessary since
             transform / untransform cycle introduces numerical errors which lead
             to upstream errors during training.
+        _is_fully_bayesian: Returns `True` if this is a fully Bayesian model.
+        _is_ensemble: Returns `True` if this model consists of multiple models
+            that are stored in an additional batch dimension. This is true for the fully
+            Bayesian models.
     """  # noqa: E501
 
     _has_transformed_inputs: bool = False
     _original_train_inputs: Optional[Tensor] = None
+    _is_fully_bayesian = False
+    _is_ensemble = False
 
     @abstractmethod
     def posterior(
         self,
         X: Tensor,
         output_indices: Optional[List[int]] = None,
         observation_noise: Union[bool, Tensor] = False,
@@ -176,15 +181,15 @@
         raise NotImplementedError(
             f"`condition_on_observations` not implemented for {self.__class__.__name__}"
         )
 
     @classmethod
     def construct_inputs(
         cls,
-        training_data: Union[SupervisedDataset, Dict[Hashable, SupervisedDataset]],
+        training_data: SupervisedDataset,
         **kwargs: Any,
     ) -> Dict[str, Any]:
         r"""Construct `Model` keyword arguments from a dict of `SupervisedDataset`."""
         from botorch.models.utils.parse_training_data import parse_training_data
 
         return parse_training_data(cls, training_data, **kwargs)
 
@@ -370,14 +375,16 @@
             output_shape = (
                 sampler.sample_shape
                 + X.shape[:-2]
                 + self.batch_shape
                 + torch.Size([0, self.num_outputs])
             )
             Y = torch.empty(output_shape, dtype=X.dtype, device=X.device)
+            if observation_noise is not None:
+                kwargs["noise"] = observation_noise.expand(Y.shape[1:])
             return self.condition_on_observations(
                 X=self.transform_inputs(X),
                 Y=Y,
                 **kwargs,
             )
         propagate_grads = kwargs.pop("propagate_grads", False)
         with fantasize_flag():
@@ -651,15 +658,17 @@
                 # TODO (T158701749): implement a QMC DecoupledSampler that draws all
                 # samples from a single Sobol sequence or consider requiring that the
                 # sampling is IID to ensure good coverage.
                 sampler_i = sampler.samplers[i]
                 if observation_noise is not None:
                     observation_noise_i = observation_noise[..., mask_i, i : i + 1]
             else:
-                sampler_i = sampler
+                sampler_i = (
+                    sampler.samplers[i] if isinstance(sampler, ListSampler) else sampler
+                )
 
             fant_model = self.models[i].fantasize(
                 X=X_i,
                 sampler=sampler_i,
                 observation_noise=observation_noise_i,
                 **kwargs,
             )
```

### Comparing `botorch-0.9.4/botorch/models/model_list_gp_regression.py` & `botorch-0.9.5/botorch/models/model_list_gp_regression.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/multitask.py` & `botorch-0.9.5/botorch/models/multitask.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from botorch.models.transforms.input import InputTransform
 from botorch.models.transforms.outcome import OutcomeTransform
 from botorch.models.utils.gpytorch_modules import (
     get_matern_kernel_with_gamma_prior,
     MIN_INFERRED_NOISE_LEVEL,
 )
 from botorch.posteriors.multitask import MultitaskGPPosterior
-from botorch.utils.datasets import SupervisedDataset
+from botorch.utils.datasets import MultiTaskDataset, SupervisedDataset
 from gpytorch.constraints import GreaterThan
 from gpytorch.distributions.multitask_multivariate_normal import (
     MultitaskMultivariateNormal,
 )
 from gpytorch.distributions.multivariate_normal import MultivariateNormal
 from gpytorch.kernels.index_kernel import IndexKernel
 from gpytorch.kernels.matern_kernel import MaternKernel
@@ -267,26 +267,26 @@
         task_feature = task_feature % (d + 1)
         all_tasks = train_X[:, task_feature].unique().to(dtype=torch.long).tolist()
         return all_tasks, task_feature, d
 
     @classmethod
     def construct_inputs(
         cls,
-        training_data: Dict[str, SupervisedDataset],
+        training_data: Union[SupervisedDataset, MultiTaskDataset],
         task_feature: int,
         output_tasks: Optional[List[int]] = None,
         task_covar_prior: Optional[Prior] = None,
         prior_config: Optional[dict] = None,
         rank: Optional[int] = None,
         **kwargs,
     ) -> Dict[str, Any]:
-        r"""Construct `Model` keyword arguments from dictionary of `SupervisedDataset`.
+        r"""Construct `Model` keyword arguments from a dataset and other args.
 
         Args:
-            training_data: Dictionary of `SupervisedDataset`.
+            training_data: A `SupervisedDataset` or a `MultiTaskDataset`.
             task_feature: Column index of embedded task indicator features. For details,
                 see `parse_training_data`.
             output_tasks: A list of task indices for which to compute model
                 outputs for. If omitted, return outputs for all task indices.
             task_covar_prior: A GPyTorch `Prior` object to use as prior on
                 the cross-task covariance matrix,
             prior_config: Configuration for inter-task covariance prior.
@@ -299,15 +299,15 @@
                 "Only one of `task_covar_prior` and `prior_config` arguments expected."
             )
 
         if prior_config is not None:
             if not prior_config.get("use_LKJ_prior"):
                 raise ValueError("Currently only config for LKJ prior is supported.")
 
-            num_tasks = len(training_data)
+            num_tasks = training_data.X[task_feature].unique().numel()
             sd_prior = GammaPrior(1.0, 0.15)
             sd_prior._event_shape = torch.Size([num_tasks])
             eta = prior_config.get("eta", 0.5)
             if not isinstance(eta, float) and not isinstance(eta, int):
                 raise ValueError(f"eta must be a real number, your eta was {eta}.")
             task_covar_prior = LKJCovariancePrior(num_tasks, eta, sd_prior)
```

### Comparing `botorch-0.9.4/botorch/models/pairwise_gp.py` & `botorch-0.9.5/botorch/models/pairwise_gp.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/transforms/__init__.py` & `botorch-0.9.5/botorch/models/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/transforms/factory.py` & `botorch-0.9.5/botorch/models/transforms/factory.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/transforms/input.py` & `botorch-0.9.5/botorch/models/transforms/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,15 +946,18 @@
             reverse: A boolean indicating whether the forward pass should untransform
                 the inputs.
             eps: A small value used to clip values to be in the interval (0, 1).
             concentration1_prior: A prior distribution on the concentration1 parameter
                 of the Kumaraswamy distribution.
             concentration0_prior: A prior distribution on the concentration0 parameter
                 of the Kumaraswamy distribution.
-            batch_shape: The batch shape.
+            batch_shape: An optional batch shape, for learning independent warping
+                parameters for each batch of inputs. This should match the input batch
+                shape of the model (i.e., `train_X.shape[:-2]`).
+                NOTE: This is only supported for single-output models.
         """
         super().__init__()
         self.register_buffer("indices", torch.tensor(indices, dtype=torch.long))
         self.transform_on_train = transform_on_train
         self.transform_on_eval = transform_on_eval
         self.transform_on_fantasize = transform_on_fantasize
         self.reverse = reverse
```

### Comparing `botorch-0.9.4/botorch/models/transforms/outcome.py` & `botorch-0.9.5/botorch/models/transforms/outcome.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/transforms/utils.py` & `botorch-0.9.5/botorch/models/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/utils/__init__.py` & `botorch-0.9.5/botorch/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/utils/assorted.py` & `botorch-0.9.5/botorch/models/utils/assorted.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,16 @@
         # check that X_batch_shape supports broadcasting or augments
         # original_batch_shape with extra batch dims
         try:
             torch.broadcast_shapes(X_batch_shape, original_batch_shape)
         except RuntimeError:
             raise RuntimeError(
                 "The trailing batch dimensions of X must match the trailing "
-                "batch dimensions of the training inputs."
+                f"batch dimensions of the training inputs. Got {X.shape=} "
+                f"and {original_batch_shape=}."
             )
     # insert `m` dimension
     X = X.unsqueeze(-3)
     output_dim_idx = max(len(original_batch_shape), len(X_batch_shape))
     return X, output_dim_idx
```

### Comparing `botorch-0.9.4/botorch/models/utils/gpytorch_modules.py` & `botorch-0.9.5/botorch/models/utils/gpytorch_modules.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/models/utils/inducing_point_allocators.py` & `botorch-0.9.5/botorch/models/utils/inducing_point_allocators.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/__init__.py` & `botorch-0.9.5/botorch/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/closures/__init__.py` & `botorch-0.9.5/botorch/optim/closures/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/closures/core.py` & `botorch-0.9.5/botorch/optim/closures/core.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/closures/model_closures.py` & `botorch-0.9.5/botorch/optim/closures/model_closures.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/core.py` & `botorch-0.9.5/botorch/optim/core.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/fit.py` & `botorch-0.9.5/botorch/optim/fit.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/homotopy.py` & `botorch-0.9.5/botorch/optim/homotopy.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/initializers.py` & `botorch-0.9.5/botorch/optim/initializers.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,18 +18,24 @@
 from math import ceil
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import torch
 from botorch import settings
 from botorch.acquisition import analytic, monte_carlo, multi_objective
 from botorch.acquisition.acquisition import AcquisitionFunction
+from botorch.acquisition.fixed_feature import FixedFeatureAcquisitionFunction
 from botorch.acquisition.knowledge_gradient import (
     _get_value_function,
     qKnowledgeGradient,
 )
+from botorch.acquisition.multi_objective.hypervolume_knowledge_gradient import (
+    _get_hv_value_function,
+    qHypervolumeKnowledgeGradient,
+    qMultiFidelityHypervolumeKnowledgeGradient,
+)
 from botorch.exceptions.errors import BotorchTensorDimensionError, UnsupportedError
 from botorch.exceptions.warnings import (
     BadInitialCandidatesWarning,
     BotorchWarning,
     SamplingWarning,
 )
 from botorch.models.model import Model
@@ -241,14 +247,15 @@
     num_restarts: int,
     raw_samples: int,
     fixed_features: Optional[Dict[int, float]] = None,
     options: Optional[Dict[str, Union[bool, float, int]]] = None,
     inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
     equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
     generator: Optional[Callable[[int, int, int], Tensor]] = None,
+    fixed_X_fantasies: Optional[Tensor] = None,
 ) -> Tensor:
     r"""Generate a batch of initial conditions for random-restart optimziation.
 
     TODO: Support t-batches of initial conditions.
 
     Args:
         acq_function: The acquisition function to be optimized.
@@ -274,14 +281,19 @@
             `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`.
         equality constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
         generator: Callable for generating samples that are then further
             processed. It receives `n`, `q` and `seed` as arguments and
             returns a tensor of shape `n x q x d`.
+        fixed_X_fantasies: A fixed set of fantasy points to concatenate to
+            the `q` candidates being initialized along the `-2` dimension. The
+            shape should be `num_pseudo_points x d`. E.g., this should be
+            `num_fantasies x d` for KG and `num_fantasies*num_pareto x d`
+            for HVKG.
 
     Returns:
         A `num_restarts x q x d` tensor of initial conditions.
 
     Example:
         >>> qEI = qExpectedImprovement(model, best_f=0.2)
         >>> bounds = torch.tensor([[0.], [1.]])
@@ -375,14 +387,30 @@
                         [
                             X_rnd,
                             X_best_rnd.view(n, q, bounds.shape[-1]).cpu(),
                         ],
                         dim=0,
                     )
             X_rnd = fix_features(X_rnd, fixed_features=fixed_features)
+            if fixed_X_fantasies is not None:
+                if (d_f := fixed_X_fantasies.shape[-1]) != (d_r := X_rnd.shape[-1]):
+                    raise BotorchTensorDimensionError(
+                        "`fixed_X_fantasies` and `bounds` must both have the same "
+                        f"trailing dimension `d`, but have {d_f} and {d_r}, "
+                        "respectively."
+                    )
+                X_rnd = torch.cat(
+                    [
+                        X_rnd,
+                        fixed_X_fantasies.cpu()
+                        .unsqueeze(0)
+                        .expand(X_rnd.shape[0], *fixed_X_fantasies.shape),
+                    ],
+                    dim=-2,
+                )
             with torch.no_grad():
                 if batch_limit is None:
                     batch_limit = X_rnd.shape[0]
                 Y_rnd_list = []
                 start_idx = 0
                 while start_idx < X_rnd.shape[0]:
                     end_idx = min(start_idx + batch_limit, X_rnd.shape[0])
@@ -421,26 +449,26 @@
     equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
 ) -> Optional[Tensor]:
     r"""Generate a batch of smart initializations for qKnowledgeGradient.
 
     This function generates initial conditions for optimizing one-shot KG using
     the maximizer of the posterior objective. Intutively, the maximizer of the
     fantasized posterior will often be close to a maximizer of the current
-    posterior. This function uses that fact to generate the initital conditions
+    posterior. This function uses that fact to generate the initial conditions
     for the fantasy points. Specifically, a fraction of `1 - frac_random` (see
     options) is generated by sampling from the set of maximizers of the
     posterior objective (obtained via random restart optimization) according to
     a softmax transformation of their respective values. This means that this
     initialization strategy internally solves an acquisition function
     maximization problem. The remaining `frac_random` fantasy points as well as
     all `q` candidate points are chosen according to the standard initialization
     strategy in `gen_batch_initial_conditions`.
 
     Args:
-        acq_function: The qKnowledgeGradient instance to be optimized.
+        acq_function: The qHypervolumeKnowledgeGradient instance to be optimized.
         bounds: A `2 x d` tensor of lower and upper bounds for each column of
             task features.
         q: The number of candidates to consider.
         num_restarts: The number of starting points for multistart acquisition
             function optimization.
         raw_samples: The number of raw samples to consider in the initialization
             heuristic.
@@ -463,18 +491,18 @@
 
     Returns:
         A `num_restarts x q' x d` tensor that can be used as initial conditions
         for `optimize_acqf()`. Here `q' = q + num_fantasies` is the total number
         of points (candidate points plus fantasy points).
 
     Example:
-        >>> qKG = qKnowledgeGradient(model, num_fantasies=64)
+        >>> qHVKG = qHypervolumeKnowledgeGradient(model, ref_point=num_fantasies=64)
         >>> bounds = torch.tensor([[0., 0.], [1., 1.]])
-        >>> Xinit = gen_one_shot_kg_initial_conditions(
-        >>>     qKG, bounds, q=3, num_restarts=10, raw_samples=512,
+        >>> Xinit = gen_one_shot_hvkg_initial_conditions(
+        >>>     qHVKG, bounds, q=3, num_restarts=10, raw_samples=512,
         >>>     options={"frac_random": 0.25},
         >>> )
     """
     options = options or {}
     frac_random: float = options.get("frac_random", 0.1)
     if not 0 < frac_random < 1:
         raise ValueError(
@@ -524,14 +552,212 @@
     idx = torch.multinomial(weights, num_restarts * n_value, replacement=True)
 
     # set the respective initial conditions to the sampled optimizers
     ics[..., -n_value:, :] = fantasy_cands[idx, 0].view(num_restarts, n_value, -1)
     return ics
 
 
+def gen_one_shot_hvkg_initial_conditions(
+    acq_function: qHypervolumeKnowledgeGradient,
+    bounds: Tensor,
+    q: int,
+    num_restarts: int,
+    raw_samples: int,
+    fixed_features: Optional[Dict[int, float]] = None,
+    options: Optional[Dict[str, Union[bool, float, int]]] = None,
+    inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
+    equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
+) -> Optional[Tensor]:
+    r"""Generate a batch of smart initializations for qHypervolumeKnowledgeGradient.
+
+    This function generates initial conditions for optimizing one-shot HVKG using
+    the hypervolume maximizing set (of fixed size) under the posterior mean.
+    Intutively, the hypervolume maximizing set of the fantasized posterior mean
+    will often be close to a hypervolume maximizing set under the current posterior
+    mean. This function uses that fact to generate the initial conditions
+    for the fantasy points. Specifically, a fraction of `1 - frac_random` (see
+    options) of the restarts are generated by learning the hypervolume maximizing sets
+    under the current posterior mean, where each hypervolume maximizing set is
+    obtained from maximizing the hypervolume from a different starting point. Given
+    a hypervolume maximizing set, the `q` candidate points are selected using to the
+    standard initialization strategy in `gen_batch_initial_conditions`, with the fixed
+    hypervolume maximizing set. The remaining `frac_random` restarts fantasy points
+    as well as all `q` candidate points are chosen according to the standard
+    initialization strategy in `gen_batch_initial_conditions`.
+
+    Args:
+        acq_function: The qKnowledgeGradient instance to be optimized.
+        bounds: A `2 x d` tensor of lower and upper bounds for each column of
+            task features.
+        q: The number of candidates to consider.
+        num_restarts: The number of starting points for multistart acquisition
+            function optimization.
+        raw_samples: The number of raw samples to consider in the initialization
+            heuristic.
+        fixed_features: A map `{feature_index: value}` for features that
+            should be fixed to a particular value during generation.
+        options: Options for initial condition generation. These contain all
+            settings for the standard heuristic initialization from
+            `gen_batch_initial_conditions`. In addition, they contain
+            `frac_random` (the fraction of fully random fantasy points),
+            `num_inner_restarts` and `raw_inner_samples` (the number of random
+            restarts and raw samples for solving the posterior objective
+            maximization problem, respectively) and `eta` (temperature parameter
+            for sampling heuristic from posterior objective maximizers).
+        inequality constraints: A list of tuples (indices, coefficients, rhs),
+            with each tuple encoding an inequality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`.
+        equality constraints: A list of tuples (indices, coefficients, rhs),
+            with each tuple encoding an inequality constraint of the form
+            `\sum_i (X[indices[i]] * coefficients[i]) = rhs`.
+
+    Returns:
+        A `num_restarts x q' x d` tensor that can be used as initial conditions
+        for `optimize_acqf()`. Here `q' = q + num_fantasies` is the total number
+        of points (candidate points plus fantasy points).
+
+    Example:
+        >>> qHVKG = qHypervolumeKnowledgeGradient(model, ref_point)
+        >>> bounds = torch.tensor([[0., 0.], [1., 1.]])
+        >>> Xinit = gen_one_shot_hvkg_initial_conditions(
+        >>>     qHVKG, bounds, q=3, num_restarts=10, raw_samples=512,
+        >>>     options={"frac_random": 0.25},
+        >>> )
+    """
+    from botorch.optim.optimize import optimize_acqf
+
+    options = options or {}
+    frac_random: float = options.get("frac_random", 0.1)
+    if not 0 < frac_random < 1:
+        raise ValueError(
+            f"frac_random must take on values in (0,1). Value: {frac_random}"
+        )
+
+    value_function = _get_hv_value_function(
+        model=acq_function.model,
+        ref_point=acq_function.ref_point,
+        objective=acq_function.objective,
+        sampler=acq_function.inner_sampler,
+        use_posterior_mean=acq_function.use_posterior_mean,
+    )
+
+    is_mf_hvkg = isinstance(acq_function, qMultiFidelityHypervolumeKnowledgeGradient)
+    if is_mf_hvkg:
+        dim = bounds.shape[-1]
+        fidelity_dims, fidelity_targets = zip(*acq_function.target_fidelities.items())
+        value_function = FixedFeatureAcquisitionFunction(
+            acq_function=value_function,
+            d=dim,
+            columns=fidelity_dims,
+            values=fidelity_targets,
+        )
+
+        non_fidelity_dims = list(set(range(dim)) - set(fidelity_dims))
+
+    num_optim_restarts = int(round(num_restarts * (1 - frac_random)))
+    fantasy_cands, fantasy_vals = optimize_acqf(
+        acq_function=value_function,
+        bounds=bounds[:, non_fidelity_dims] if is_mf_hvkg else bounds,
+        q=acq_function.num_pareto,
+        num_restarts=options.get("num_inner_restarts", 20),
+        raw_samples=options.get("raw_inner_samples", 1024),
+        fixed_features=fixed_features,
+        return_best_only=False,
+        options=options,
+        inequality_constraints=inequality_constraints,
+        equality_constraints=equality_constraints,
+        sequential=False,
+    )
+    # sampling from the optimizers
+    eta = options.get("eta", 2.0)
+    if num_optim_restarts > 0:
+        probs = torch.nn.functional.softmax(eta * standardize(fantasy_vals), dim=0)
+        idx = torch.multinomial(
+            probs,
+            num_optim_restarts * acq_function.num_fantasies,
+            replacement=True,
+        )
+        optim_ics = fantasy_cands[idx]
+        if is_mf_hvkg:
+            # add fixed features
+            optim_ics = value_function._construct_X_full(optim_ics)
+        optim_ics = optim_ics.reshape(
+            num_optim_restarts, acq_function.num_pseudo_points, bounds.shape[-1]
+        )
+
+    # get random initial conditions
+    num_random_restarts = num_restarts - num_optim_restarts
+    if num_random_restarts > 0:
+        q_aug = acq_function.get_augmented_q_batch_size(q=q)
+        base_ics = gen_batch_initial_conditions(
+            acq_function=acq_function,
+            bounds=bounds,
+            q=q_aug,
+            num_restarts=num_restarts,
+            raw_samples=raw_samples,
+            fixed_features=fixed_features,
+            options=options,
+            inequality_constraints=inequality_constraints,
+            equality_constraints=equality_constraints,
+        )
+
+        if num_optim_restarts > 0:
+            probs = torch.full(
+                (num_restarts,),
+                1.0 / num_restarts,
+                dtype=optim_ics.dtype,
+                device=optim_ics.device,
+            )
+            optim_idxr = probs.multinomial(
+                num_samples=num_optim_restarts, replacement=False
+            )
+            base_ics[optim_idxr, q:] = optim_ics
+    else:
+        # optim_ics is num_restarts x num_pseudo_points x d
+        # add padding so that base_ics is num_restarts x q+num_pseudo_points x d
+        q_padding = torch.zeros(
+            optim_ics.shape[0],
+            q,
+            optim_ics.shape[-1],
+            dtype=optim_ics.dtype,
+            device=optim_ics.device,
+        )
+        base_ics = torch.cat([q_padding, optim_ics], dim=-2)
+
+    if num_optim_restarts > 0:
+        all_ics = []
+        if num_random_restarts > 0:
+            optim_idcs = optim_idxr.view(-1).tolist()
+        else:
+            optim_idcs = list(range(num_restarts))
+        for i in list(range(num_restarts)):
+            if i in optim_idcs:
+                # optimize the q points,
+                # given fixed, optimized fantasy designs
+                ics = gen_batch_initial_conditions(
+                    acq_function=acq_function,
+                    bounds=bounds,
+                    q=q,
+                    num_restarts=1,
+                    raw_samples=raw_samples,
+                    fixed_features=fixed_features,
+                    options=options,
+                    inequality_constraints=inequality_constraints,
+                    equality_constraints=equality_constraints,
+                    fixed_X_fantasies=base_ics[i, q:],
+                )
+            else:
+                # ics are all randomly sampled
+                ics = base_ics[i : i + 1]
+            all_ics.append(ics)
+        return torch.cat(all_ics, dim=0)
+
+    return base_ics
+
+
 def gen_value_function_initial_conditions(
     acq_function: AcquisitionFunction,
     bounds: Tensor,
     num_restarts: int,
     raw_samples: int,
     current_model: Model,
     fixed_features: Optional[Dict[int, float]] = None,
```

### Comparing `botorch-0.9.4/botorch/optim/optimize.py` & `botorch-0.9.5/botorch/optim/optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,24 @@
 
 import torch
 from botorch.acquisition.acquisition import (
     AcquisitionFunction,
     OneShotAcquisitionFunction,
 )
 from botorch.acquisition.knowledge_gradient import qKnowledgeGradient
+from botorch.acquisition.multi_objective.hypervolume_knowledge_gradient import (
+    qHypervolumeKnowledgeGradient,
+)
 from botorch.exceptions import InputDataError, UnsupportedError
 from botorch.exceptions.warnings import OptimizationWarning
 from botorch.generation.gen import gen_candidates_scipy, TGenCandidates
 from botorch.logging import logger
 from botorch.optim.initializers import (
     gen_batch_initial_conditions,
+    gen_one_shot_hvkg_initial_conditions,
     gen_one_shot_kg_initial_conditions,
     TGenInitialConditions,
 )
 from botorch.optim.stopping import ExpMAStoppingCriterion
 from botorch.optim.utils import _filter_kwargs
 from torch import Tensor
 
@@ -65,15 +69,15 @@
     bounds: Tensor
     q: int
     num_restarts: int
     raw_samples: Optional[int]
     options: Optional[Dict[str, Union[bool, float, int, str]]]
     inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]]
     equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]]
-    nonlinear_inequality_constraints: Optional[List[Callable]]
+    nonlinear_inequality_constraints: Optional[List[Tuple[Callable, bool]]]
     fixed_features: Optional[Dict[int, float]]
     post_processing_func: Optional[Callable[[Tensor], Tensor]]
     batch_initial_conditions: Optional[Tensor]
     return_best_only: bool
     gen_candidates: TGenCandidates
     sequential: bool
     ic_generator: Optional[TGenInitialConditions] = None
@@ -125,14 +129,16 @@
                 )
 
     def get_ic_generator(self) -> TGenInitialConditions:
         if self.ic_generator is not None:
             return self.ic_generator
         elif isinstance(self.acq_function, qKnowledgeGradient):
             return gen_one_shot_kg_initial_conditions
+        elif isinstance(self.acq_function, qHypervolumeKnowledgeGradient):
+            return gen_one_shot_hvkg_initial_conditions
         return gen_batch_initial_conditions
 
 
 def _raise_deprecation_warning_if_kwargs(fn_name: str, kwargs: Dict[str, Any]) -> None:
     """
     Raise a warning if kwargs are provided.
 
@@ -237,15 +243,14 @@
         q=1,
         batch_initial_conditions=None,
         return_best_only=True,
         sequential=False,
         timeout_sec=timeout_sec,
     )
     for i in range(opt_inputs.q):
-
         candidate, acq_value = _optimize_acqf_batch(new_inputs)
 
         candidate_list.append(candidate)
         acq_value_list.append(acq_value)
         candidates = torch.cat(candidate_list, dim=-2)
         new_inputs.acq_function.set_X_pending(
             torch.cat([base_X_pending, candidates], dim=-2)
@@ -414,15 +419,15 @@
     bounds: Tensor,
     q: int,
     num_restarts: int,
     raw_samples: Optional[int] = None,
     options: Optional[Dict[str, Union[bool, float, int, str]]] = None,
     inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
     equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
-    nonlinear_inequality_constraints: Optional[List[Callable]] = None,
+    nonlinear_inequality_constraints: Optional[List[Tuple[Callable, bool]]] = None,
     fixed_features: Optional[Dict[int, float]] = None,
     post_processing_func: Optional[Callable[[Tensor], Tensor]] = None,
     batch_initial_conditions: Optional[Tensor] = None,
     return_best_only: bool = True,
     gen_candidates: Optional[TGenCandidates] = None,
     sequential: bool = False,
     *,
@@ -446,32 +451,40 @@
             if `batch_initial_conditions` is not specified.
         options: Options for candidate generation.
         inequality_constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`. `indices` and
             `coefficients` should be torch tensors. See the docstring of
             `make_scipy_linear_constraints` for an example. When q=1, or when
-            applying the same constraint to each candidate in the batch,
-            `indices` should be a 1-d tensor. For inter-point constraints,
-            `indices` must be a 2-d Tensor, where in each row `indices[i] =
-            (k_i, l_i)` the first index `k_i` corresponds to the `k_i`-th
-            element of the `q`-batch and the second index `l_i` corresponds to
-            the `l_i`-th feature of that element.
+            applying the same constraint to each candidate in the batch
+            (intra-point constraint), `indices` should be a 1-d tensor.
+            For inter-point constraints, in which the constraint is applied to the
+            whole batch of candidates, `indices` must be a 2-d tensor, where
+            in each row `indices[i] =(k_i, l_i)` the first index `k_i` corresponds
+            to the `k_i`-th element of the `q`-batch and the second index `l_i`
+            corresponds to the `l_i`-th feature of that element.
         equality_constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an equality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) = rhs`. See the docstring of
             `make_scipy_linear_constraints` for an example.
-        nonlinear_inequality_constraints: A list of callables with that represent
-            non-linear inequality constraints of the form `callable(x) >= 0`. Each
-            callable is expected to take a `(num_restarts) x q x d`-dim tensor as an
-            input and return a `(num_restarts) x q`-dim tensor with the constraint
-            values. The constraints will later be passed to SLSQP. You need to pass in
-            `batch_initial_conditions` in this case. Using non-linear inequality
-            constraints also requires that `batch_limit` is set to 1, which will be
-            done automatically if not specified in `options`.
+        nonlinear_inequality_constraints: A list of tuples representing the nonlinear
+            inequality constraints. The first element in the tuple is a callable
+            representing a constraint of the form `callable(x) >= 0`. In case of an
+            intra-point constraint, `callable()`takes in an one-dimensional tensor of
+            shape `d` and returns a scalar. In case of an inter-point constraint,
+            `callable()` takes a two dimensional tensor of shape `q x d` and again
+            returns a scalar. The second element is a boolean, indicating if it is an
+            intra-point or inter-point constraint (`True` for intra-point. `False` for
+            inter-point). For more information on intra-point vs inter-point
+            constraints, see the docstring of the `inequality_constraints` argument to
+            `optimize_acqf()`. The constraints will later be passed to the scipy
+            solver. You need to pass in `batch_initial_conditions` in this case.
+            Using non-linear inequality constraints also requires that `batch_limit`
+            is set to 1, which will be done automatically if not specified in
+            `options`.
         fixed_features: A map `{feature_index: value}` for features that
             should be fixed to a particular value during generation.
         post_processing_func: A function that post-processes an optimization
             result appropriately (i.e., according to `round-trip`
             transformations).
         batch_initial_conditions: A tensor to specify the initial conditions. Set
             this if you do not want to use default initialization strategy.
@@ -547,15 +560,14 @@
         retry_on_optimization_warning=retry_on_optimization_warning,
         ic_gen_kwargs=ic_gen_kwargs,
     )
     return _optimize_acqf(opt_acqf_inputs)
 
 
 def _optimize_acqf(opt_inputs: OptimizeAcqfInputs) -> Tuple[Tensor, Tensor]:
-
     # Handle the trivial case when all features are fixed
     if (
         opt_inputs.fixed_features is not None
         and len(opt_inputs.fixed_features) == opt_inputs.bounds.shape[-1]
     ):
         return _optimize_acqf_all_features_fixed(
             bounds=opt_inputs.bounds,
@@ -712,15 +724,15 @@
     acq_function_list: List[AcquisitionFunction],
     bounds: Tensor,
     num_restarts: int,
     raw_samples: Optional[int] = None,
     options: Optional[Dict[str, Union[bool, float, int, str]]] = None,
     inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
     equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
-    nonlinear_inequality_constraints: Optional[List[Callable]] = None,
+    nonlinear_inequality_constraints: Optional[List[Tuple[Callable, bool]]] = None,
     fixed_features: Optional[Dict[int, float]] = None,
     fixed_features_list: Optional[List[Dict[int, float]]] = None,
     post_processing_func: Optional[Callable[[Tensor], Tensor]] = None,
     ic_generator: Optional[TGenInitialConditions] = None,
     ic_gen_kwargs: Optional[Dict] = None,
 ) -> Tuple[Tensor, Tensor]:
     r"""Generate a list of candidates from a list of acquisition functions.
@@ -740,22 +752,29 @@
         options: Options for candidate generation.
         inequality constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`
         equality constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) = rhs`
-        nonlinear_inequality_constraints: A list of callables with that represent
-            non-linear inequality constraints of the form `callable(x) >= 0`. Each
-            callable is expected to take a `(num_restarts) x q x d`-dim tensor as an
-            input and return a `(num_restarts) x q`-dim tensor with the constraint
-            values. The constraints will later be passed to SLSQP. You need to pass in
-            `batch_initial_conditions` in this case. Using non-linear inequality
-            constraints also requires that `batch_limit` is set to 1, which will be
-            done automatically if not specified in `options`.
+        nonlinear_inequality_constraints: A list of tuples representing the nonlinear
+            inequality constraints. The first element in the tuple is a callable
+            representing a constraint of the form `callable(x) >= 0`. In case of an
+            intra-point constraint, `callable()`takes in an one-dimensional tensor of
+            shape `d` and returns a scalar. In case of an inter-point constraint,
+            `callable()` takes a two dimensional tensor of shape `q x d` and again
+            returns a scalar. The second element is a boolean, indicating if it is an
+            intra-point or inter-point constraint (`True` for intra-point. `False` for
+            inter-point). For more information on intra-point vs inter-point
+            constraints, see the docstring of the `inequality_constraints` argument to
+            `optimize_acqf()`. The constraints will later be passed to the scipy
+            solver. You need to pass in `batch_initial_conditions` in this case.
+            Using non-linear inequality constraints also requires that `batch_limit`
+            is set to 1, which will be done automatically if not specified in
+            `options`.
         fixed_features: A map `{feature_index: value}` for features that
             should be fixed to a particular value during generation.
         fixed_features_list: A list of maps `{feature_index: value}`. The i-th
             item represents the fixed_feature for the i-th optimization. If
             `fixed_features_list` is provided, `optimize_acqf_mixed` is invoked.
         post_processing_func: A function that post-processes an optimization
             result appropriately (i.e., according to `round-trip`
@@ -839,15 +858,15 @@
     q: int,
     num_restarts: int,
     fixed_features_list: List[Dict[int, float]],
     raw_samples: Optional[int] = None,
     options: Optional[Dict[str, Union[bool, float, int, str]]] = None,
     inequality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
     equality_constraints: Optional[List[Tuple[Tensor, Tensor, float]]] = None,
-    nonlinear_inequality_constraints: Optional[List[Callable]] = None,
+    nonlinear_inequality_constraints: Optional[List[Tuple[Callable, bool]]] = None,
     post_processing_func: Optional[Callable[[Tensor], Tensor]] = None,
     batch_initial_conditions: Optional[Tensor] = None,
     ic_generator: Optional[TGenInitialConditions] = None,
     ic_gen_kwargs: Optional[Dict] = None,
     **kwargs: Any,
 ) -> Tuple[Tensor, Tensor]:
     r"""Optimize over a list of fixed_features and returns the best solution.
@@ -871,22 +890,29 @@
         options: Options for candidate generation.
         inequality constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) >= rhs`
         equality constraints: A list of tuples (indices, coefficients, rhs),
             with each tuple encoding an inequality constraint of the form
             `\sum_i (X[indices[i]] * coefficients[i]) = rhs`
-        nonlinear_inequality_constraints: A list of callables with that represent
-            non-linear inequality constraints of the form `callable(x) >= 0`. Each
-            callable is expected to take a `(num_restarts) x q x d`-dim tensor as an
-            input and return a `(num_restarts) x q`-dim tensor with the constraint
-            values. The constraints will later be passed to SLSQP. You need to pass in
-            `batch_initial_conditions` in this case. Using non-linear inequality
-            constraints also requires that `batch_limit` is set to 1, which will be
-            done automatically if not specified in `options`.
+        nonlinear_inequality_constraints: A list of tuples representing the nonlinear
+            inequality constraints. The first element in the tuple is a callable
+            representing a constraint of the form `callable(x) >= 0`. In case of an
+            intra-point constraint, `callable()`takes in an one-dimensional tensor of
+            shape `d` and returns a scalar. In case of an inter-point constraint,
+            `callable()` takes a two dimensional tensor of shape `q x d` and again
+            returns a scalar. The second element is a boolean, indicating if it is an
+            intra-point or inter-point constraint (`True` for intra-point. `False` for
+            inter-point). For more information on intra-point vs inter-point
+            constraints, see the docstring of the `inequality_constraints` argument to
+            `optimize_acqf()`. The constraints will later be passed to the scipy
+            solver. You need to pass in `batch_initial_conditions` in this case.
+            Using non-linear inequality constraints also requires that `batch_limit`
+            is set to 1, which will be done automatically if not specified in
+            `options`.
         post_processing_func: A function that post-processes an optimization
             result appropriately (i.e., according to `round-trip`
             transformations).
         batch_initial_conditions: A tensor to specify the initial conditions. Set
             this if you do not want to use default initialization strategy.
         ic_generator: Function for generating initial conditions. Not needed when
             `batch_initial_conditions` are provided. Defaults to
@@ -1091,15 +1117,15 @@
 
 
 def _filter_infeasible(
     X: Tensor, inequality_constraints: List[Tuple[Tensor, Tensor, float]]
 ):
     """Remove all points from `X` that don't satisfy the constraints."""
     is_feasible = torch.ones(X.shape[0], dtype=torch.bool, device=X.device)
-    for (inds, weights, bound) in inequality_constraints:
+    for inds, weights, bound in inequality_constraints:
         is_feasible &= (X[..., inds] * weights).sum(dim=-1) >= bound
     return X[is_feasible]
 
 
 def _filter_invalid(X: Tensor, X_avoid: Tensor):
     """Remove all occurences of `X_avoid` from `X`."""
     return X[~(X == X_avoid.unsqueeze(-2)).all(dim=-1).any(dim=-2)]
```

### Comparing `botorch-0.9.4/botorch/optim/optimize_homotopy.py` & `botorch-0.9.5/botorch/optim/optimize_homotopy.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/parameter_constraints.py` & `botorch-0.9.5/botorch/optim/parameter_constraints.py`

 * *Files 16% similar despite different names*

```diff
@@ -308,16 +308,73 @@
                     eval_lin_constraint, flat_idxr=idxr, coeffs=coeffs, rhs=float(rhs)
                 )
                 jac = partial(lin_constraint_jac, flat_idxr=idxr, coeffs=coeffs, n=n)
                 constraints.append({"type": ctype, "fun": fun, "jac": jac})
     return constraints
 
 
+def _make_nonlinear_constraints(
+    f_np_wrapper: Callable, nlc: Callable, is_intrapoint: bool, shapeX: torch.Size
+) -> List[ScipyConstraintDict]:
+    """Create nonlinear constraints to be used by `scipy.minimize`.
+
+    Args:
+        f_np_wrapper: A wrapper function that given a constraint evaluates
+            the value and gradient (using autograd) of a numpy input and returns both
+            the objective and the gradient.
+        nlc: Callable representing a constraint of the form `callable(x) >= 0`. In case
+            of an intra-point constraint, `callable()`takes in an one-dimensional tensor
+            of shape `d` and returns a scalar. In case of an inter-point constraint,
+            `callable()` takes a two dimensional tensor of shape `q x d` and again
+            returns a scalar.
+        is_intrapoint: A Boolean indicating if a constraint is an intra-point or
+            inter-point constraint (see the docstring of the `inequality_constraints`
+            argument to `optimize_acqf()`).
+        shapeX: Shape of the three-dimensional batch X, that should be optimized.
+
+    Returns:
+        A list of constraint dictionaries with the following keys
+
+        - "type": Indicates the type of the constraint, here always "ineq".
+        - "fun": A callable evaluating the constraint value on `x`, a flattened
+            version of the input tensor `X`, returning a scalar.
+        - "jac": A callable evaluating the constraint's Jacobian on `x`, a flattened
+            version of the input tensor `X`, returning a numpy array.
+    """
+    shapeX = _validate_linear_constraints_shape_input(shapeX)
+    b, q, _ = shapeX
+    constraints = []
+
+    def get_intrapoint_constraint(b: int, q: int, nlc: Callable) -> Callable:
+        return lambda x: nlc(x[b, q])
+
+    def get_interpoint_constraint(b: int, nlc: Callable) -> Callable:
+        return lambda x: nlc(x[b])
+
+    if is_intrapoint:
+        for i in range(b):
+            for j in range(q):
+                f_obj, f_grad = _make_f_and_grad_nonlinear_inequality_constraints(
+                    f_np_wrapper=f_np_wrapper,
+                    nlc=get_intrapoint_constraint(b=i, q=j, nlc=nlc),
+                )
+                constraints.append({"type": "ineq", "fun": f_obj, "jac": f_grad})
+    else:
+        for i in range(b):
+            f_obj, f_grad = _make_f_and_grad_nonlinear_inequality_constraints(
+                f_np_wrapper=f_np_wrapper,
+                nlc=get_interpoint_constraint(b=i, nlc=nlc),
+            )
+            constraints.append({"type": "ineq", "fun": f_obj, "jac": f_grad})
+
+    return constraints
+
+
 def _generate_unfixed_nonlin_constraints(
-    constraints: Optional[List[Callable[[Tensor], Tensor]]],
+    constraints: Optional[List[Tuple[Callable[[Tensor], Tensor], bool]]],
     fixed_features: Dict[int, float],
     dimension: int,
 ) -> Optional[List[Callable[[Tensor], Tensor]]]:
     """Given a dictionary of fixed features, returns a list of callables for
     nonlinear inequality constraints expecting only a tensor with the non-fixed
     features as input.
     """
@@ -343,15 +400,16 @@
             ivalues = values.to(X).expand(*X.shape[:-1], len(fixed_features))
             X_perm = torch.cat([X, ivalues], dim=-1)
             return constraint(X_perm[..., selector])
 
         return new_nonlin_constraint
 
     return [
-        _wrap_nonlin_constraint(constraint=constraint) for constraint in constraints
+        (_wrap_nonlin_constraint(constraint=nlc), is_intrapoint)
+        for nlc, is_intrapoint in constraints
     ]
 
 
 def _generate_unfixed_lin_constraints(
     constraints: Optional[List[Tuple[Tensor, Tensor, float]]],
     fixed_features: Dict[int, float],
     dimension: int,
@@ -415,15 +473,15 @@
 
 def _make_f_and_grad_nonlinear_inequality_constraints(
     f_np_wrapper: Callable, nlc: Callable
 ) -> Tuple[Callable[[Tensor], Tensor], Callable[[Tensor], Tensor]]:
     """
     Create callables for objective + grad for the nonlinear inequality constraints.
     The Scipy interface requires specifying separate callables and we use caching to
-    avoid evaluating the same input twice. This caching onlh works if
+    avoid evaluating the same input twice. This caching only works if
     the returned functions are evaluated on the same input in immediate
     sequence (i.e., calling `f_obj(X_1)`, `f_grad(X_1)` will result in a
     single forward pass, while `f_obj(X_1)`, `f_grad(X_2)`, `f_obj(X_1)`
     will result in three forward passes).
     """
 
     def f_obj_and_grad(x):
@@ -445,54 +503,99 @@
             cache["X"] = X.copy()
             cache["obj"], cache["grad"] = f_obj_and_grad(X)
         return cache["grad"]
 
     return f_obj, f_grad
 
 
+def nonlinear_constraint_is_feasible(
+    nonlinear_inequality_constraint: Callable, is_intrapoint: bool, x: Tensor
+) -> bool:
+    """Checks if a nonlinear inequality constraint is fulfilled.
+
+    Args:
+        nonlinear_inequality_constraint: Callable to evaluate the
+            constraint.
+        intra: If True, the constraint is an intra-point constraint that
+            is applied pointwise and is broadcasted over the q-batch. Else, the
+            constraint has to evaluated over the whole q-batch and is a an
+            inter-point constraint.
+        x: Tensor of shape (b x q x d).
+
+    Returns:
+        bool: True if the constraint is fulfilled, else False.
+    """
+
+    def check_x(x: Tensor) -> bool:
+        return _arrayify(nonlinear_inequality_constraint(x)).item() >= NLC_TOL
+
+    for x_ in x:
+        if is_intrapoint:
+            if not all(check_x(x__) for x__ in x_):
+                return False
+        else:
+            if not check_x(x_):
+                return False
+    return True
+
+
 def make_scipy_nonlinear_inequality_constraints(
-    nonlinear_inequality_constraints: List[Callable],
+    nonlinear_inequality_constraints: List[Tuple[Callable, bool]],
     f_np_wrapper: Callable,
     x0: Tensor,
+    shapeX: torch.Size,
 ) -> List[Dict]:
     r"""Generate Scipy nonlinear inequality constraints from callables.
 
     Args:
-        nonlinear_inequality_constraints: List of callables for the nonlinear
-            inequality constraints. Each callable represents a constraint of the
-            form >= 0 and takes a torch tensor of size (p x q x dim) and returns a
-            torch tensor of size (p x q).
+        nonlinear_inequality_constraints: A list of tuples representing the nonlinear
+            inequality constraints. The first element in the tuple is a callable
+            representing a constraint of the form `callable(x) >= 0`. In case of an
+            intra-point constraint, `callable()`takes in an one-dimensional tensor of
+            shape `d` and returns a scalar. In case of an inter-point constraint,
+            `callable()` takes a two dimensional tensor of shape `q x d` and again
+            returns a scalar. The second element is a boolean, indicating if it is an
+            intra-point or inter-point constraint (`True` for intra-point. `False` for
+            inter-point). For more information on intra-point vs inter-point
+            constraints, see the docstring of the `inequality_constraints` argument to
+            `optimize_acqf()`. The constraints will later be passed to the scipy
+            solver.
         f_np_wrapper: A wrapper function that given a constraint evaluates the value
              and gradient (using autograd) of a numpy input and returns both the
              objective and the gradient.
         x0: The starting point for SLSQP. We return this starting point in (rare)
             cases where SLSQP fails and thus require it to be feasible.
+        shapeX: Shape of the three-dimensional batch X, that should be optimized.
 
     Returns:
         A list of dictionaries containing callables for constraint function
         values and Jacobians and a string indicating the associated constraint
         type ("eq", "ineq"), as expected by `scipy.minimize`.
     """
-    if not isinstance(nonlinear_inequality_constraints, list):
-        raise ValueError(
-            "`nonlinear_inequality_constraints` must be a list of callables, "
-            f"got {type(nonlinear_inequality_constraints)}."
-        )
 
     scipy_nonlinear_inequality_constraints = []
-    for nlc in nonlinear_inequality_constraints:
-        if _arrayify(nlc(x0)).item() < NLC_TOL:
+    for constraint in nonlinear_inequality_constraints:
+        if not isinstance(constraint, tuple):
+            raise ValueError(
+                f"A nonlinear constraint has to be a tuple, got {type(constraint)}."
+            )
+        if len(constraint) != 2:
+            raise ValueError(
+                "A nonlinear constraint has to be a tuple of length 2, "
+                f"got length {len(constraint)}."
+            )
+        nlc, is_intrapoint = constraint
+        if not nonlinear_constraint_is_feasible(
+            nlc, is_intrapoint=is_intrapoint, x=x0.reshape(shapeX)
+        ):
             raise ValueError(
                 "`batch_initial_conditions` must satisfy the non-linear inequality "
                 "constraints."
             )
-        f_obj, f_grad = _make_f_and_grad_nonlinear_inequality_constraints(
-            f_np_wrapper=f_np_wrapper, nlc=nlc
-        )
-        scipy_nonlinear_inequality_constraints.append(
-            {
-                "type": "ineq",
-                "fun": f_obj,
-                "jac": f_grad,
-            }
+
+        scipy_nonlinear_inequality_constraints += _make_nonlinear_constraints(
+            f_np_wrapper=f_np_wrapper,
+            nlc=nlc,
+            is_intrapoint=is_intrapoint,
+            shapeX=shapeX,
         )
     return scipy_nonlinear_inequality_constraints
```

### Comparing `botorch-0.9.4/botorch/optim/stopping.py` & `botorch-0.9.5/botorch/optim/stopping.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/utils/__init__.py` & `botorch-0.9.5/botorch/optim/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/utils/acquisition_utils.py` & `botorch-0.9.5/botorch/optim/utils/acquisition_utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/utils/common.py` & `botorch-0.9.5/botorch/optim/utils/common.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/utils/model_utils.py` & `botorch-0.9.5/botorch/optim/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/utils/numpy_utils.py` & `botorch-0.9.5/botorch/optim/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/optim/utils/timeout.py` & `botorch-0.9.5/botorch/optim/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/posteriors/__init__.py` & `botorch-0.9.5/botorch/posteriors/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from botorch.posteriors.deterministic import DeterministicPosterior
-from botorch.posteriors.fully_bayesian import FullyBayesianPosterior
+from botorch.posteriors.fully_bayesian import (
+    FullyBayesianPosterior,
+    GaussianMixturePosterior,
+)
 from botorch.posteriors.gpytorch import GPyTorchPosterior
 from botorch.posteriors.higher_order import HigherOrderGPPosterior
 from botorch.posteriors.multitask import MultitaskGPPosterior
 from botorch.posteriors.posterior import Posterior
 from botorch.posteriors.posterior_list import PosteriorList
 from botorch.posteriors.torch import TorchPosterior
 from botorch.posteriors.transformed import TransformedPosterior
 
 __all__ = [
     "DeterministicPosterior",
+    "GaussianMixturePosterior",
     "FullyBayesianPosterior",
     "GPyTorchPosterior",
     "HigherOrderGPPosterior",
     "MultitaskGPPosterior",
     "Posterior",
     "PosteriorList",
     "TorchPosterior",
```

### Comparing `botorch-0.9.4/botorch/posteriors/base_samples.py` & `botorch-0.9.5/botorch/posteriors/base_samples.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/posteriors/deterministic.py` & `botorch-0.9.5/botorch/posteriors/deterministic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/posteriors/ensemble.py` & `botorch-0.9.5/botorch/posteriors/ensemble.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/posteriors/fully_bayesian.py` & `botorch-0.9.5/botorch/posteriors/fully_bayesian.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 from typing import Callable, Optional, Tuple
+from warnings import warn
 
 import torch
 from botorch.posteriors.gpytorch import GPyTorchPosterior
 from gpytorch.distributions import MultivariateNormal
 from torch import Tensor
 
 
@@ -50,15 +51,15 @@
         f_center = f(center)
         # Check convergence
         if (f_center - target).abs().max() <= tol:
             return center
     return center
 
 
-def _quantile(posterior: FullyBayesianPosterior, value: Tensor) -> Tensor:
+def _quantile(posterior: GaussianMixturePosterior, value: Tensor) -> Tensor:
     r"""Compute the posterior quantiles for the mixture of models."""
     if value.numel() > 1:
         return torch.stack(
             [_quantile(posterior=posterior, value=v) for v in value], dim=0
         )
     if value <= 0 or value >= 1:
         raise ValueError("value is expected to be in the range (0, 1).")
@@ -74,21 +75,21 @@
     return batched_bisect(
         f=lambda x: dist.cdf(x.unsqueeze(MCMC_DIM)).mean(dim=MCMC_DIM),
         target=value.item(),
         bounds=bounds,
     )
 
 
-class FullyBayesianPosterior(GPyTorchPosterior):
-    r"""A posterior for a fully Bayesian model.
+class GaussianMixturePosterior(GPyTorchPosterior):
+    r"""A Gaussian mixture posterior.
 
     The MCMC batch dimension that corresponds to the models in the mixture is located
     at `MCMC_DIM` (defined at the top of this file). Note that while each MCMC sample
-    corresponds to a Gaussian posterior, the fully Bayesian posterior is rather a
-    mixture of Gaussian distributions.
+    corresponds to a Gaussian posterior, the posterior is rather a mixture of Gaussian
+    distributions.
     """
 
     def __init__(self, distribution: MultivariateNormal) -> None:
         r"""A posterior for a fully Bayesian model.
 
         Args:
             distribution: A GPyTorch MultivariateNormal (single-output case)
@@ -133,11 +134,21 @@
         r"""The t-batch range.
 
         This is used in samplers to identify the t-batch component of the
         `base_sample_shape`. The base samples are expanded over the t-batches to
         provide consistency in the acquisition values, i.e., to ensure that a
         candidate produces same value regardless of its position on the t-batch.
         """
-        if self._is_mt:
-            return (0, -2)
-        else:
-            return (0, -1)
+        return (0, -2) if self._is_mt else (0, -1)
+
+
+class FullyBayesianPosterior(GaussianMixturePosterior):
+    """For backwards compatibility."""
+
+    def __init__(self, distribution: MultivariateNormal) -> None:
+        """DEPRECATED."""
+        warn(
+            "`FullyBayesianPosterior` is marked for deprecation, consider using "
+            "`GaussianMixturePosterior` instead.",
+            DeprecationWarning,
+        )
+        super().__init__(distribution=distribution)
```

### Comparing `botorch-0.9.4/botorch/posteriors/gpytorch.py` & `botorch-0.9.5/botorch/posteriors/gpytorch.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/posteriors/higher_order.py` & `botorch-0.9.5/botorch/posteriors/higher_order.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/posteriors/multitask.py` & `botorch-0.9.5/botorch/posteriors/multitask.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/posteriors/posterior.py` & `botorch-0.9.5/botorch/posteriors/posterior.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/posteriors/posterior_list.py` & `botorch-0.9.5/botorch/posteriors/posterior_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,28 +7,27 @@
 r"""
 Abstract base module for all botorch posteriors.
 """
 
 from __future__ import annotations
 
 from functools import cached_property
-
 from typing import Any, List, Optional
 
 import torch
-from botorch.posteriors.fully_bayesian import FullyBayesianPosterior, MCMC_DIM
+from botorch.posteriors.fully_bayesian import GaussianMixturePosterior, MCMC_DIM
 from botorch.posteriors.posterior import Posterior
 from torch import Tensor
 
 
 class PosteriorList(Posterior):
     r"""A Posterior represented by a list of independent Posteriors.
 
-    When at least one of the posteriors is a `FullyBayesianPosterior`, the other
-    posteriors are expanded to match the size of the `FullyBayesianPosterior`.
+    When at least one of the posteriors is a `GaussianMixturePosterior`, the other
+    posteriors are expanded to match the size of the `GaussianMixturePosterior`.
     """
 
     def __init__(self, *posteriors: Posterior) -> None:
         r"""A Posterior represented by a list of independent Posteriors.
 
         Args:
             *posteriors: A variable number of single-outcome posteriors.
@@ -40,24 +39,24 @@
 
         Note: This is typically produced automatically in `ModelList`; it should
         generally not be necessary for the end user to invoke it manually.
         """
         self.posteriors = list(posteriors)
 
     @cached_property
-    def _is_fully_bayesian(self) -> bool:
-        r"""Check if any of the posteriors is a `FullyBayesianPosterior`."""
-        return any(isinstance(p, FullyBayesianPosterior) for p in self.posteriors)
+    def _is_gaussian_mixture(self) -> bool:
+        r"""Check if any of the posteriors is a `GaussianMixturePosterior`."""
+        return any(isinstance(p, GaussianMixturePosterior) for p in self.posteriors)
 
     def _get_mcmc_batch_dimension(self) -> int:
         """Return the number of MCMC samples in the corresponding batch dimension."""
         mcmc_samples = [
             p.mean.shape[MCMC_DIM]
             for p in self.posteriors
-            if isinstance(p, FullyBayesianPosterior)
+            if isinstance(p, GaussianMixturePosterior)
         ]
         if len(set(mcmc_samples)) > 1:
             raise NotImplementedError(
                 "All MCMC batch dimensions must have the same size, got shapes: "
                 f"{mcmc_samples}."
             )
         return mcmc_samples[0]
@@ -66,20 +65,20 @@
     def _reshape_tensor(X: Tensor, mcmc_samples: int) -> Tensor:
         """Reshape a tensor without an MCMC batch dimension to match the shape."""
         X = X.unsqueeze(MCMC_DIM)
         return X.expand(*X.shape[:MCMC_DIM], mcmc_samples, *X.shape[MCMC_DIM + 1 :])
 
     def _reshape_and_cat(self, tensors: List[Tensor]):
         r"""Reshape, if needed, and concatenate (across dim=-1) a list of tensors."""
-        if self._is_fully_bayesian:
+        if self._is_gaussian_mixture:
             mcmc_samples = self._get_mcmc_batch_dimension()
             return torch.cat(
                 [
                     x
-                    if isinstance(p, FullyBayesianPosterior)
+                    if isinstance(p, GaussianMixturePosterior)
                     else self._reshape_tensor(x, mcmc_samples=mcmc_samples)
                     for x, p in zip(tensors, self.posteriors)
                 ],
                 dim=-1,
             )
         else:
             return torch.cat(tensors, dim=-1)
@@ -108,24 +107,26 @@
 
     def _extended_shape(
         self, sample_shape: torch.Size = torch.Size()  # noqa: B008
     ) -> torch.Size:
         r"""Returns the shape of the samples produced by the posterior with
         the given `sample_shape`.
 
-        If there's at least one `FullyBayesianPosterior`, the MCMC dimension
+        If there's at least one `GaussianMixturePosterior`, the MCMC dimension
         is included the `_extended_shape`.
         """
-        if self._is_fully_bayesian:
+        if self._is_gaussian_mixture:
             mcmc_shape = torch.Size([self._get_mcmc_batch_dimension()])
             extend_dim = MCMC_DIM + 1  # The dimension to inject MCMC shape.
         extended_shapes = []
         for p in self.posteriors:
             es = p._extended_shape(sample_shape=sample_shape)
-            if self._is_fully_bayesian and not isinstance(p, FullyBayesianPosterior):
+            if self._is_gaussian_mixture and not isinstance(
+                p, GaussianMixturePosterior
+            ):
                 # Extend the shapes of non-fully Bayesian ones to match.
                 extended_shapes.append(es[:extend_dim] + mcmc_shape + es[extend_dim:])
             else:
                 extended_shapes.append(es)
         batch_shapes = [es[:-1] for es in extended_shapes]
         if len(set(batch_shapes)) > 1:
             raise NotImplementedError(
```

### Comparing `botorch-0.9.4/botorch/posteriors/torch.py` & `botorch-0.9.5/botorch/posteriors/torch.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/posteriors/transformed.py` & `botorch-0.9.5/botorch/posteriors/transformed.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/__init__.py` & `botorch-0.9.5/botorch/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/base.py` & `botorch-0.9.5/botorch/sampling/base.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/deterministic.py` & `botorch-0.9.5/botorch/sampling/deterministic.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/get_sampler.py` & `botorch-0.9.5/botorch/sampling/get_sampler.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/index_sampler.py` & `botorch-0.9.5/botorch/sampling/index_sampler.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/list_sampler.py` & `botorch-0.9.5/botorch/sampling/list_sampler.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/normal.py` & `botorch-0.9.5/botorch/sampling/normal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/pairwise_samplers.py` & `botorch-0.9.5/botorch/sampling/pairwise_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/pathwise/__init__.py` & `botorch-0.9.5/botorch/sampling/pathwise/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/pathwise/features/__init__.py` & `botorch-0.9.5/botorch/sampling/pathwise/features/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/pathwise/features/generators.py` & `botorch-0.9.5/botorch/sampling/pathwise/features/generators.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/pathwise/features/maps.py` & `botorch-0.9.5/botorch/sampling/pathwise/features/maps.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/pathwise/paths.py` & `botorch-0.9.5/botorch/sampling/pathwise/paths.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/pathwise/posterior_samplers.py` & `botorch-0.9.5/botorch/sampling/pathwise/posterior_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/pathwise/prior_samplers.py` & `botorch-0.9.5/botorch/sampling/pathwise/prior_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/pathwise/update_strategies.py` & `botorch-0.9.5/botorch/sampling/pathwise/update_strategies.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/pathwise/utils.py` & `botorch-0.9.5/botorch/sampling/pathwise/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/qmc.py` & `botorch-0.9.5/botorch/sampling/qmc.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/sampling/stochastic_samplers.py` & `botorch-0.9.5/botorch/sampling/stochastic_samplers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/settings.py` & `botorch-0.9.5/botorch/settings.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/test_functions/__init__.py` & `botorch-0.9.5/botorch/test_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/test_functions/base.py` & `botorch-0.9.5/botorch/test_functions/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,34 +7,41 @@
 r"""
 Base class for test functions for optimization benchmarks.
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import List, Optional, Tuple
+from typing import List, Tuple, Union
 
 import torch
+
 from botorch.exceptions.errors import InputDataError
 from torch import Tensor
 from torch.nn import Module
 
 
 class BaseTestProblem(Module, ABC):
     r"""Base class for test functions."""
 
     dim: int
     _bounds: List[Tuple[float, float]]
     _check_grad_at_opt: bool = True
 
-    def __init__(self, noise_std: Optional[float] = None, negate: bool = False) -> None:
+    def __init__(
+        self,
+        noise_std: Union[None, float, List[float]] = None,
+        negate: bool = False,
+    ) -> None:
         r"""Base constructor for test functions.
 
         Args:
-            noise_std: Standard deviation of the observation noise.
+            noise_std: Standard deviation of the observation noise. If a list is
+                provided, specifies separate noise standard deviations for each
+                objective in a multiobjective problem.
             negate: If True, negate the function.
         """
         super().__init__()
         self.noise_std = noise_std
         self.negate = negate
         if len(self._bounds) != self.dim:
             raise InputDataError(
@@ -56,15 +63,16 @@
         Returns:
             A `batch_shape`-dim tensor ouf function evaluations.
         """
         batch = X.ndimension() > 1
         X = X if batch else X.unsqueeze(0)
         f = self.evaluate_true(X=X)
         if noise and self.noise_std is not None:
-            f += self.noise_std * torch.randn_like(f)
+            _noise = torch.tensor(self.noise_std, device=X.device, dtype=X.dtype)
+            f += _noise * torch.randn_like(f)
         if self.negate:
             f = -f
         return f if batch else f.squeeze(0)
 
     @abstractmethod
     def evaluate_true(self, X: Tensor) -> Tensor:
         r"""Evaluate the function (w/o observation noise) on a set of points."""
@@ -78,14 +86,15 @@
     constraints of the form `c_i(x) >= 0` for `i=1, ..., n_c`.
 
     This base class provides common functionality for such problems.
     """
 
     num_constraints: int
     _check_grad_at_opt: bool = False
+    constraint_noise_std: Union[None, float, List[float]] = None
 
     def evaluate_slack(self, X: Tensor, noise: bool = True) -> Tensor:
         r"""Evaluate the constraint slack on a set of points.
 
         Constraints `i` is assumed to be feasible at `x` if the associated slack
         `c_i(x)` is positive. Zero slack means that the constraint is active. Negative
         slack means that the constraint is violated.
@@ -97,18 +106,19 @@
                 `noise_std`.
 
         Returns:
             A `batch_shape x n_c`-dim tensor of constraint slack (where positive slack
                 corresponds to the constraint being feasible).
         """
         cons = self.evaluate_slack_true(X=X)
-        if noise and self.noise_std is not None:
-            # TODO: Allow different noise levels for objective and constraints (and
-            # different noise levels between different constraints)
-            cons += self.noise_std * torch.randn_like(cons)
+        if noise and self.constraint_noise_std is not None:
+            _constraint_noise = torch.tensor(
+                self.constraint_noise_std, device=X.device, dtype=X.dtype
+            )
+            cons += _constraint_noise * torch.randn_like(cons)
         return cons
 
     def is_feasible(self, X: Tensor, noise: bool = True) -> Tensor:
         r"""Evaluate whether the constraints are feasible on a set of points.
 
         Args:
             X: A `batch_shape x d`-dim tensor of point(s) at which to evaluate the
@@ -143,21 +153,32 @@
     between a provided point and the closest point on the true pareto front.
     """
 
     num_objectives: int
     _ref_point: List[float]
     _max_hv: float
 
-    def __init__(self, noise_std: Optional[float] = None, negate: bool = False) -> None:
+    def __init__(
+        self,
+        noise_std: Union[None, float, List[float]] = None,
+        negate: bool = False,
+    ) -> None:
         r"""Base constructor for multi-objective test functions.
 
         Args:
-            noise_std: Standard deviation of the observation noise.
+            noise_std: Standard deviation of the observation noise. If a list is
+                provided, specifies separate noise standard deviations for each
+                objective.
             negate: If True, negate the objectives.
         """
+        if isinstance(noise_std, list) and len(noise_std) != len(self._ref_point):
+            raise InputDataError(
+                f"If specified as a list, length of noise_std ({len(noise_std)}) "
+                f"must match the number of objectives ({len(self._ref_point)})"
+            )
         super().__init__(noise_std=noise_std, negate=negate)
         ref_point = torch.tensor(self._ref_point, dtype=torch.float)
         if negate:
             ref_point *= -1
         self.register_buffer("ref_point", ref_point)
 
     @property
```

### Comparing `botorch-0.9.4/botorch/test_functions/multi_fidelity.py` & `botorch-0.9.5/botorch/test_functions/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/test_functions/multi_objective.py` & `botorch-0.9.5/botorch/test_functions/multi_objective.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 """
 
 from __future__ import annotations
 
 import math
 from abc import ABC, abstractmethod
 from math import pi
-from typing import Optional
+from typing import List, Union
 
 import torch
 from botorch.exceptions.errors import UnsupportedError
 from botorch.test_functions.base import (
     ConstrainedBaseTestProblem,
     MultiObjectiveTestProblem,
 )
@@ -112,15 +112,19 @@
 
     dim = 2
     num_objectives = 2
     _bounds = [(0.0, 1.0), (0.0, 1.0)]
     _ref_point = [18.0, 6.0]
     _max_hv = 59.36011874867746  # this is approximated using NSGA-II
 
-    def __init__(self, noise_std: Optional[float] = None, negate: bool = False) -> None:
+    def __init__(
+        self,
+        noise_std: Union[None, float, List[float]] = None,
+        negate: bool = False,
+    ) -> None:
         r"""
         Args:
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the objectives.
         """
         super().__init__(noise_std=noise_std, negate=negate)
         self._branin = Branin()
@@ -170,15 +174,15 @@
     _x_1_lb: float
     _area_under_curve: float
     _min_dim: int
 
     def __init__(
         self,
         dim: int,
-        noise_std: Optional[float] = None,
+        noise_std: Union[None, float, List[float]] = None,
         negate: bool = False,
     ) -> None:
         r"""
         Args:
             dim: The (input) dimension.
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
@@ -330,15 +334,15 @@
     See [Deb2005dtlz]_ for more details on DTLZ.
     """
 
     def __init__(
         self,
         dim: int,
         num_objectives: int = 2,
-        noise_std: Optional[float] = None,
+        noise_std: Union[None, float, List[float]] = None,
         negate: bool = False,
     ) -> None:
         r"""
         Args:
             dim: The (input) dimension of the function.
             num_objectives: Must be less than dim.
             noise_std: Standard deviation of the observation noise.
@@ -596,15 +600,15 @@
     See [Daulton2022]_ for details on this multi-objective problem.
     """
     dim = 2
     _bounds = [(0.0, 1.0), (0.0, 1.0)]
 
     def __init__(
         self,
-        noise_std: Optional[float] = None,
+        noise_std: Union[None, float, List[float]] = None,
         negate: bool = False,
         num_objectives: int = 2,
     ) -> None:
         r"""
         Args:
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the objectives.
@@ -922,15 +926,15 @@
 
     _ref_point = [11.0, 11.0]
 
     def __init__(
         self,
         dim: int,
         num_objectives: int = 2,
-        noise_std: Optional[float] = None,
+        noise_std: Union[None, float, List[float]] = None,
         negate: bool = False,
     ) -> None:
         r"""
         Args:
             dim: The (input) dimension of the function.
             num_objectives: Number of objectives. Must not be larger than dim.
             noise_std: Standard deviation of the observation noise.
@@ -1230,15 +1234,19 @@
     num_objectives = 2
     num_constraints = 1
     _bounds = [(0.0, 1.0), (0.0, 1.0)]
     _con_bounds = [(-5.0, 10.0), (0.0, 15.0)]
     _ref_point = [80.0, 12.0]
     _max_hv = 608.4004237022673  # from NSGA-II with 90k evaluations
 
-    def __init__(self, noise_std: Optional[float] = None, negate: bool = False) -> None:
+    def __init__(
+        self,
+        noise_std: Union[None, float, List[float]] = None,
+        negate: bool = False,
+    ) -> None:
         r"""
         Args:
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
         """
         super().__init__(noise_std=noise_std, negate=negate)
         con_bounds = torch.tensor(self._con_bounds, dtype=torch.float).transpose(-1, -2)
@@ -1333,15 +1341,15 @@
     num_constraints = 2
     num_objectives = 2
     _ref_point = [1.2, 1.2]
 
     def __init__(
         self,
         dim: int,
-        noise_std: Optional[float] = None,
+        noise_std: Union[None, float, List[float]] = None,
         negate: bool = False,
     ) -> None:
         r"""
         Args:
             dim: The (input) dimension of the function. Must be at least 2.
             noise_std: Standard deviation of the observation noise.
             negate: If True, negate the function.
```

### Comparing `botorch-0.9.4/botorch/test_functions/multi_objective_multi_fidelity.py` & `botorch-0.9.5/botorch/test_functions/multi_objective_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/test_functions/sensitivity_analysis.py` & `botorch-0.9.5/botorch/test_functions/sensitivity_analysis.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/test_functions/synthetic.py` & `botorch-0.9.5/botorch/test_functions/synthetic.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,38 +43,41 @@
     Modeling an Augmented Lagrangian for Blackbox Constrained Optimization,
     Technometrics, 2016.
 """
 
 from __future__ import annotations
 
 import math
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, Union
 
 import torch
+from botorch.exceptions.errors import InputDataError
 from botorch.test_functions.base import BaseTestProblem, ConstrainedBaseTestProblem
 from botorch.test_functions.utils import round_nearest
 from torch import Tensor
 
 
 class SyntheticTestFunction(BaseTestProblem):
     r"""Base class for synthetic test functions."""
 
     _optimal_value: float
     _optimizers: Optional[List[Tuple[float, ...]]] = None
     num_objectives: int = 1
 
     def __init__(
         self,
-        noise_std: Optional[float] = None,
+        noise_std: Union[None, float, List[float]] = None,
         negate: bool = False,
         bounds: Optional[List[Tuple[float, float]]] = None,
     ) -> None:
         r"""
         Args:
-            noise_std: Standard deviation of the observation noise.
+            noise_std: Standard deviation of the observation noise. If a list is
+                provided, specifies separate noise standard deviations for each
+                objective in a multiobjective problem.
             negate: If True, negate the function.
             bounds: Custom bounds for the function specified as (lower, upper) pairs.
         """
         if bounds is not None:
             self._bounds = bounds
         super().__init__(noise_std=noise_std, negate=negate)
         if self._optimizers is not None:
@@ -798,15 +801,69 @@
         x1, x2 = X[..., 0], X[..., 1]
         return 2.0 * x1**2 - 1.05 * x1**4 + x1**6 / 6.0 + x1 * x2 + x2**2
 
 
 #  ------------ Constrained synthetic test functions ----------- #
 
 
-class ConstrainedGramacy(ConstrainedBaseTestProblem, SyntheticTestFunction):
+class ConstrainedSyntheticTestFunction(
+    ConstrainedBaseTestProblem, SyntheticTestFunction
+):
+    r"""Base class for constrained synthetic test functions."""
+
+    def __init__(
+        self,
+        noise_std: Union[None, float, List[float]] = None,
+        constraint_noise_std: Union[None, float, List[float]] = None,
+        negate: bool = False,
+        bounds: Optional[List[Tuple[float, float]]] = None,
+    ) -> None:
+        r"""
+        Args:
+            noise_std: Standard deviation of the observation noise. If a list is
+                provided, specifies separate noise standard deviations for each
+                objective in a multiobjective problem.
+            constraint_noise_std: Standard deviation of the constraint noise.
+                If a list is provided, specifies separate noise standard
+                deviations for each constraint.
+            negate: If True, negate the function.
+            bounds: Custom bounds for the function specified as (lower, upper) pairs.
+        """
+        self.constraint_noise_std = self._validate_constraint_noise(
+            constraint_noise_std
+        )
+        SyntheticTestFunction.__init__(
+            self, noise_std=noise_std, negate=negate, bounds=bounds
+        )
+
+    def _validate_constraint_noise(
+        self, constraint_noise_std
+    ) -> Union[None, float, List[float]]:
+        """
+        Validates that constraint_noise_std has length equal to
+        the number of constraints, if given as a list
+
+        Args:
+            constraint_noise_std: Standard deviation of the constraint noise.
+                If a list is provided, specifies separate noise standard
+                deviations for each constraint.
+        """
+        if (
+            isinstance(constraint_noise_std, list)
+            and len(constraint_noise_std) != self.num_constraints
+        ):
+            raise InputDataError(
+                "If specified as a list, length of constraint_noise_std "
+                f"({len(constraint_noise_std)}) must match the "
+                f"number of constraints ({self.num_constraints})"
+            )
+        return constraint_noise_std
+
+
+class ConstrainedGramacy(ConstrainedSyntheticTestFunction):
     r"""Constrained Gramacy test function.
 
     This problem comes from [Gramacy2016]_. The problem is defined
     over the unit cube and the goal is to minimize x1+x2 subject to
     1.5 - x1 - 2 * x2 - 0.5 * sin(2*pi*(x1^2 - 2 * x2)) <= 0
     and x1^2 + x2^2 - 1.5 <= 0.
     """
@@ -831,39 +888,85 @@
     def evaluate_slack_true(self, X: Tensor) -> Tensor:
         x1, x2 = X.split(1, dim=-1)
         c1 = 1.5 - x1 - 2 * x2 - 0.5 * torch.sin(2 * math.pi * (x1.pow(2) - 2 * x2))
         c2 = x1.pow(2) + x2.pow(2) - 1.5
         return torch.cat([-c1, -c2], dim=-1)
 
 
-class ConstrainedHartmann(Hartmann, ConstrainedBaseTestProblem):
+class ConstrainedHartmann(Hartmann, ConstrainedSyntheticTestFunction):
     r"""Constrained Hartmann test function.
 
     This is a constrained version of the standard Hartmann test function that
     uses `||x||_2 <= 1` as the constraint. This problem comes from [Letham2019]_.
     """
     num_constraints = 1
 
+    def __init__(
+        self,
+        dim: int = 6,
+        noise_std: Union[None, float] = None,
+        constraint_noise_std: Union[None, float, List[float]] = None,
+        negate: bool = False,
+        bounds: Optional[List[Tuple[float, float]]] = None,
+    ) -> None:
+        r"""
+        Args:
+            dim: The (input) dimension.
+            noise_std: Standard deviation of the observation noise.
+            constraint_noise_std: Standard deviation of the constraint noise.
+                If a list is provided, specifies separate noise standard
+                deviations for each constraint.
+            negate: If True, negate the function.
+            bounds: Custom bounds for the function specified as (lower, upper) pairs.
+        """
+        self._validate_constraint_noise(constraint_noise_std)
+        Hartmann.__init__(
+            self, dim=dim, noise_std=noise_std, negate=negate, bounds=bounds
+        )
+
     def evaluate_slack_true(self, X: Tensor) -> Tensor:
         return -X.norm(dim=-1, keepdim=True) + 1
 
 
-class ConstrainedHartmannSmooth(Hartmann, ConstrainedBaseTestProblem):
+class ConstrainedHartmannSmooth(Hartmann, ConstrainedSyntheticTestFunction):
     r"""Smooth constrained Hartmann test function.
 
     This is a constrained version of the standard Hartmann test function that
     uses `||x||_2^2 <= 1` as the constraint to obtain smoother constraint slack.
     """
     num_constraints = 1
 
+    def __init__(
+        self,
+        dim: int = 6,
+        noise_std: Union[None, float] = None,
+        constraint_noise_std: Union[None, float, List[float]] = None,
+        negate: bool = False,
+        bounds: Optional[List[Tuple[float, float]]] = None,
+    ) -> None:
+        r"""
+        Args:
+            dim: The (input) dimension.
+            noise_std: Standard deviation of the observation noise.
+            constraint_noise_std: Standard deviation of the constraint noise.
+                If a list is provided, specifies separate noise standard
+                deviations for each constraint.
+            negate: If True, negate the function.
+            bounds: Custom bounds for the function specified as (lower, upper) pairs.
+        """
+        self._validate_constraint_noise(constraint_noise_std)
+        Hartmann.__init__(
+            self, dim=dim, noise_std=noise_std, negate=negate, bounds=bounds
+        )
+
     def evaluate_slack_true(self, X: Tensor) -> Tensor:
         return -X.pow(2).sum(dim=-1, keepdim=True) + 1
 
 
-class PressureVessel(SyntheticTestFunction, ConstrainedBaseTestProblem):
+class PressureVessel(ConstrainedSyntheticTestFunction):
     r"""Pressure vessel design problem with constraints.
 
     The four-dimensional pressure vessel design problem with four black-box
     constraints from [CoelloCoello2002constraint]_.
     """
 
     dim = 4
@@ -890,15 +993,15 @@
                 -math.pi * (x3**2) * x4 - (4 / 3) * math.pi * (x3**3) + 1296000.0,
                 x4 - 240.0,
             ],
             dim=-1,
         )
 
 
-class WeldedBeamSO(SyntheticTestFunction, ConstrainedBaseTestProblem):
+class WeldedBeamSO(ConstrainedSyntheticTestFunction):
     r"""Welded beam design problem with constraints (single-outcome).
 
     The four-dimensional welded beam design proble problem with six
     black-box constraints from [CoelloCoello2002constraint]_.
 
     For a (somewhat modified) multi-objective version, see
     `botorch.test_functions.multi_objective.WeldedBeam`.
@@ -946,15 +1049,15 @@
         g4 = 0.10471 * x1**2 + 0.04811 * x3 * x4 * (14.0 + x2) - 5.0
         g5 = d - d_max
         g6 = P - P_c
 
         return -torch.stack([g1, g2, g3, g4, g5, g6], dim=-1)
 
 
-class TensionCompressionString(SyntheticTestFunction, ConstrainedBaseTestProblem):
+class TensionCompressionString(ConstrainedSyntheticTestFunction):
     r"""Tension compression string optimization problem with constraints.
 
     The three-dimensional tension compression string optimization problem with
     four black-box constraints from [Hedar2006derivfree]_.
     """
 
     dim = 3
@@ -977,15 +1080,15 @@
                 (x1 + x2) / 1.5 - 1,
             ],
             dim=-1,
         )
         return -constraints.clamp_max(100)
 
 
-class SpeedReducer(SyntheticTestFunction, ConstrainedBaseTestProblem):
+class SpeedReducer(ConstrainedSyntheticTestFunction):
     r"""Speed Reducer design problem with constraints.
 
     The seven-dimensional speed reducer design problem with eleven black-box
     constraints from [Lemonge2010constrained]_.
     """
 
     dim = 7
```

### Comparing `botorch-0.9.4/botorch/test_functions/utils.py` & `botorch-0.9.5/botorch/test_functions/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/__init__.py` & `botorch-0.9.5/botorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/constants.py` & `botorch-0.9.5/botorch/utils/constants.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/constraints.py` & `botorch-0.9.5/botorch/utils/constraints.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/containers.py` & `botorch-0.9.5/botorch/utils/containers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/context_managers.py` & `botorch-0.9.5/botorch/utils/context_managers.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/datasets.py` & `botorch-0.9.5/botorch/utils/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,14 +276,18 @@
             y_incr = y_incr - y_diff + 1
 
 
 class MultiTaskDataset(SupervisedDataset):
     """This is a multi-task dataset that is constructed from the datasets of
     individual tasks. It offers functionality to combine parts of individual
     datasets to construct the inputs necessary for the `MultiTaskGP` models.
+
+    The datasets of individual tasks are allowed to represent different sets
+    of features. When there are heterogeneous feature sets, calling
+    `MultiTaskDataset.X` will result in an error.
     """
 
     def __init__(
         self,
         datasets: List[SupervisedDataset],
         target_outcome_name: str,
         task_feature_index: Optional[int] = None,
@@ -305,14 +309,19 @@
         }
         self.target_outcome_name = target_outcome_name
         self.task_feature_index = task_feature_index
         self._validate_datasets(datasets=datasets)
         self.feature_names = self.datasets[target_outcome_name].feature_names
         self.outcome_names = [target_outcome_name]
 
+        # Check if the datasets have identical feature sets.
+        self.has_heterogeneous_features = any(
+            datasets[0].feature_names != ds.feature_names for ds in datasets[1:]
+        )
+
     @classmethod
     def from_joint_dataset(
         cls,
         dataset: SupervisedDataset,
         task_feature_index: int,
         target_task_value: int,
         outcome_names_per_task: Optional[Dict[int, str]] = None,
@@ -423,14 +432,19 @@
     def X(self) -> Tensor:
         """Appends task features, if needed, and concatenates the Xs of datasets to
         produce the `train_X` expected by `MultiTaskGP` and subclasses.
 
         If appending the task features, 0 is reserved for the target task and the
         remaining tasks are populated with 1, 2, ..., len(datasets) - 1.
         """
+        if self.has_heterogeneous_features:
+            raise UnsupportedError(
+                "Concatenating `X`s from datasets with heterogeneous feature sets "
+                "is not supported."
+            )
         all_Xs = []
         next_task = 1
         for outcome, ds in self.datasets.items():
             if self.task_feature_index is None:
                 # Append the task feature index.
                 if outcome == self.target_outcome_name:
                     task_feature = 0
```

### Comparing `botorch-0.9.4/botorch/utils/dispatcher.py` & `botorch-0.9.5/botorch/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/feasible_volume.py` & `botorch-0.9.5/botorch/utils/feasible_volume.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/gp_sampling.py` & `botorch-0.9.5/botorch/utils/gp_sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import torch
 from botorch.models.converter import batched_to_model_list
 from botorch.models.deterministic import GenericDeterministicModel
 from botorch.models.model import Model, ModelList
 from botorch.models.model_list_gp_regression import ModelListGP
 from botorch.models.multitask import MultiTaskGP
 from botorch.utils.sampling import manual_seed
-from botorch.utils.transforms import is_fully_bayesian
+from botorch.utils.transforms import is_ensemble
 from gpytorch.kernels import Kernel, MaternKernel, RBFKernel, ScaleKernel
 from linear_operator.utils.cholesky import psd_safe_cholesky
 from torch import Tensor
 from torch.distributions import MultivariateNormal
 from torch.nn import Module
 
 
@@ -499,15 +499,15 @@
             _octf = octfs[m]
             _intf = intfs[m]
             if _octf is not None:
                 base_gp_samples.models[m].outcome_transform = _octf
                 models[m].outcome_transform = _octf
             if _intf is not None:
                 base_gp_samples.models[m].input_transform = _intf
-        base_gp_samples.is_fully_bayesian = is_fully_bayesian(model=model)
+        base_gp_samples._is_ensemble = is_ensemble(model=model)
         return base_gp_samples
     elif n_samples > 1:
         base_gp_samples = get_deterministic_model_multi_samples(
             weights=weights,
             bases=bases,
         )
     else:
@@ -518,9 +518,9 @@
     # Load the transforms on the models.
     if intf is not None:
         base_gp_samples.input_transform = intf
         model.input_transform = intf
     if octf is not None:
         base_gp_samples.outcome_transform = octf
         model.outcome_transform = octf
-    base_gp_samples.is_fully_bayesian = is_fully_bayesian(model=model)
+    base_gp_samples._is_ensemble = is_ensemble(model=model)
     return base_gp_samples
```

### Comparing `botorch-0.9.4/botorch/utils/low_rank.py` & `botorch-0.9.5/botorch/utils/low_rank.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/multi_objective/__init__.py` & `botorch-0.9.5/botorch/utils/multi_objective/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/multi_objective/box_decompositions/__init__.py` & `botorch-0.9.5/botorch/utils/multi_objective/box_decompositions/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/multi_objective/box_decompositions/box_decomposition.py` & `botorch-0.9.5/botorch/utils/multi_objective/box_decompositions/box_decomposition.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py` & `botorch-0.9.5/botorch/utils/multi_objective/box_decompositions/box_decomposition_list.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/multi_objective/box_decompositions/dominated.py` & `botorch-0.9.5/botorch/utils/multi_objective/box_decompositions/dominated.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/multi_objective/box_decompositions/non_dominated.py` & `botorch-0.9.5/botorch/utils/multi_objective/box_decompositions/non_dominated.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/multi_objective/box_decompositions/utils.py` & `botorch-0.9.5/botorch/utils/multi_objective/box_decompositions/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/multi_objective/hypervolume.py` & `botorch-0.9.5/botorch/utils/multi_objective/hypervolume.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/multi_objective/pareto.py` & `botorch-0.9.5/botorch/utils/multi_objective/pareto.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/multi_objective/scalarization.py` & `botorch-0.9.5/botorch/utils/multi_objective/scalarization.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/objective.py` & `botorch-0.9.5/botorch/utils/objective.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/probability/__init__.py` & `botorch-0.9.5/botorch/utils/probability/__init__.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/probability/bvn.py` & `botorch-0.9.5/botorch/utils/probability/bvn.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/probability/lin_ess.py` & `botorch-0.9.5/botorch/utils/probability/lin_ess.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/probability/linalg.py` & `botorch-0.9.5/botorch/utils/probability/linalg.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/probability/mvnxpb.py` & `botorch-0.9.5/botorch/utils/probability/mvnxpb.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/probability/truncated_multivariate_normal.py` & `botorch-0.9.5/botorch/utils/probability/truncated_multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/probability/unified_skew_normal.py` & `botorch-0.9.5/botorch/utils/probability/unified_skew_normal.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/probability/utils.py` & `botorch-0.9.5/botorch/utils/probability/utils.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/rounding.py` & `botorch-0.9.5/botorch/utils/rounding.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/safe_math.py` & `botorch-0.9.5/botorch/utils/safe_math.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/sampling.py` & `botorch-0.9.5/botorch/utils/sampling.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/testing.py` & `botorch-0.9.5/botorch/utils/testing.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/torch.py` & `botorch-0.9.5/botorch/utils/torch.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch/utils/transforms.py` & `botorch-0.9.5/botorch/utils/transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from functools import wraps
 from typing import Any, Callable, List, Optional, TYPE_CHECKING
 
 import torch
 from botorch.utils.safe_math import logmeanexp
 from torch import Tensor
 
-if TYPE_CHECKING:
-    from botorch.acquisition import AcquisitionFunction  # pragma: no cover
-    from botorch.model import Model  # pragma: no cover
+if TYPE_CHECKING:  # pragma: no cover
+    from botorch.acquisition import AcquisitionFunction
+    from botorch.models.model import Model
 
 
 def standardize(Y: Tensor) -> Tensor:
     r"""Standardizes (zero mean, unit variance) a tensor by dim=-2.
 
     If the tensor is single-dimensional, simply standardizes the tensor.
     If for some batch index all elements are equal (or if there is only a single
@@ -161,41 +161,43 @@
             f"{X.shape}. Make sure that this is the intended behavior!",
             RuntimeWarning,
         )
         return True
 
 
 def is_fully_bayesian(model: Model) -> bool:
-    r"""Check if at least one model is a SaasFullyBayesianSingleTaskGP
+    r"""Check if at least one model is a fully Bayesian model.
 
     Args:
         model: A BoTorch model (may be a `ModelList` or `ModelListGP`)
-        d: The dimension of the tensor to index.
 
     Returns:
-        True if at least one model is a `SaasFullyBayesianSingleTaskGP`
+       True if at least one model is a fully Bayesian model.
     """
     from botorch.models import ModelList
-    from botorch.models.fully_bayesian import SaasFullyBayesianSingleTaskGP
-    from botorch.models.fully_bayesian_multitask import SaasFullyBayesianMultiTaskGP
 
-    full_bayesian_model_cls = (
-        SaasFullyBayesianSingleTaskGP,
-        SaasFullyBayesianMultiTaskGP,
-    )
-
-    if isinstance(model, full_bayesian_model_cls) or getattr(
-        model, "is_fully_bayesian", False
-    ):
-        return True
-    elif isinstance(model, ModelList):
-        for m in model.models:
-            if is_fully_bayesian(m):
-                return True
-    return False
+    if isinstance(model, ModelList):
+        return any(is_fully_bayesian(m) for m in model.models)
+    return getattr(model, "_is_fully_bayesian", False)
+
+
+def is_ensemble(model: Model) -> bool:
+    r"""Check if at least one model is an ensemble model.
+
+    Args:
+        model: A BoTorch model (may be a `ModelList` or `ModelListGP`)
+
+    Returns:
+       True if at least one model is an ensemble model.
+    """
+    from botorch.models import ModelList
+
+    if isinstance(model, ModelList):
+        return any(is_ensemble(m) for m in model.models)
+    return getattr(model, "_is_ensemble", False)
 
 
 def t_batch_mode_transform(
     expected_q: Optional[int] = None,
     assert_output_shape: bool = True,
 ) -> Callable[
     [Callable[[AcquisitionFunction, Any], Any]],
@@ -251,15 +253,15 @@
                 raise AssertionError(
                     f"Expected X to be `batch_shape x q={expected_q} x d`, but"
                     f" got X with shape {X.shape}."
                 )
             # add t-batch dim
             X = X if X.dim() > 2 else X.unsqueeze(0)
             output = method(acqf, X, *args, **kwargs)
-            if hasattr(acqf, "model") and is_fully_bayesian(acqf.model):
+            if hasattr(acqf, "model") and is_ensemble(acqf.model):
                 # IDEA: this could be wrapped into SampleReducingMCAcquisitionFunction
                 output = (
                     output.mean(dim=-1) if not acqf._log else logmeanexp(output, dim=-1)
                 )
             if assert_output_shape and not _verify_output_shape(
                 acqf=acqf,
                 X=X,
```

### Comparing `botorch-0.9.4/botorch/utils/types.py` & `botorch-0.9.5/botorch/utils/types.py`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch.egg-info/PKG-INFO` & `botorch-0.9.5/botorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botorch
-Version: 0.9.4
+Version: 0.9.5
 Summary: Bayesian Optimization in PyTorch
 Home-page: https://botorch.org
 Author: Meta Platforms, Inc.
 License: MIT
 Project-URL: Documentation, https://botorch.org
 Project-URL: Source, https://github.com/pytorch/botorch
 Project-URL: conda, https://anaconda.org/pytorch/botorch
@@ -28,15 +28,15 @@
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: ufmt; extra == "dev"
 Requires-Dist: flake8-docstrings; extra == "dev"
 Requires-Dist: black==22.3.0; extra == "dev"
 Requires-Dist: usort==1.0.2; extra == "dev"
-Requires-Dist: sphinx<=7.1.2; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: tutorials
 Requires-Dist: ax-platform; extra == "tutorials"
 Requires-Dist: cma; extra == "tutorials"
 Requires-Dist: jupyter; extra == "tutorials"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botorch Version: 0.9.4 Summary: Bayesian
+Metadata-Version: 2.1 Name: botorch Version: 0.9.5 Summary: Bayesian
 Optimization in PyTorch Home-page: https://botorch.org Author: Meta Platforms,
 Inc. License: MIT Project-URL: Documentation, https://botorch.org Project-URL:
 Source, https://github.com/pytorch/botorch Project-URL: conda, https://
 anaconda.org/pytorch/botorch Keywords: Bayesian optimization,PyTorch
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering Classifier: Intended Audience ::
@@ -10,23 +10,23 @@
 >=3.9 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: multipledispatch Requires-Dist: scipy Requires-Dist: torch>=1.13.1
 Requires-Dist: pyro-ppl>=1.8.4 Requires-Dist: gpytorch==1.11 Requires-Dist:
 linear_operator==0.5.1 Provides-Extra: dev Requires-Dist: pytest; extra ==
 "dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: flake8; extra ==
 "dev" Requires-Dist: ufmt; extra == "dev" Requires-Dist: flake8-docstrings;
 extra == "dev" Requires-Dist: black==22.3.0; extra == "dev" Requires-Dist:
-usort==1.0.2; extra == "dev" Requires-Dist: sphinx<=7.1.2; extra == "dev"
-Provides-Extra: test Requires-Dist: pytest; extra == "test" Requires-Dist:
-pytest-cov; extra == "test" Provides-Extra: tutorials Requires-Dist: ax-
-platform; extra == "tutorials" Requires-Dist: cma; extra == "tutorials"
-Requires-Dist: jupyter; extra == "tutorials" Requires-Dist: kaleido; extra ==
-"tutorials" Requires-Dist: matplotlib; extra == "tutorials" Requires-Dist:
-memory_profiler; extra == "tutorials" Requires-Dist: papermill; extra ==
-"tutorials" Requires-Dist: pykeops; extra == "tutorials" Requires-Dist:
-torchvision; extra == "tutorials" _[_B_o_T_o_r_c_h_ _L_o_g_o_]
+usort==1.0.2; extra == "dev" Requires-Dist: sphinx; extra == "dev" Provides-
+Extra: test Requires-Dist: pytest; extra == "test" Requires-Dist: pytest-cov;
+extra == "test" Provides-Extra: tutorials Requires-Dist: ax-platform; extra ==
+"tutorials" Requires-Dist: cma; extra == "tutorials" Requires-Dist: jupyter;
+extra == "tutorials" Requires-Dist: kaleido; extra == "tutorials" Requires-
+Dist: matplotlib; extra == "tutorials" Requires-Dist: memory_profiler; extra ==
+"tutorials" Requires-Dist: papermill; extra == "tutorials" Requires-Dist:
+pykeops; extra == "tutorials" Requires-Dist: torchvision; extra == "tutorials"
+_[_B_o_T_o_r_c_h_ _L_o_g_o_]
 ===============================================================================
 [![Support Ukraine](https://img.shields.io/badge/Support-Ukraine-
 FFD500?style=flat&labelColor=005BBB)](https://opensource.fb.com/support-
 ukraine) [![Lint](https://github.com/pytorch/botorch/workflows/Lint/badge.svg)]
 (https://github.com/pytorch/botorch/actions?query=workflow%3ALint) [![Test]
 (https://github.com/pytorch/botorch/workflows/Test/badge.svg)](https://
 github.com/pytorch/botorch/actions?query=workflow%3ATest) [![Docs](https://
```

### Comparing `botorch-0.9.4/botorch.egg-info/SOURCES.txt` & `botorch-0.9.5/botorch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 botorch/acquisition/preference.py
 botorch/acquisition/prior_guided.py
 botorch/acquisition/proximal.py
 botorch/acquisition/risk_measures.py
 botorch/acquisition/utils.py
 botorch/acquisition/multi_objective/__init__.py
 botorch/acquisition/multi_objective/analytic.py
+botorch/acquisition/multi_objective/hypervolume_knowledge_gradient.py
 botorch/acquisition/multi_objective/joint_entropy_search.py
 botorch/acquisition/multi_objective/logei.py
 botorch/acquisition/multi_objective/max_value_entropy_search.py
 botorch/acquisition/multi_objective/monte_carlo.py
 botorch/acquisition/multi_objective/multi_fidelity.py
 botorch/acquisition/multi_objective/multi_output_risk_measures.py
 botorch/acquisition/multi_objective/objective.py
@@ -188,14 +189,15 @@
 botorch/utils/feasible_volume.py
 botorch/utils/gp_sampling.py
 botorch/utils/low_rank.py
 botorch/utils/objective.py
 botorch/utils/rounding.py
 botorch/utils/safe_math.py
 botorch/utils/sampling.py
+botorch/utils/test_helpers.py
 botorch/utils/testing.py
 botorch/utils/torch.py
 botorch/utils/transforms.py
 botorch/utils/types.py
 botorch/utils/multi_objective/__init__.py
 botorch/utils/multi_objective/hypervolume.py
 botorch/utils/multi_objective/pareto.py
```

### Comparing `botorch-0.9.4/botorch_logo_lockup.png` & `botorch-0.9.5/botorch_logo_lockup.png`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/botorch_logo_lockup.svg` & `botorch-0.9.5/botorch_logo_lockup.svg`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/notebooks/tutorials_performance_tracking.ipynb` & `botorch-0.9.5/notebooks/tutorials_performance_tracking.ipynb`

 * *Files identical despite different names*

### Comparing `botorch-0.9.4/setup.py` & `botorch-0.9.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         else dep
         for dep in install_requires
     ]
 
 # Read in pinned versions of the formatting tools
 FMT_REQUIRES += read_deps_from_file("requirements-fmt.txt")
 # Dev is test + formatting + docs generation
-DEV_REQUIRES = TEST_REQUIRES + FMT_REQUIRES + ["sphinx<=7.1.2"]
+DEV_REQUIRES = TEST_REQUIRES + FMT_REQUIRES + ["sphinx"]
 
 # read in README.md as the long description
 with open(os.path.join(root_dir, "README.md"), "r") as fh:
     long_description = fh.read()
 
 setup(
     name="botorch",
```

