# Comparing `tmp/metcalcpy-2.0.2.tar.gz` & `tmp/metcalcpy-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metcalcpy-2.0.2.tar", last modified: Thu Mar  2 22:39:00 2023, max compression
+gzip compressed data, was "metcalcpy-2.1.tar", last modified: Tue Aug  1 23:44:24 2023, max compression
```

## Comparing `metcalcpy-2.0.2.tar` & `metcalcpy-2.1.tar`

### file list

```diff
@@ -1,110 +1,112 @@
-drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:39:00.578368 metcalcpy-2.0.2/
--rw-r--r--   0 minnawin  (8494) rap       (1500)    10141 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/LICENSE.md
--rw-r--r--   0 minnawin  (8494) rap       (1500)     2160 2023-03-02 22:39:00.577878 metcalcpy-2.0.2/PKG-INFO
--rw-r--r--   0 minnawin  (8494) rap       (1500)     1746 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/README.md
-drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:39:00.514944 metcalcpy-2.0.2/metcalcpy/
--rw-r--r--   0 minnawin  (8494) rap       (1500)      455 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/__init__.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    13080 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/agg_eclv.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    52230 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/agg_stat.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    15049 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/agg_stat_bootstrap.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     6014 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/agg_stat_eqz.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     6736 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/agg_stat_event_equalize.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    24086 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/bootstrap.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     6730 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/calc_difficulty_index.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     9426 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/compare_images.py
-drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:39:00.519062 metcalcpy-2.0.2/metcalcpy/contributed/
--rw-r--r--   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/__init__.py
-drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:39:00.522070 metcalcpy-2.0.2/metcalcpy/contributed/blocking_weather_regime/
--rw-r--r--   0 minnawin  (8494) rap       (1500)    16138 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/blocking_weather_regime/Blocking.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     7463 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/blocking_weather_regime/Blocking_WeatherRegime_util.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     9095 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/blocking_weather_regime/WeatherRegime.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/blocking_weather_regime/__init__.py
-drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:39:00.523355 metcalcpy-2.0.2/metcalcpy/contributed/mjo_enso/
--rw-r--r--   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/mjo_enso/__init__.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     5656 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/mjo_enso/compute_mjo_enso.py
-drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:39:00.524893 metcalcpy-2.0.2/metcalcpy/contributed/rmm_omi/
--rwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/rmm_omi/__init__.py
--rwxr-xr-x   0 minnawin  (8494) rap       (1500)    20930 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/rmm_omi/compute_mjo_indices.py
-drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:39:00.528920 metcalcpy-2.0.2/metcalcpy/contributed/spacetime/
--rw-r--r--   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/spacetime/__init__.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     4955 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/spacetime/cross_spectra.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    19340 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/spacetime/matsuno_plot.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    21177 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/spacetime/spacetime.py
--rwxr-xr-x   0 minnawin  (8494) rap       (1500)     2922 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/spacetime/spacetime_utils.py
-drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:39:00.534554 metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/
--rw-r--r--   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/__init__.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    13787 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/ccew_activity.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     1593 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/compute_omi_example.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     2455 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/compute_rmm_example.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     2352 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/example_kelvin_activity.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     1734 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/phase_diagram_example.py
--rwxr-xr-x   0 minnawin  (8494) rap       (1500)     2817 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/utils.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     7610 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/event_equalize.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     2401 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/event_equalize_against_values.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     2543 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/piecewise_linear.py
-drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:39:00.536745 metcalcpy-2.0.2/metcalcpy/pre_processing/
--rw-r--r--   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/pre_processing/__init__.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     2188 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/pre_processing/directional_means.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     9683 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/pre_processing/waves.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     6551 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/process_tcrmw.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    21076 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/scorecard.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    13914 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/sum_stat.py
-drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:39:00.561382 metcalcpy-2.0.2/metcalcpy/util/
--rw-r--r--   0 minnawin  (8494) rap       (1500)      309 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/__init__.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    41233 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/correlation.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    42550 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/ctc_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     3744 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/eclv_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    23991 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/ecnt_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     9142 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/grad_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     2562 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/mcts_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     1929 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/met_stats.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    24567 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/mode_2d_arearat_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    25000 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/mode_2d_ratio_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    23625 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/mode_3d_ratio_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    27185 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/mode_3d_volrat_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    43516 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/mode_arearat_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    39198 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/mode_ratio_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     7794 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/nbrcnt_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     9225 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/nbrctc_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    15802 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/pstd_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     2276 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/read_env_vars_in_config.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     4268 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/read_file.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     4468 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/rps_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     6174 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/sal1l2_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    24743 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/sl1l2_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    12963 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/ssvar_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     6316 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/tost_paired.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    52711 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/utils.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     3697 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/val1l2_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    24160 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/vcnt_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    10330 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/vl1l2_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     3101 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/util/wald_wolfowitz_runs_test.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     9261 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/validate_mv_python.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    24014 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/metcalcpy/vertical_interp.py
-drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:39:00.518244 metcalcpy-2.0.2/metcalcpy.egg-info/
--rw-r--r--   0 minnawin  (8494) rap       (1500)     2160 2023-03-02 22:38:59.000000 metcalcpy-2.0.2/metcalcpy.egg-info/PKG-INFO
--rw-r--r--   0 minnawin  (8494) rap       (1500)     3467 2023-03-02 22:39:00.000000 metcalcpy-2.0.2/metcalcpy.egg-info/SOURCES.txt
--rw-r--r--   0 minnawin  (8494) rap       (1500)        1 2023-03-02 22:39:00.000000 metcalcpy-2.0.2/metcalcpy.egg-info/dependency_links.txt
--rw-r--r--   0 minnawin  (8494) rap       (1500)       15 2023-03-02 22:39:00.000000 metcalcpy-2.0.2/metcalcpy.egg-info/top_level.txt
--rw-r--r--   0 minnawin  (8494) rap       (1500)       38 2023-03-02 22:39:00.578509 metcalcpy-2.0.2/setup.cfg
--rw-r--r--   0 minnawin  (8494) rap       (1500)      861 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/setup.py
-drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-03-02 22:39:00.577063 metcalcpy-2.0.2/test/
--rw-r--r--   0 minnawin  (8494) rap       (1500)       68 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/__init__.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     1723 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_agg_eclv.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)    11610 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_agg_stats_and_boot.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     2091 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_agg_stats_with_groups.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     1897 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_calc_difficulty_index.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)      645 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_compare_images.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)      543 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_convert_lon_indices.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     5105 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_ctc_statistics.py
--rwxr-xr-x   0 minnawin  (8494) rap       (1500)     7182 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_event_equalize.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     2052 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_event_equalize_against_values.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     7732 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_future_warnings.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     2381 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_grid_diag.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)      892 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_lon_360_to_180.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     3346 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_scorecard.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     6592 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_spacetime.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     3069 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_statistics.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     1230 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_tost_paired.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     9228 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_utils.py
--rw-r--r--   0 minnawin  (8494) rap       (1500)     1002 2023-03-02 22:38:10.000000 metcalcpy-2.0.2/test/test_validate_mv_python.py
+drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-08-01 23:44:24.609673 metcalcpy-2.1/
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    10141 2023-08-01 22:27:52.000000 metcalcpy-2.1/LICENSE.md
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     2373 2023-08-01 23:44:24.609171 metcalcpy-2.1/PKG-INFO
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     1928 2023-08-01 23:38:46.000000 metcalcpy-2.1/README.md
+drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-08-01 23:44:24.504892 metcalcpy-2.1/metcalcpy/
+-rw-r--r--   0 minnawin  (8494) rap       (1500)      455 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/__init__.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    13080 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/agg_eclv.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    53619 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/agg_stat.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    15049 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/agg_stat_bootstrap.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     6014 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/agg_stat_eqz.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     6736 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/agg_stat_event_equalize.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    24076 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/bootstrap.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     6730 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/calc_difficulty_index.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     9426 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/compare_images.py
+drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-08-01 23:44:24.509647 metcalcpy-2.1/metcalcpy/contributed/
+-rw-r--r--   0 minnawin  (8494) rap       (1500)        0 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/__init__.py
+drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-08-01 23:44:24.513981 metcalcpy-2.1/metcalcpy/contributed/blocking_weather_regime/
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    16138 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/blocking_weather_regime/Blocking.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     7465 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/blocking_weather_regime/Blocking_WeatherRegime_util.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     9095 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/blocking_weather_regime/WeatherRegime.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)        0 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/blocking_weather_regime/__init__.py
+drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-08-01 23:44:24.516747 metcalcpy-2.1/metcalcpy/contributed/mjo_enso/
+-rw-r--r--   0 minnawin  (8494) rap       (1500)        0 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/mjo_enso/__init__.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     5656 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/mjo_enso/compute_mjo_enso.py
+drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-08-01 23:44:24.518457 metcalcpy-2.1/metcalcpy/contributed/rmm_omi/
+-rwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/rmm_omi/__init__.py
+-rwxr-xr-x   0 minnawin  (8494) rap       (1500)    20930 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/rmm_omi/compute_mjo_indices.py
+drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-08-01 23:44:24.525666 metcalcpy-2.1/metcalcpy/contributed/spacetime/
+-rw-r--r--   0 minnawin  (8494) rap       (1500)        0 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/spacetime/__init__.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     6022 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/spacetime/cross_spectra.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    19340 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/spacetime/matsuno_plot.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    21177 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/spacetime/spacetime.py
+-rwxr-xr-x   0 minnawin  (8494) rap       (1500)     2922 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/spacetime/spacetime_utils.py
+drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-08-01 23:44:24.532626 metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/
+-rw-r--r--   0 minnawin  (8494) rap       (1500)        0 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/__init__.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    13787 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/ccew_activity.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     1593 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/compute_omi_example.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     2455 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/compute_rmm_example.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     2352 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/example_kelvin_activity.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     1734 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/phase_diagram_example.py
+-rwxr-xr-x   0 minnawin  (8494) rap       (1500)     2817 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/utils.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     7713 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/event_equalize.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     2401 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/event_equalize_against_values.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     2543 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/piecewise_linear.py
+drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-08-01 23:44:24.535216 metcalcpy-2.1/metcalcpy/pre_processing/
+-rw-r--r--   0 minnawin  (8494) rap       (1500)        0 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/pre_processing/__init__.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     2188 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/pre_processing/directional_means.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     9683 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/pre_processing/waves.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     6955 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/process_tcrmw.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    21076 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/scorecard.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    13914 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/sum_stat.py
+drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-08-01 23:44:24.588993 metcalcpy-2.1/metcalcpy/util/
+-rw-r--r--   0 minnawin  (8494) rap       (1500)      309 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/__init__.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    41233 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/correlation.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    42550 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/ctc_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     3744 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/eclv_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    23991 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/ecnt_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     9142 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/grad_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     2562 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/mcts_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     1929 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/met_stats.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    24567 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/mode_2d_arearat_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    25000 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/mode_2d_ratio_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    23625 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/mode_3d_ratio_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    27185 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/mode_3d_volrat_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    43516 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/mode_arearat_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    39198 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/mode_ratio_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     7794 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/nbrcnt_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     9225 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/nbrctc_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    16115 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/pstd_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     2276 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/read_env_vars_in_config.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     4268 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/read_file.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     4468 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/rps_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     6174 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/sal1l2_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    24743 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/sl1l2_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    12963 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/ssvar_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     6316 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/tost_paired.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    52328 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/utils.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     3697 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/val1l2_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    24160 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/vcnt_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    10330 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/vl1l2_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     3101 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/util/wald_wolfowitz_runs_test.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     9261 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/validate_mv_python.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    24014 2023-08-01 22:27:52.000000 metcalcpy-2.1/metcalcpy/vertical_interp.py
+drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-08-01 23:44:24.508764 metcalcpy-2.1/metcalcpy.egg-info/
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     2373 2023-08-01 23:44:24.000000 metcalcpy-2.1/metcalcpy.egg-info/PKG-INFO
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     3518 2023-08-01 23:44:24.000000 metcalcpy-2.1/metcalcpy.egg-info/SOURCES.txt
+-rw-r--r--   0 minnawin  (8494) rap       (1500)        1 2023-08-01 23:44:24.000000 metcalcpy-2.1/metcalcpy.egg-info/dependency_links.txt
+-rw-r--r--   0 minnawin  (8494) rap       (1500)       15 2023-08-01 23:44:24.000000 metcalcpy-2.1/metcalcpy.egg-info/top_level.txt
+-rw-r--r--   0 minnawin  (8494) rap       (1500)       38 2023-08-01 23:44:24.609808 metcalcpy-2.1/setup.cfg
+-rw-r--r--   0 minnawin  (8494) rap       (1500)      900 2023-08-01 23:34:13.000000 metcalcpy-2.1/setup.py
+drwxr-xr-x   0 minnawin  (8494) rap       (1500)        0 2023-08-01 23:44:24.608297 metcalcpy-2.1/test/
+-rw-r--r--   0 minnawin  (8494) rap       (1500)       68 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/__init__.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     1723 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_agg_eclv.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     2791 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_agg_ratio.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)    13553 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_agg_stats_and_boot.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     2091 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_agg_stats_with_groups.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     1897 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_calc_difficulty_index.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)      645 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_compare_images.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)      543 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_convert_lon_indices.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     5105 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_ctc_statistics.py
+-rwxr-xr-x   0 minnawin  (8494) rap       (1500)     7182 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_event_equalize.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     2052 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_event_equalize_against_values.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     7732 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_future_warnings.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     2381 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_grid_diag.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)      892 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_lon_360_to_180.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)      640 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_no_ARIMA_utils.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     3346 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_scorecard.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     6592 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_spacetime.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     3069 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_statistics.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     1230 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_tost_paired.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     9228 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_utils.py
+-rw-r--r--   0 minnawin  (8494) rap       (1500)     1002 2023-08-01 22:27:52.000000 metcalcpy-2.1/test/test_validate_mv_python.py
```

### Comparing `metcalcpy-2.0.2/LICENSE.md` & `metcalcpy-2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/PKG-INFO` & `metcalcpy-2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,21 @@
-Metadata-Version: 2.1
-Name: metcalcpy
-Version: 2.0.2
-Summary: statistics and util package for METplus
-Home-page: https://github.com/dtcenter/METcalcpy
-Author: METplus
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # METcalcpy
 Provides libraries for the following: calculation of statistics, pre-processing input, and performing diagnostics for METviewer, 
 METexpress, and the plotting scripts in METplotpy.
 
 Please see the [METcalcpy User's Guide](https://metcalcpy.readthedocs.io/en/latest) for more information.
 
 Support for the METplus components is provided through the
 [METplus Discussions](https://github.com/dtcenter/METplus/discussions) forum.
 Users are welcome and encouraged to answer or address each other's questions there!  For more
 information, please read
 "[Welcome to the METplus Components Discussions](https://github.com/dtcenter/METplus/discussions/939)".
 
+For information about the support provided for releases, see our [Release Support Policy](https://metplus.readthedocs.io/en/develop/Release_Guide/index.html#release-support-policy).
+
 Instructions for installing the metcalcpy package locally
 ---------------------------------------------------------
 - activate your conda environment (i.e. 'conda activate your-conda-env-name')
 - from within your active conda environment, cd to the METcalcpy/ directory, where you will see the setup.py script
 - from this directory, run the following on the command line: pip install -e .
 - the -e option stands for editable, which is useful in that you can update your METcalcpy/metcalcpy source without reinstalling it 
 - the . indicates that you should search the current directory for the setup.py script
@@ -36,10 +25,10 @@
    
     - import metcalcpy.util.ctc_statistics as cstats
         - to use the functions in the ctc_statistics module
   
 Instructions for installing the metcalcpy package from PyPI
 -----------------------------------------------------------
 
-- activate your Python 3.8.6+ conda environment
+- activate your Python 3.10+ conda environment
 - run the following from the command line:
    -  pip install metcalcpy==x.y.z  where x.y.z is the version number of interest
```

### Comparing `metcalcpy-2.0.2/metcalcpy/agg_eclv.py` & `metcalcpy-2.1/metcalcpy/agg_eclv.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/agg_stat.py` & `metcalcpy-2.1/metcalcpy/agg_stat.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,30 +298,46 @@
             # The single value case
             num_of_columns = values_both_arrays.shape[1] - 1
             # get values for the 1st array
             values_1 = values_both_arrays[:, 0:int(num_of_columns / 2)]
             # get values for the 2nd array
             values_2 = values_both_arrays[:, int(num_of_columns / 2):num_of_columns]
 
-            func_name = f'calculate_{self.statistic}'
+            try:
+                # find the index of the stat column
+                stat_column_index = np.where(self.column_names == 'stat_name')[0][0]
+                # find the actual statistic and corresponding functions for both curves
+                stat_1 = values_1[0, stat_column_index].lower()
+                stat_2 = values_2[0, stat_column_index].lower()
+                func_name_1 = f'calculate_{stat_1}'
+                func_name_2 = f'calculate_{stat_2}'
+            except ValueError:
+                func_name_1 = f'calculate_{self.statistic}'
+                func_name_2 = f'calculate_{self.statistic}'
+
+
+
             # some functions have an extra 3rd parameter that represents
             # if some data preliminary data aggregation was done
             # if this parameter is present we need to add it
-            num_parameters = len(signature(globals()[func_name]).parameters)
+            num_parameters_1 = len(signature(globals()[func_name_1]).parameters)
+            num_parameters_2 = len(signature(globals()[func_name_2]).parameters)
 
-            if num_parameters == 2:
-                # calculate stat for the 1st array
-                stat_values_1 = [globals()[func_name](values_1, self.column_names)]
-                # calculate stat for the 2nd array
-                stat_values_2 = [globals()[func_name](values_2, self.column_names)]
+
+            # calculate stat for the 1st array
+            if num_parameters_1 == 2:
+                stat_values_1 = [globals()[func_name_1](values_1, self.column_names)]
             else:
-                # calculate stat for the 1st array
-                stat_values_1 = [globals()[func_name](values_1, self.column_names, True)]
-                # calculate stat for the 2nd array
-                stat_values_2 = [globals()[func_name](values_2, self.column_names, True)]
+                stat_values_1 = [globals()[func_name_1](values_1, self.column_names, True)]
+
+            # calculate stat for the 2nd array
+            if num_parameters_2 == 2:
+                stat_values_2 = [globals()[func_name_2](values_2, self.column_names)]
+            else:
+                stat_values_2 = [globals()[func_name_2](values_2, self.column_names, True)]
 
             # calculate derived stat
             stat_values = calc_derived_curve_value(
                 stat_values_1,
                 stat_values_2,
                 values_both_arrays[0, -1])
             if not isinstance(stat_values, list):
@@ -333,30 +349,44 @@
             for row in values_both_arrays:
 
                 # get values for the 1st array
                 values_1 = row[:, 0:int(num_of_columns / 2)]
                 # get values for the 2nd array
                 values_2 = row[:, int(num_of_columns / 2):num_of_columns]
 
-                func_name = f'calculate_{self.statistic}'
+                try:
+                    # find the index of the stat column
+                    stat_column_index = np.where(self.column_names == 'stat_name')[0][0]
+                    # find the actual statistic and corresponding functions for both curves
+                    stat_1 = values_1[0, stat_column_index].lower()
+                    stat_2 = values_2[0, stat_column_index].lower()
+                    func_name_1 = f'calculate_{stat_1}'
+                    func_name_2 = f'calculate_{stat_2}'
+                except ValueError:
+                    func_name_1 = f'calculate_{self.statistic}'
+                    func_name_2 = f'calculate_{self.statistic}'
+
                 # some functions have an extra 3rd parameter that represents
                 # if some data preliminary data aggregation was done
                 # if this parameter is present we need to add it
-                num_parameters = len(signature(globals()[func_name]).parameters)
+                num_parameters_1 = len(signature(globals()[func_name_1]).parameters)
+                num_parameters_2 = len(signature(globals()[func_name_2]).parameters)
 
-                if num_parameters == 2:
-                    # calculate stat for the 1st array
-                    stat_values_1 = [globals()[func_name](values_1, self.column_names)]
-                    # calculate stat for the 2nd array
-                    stat_values_2 = [globals()[func_name](values_2, self.column_names)]
+                # calculate stat for the 1st array
+                if num_parameters_1 == 2:
+                    stat_values_1 = [globals()[func_name_1](values_1, self.column_names)]
                 else:
-                    # calculate stat for the 1st array
-                    stat_values_1 = [globals()[func_name](values_1, self.column_names, True)]
-                    # calculate stat for the 2nd array
-                    stat_values_2 = [globals()[func_name](values_2, self.column_names, True)]
+                    stat_values_1 = [globals()[func_name_1](values_1, self.column_names, True)]
+
+                # calculate stat for the 2nd array
+                if num_parameters_2 == 2:
+                    stat_values_2 = [globals()[func_name_2](values_2, self.column_names)]
+                else:
+                    stat_values_2 = [globals()[func_name_2](values_2, self.column_names, True)]
+
 
                 # calculate derived stat
                 stat_value = calc_derived_curve_value(
                     stat_values_1,
                     stat_values_2,
                     row[0, -1])
                 if not isinstance(stat_value, list):
@@ -1126,15 +1156,16 @@
             self.input_data = perform_event_equalization(self.params, self.input_data)
 
         # get results for axis1
         out_frame = self._proceed_with_axis("1")
 
         # get results for axis2 if needed
         if self.params['series_val_2']:
-            out_frame = out_frame.append(self._proceed_with_axis("2"))
+            axis_2_frame= self._proceed_with_axis("2")
+            out_frame = pd.concat([out_frame, axis_2_frame], ignore_index=True)
 
         header = True
         mode = 'w'
 
         if 'append_to_file' in self.params.keys() and self.params['append_to_file'] == 'True':
             header = False
             mode = 'a'
@@ -1146,11 +1177,12 @@
 
 if __name__ == "__main__":
     PARSER = argparse.ArgumentParser(description='List of agg_stat arguments')
     PARSER.add_argument("parameters_file", help="Path to YAML parameters file",
                         type=argparse.FileType('r'),
                         default=sys.stdin)
     ARGS = PARSER.parse_args()
-    PARAMS = yaml.load(ARGS.parameters_file, Loader=yaml.FullLoader)
+    with ARGS.parameters_file as parameters_file:
+        PARAMS = yaml.load(parameters_file, Loader=yaml.FullLoader)
 
     AGG_STAT = AggStat(PARAMS)
     AGG_STAT.calculate_stats_and_ci()
```

### Comparing `metcalcpy-2.0.2/metcalcpy/agg_stat_bootstrap.py` & `metcalcpy-2.1/metcalcpy/agg_stat_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/agg_stat_eqz.py` & `metcalcpy-2.1/metcalcpy/agg_stat_eqz.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/agg_stat_event_equalize.py` & `metcalcpy-2.1/metcalcpy/agg_stat_event_equalize.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/bootstrap.py` & `metcalcpy-2.1/metcalcpy/bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
  
  
 """
 Program Name: bootstrap.py
 """
 
 import numpy as _np
-from collections import Iterable
+from collections.abc import Iterable
 import multiprocessing as _multiprocessing
 import scipy.sparse as _sparse
 
 __author__ = 'Tatiana Burek'
 __version__ = '0.1.0'
 
 
@@ -334,16 +334,16 @@
         # display a warning and do not calculate CIs - like boot.ci in R
         if _all_the_same(bootstrap_dist):
             print(f'All values of t are equal to {bootstrap_dist[0]}. Cannot calculate confidence intervals')
             low = None
             high = None
         else:
             bd = bootstrap_dist[bootstrap_dist != _np.array([None])]
-            low = _np.percentile(bd, 100 * (alpha / 2.), interpolation='linear')
-            high = _np.percentile(bd, 100 * (1 - alpha / 2.), interpolation='linear')
+            low = _np.percentile(bd, 100 * (alpha / 2.), method='linear')
+            high = _np.percentile(bd, 100 * (1 - alpha / 2.), method='linear')
         val = stat_val
     else:
         low = None
         val = None
         high = None
     return BootstrapResults(lower_bound=low,
                             value=val,
```

### Comparing `metcalcpy-2.0.2/metcalcpy/calc_difficulty_index.py` & `metcalcpy-2.1/metcalcpy/calc_difficulty_index.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/compare_images.py` & `metcalcpy-2.1/metcalcpy/compare_images.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/blocking_weather_regime/Blocking.py` & `metcalcpy-2.1/metcalcpy/contributed/blocking_weather_regime/Blocking.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/blocking_weather_regime/Blocking_WeatherRegime_util.py` & `metcalcpy-2.1/metcalcpy/contributed/blocking_weather_regime/Blocking_WeatherRegime_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             valid_time_str = indata.variables[invar].getncattr('valid_time')
             lead_dt = datetime.datetime.strptime(valid_time_str,'%Y%m%d_%H%M%S') - datetime.datetime.strptime(init_time_str,'%Y%m%d_%H%M%S')
             leadmin,leadsec = divmod(lead_dt.total_seconds(), 60)
             leadhr,leadmin = divmod(leadmin,60)
             lead_str = str(int(leadhr)).zfill(2)+str(int(leadmin)).zfill(2)+str(int(leadsec)).zfill(2)
             indata.close()
         else:
-            new_invar = np.empty((1,len(var_3d[0,:,0]),len(var_3d[0,0,:])),dtype=np.float)
+            new_invar = np.empty((1,len(var_3d[0,:,0]),len(var_3d[0,0,:])),dtype=np.float64)
             init_time_str = ''
             valid_time_str = ''
             lead_str = ''
             new_invar[:] = np.nan
         init_list.append(init_time_str)
         valid_list.append(valid_time_str)
         lead_list.append(lead_str)
```

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/blocking_weather_regime/WeatherRegime.py` & `metcalcpy-2.1/metcalcpy/contributed/blocking_weather_regime/WeatherRegime.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/mjo_enso/compute_mjo_enso.py` & `metcalcpy-2.1/metcalcpy/contributed/mjo_enso/compute_mjo_enso.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/rmm_omi/compute_mjo_indices.py` & `metcalcpy-2.1/metcalcpy/contributed/rmm_omi/compute_mjo_indices.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/spacetime/matsuno_plot.py` & `metcalcpy-2.1/metcalcpy/contributed/spacetime/matsuno_plot.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/spacetime/spacetime.py` & `metcalcpy-2.1/metcalcpy/contributed/spacetime/spacetime.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/spacetime/spacetime_utils.py` & `metcalcpy-2.1/metcalcpy/contributed/spacetime/spacetime_utils.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/ccew_activity.py` & `metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/ccew_activity.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/compute_omi_example.py` & `metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/compute_omi_example.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/compute_rmm_example.py` & `metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/compute_rmm_example.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/example_kelvin_activity.py` & `metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/example_kelvin_activity.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/phase_diagram_example.py` & `metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/phase_diagram_example.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/contributed/tropical_diagnostics/utils.py` & `metcalcpy-2.1/metcalcpy/contributed/tropical_diagnostics/utils.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/event_equalize.py` & `metcalcpy-2.1/metcalcpy/event_equalize.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,28 +46,31 @@
                 at each combination of fcst_valid_beg, series values and independent value
                 - for example with MODE objects
     Returns:
         A data frame that contains equalized records
     """
     pd.options.mode.chained_assignment = None
     column_names = list(series_data)
-    exception_columns = ["", "fcst_valid_beg", 'fcst_lead', 'fcst_valid', 'fcst_init', 'fcst_init_beg']
+    exception_columns = ["", "fcst_valid_beg", 'fcst_lead', 'fcst_valid', 'fcst_init', 'fcst_init_beg', 'VALID', 'LEAD']
     if isinstance(fix_vars, str):
         fix_vars = [fix_vars]
-    if 'fcst_valid_beg' in column_names:
-        series_data['equalize'] = series_data.loc[:, 'fcst_valid_beg'].astype(str) \
-                                  + ' ' + series_data.loc[:, 'fcst_lead'].astype(str)
-    elif 'fcst_valid' in column_names:
-        series_data['equalize'] = series_data.loc[:, 'fcst_valid'].astype(str) + ' ' \
-                                  + series_data.loc[:, 'fcst_lead'].astype(str)
+
+    if 'equalize' not  in  series_data.columns:
+        if 'fcst_valid_beg' in column_names:
+            series_data['equalize'] = series_data.loc[:, 'fcst_valid_beg'].astype(str) \
+                                          + ' ' + series_data.loc[:, 'fcst_lead'].astype(str)
+        elif 'fcst_valid' in column_names:
+            series_data['equalize'] = series_data.loc[:, 'fcst_valid'].astype(str) + ' ' \
+                                          + series_data.loc[:, 'fcst_lead'].astype(str)
+
 
     # add independent variable if needed
     if equalize_by_indep and indy_var not in exception_columns:
         series_data['equalize'] = series_data.loc[:, 'equalize'].astype(str) + " " \
-                                  + series_data.loc[:, indy_var].astype(str)
+                                      + series_data.loc[:, indy_var].astype(str)
 
     vars_for_ee = dict()
 
     # add series variables
     if series_var_vals:
         for series_var, series_vals in series_var_vals.items():
             if series_var not in exception_columns:
```

### Comparing `metcalcpy-2.0.2/metcalcpy/event_equalize_against_values.py` & `metcalcpy-2.1/metcalcpy/event_equalize_against_values.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/piecewise_linear.py` & `metcalcpy-2.1/metcalcpy/piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/pre_processing/directional_means.py` & `metcalcpy-2.1/metcalcpy/pre_processing/directional_means.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/pre_processing/waves.py` & `metcalcpy-2.1/metcalcpy/pre_processing/waves.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/process_tcrmw.py` & `metcalcpy-2.1/metcalcpy/process_tcrmw.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,101 +4,107 @@
 import logging
 import numpy as np
 import xarray as xr
 
 
 def read_tcrmw(filename):
     ds = xr.open_dataset(filename)
-    # range, azimuth, pressure, track_point
-    for var in ds.keys():
-        logging.info((var, ds[var].dims))
-    for coord in ds.coords:
-        logging.debug((coord, ds[coord].values))
+    # Original data dimensions: range, azimuth, pressure, track_point.
+    # Recently updated data is: track_point, pressure, range, azimuth.
+    # Use xarray's transpose() to reorder to original data's dimension.
+    ds_transposed = ds.transpose('range', 'azimuth', 'pressure', 'track_point',  \
+                                 'track_line')
+    for var in ds_transposed.keys():
+        logging.info((var, ds_transposed[var].dims))
+    for coord in ds_transposed.coords:
+        logging.debug((coord, ds_transposed[coord].values))
 
-    return ds
+    return ds_transposed
 
 
-def compute_interpolation_weights(args, ds, levels):
+def compute_interpolation_weights(args, ds):
     dims = ds[args.T].dims
-    logging.info(dims)
+    logging.info(f"compute_interpolation_weights, dims:  {dims}")
     nr, na, nl, nt = ds[args.T].shape
-    logging.info((nr, na, nl, nt))
+
+    logging.info(f"compute_interpolation_weights||nr, na, nl, nt: "
+                 f"({nr, na, nl, nt})")
 
 
 def compute_wind_components(args, ds):
     """
     e_r = cos(theta) e_x + sin(theta) e_y
     e_theta = - sin(theta) e_x + cos(theta) e_y
     """
+
     nr, na, nl, nt = ds[args.T].shape
-    logging.info((nr, na, nl, nt))
     theta = np.empty((nr, na, nl, nt), dtype=np.float32)
     for i in range(nr):
         for k in range(nl):
             for t in range(nt):
-                theta[i, :, k, t] \
-                    = (np.pi / 180) * ds['azimuth'].values + np.pi / 2
+                theta[i, :, k, t] = (np.pi / 180) * ds['azimuth'].values + np.pi / 2
     mask = np.greater(theta, 2 * np.pi)
     theta[mask] = theta[mask] - 2 * np.pi
     u_radial = np.cos(theta) * ds[args.u].values + np.sin(theta) * ds[args.v].values
-    u_tangential = - np.sin(theta) * ds[args.u].values + np.cos(theta) * ds[args.v].values
+    u_tangential = - np.sin(theta) * ds[args.u].values + np.cos(theta) * ds[
+        args.v].values
     return u_radial, u_tangential
 
 
 def test_plot_pressure_lev(args, ds, track_index=0):
     # Plot setup
     import matplotlib.pyplot as plt
-    #import seaborn as sns
+    # import seaborn as sns
     # Set for dark PyCharm theme
-    #plt.style.use('dark_background')
+    # plt.style.use('dark_background')
     textcolor = (175 / 255, 177 / 255, 179 / 255)
-#    facecolor = (60 / 255, 63 / 255, 65 / 255)
+    #    facecolor = (60 / 255, 63 / 255, 65 / 255)
     # textcolor = (0, 0, 0)
     # facecolor = (1, 1, 1)
-    #sns.set_context('notebook')
+    # sns.set_context('notebook')
     plt.rcParams['figure.dpi'] = 300
     plt.rcParams['text.color'] = textcolor
     plt.rcParams['axes.edgecolor'] = textcolor
     plt.rcParams['axes.labelcolor'] = textcolor
     plt.rcParams['xtick.color'] = textcolor
     plt.rcParams['ytick.color'] = textcolor
     fig = plt.figure(figsize=(10, 5))
-    #fig.patch.set_facecolor(facecolor)
+    # fig.patch.set_facecolor(facecolor)
     ax = fig.add_subplot()
-    #ax.set_facecolor(facecolor)
+    # ax.set_facecolor(facecolor)
     ax.annotate('Tangential Wind (m s-1)', xy=(14, 350), color='darkgreen')
     ax.annotate('Temperature (K)', xy=(14, 370), color='darkblue')
     # nautical miles to kilometers conversion factor
     nm_to_km = 1.852
     ax.set_xlabel(
         'Range (RMW = %4.1f km)' % (nm_to_km * ds['RMW'][track_index]))
     ax.set_xticks(np.arange(1, 20))
     ax.set_ylabel('Pressure (mb)')
     ax.set_yscale('symlog')
     ax.set_ylim(1000, 250)
     ax.set_yticks(np.arange(1000, 250, -100))
     ax.set_yticklabels(np.arange(1000, 250, -100))
 
     # Azimuthal averages
-    u_radial_azi_mean = np.mean(ds['u_radial'].values, axis=1)
+    # u_radial_azi_mean
+    _ = np.mean(ds['u_radial'].values, axis=1)
     u_tangential_azi_mean = np.mean(ds['u_tangential'].values, axis=1)
-    T_azi_mean = np.mean(ds[args.T].values, axis=1)
+    t_azi_mean = np.mean(ds[args.T].values, axis=1)
 
     # Contour plots
     u_contour = ax.contour(ds['range'].values, ds['pressure'].values,
-        u_tangential_azi_mean[:, :, track_index].transpose(),
-        levels=np.arange(5, 40, 5), colors='darkgreen', linewidths=1)
+                           u_tangential_azi_mean[:, :, track_index].transpose(),
+                           levels=np.arange(5, 40, 5), colors='darkgreen', linewidths=1)
     ax.clabel(u_contour, colors='darkgreen', fmt='%1.0f')
-    T_contour = ax.contour(ds['range'].values, ds['pressure'].values,
-        T_azi_mean[:, :, track_index].transpose(),
-        levels=np.arange(250, 300, 10), colors='darkblue', linewidths=1)
-    ax.clabel(T_contour, colors='darkblue', fmt='%1.0f')
+    t_contour = ax.contour(ds['range'].values, ds['pressure'].values,
+                           t_azi_mean[:, :, track_index].transpose(),
+                           levels=np.arange(250, 300, 10), colors='darkblue',
+                           linewidths=1)
+    ax.clabel(t_contour, colors='darkblue', fmt='%1.0f')
 
-    # plt.savefig(os.path.join(args.datadir, 'test.pdf'))
-    # plt.savefig(os.path.join(args.datadir, 'test.png'), dpi=300)
     plt.show()
 
 
 if __name__ == '__main__':
     """
     Parse command line arguments
     """
@@ -170,15 +176,15 @@
     Open dataset
     """
     ds = read_tcrmw(filename_in)
 
     """
     Compute interpolation weights
     """
-    compute_interpolation_weights(args, ds, levels)
+    compute_interpolation_weights(args, ds)
 
     """
     Compute tangential and radial wind components
     """
     u_radial, u_tangential = compute_wind_components(args, ds)
 
     """
```

### Comparing `metcalcpy-2.0.2/metcalcpy/scorecard.py` & `metcalcpy-2.1/metcalcpy/scorecard.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/sum_stat.py` & `metcalcpy-2.1/metcalcpy/sum_stat.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/correlation.py` & `metcalcpy-2.1/metcalcpy/util/correlation.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/ctc_statistics.py` & `metcalcpy-2.1/metcalcpy/util/ctc_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/eclv_statistics.py` & `metcalcpy-2.1/metcalcpy/util/eclv_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/ecnt_statistics.py` & `metcalcpy-2.1/metcalcpy/util/ecnt_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/grad_statistics.py` & `metcalcpy-2.1/metcalcpy/util/grad_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/mcts_statistics.py` & `metcalcpy-2.1/metcalcpy/util/mcts_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/met_stats.py` & `metcalcpy-2.1/metcalcpy/util/met_stats.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/mode_2d_arearat_statistics.py` & `metcalcpy-2.1/metcalcpy/util/mode_2d_arearat_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/mode_2d_ratio_statistics.py` & `metcalcpy-2.1/metcalcpy/util/mode_2d_ratio_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/mode_3d_ratio_statistics.py` & `metcalcpy-2.1/metcalcpy/util/mode_3d_ratio_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/mode_3d_volrat_statistics.py` & `metcalcpy-2.1/metcalcpy/util/mode_3d_volrat_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/mode_arearat_statistics.py` & `metcalcpy-2.1/metcalcpy/util/mode_arearat_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/mode_ratio_statistics.py` & `metcalcpy-2.1/metcalcpy/util/mode_ratio_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/nbrcnt_statistics.py` & `metcalcpy-2.1/metcalcpy/util/nbrcnt_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/nbrctc_statistics.py` & `metcalcpy-2.1/metcalcpy/util/nbrctc_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/pstd_statistics.py` & `metcalcpy-2.1/metcalcpy/util/pstd_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     warnings.filterwarnings('error')
     try:
         df_pct_perm = _calc_common_stats(columns_names, input_data)
         t_table = df_pct_perm['n_i'].sum()
         o_bar_table = df_pct_perm['oy_i'].sum() / t_table
         o_bar = input_data[0, get_column_index_by_name(columns_names, 'o_bar')]
 
+        t_table.reset_index(inplace=True, drop=True)
+
         reliability = calc_reliability(t_table, df_pct_perm)
         resolution = calc_resolution(t_table, df_pct_perm, o_bar)
         uncertainty = calc_uncertainty(o_bar_table)
 
         brier = reliability - resolution + uncertainty
         result = round_half_up(brier, PRECISION)
     except (TypeError, ZeroDivisionError, Warning, ValueError):
@@ -70,14 +72,15 @@
     warnings.filterwarnings('error')
     try:
         df_pct_perm = _calc_common_stats(columns_names, input_data)
         t_table = df_pct_perm['n_i'].sum()
         o_bar_table = df_pct_perm['oy_i'].sum() / t_table
         o_bar = input_data[0, get_column_index_by_name(columns_names, 'o_bar')]
 
+        t_table.reset_index(inplace=True, drop=True)
         reliability = calc_reliability(t_table, df_pct_perm)
         resolution = calc_resolution(t_table, df_pct_perm, o_bar)
         uncertainty = calc_uncertainty(o_bar_table)
 
         bss_smpl = (resolution - reliability) / uncertainty
         result = round_half_up(bss_smpl, PRECISION)
 
@@ -154,15 +157,15 @@
             or None if some of the data values are missing or invalid
     """
     warnings.filterwarnings('error')
     try:
         df_pct_perm = _calc_common_stats(columns_names, input_data)
         o_bar = input_data[0, get_column_index_by_name(columns_names, 'o_bar')]
         t_table = df_pct_perm['n_i'].sum()
-
+        t_table.reset_index(inplace=True, drop=True)
         resolution = calc_resolution(t_table, df_pct_perm, o_bar)
         result = round_half_up(resolution, PRECISION)
     except (TypeError, ZeroDivisionError, Warning, ValueError):
         result = None
     warnings.filterwarnings('ignore')
     return result
 
@@ -270,14 +273,15 @@
         index=[0])
     final_roc = pd.concat([final_roc, roc])
     final_roc = pd.concat([final_roc,
         pd.DataFrame(
             {'thresh': 0, 'n11': 0, 'n10': 0, 'n01': 0, 'n00': 0, 'pody': 0, 'pofd': 0},
             index=[0]) ])
 
+    final_roc.reset_index(inplace=True, drop=True)
     roc_auc = 0
     for index, row in final_roc.iterrows():
         if index != 0:
             roc_auc = roc_auc + 0.5 * (final_roc.iloc[index - 1]['pody'] + row.pody) \
                       * (final_roc.iloc[index - 1]['pofd'] - row.pofd)
 
     result = round_half_up(roc_auc, PRECISION)
@@ -348,14 +352,16 @@
         elif "on_i" in column:
             sum_val = sum_column_data_by_name(input_data, columns_names, column)
             pct_perm['on_i'].append(sum_val)
         elif 'thresh_i' in column:
             pct_perm['thresh_i'].append(input_data[0, index])
     # calculate vectors and constants to use below
     df_pct_perm = pd.DataFrame(pct_perm)
+    df_pct_perm.reset_index(inplace=True, drop=True)
+
     n_i = [row.oy_i + row.on_i for index, row in df_pct_perm.iterrows()]
     df_pct_perm['n_i'] = n_i
 
     # use only records with n_i != 0
     df_pct_perm = df_pct_perm[df_pct_perm['n_i'] != 0]
     o_bar_i = [row.oy_i / row.n_i for index, row in df_pct_perm.iterrows()]
     calibration_i = [row.oy_i / row.n_i for index, row in df_pct_perm.iterrows()]
@@ -397,14 +403,16 @@
         df_roc.loc[df_roc.index[df_roc["thresh"] == thresh], 'n10'] = sum(data[is_bigger]['on_i'])
 
         is_less = data['thresh_i'] <= thresh
         # use df_roc.loc rather than df_roc.at in pandas versions above 1.2.3
         df_roc.loc[df_roc.index[df_roc["thresh"] == thresh], 'n01'] = sum(data[is_less]['oy_i'])
         df_roc.loc[df_roc.index[df_roc["thresh"] == thresh], 'n00'] = sum(data[is_less]['on_i'])
 
+    df_roc.reset_index(inplace=True, drop=True)
+
     # generate the pody and pofd scores from the contingency tables
     df_roc['pody'] = [row.n11 / (row.n11 + row.n01) for index, row in df_roc.iterrows()]
     df_roc['pofd'] = [row.n10 / (row.n10 + row.n00) for index, row in df_roc.iterrows()]
 
     return df_roc
```

### Comparing `metcalcpy-2.0.2/metcalcpy/util/read_env_vars_in_config.py` & `metcalcpy-2.1/metcalcpy/util/read_env_vars_in_config.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/read_file.py` & `metcalcpy-2.1/metcalcpy/util/read_file.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/rps_statistics.py` & `metcalcpy-2.1/metcalcpy/util/rps_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/sal1l2_statistics.py` & `metcalcpy-2.1/metcalcpy/util/sal1l2_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/sl1l2_statistics.py` & `metcalcpy-2.1/metcalcpy/util/sl1l2_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/ssvar_statistics.py` & `metcalcpy-2.1/metcalcpy/util/ssvar_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/tost_paired.py` & `metcalcpy-2.1/metcalcpy/util/tost_paired.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/utils.py` & `metcalcpy-2.1/metcalcpy/util/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -937,25 +937,15 @@
     number_of_none = sum(x is None or np.isnan(x) for x in data)
 
     if iqr > 0.0 and (len(data) - number_of_none) > 2:
         # Compute the first order auto-correlation coefficient
         # using a vector that is the same size as "data", but represents
         # represents excusions from the median of the data.
 
-        # Use excursions from the median to compute the first order auto-correlation coefficient.
-        data_excursions = list()
-        median = st.median(data)
-        for val in data:
-            if val >= median:
-                data_excursions.append(1)
-            else:
-                data_excursions.append(0)
-
-        arima = ARIMA(data_excursions, order=(1, 0, 0))
-        ar_1 = arima.fit().arparams[0]
+        ar_1 = autocor_coef(data)
 
         # Compute an variance inflation factor
         # (having removed that portion of the time series that was correlated).
         ratio = (1 + ar_1) / (1 - ar_1)
 
         # Check for a zero RATIO, that will then be operated on by SQRT.
         if ratio < 0.0:
```

### Comparing `metcalcpy-2.0.2/metcalcpy/util/val1l2_statistics.py` & `metcalcpy-2.1/metcalcpy/util/val1l2_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/vcnt_statistics.py` & `metcalcpy-2.1/metcalcpy/util/vcnt_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/vl1l2_statistics.py` & `metcalcpy-2.1/metcalcpy/util/vl1l2_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/util/wald_wolfowitz_runs_test.py` & `metcalcpy-2.1/metcalcpy/util/wald_wolfowitz_runs_test.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/validate_mv_python.py` & `metcalcpy-2.1/metcalcpy/validate_mv_python.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy/vertical_interp.py` & `metcalcpy-2.1/metcalcpy/vertical_interp.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/metcalcpy.egg-info/PKG-INFO` & `metcalcpy-2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: metcalcpy
-Version: 2.0.2
+Version: 2.1
 Summary: statistics and util package for METplus
 Home-page: https://github.com/dtcenter/METcalcpy
 Author: METplus
+Author-email: met-help@ucar.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # METcalcpy
 Provides libraries for the following: calculation of statistics, pre-processing input, and performing diagnostics for METviewer, 
 METexpress, and the plotting scripts in METplotpy.
 
@@ -19,14 +20,16 @@
 
 Support for the METplus components is provided through the
 [METplus Discussions](https://github.com/dtcenter/METplus/discussions) forum.
 Users are welcome and encouraged to answer or address each other's questions there!  For more
 information, please read
 "[Welcome to the METplus Components Discussions](https://github.com/dtcenter/METplus/discussions/939)".
 
+For information about the support provided for releases, see our [Release Support Policy](https://metplus.readthedocs.io/en/develop/Release_Guide/index.html#release-support-policy).
+
 Instructions for installing the metcalcpy package locally
 ---------------------------------------------------------
 - activate your conda environment (i.e. 'conda activate your-conda-env-name')
 - from within your active conda environment, cd to the METcalcpy/ directory, where you will see the setup.py script
 - from this directory, run the following on the command line: pip install -e .
 - the -e option stands for editable, which is useful in that you can update your METcalcpy/metcalcpy source without reinstalling it 
 - the . indicates that you should search the current directory for the setup.py script
@@ -36,10 +39,10 @@
    
     - import metcalcpy.util.ctc_statistics as cstats
         - to use the functions in the ctc_statistics module
   
 Instructions for installing the metcalcpy package from PyPI
 -----------------------------------------------------------
 
-- activate your Python 3.8.6+ conda environment
+- activate your Python 3.10+ conda environment
 - run the following from the command line:
    -  pip install metcalcpy==x.y.z  where x.y.z is the version number of interest
```

### Comparing `metcalcpy-2.0.2/metcalcpy.egg-info/SOURCES.txt` & `metcalcpy-2.1/metcalcpy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -73,24 +73,26 @@
 metcalcpy/util/utils.py
 metcalcpy/util/val1l2_statistics.py
 metcalcpy/util/vcnt_statistics.py
 metcalcpy/util/vl1l2_statistics.py
 metcalcpy/util/wald_wolfowitz_runs_test.py
 test/__init__.py
 test/test_agg_eclv.py
+test/test_agg_ratio.py
 test/test_agg_stats_and_boot.py
 test/test_agg_stats_with_groups.py
 test/test_calc_difficulty_index.py
 test/test_compare_images.py
 test/test_convert_lon_indices.py
 test/test_ctc_statistics.py
 test/test_event_equalize.py
 test/test_event_equalize_against_values.py
 test/test_future_warnings.py
 test/test_grid_diag.py
 test/test_lon_360_to_180.py
+test/test_no_ARIMA_utils.py
 test/test_scorecard.py
 test/test_spacetime.py
 test/test_statistics.py
 test/test_tost_paired.py
 test/test_utils.py
 test/test_validate_mv_python.py
```

### Comparing `metcalcpy-2.0.2/setup.py` & `metcalcpy-2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 with open(version_path) as version_file:
     exec(version_file.read(), main_ns)
 
 setuptools.setup(
     name="metcalcpy",
     version=main_ns['__version__'],
     author="METplus",
+    author_email="met-help@ucar.edu",
     description="statistics and util package for METplus",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dtcenter/METcalcpy",
     packages=setuptools.find_packages(),
     classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: Apache Software License",
          "Operating System :: OS Independent",
     ],
-    python_requires='>=3.8',
+    python_requires='>=3.10',
 )
```

### Comparing `metcalcpy-2.0.2/test/test_agg_eclv.py` & `metcalcpy-2.1/test/test_agg_eclv.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_agg_stats_and_boot.py` & `metcalcpy-2.1/test/test_agg_stats_and_boot.py`

 * *Files 16% similar despite different names*

```diff
@@ -166,14 +166,32 @@
 
     # get the number of rejected
     number_of_rejected = sum(x == 1 for x in reject)
     percent_of_rejected = number_of_rejected * 100 / TEST_LENGTH
     return percent_of_rejected
 
 
+def test_roc_auc(settings_pstd):
+    agg_stat = settings_pstd['agg_stat_pstd']
+    agg_stat.calculate_stats_and_ci()
+    result_frame = pd.read_csv(
+        agg_stat.params['agg_stat_output'],
+        header=[0],
+        sep='\t'
+    )
+    assert result_frame.size == 64
+    assert result_frame.shape == (8, 8)
+    assert np.allclose(result_frame['stat_value'][0], 0.9545967)
+    assert np.allclose(result_frame['stat_value'][1], 0.9518047)
+    assert np.allclose(result_frame['stat_value'][2], 0.9522863)
+    assert np.allclose(result_frame['stat_value'][3], 0.9501665)
+    assert np.allclose(result_frame['stat_value'][4], 0.9596318)
+    assert np.allclose(result_frame['stat_value'][5], 0.9590124)
+
+
 def test_prepare_sl1l2_data(settings):
     agg_stat = settings['agg_stat']
     series_data = agg_stat.input_data[
         (agg_stat.input_data['model'] == 'ENS001v3.6.1_d01')
         & (agg_stat.input_data["fcst_lead"] == 60000)]
     agg_stat.statistic = agg_stat.params['list_stat_1'][0].lower()
     agg_stat._prepare_sl1l2_data(series_data)
@@ -273,7 +291,36 @@
               'list_stat_1': ['FBAR'],
               'list_stat_2': [],
               'circular_block_bootstrap': False}
     agg_stat = AggStat(params)
     settings_dict = dict()
     settings_dict['agg_stat'] = agg_stat
     return settings_dict
+@pytest.fixture
+def settings_pstd():
+    """Initialise values for testing.
+
+    Returns:
+        dictionary with values of different type
+    """
+    params = {'random_seed': 1, 'indy_var': 'fcst_lead',
+               'method': 'perc',
+              'num_iterations': 1, 'event_equal': 'False',
+              'derived_series_1': [],
+              'derived_series_2': [],
+              'agg_stat_input': 'data/pstd.data.agg_stat',
+              'fcst_var_val_1': {'DPT_ENS_FREQ_ge288': ['PSTD_ROC_AUC']},
+              'fcst_var_val_2': {},
+              'agg_stat_output': 'data/pstd.data',
+              'fixed_vars_vals_input': {},
+              'series_val_1': {'model': ['RRFSE_CONUS_ICperts_nostoch.rrfs_conuscompact_3km_prob', 'RRFSE_CONUS_ICperts_stoch.rrfs_conuscompact_3km_prob']},
+              'series_val_2': {},
+              'alpha': 0.05, 'line_type': 'pct',
+              'num_threads': -1,
+              'indy_vals': ['160000', '170000', '180000', '190000'],
+              'list_stat_1': ['PSTD_ROC_AUC'],
+              'list_stat_2': [],
+              'circular_block_bootstrap': True}
+    pstd = AggStat(params)
+    settings_dict_pstd = dict()
+    settings_dict_pstd['agg_stat_pstd'] = pstd
+    return settings_dict_pstd
```

### Comparing `metcalcpy-2.0.2/test/test_agg_stats_with_groups.py` & `metcalcpy-2.1/test/test_agg_stats_with_groups.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_calc_difficulty_index.py` & `metcalcpy-2.1/test/test_calc_difficulty_index.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_compare_images.py` & `metcalcpy-2.1/test/test_compare_images.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_convert_lon_indices.py` & `metcalcpy-2.1/test/test_convert_lon_indices.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_ctc_statistics.py` & `metcalcpy-2.1/test/test_ctc_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_event_equalize.py` & `metcalcpy-2.1/test/test_event_equalize.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_event_equalize_against_values.py` & `metcalcpy-2.1/test/test_event_equalize_against_values.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_future_warnings.py` & `metcalcpy-2.1/test/test_future_warnings.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_grid_diag.py` & `metcalcpy-2.1/test/test_grid_diag.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_lon_360_to_180.py` & `metcalcpy-2.1/test/test_lon_360_to_180.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_scorecard.py` & `metcalcpy-2.1/test/test_scorecard.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_spacetime.py` & `metcalcpy-2.1/test/test_spacetime.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_statistics.py` & `metcalcpy-2.1/test/test_statistics.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_tost_paired.py` & `metcalcpy-2.1/test/test_tost_paired.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_utils.py` & `metcalcpy-2.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `metcalcpy-2.0.2/test/test_validate_mv_python.py` & `metcalcpy-2.1/test/test_validate_mv_python.py`

 * *Files identical despite different names*

