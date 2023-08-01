# Comparing `tmp/forked_ecephys_spike_sorting-0.1.0.tar.gz` & `tmp/forked_ecephys_spike_sorting-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forked_ecephys_spike_sorting-0.1.0.tar", last modified: Tue Aug  1 21:51:55 2023, max compression
+gzip compressed data, was "forked_ecephys_spike_sorting-0.1.1.tar", last modified: Tue Aug  1 22:52:38 2023, max compression
```

## Comparing `forked_ecephys_spike_sorting-0.1.0.tar` & `forked_ecephys_spike_sorting-0.1.1.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.524505 forked_ecephys_spike_sorting-0.1.0/
--rw-rw-rw-   0        0        0      327 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0       69 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1996 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      316 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      446 2023-08-01 21:51:55.524505 forked_ecephys_spike_sorting-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5828 2023-08-01 21:51:37.000000 forked_ecephys_spike_sorting-0.1.0/README.md
--rw-rw-rw-   0        0        0       56 2023-08-01 21:45:23.000000 forked_ecephys_spike_sorting-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.392502 forked_ecephys_spike_sorting-0.1.0/docs/
--rw-rw-rw-   0        0        0     7156 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.355502 forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.356502 forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.356502 forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/external_assets/
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.401502 forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/external_assets/images/
--rw-rw-rw-   0        0        0       58 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/external_assets/images/arrow_off.gif
--rw-rw-rw-   0        0        0       58 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/external_assets/images/arrow_on.gif
--rw-rw-rw-   0        0        0       58 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/external_assets/images/arrow_over.gif
--rw-rw-rw-   0        0        0    17447 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/external_assets/images/logo_AIBS.gif
--rw-rw-rw-   0        0        0     8238 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/external_assets/images/progress_indicator.gif
--rw-rw-rw-   0        0        0      351 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/external_assets/images/tab_blue.gif
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.403502 forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/style/
--rw-rw-rw-   0        0        0      401 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/style/comment.png
--rw-rw-rw-   0        0        0      415 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/style/nocomment.png
--rw-rw-rw-   0        0        0       29 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/authors.rst
--rw-rw-rw-   0        0        0     9531 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0       29 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/history.rst
--rw-rw-rw-   0        0        0      365 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/index.rst
--rw-rw-rw-   0        0        0      269 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/installation.rst
--rwxrwxrwx   0        0        0     6731 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/make.bat
--rw-rw-rw-   0        0        0       53 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/readme.rst
--rw-rw-rw-   0        0        0      109 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.405502 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.413502 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/common/
--rw-rw-rw-   0        0        0     2486 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/common/OEFileInfo.py
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/common/__init__.py
--rw-rw-rw-   0        0        0     2620 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/common/epoch.py
--rw-rw-rw-   0        0        0     2076 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/common/schemas.py
--rw-rw-rw-   0        0        0    13330 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/common/utils.py
--rw-rw-rw-   0        0        0    12514 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/common/visualization.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.415502 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.425502 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/__init__.py
--rw-rw-rw-   0        0        0     1613 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/__main__.py
--rw-rw-rw-   0        0        0     1028 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/_schemas.py
--rw-rw-rw-   0        0        0     3617 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/automerging.py
--rw-rw-rw-   0        0        0     4831 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/merges.py
--rw-rw-rw-   0        0        0     5177 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/metrics.py
--rw-rw-rw-   0        0        0    10898 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/spike_ISI.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.430503 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/depth_estimation/
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/depth_estimation/__init__.py
--rw-rw-rw-   0        0        0     2492 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/depth_estimation/__main__.py
--rw-rw-rw-   0        0        0     2692 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/depth_estimation/_schemas.py
--rw-rw-rw-   0        0        0     6777 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/depth_estimation/depth_estimation.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.436502 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/extract_from_npx/
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/extract_from_npx/__init__.py
--rw-rw-rw-   0        0        0     2312 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/extract_from_npx/__main__.py
--rw-rw-rw-   0        0        0     1311 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/extract_from_npx/_schemas.py
--rw-rw-rw-   0        0        0     2206 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/extract_from_npx/create_settings_json.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.442503 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_helper/
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_helper/__init__.py
--rw-rw-rw-   0        0        0     5504 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_helper/__main__.py
--rw-rw-rw-   0        0        0     7454 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_helper/_schemas.py
--rw-rw-rw-   0        0        0     9878 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_helper/matlab_file_generator.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.448503 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_postprocessing/
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_postprocessing/__init__.py
--rw-rw-rw-   0        0        0     3601 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_postprocessing/__main__.py
--rw-rw-rw-   0        0        0     1259 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_postprocessing/_schemas.py
--rw-rw-rw-   0        0        0     9270 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_postprocessing/postprocessing.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.455504 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/mean_waveforms/
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/mean_waveforms/__init__.py
--rw-rw-rw-   0        0        0     2283 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/mean_waveforms/__main__.py
--rw-rw-rw-   0        0        0     1762 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/mean_waveforms/_schemas.py
--rw-rw-rw-   0        0        0     7817 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/mean_waveforms/extract_waveforms.py
--rw-rw-rw-   0        0        0    12878 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/mean_waveforms/waveform_metrics.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.460505 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/median_subtraction/
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/median_subtraction/__init__.py
--rw-rw-rw-   0        0        0     1787 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/median_subtraction/__main__.py
--rw-rw-rw-   0        0        0     1187 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/median_subtraction/_schemas.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.469502 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/noise_templates/
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/noise_templates/__init__.py
--rw-rw-rw-   0        0        0     1841 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/noise_templates/__main__.py
--rw-rw-rw-   0        0        0     2909 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/noise_templates/_schemas.py
--rw-rw-rw-   0        0        0    11173 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/noise_templates/id_noise_templates.py
--rw-rw-rw-   0        0        0     9701 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/noise_templates/template_classifier_app.py
--rw-rw-rw-   0        0        0     4575 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/noise_templates/train_classifier.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.475506 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/quality_metrics/
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/quality_metrics/__init__.py
--rw-rw-rw-   0        0        0     3047 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/quality_metrics/__main__.py
--rw-rw-rw-   0        0        0     2258 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/quality_metrics/_schemas.py
--rw-rw-rw-   0        0        0    32978 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/quality_metrics/metrics.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.493503 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/__init__.py
--rw-rw-rw-   0        0        0      578 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_plotting.py
--rw-rw-rw-   0        0        0     1010 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing.py
--rw-rw-rw-   0        0        0     2505 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_320rack.py
--rw-rw-rw-   0        0        0     2091 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_NP0.py
--rw-rw-rw-   0        0        0     3900 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_NP0_ks.py
--rw-rw-rw-   0        0        0    38088 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_gui.py
--rw-rw-rw-   0        0        0    36369 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_parallel.py
--rw-rw-rw-   0        0        0    36372 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_parallel_extract_from_network.py
--rw-rw-rw-   0        0        0     3180 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_serial.py
--rw-rw-rw-   0        0        0     7786 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/create_input_json.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.499503 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/helpers/
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/helpers/__init__.py
--rw-rw-rw-   0        0        0    15435 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/helpers/check_data_processing.py
--rw-rw-rw-   0        0        0     1512 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/helpers/plot_raw_data.py
--rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/helpers/processing.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.508504 forked_ecephys_spike_sorting-0.1.0/forked_ecephys_spike_sorting.egg-info/
--rw-rw-rw-   0        0        0      446 2023-08-01 21:51:54.000000 forked_ecephys_spike_sorting-0.1.0/forked_ecephys_spike_sorting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5084 2023-08-01 21:51:54.000000 forked_ecephys_spike_sorting-0.1.0/forked_ecephys_spike_sorting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 21:51:54.000000 forked_ecephys_spike_sorting-0.1.0/forked_ecephys_spike_sorting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      737 2023-08-01 21:51:54.000000 forked_ecephys_spike_sorting-0.1.0/forked_ecephys_spike_sorting.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-08-01 21:51:54.000000 forked_ecephys_spike_sorting-0.1.0/forked_ecephys_spike_sorting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-08-01 21:51:54.000000 forked_ecephys_spike_sorting-0.1.0/forked_ecephys_spike_sorting.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       99 2023-08-01 21:49:10.000000 forked_ecephys_spike_sorting-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0      102 2023-08-01 21:51:55.525504 forked_ecephys_spike_sorting-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1736 2023-08-01 21:45:23.000000 forked_ecephys_spike_sorting-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.509504 forked_ecephys_spike_sorting-0.1.0/tests/
--rw-rw-rw-   0        0        0      275 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.511501 forked_ecephys_spike_sorting-0.1.0/tests/integration/
--rw-rw-rw-   0        0        0      275 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/tests/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.365502 forked_ecephys_spike_sorting-0.1.0/tests/unit/
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.512500 forked_ecephys_spike_sorting-0.1.0/tests/unit/common/
--rw-rw-rw-   0        0        0     1221 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/tests/unit/common/test_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.368502 forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.514501 forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/automerging/
--rw-rw-rw-   0        0        0      737 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/automerging/test_automerging.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.515502 forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/depth_estimation/
--rw-rw-rw-   0        0        0     1557 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/depth_estimation/test_depth_estimation.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.517503 forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/extract_from_npx/
--rw-rw-rw-   0        0        0      415 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/extract_from_npx/test_extract_from_npx.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.519504 forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/mean_waveforms/
--rw-rw-rw-   0        0        0     1098 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/mean_waveforms/test_mean_waveforms.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.520506 forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/noise_templates/
--rw-rw-rw-   0        0        0      759 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/noise_templates/test_noise_templates.py
-drwxrwxrwx   0        0        0        0 2023-08-01 21:51:55.522502 forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/quality_metrics/
--rw-rw-rw-   0        0        0     1059 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/quality_metrics/test_quality_metrics.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.666119 forked_ecephys_spike_sorting-0.1.1/
+-rw-rw-rw-   0        0        0      327 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0       69 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1996 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      316 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      446 2023-08-01 22:52:38.666119 forked_ecephys_spike_sorting-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5828 2023-08-01 21:51:37.000000 forked_ecephys_spike_sorting-0.1.1/README.md
+-rw-rw-rw-   0        0        0       56 2023-08-01 21:45:23.000000 forked_ecephys_spike_sorting-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.535119 forked_ecephys_spike_sorting-0.1.1/docs/
+-rw-rw-rw-   0        0        0     7156 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.494118 forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.495118 forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.494118 forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/external_assets/
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.545120 forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/external_assets/images/
+-rw-rw-rw-   0        0        0       58 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/external_assets/images/arrow_off.gif
+-rw-rw-rw-   0        0        0       58 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/external_assets/images/arrow_on.gif
+-rw-rw-rw-   0        0        0       58 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/external_assets/images/arrow_over.gif
+-rw-rw-rw-   0        0        0    17447 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/external_assets/images/logo_AIBS.gif
+-rw-rw-rw-   0        0        0     8238 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/external_assets/images/progress_indicator.gif
+-rw-rw-rw-   0        0        0      351 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/external_assets/images/tab_blue.gif
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.548119 forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/style/
+-rw-rw-rw-   0        0        0      401 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/style/comment.png
+-rw-rw-rw-   0        0        0      415 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/style/nocomment.png
+-rw-rw-rw-   0        0        0       29 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/authors.rst
+-rw-rw-rw-   0        0        0     9531 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0       29 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/history.rst
+-rw-rw-rw-   0        0        0      365 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/index.rst
+-rw-rw-rw-   0        0        0      269 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/installation.rst
+-rwxrwxrwx   0        0        0     6731 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/make.bat
+-rw-rw-rw-   0        0        0       53 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/readme.rst
+-rw-rw-rw-   0        0        0      109 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.550119 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.558119 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/common/
+-rw-rw-rw-   0        0        0     2486 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/common/OEFileInfo.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/common/__init__.py
+-rw-rw-rw-   0        0        0     2620 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/common/epoch.py
+-rw-rw-rw-   0        0        0     2076 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/common/schemas.py
+-rw-rw-rw-   0        0        0    13330 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/common/utils.py
+-rw-rw-rw-   0        0        0    12514 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/common/visualization.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.560119 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.570119 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/__init__.py
+-rw-rw-rw-   0        0        0     1613 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/__main__.py
+-rw-rw-rw-   0        0        0     1028 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/_schemas.py
+-rw-rw-rw-   0        0        0     3617 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/automerging.py
+-rw-rw-rw-   0        0        0     4831 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/merges.py
+-rw-rw-rw-   0        0        0     5177 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/metrics.py
+-rw-rw-rw-   0        0        0    10898 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/spike_ISI.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.576122 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/depth_estimation/
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/depth_estimation/__init__.py
+-rw-rw-rw-   0        0        0     2492 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/depth_estimation/__main__.py
+-rw-rw-rw-   0        0        0     2692 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/depth_estimation/_schemas.py
+-rw-rw-rw-   0        0        0     6777 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/depth_estimation/depth_estimation.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.583119 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/extract_from_npx/
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/extract_from_npx/__init__.py
+-rw-rw-rw-   0        0        0     2312 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/extract_from_npx/__main__.py
+-rw-rw-rw-   0        0        0     1311 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/extract_from_npx/_schemas.py
+-rw-rw-rw-   0        0        0     2206 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/extract_from_npx/create_settings_json.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.589119 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_helper/
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_helper/__init__.py
+-rw-rw-rw-   0        0        0     5504 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_helper/__main__.py
+-rw-rw-rw-   0        0        0     7454 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_helper/_schemas.py
+-rw-rw-rw-   0        0        0     9878 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_helper/matlab_file_generator.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.595120 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_postprocessing/
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     3601 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_postprocessing/__main__.py
+-rw-rw-rw-   0        0        0     1259 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_postprocessing/_schemas.py
+-rw-rw-rw-   0        0        0     9270 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_postprocessing/postprocessing.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.602119 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/mean_waveforms/
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/mean_waveforms/__init__.py
+-rw-rw-rw-   0        0        0     2283 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/mean_waveforms/__main__.py
+-rw-rw-rw-   0        0        0     1762 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/mean_waveforms/_schemas.py
+-rw-rw-rw-   0        0        0     7817 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/mean_waveforms/extract_waveforms.py
+-rw-rw-rw-   0        0        0    12878 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/mean_waveforms/waveform_metrics.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.606119 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/median_subtraction/
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/median_subtraction/__init__.py
+-rw-rw-rw-   0        0        0     1787 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/median_subtraction/__main__.py
+-rw-rw-rw-   0        0        0     1187 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/median_subtraction/_schemas.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.614119 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/noise_templates/
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/noise_templates/__init__.py
+-rw-rw-rw-   0        0        0     1841 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/noise_templates/__main__.py
+-rw-rw-rw-   0        0        0     2909 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/noise_templates/_schemas.py
+-rw-rw-rw-   0        0        0    11173 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/noise_templates/id_noise_templates.py
+-rw-rw-rw-   0        0        0     9701 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/noise_templates/template_classifier_app.py
+-rw-rw-rw-   0        0        0     4575 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/noise_templates/train_classifier.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.620119 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/quality_metrics/
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/quality_metrics/__init__.py
+-rw-rw-rw-   0        0        0     3047 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/quality_metrics/__main__.py
+-rw-rw-rw-   0        0        0     2258 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/quality_metrics/_schemas.py
+-rw-rw-rw-   0        0        0    32978 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/quality_metrics/metrics.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.637119 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/__init__.py
+-rw-rw-rw-   0        0        0      578 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_plotting.py
+-rw-rw-rw-   0        0        0     1010 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing.py
+-rw-rw-rw-   0        0        0     2505 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_320rack.py
+-rw-rw-rw-   0        0        0     2091 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_NP0.py
+-rw-rw-rw-   0        0        0     3900 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_NP0_ks.py
+-rw-rw-rw-   0        0        0    38088 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_gui.py
+-rw-rw-rw-   0        0        0    36369 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_parallel.py
+-rw-rw-rw-   0        0        0    36372 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_parallel_extract_from_network.py
+-rw-rw-rw-   0        0        0     3180 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_serial.py
+-rw-rw-rw-   0        0        0     7786 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/create_input_json.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.643119 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/helpers/
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/helpers/__init__.py
+-rw-rw-rw-   0        0        0    15435 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/helpers/check_data_processing.py
+-rw-rw-rw-   0        0        0     1512 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/helpers/plot_raw_data.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/helpers/processing.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.652119 forked_ecephys_spike_sorting-0.1.1/forked_ecephys_spike_sorting.egg-info/
+-rw-rw-rw-   0        0        0      446 2023-08-01 22:52:38.000000 forked_ecephys_spike_sorting-0.1.1/forked_ecephys_spike_sorting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5084 2023-08-01 22:52:38.000000 forked_ecephys_spike_sorting-0.1.1/forked_ecephys_spike_sorting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 22:52:38.000000 forked_ecephys_spike_sorting-0.1.1/forked_ecephys_spike_sorting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      737 2023-08-01 22:52:38.000000 forked_ecephys_spike_sorting-0.1.1/forked_ecephys_spike_sorting.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-08-01 22:52:38.000000 forked_ecephys_spike_sorting-0.1.1/forked_ecephys_spike_sorting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-08-01 22:52:38.000000 forked_ecephys_spike_sorting-0.1.1/forked_ecephys_spike_sorting.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       99 2023-08-01 21:49:10.000000 forked_ecephys_spike_sorting-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0      102 2023-08-01 22:52:38.667118 forked_ecephys_spike_sorting-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1753 2023-08-01 22:52:37.000000 forked_ecephys_spike_sorting-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.654119 forked_ecephys_spike_sorting-0.1.1/tests/
+-rw-rw-rw-   0        0        0      275 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.655119 forked_ecephys_spike_sorting-0.1.1/tests/integration/
+-rw-rw-rw-   0        0        0      275 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/tests/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.505120 forked_ecephys_spike_sorting-0.1.1/tests/unit/
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.656119 forked_ecephys_spike_sorting-0.1.1/tests/unit/common/
+-rw-rw-rw-   0        0        0     1221 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/tests/unit/common/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.508120 forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.658119 forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/automerging/
+-rw-rw-rw-   0        0        0      737 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/automerging/test_automerging.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.659119 forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/depth_estimation/
+-rw-rw-rw-   0        0        0     1557 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/depth_estimation/test_depth_estimation.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.661119 forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/extract_from_npx/
+-rw-rw-rw-   0        0        0      415 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/extract_from_npx/test_extract_from_npx.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.662119 forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/mean_waveforms/
+-rw-rw-rw-   0        0        0     1098 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/mean_waveforms/test_mean_waveforms.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.663119 forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/noise_templates/
+-rw-rw-rw-   0        0        0      759 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/noise_templates/test_noise_templates.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:52:38.665119 forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/quality_metrics/
+-rw-rw-rw-   0        0        0     1059 2023-08-01 21:37:33.000000 forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/quality_metrics/test_quality_metrics.py
```

### Comparing `forked_ecephys_spike_sorting-0.1.0/LICENSE.txt` & `forked_ecephys_spike_sorting-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/README.md` & `forked_ecephys_spike_sorting-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/docs/Makefile` & `forked_ecephys_spike_sorting-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/external_assets/images/logo_AIBS.gif` & `forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/external_assets/images/logo_AIBS.gif`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/docs/aibs_sphinx/static/external_assets/images/progress_indicator.gif` & `forked_ecephys_spike_sorting-0.1.1/docs/aibs_sphinx/static/external_assets/images/progress_indicator.gif`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/docs/conf.py` & `forked_ecephys_spike_sorting-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/docs/make.bat` & `forked_ecephys_spike_sorting-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/common/OEFileInfo.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/common/OEFileInfo.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/common/epoch.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/common/epoch.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/common/schemas.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/common/schemas.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/common/utils.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/common/utils.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/common/visualization.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/common/visualization.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/__main__.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/__main__.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/_schemas.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/_schemas.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/automerging.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/automerging.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/merges.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/merges.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/metrics.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/metrics.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/automerging/spike_ISI.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/automerging/spike_ISI.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/depth_estimation/__main__.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/depth_estimation/__main__.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/depth_estimation/_schemas.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/depth_estimation/_schemas.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/depth_estimation/depth_estimation.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/depth_estimation/depth_estimation.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/extract_from_npx/__main__.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/extract_from_npx/__main__.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/extract_from_npx/_schemas.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/extract_from_npx/_schemas.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/extract_from_npx/create_settings_json.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/extract_from_npx/create_settings_json.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_helper/__main__.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_helper/__main__.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_helper/_schemas.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_helper/_schemas.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_helper/matlab_file_generator.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_helper/matlab_file_generator.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_postprocessing/__main__.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_postprocessing/__main__.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_postprocessing/_schemas.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_postprocessing/_schemas.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/kilosort_postprocessing/postprocessing.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/kilosort_postprocessing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/mean_waveforms/__main__.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/mean_waveforms/__main__.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/mean_waveforms/_schemas.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/mean_waveforms/_schemas.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/mean_waveforms/extract_waveforms.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/mean_waveforms/extract_waveforms.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/mean_waveforms/waveform_metrics.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/mean_waveforms/waveform_metrics.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/median_subtraction/__main__.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/median_subtraction/__main__.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/median_subtraction/_schemas.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/median_subtraction/_schemas.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/noise_templates/__main__.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/noise_templates/__main__.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/noise_templates/_schemas.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/noise_templates/_schemas.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/noise_templates/id_noise_templates.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/noise_templates/id_noise_templates.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/noise_templates/template_classifier_app.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/noise_templates/template_classifier_app.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/noise_templates/train_classifier.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/noise_templates/train_classifier.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/quality_metrics/__main__.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/quality_metrics/__main__.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/quality_metrics/_schemas.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/quality_metrics/_schemas.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/modules/quality_metrics/metrics.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/modules/quality_metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_plotting.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_plotting.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_320rack.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_320rack.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_NP0.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_NP0.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_NP0_ks.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_NP0_ks.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_gui.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_gui.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_parallel.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_parallel.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_parallel_extract_from_network.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_parallel_extract_from_network.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/batch_processing_serial.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/batch_processing_serial.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/create_input_json.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/create_input_json.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/helpers/check_data_processing.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/helpers/check_data_processing.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/ecephys_spike_sorting/scripts/helpers/plot_raw_data.py` & `forked_ecephys_spike_sorting-0.1.1/ecephys_spike_sorting/scripts/helpers/plot_raw_data.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/forked_ecephys_spike_sorting.egg-info/SOURCES.txt` & `forked_ecephys_spike_sorting-0.1.1/forked_ecephys_spike_sorting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/forked_ecephys_spike_sorting.egg-info/entry_points.txt` & `forked_ecephys_spike_sorting-0.1.1/forked_ecephys_spike_sorting.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/setup.py` & `forked_ecephys_spike_sorting-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'forked_ecephys_spike_sorting',
-    version = '0.1.0',
+    version = '0.1.1',
     description = """Tools for spike-sorting Allen Institute Neuropixels data""",
     author = "Josh Siegle, Nile Graddis, Xiaoxuan Jia, Gregg Heller, Chris Mochizuki, Dan Denman",
     author_email = "joshs@alleninstitute.org",
     url = 'https://github.com/AllenInstitute/ecephys_spike_sorting',
     packages = find_packages(),
     include_package_data=True,
     entry_points={
@@ -30,10 +30,11 @@
         'pandas',
         'GitPython',
         'pillow',
         'argschema',
         'xmljson',
         'xarray',
         'scikit-learn',
+        'h5py',
         'joblib'
     ],
 )
```

### Comparing `forked_ecephys_spike_sorting-0.1.0/tests/unit/common/test_utils.py` & `forked_ecephys_spike_sorting-0.1.1/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/automerging/test_automerging.py` & `forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/automerging/test_automerging.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/depth_estimation/test_depth_estimation.py` & `forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/depth_estimation/test_depth_estimation.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/mean_waveforms/test_mean_waveforms.py` & `forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/mean_waveforms/test_mean_waveforms.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/noise_templates/test_noise_templates.py` & `forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/noise_templates/test_noise_templates.py`

 * *Files identical despite different names*

### Comparing `forked_ecephys_spike_sorting-0.1.0/tests/unit/modules/quality_metrics/test_quality_metrics.py` & `forked_ecephys_spike_sorting-0.1.1/tests/unit/modules/quality_metrics/test_quality_metrics.py`

 * *Files identical despite different names*

