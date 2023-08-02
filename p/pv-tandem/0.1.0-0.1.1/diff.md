# Comparing `tmp/pv_tandem-0.1.0.tar.gz` & `tmp/pv_tandem-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pv_tandem-0.1.0.tar", last modified: Wed Jul 26 16:00:33 2023, max compression
+gzip compressed data, was "pv_tandem-0.1.1.tar", last modified: Wed Aug  2 16:05:02 2023, max compression
```

## Comparing `pv_tandem-0.1.0.tar` & `pv_tandem-0.1.1.tar`

### file list

```diff
@@ -1,117 +1,149 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 16:00:33.212174 pv_tandem-0.1.0/
--rw-rw-rw-   0        0        0      187 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3666 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1095 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      273 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2703 2023-07-26 16:00:33.212697 pv_tandem-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1733 2023-07-18 09:21:10.000000 pv_tandem-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 16:00:33.042760 pv_tandem-0.1.0/docs/
--rw-rw-rw-   0        0        0      630 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-07-26 16:00:32.982653 pv_tandem-0.1.0/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-07-26 16:00:32.982653 pv_tandem-0.1.0/docs/_build/html/
-drwxrwxrwx   0        0        0        0 2023-07-26 16:00:33.084550 pv_tandem-0.1.0/docs/_build/html/_images/
--rw-rw-rw-   0        0        0    26794 2023-07-26 13:09:51.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_lambertw_num_testing_thumb.png
--rw-rw-rw-   0        0        0    48268 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_001.png
--rw-rw-rw-   0        0        0    59501 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_002.png
--rw-rw-rw-   0        0        0    70269 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_003.png
--rw-rw-rw-   0        0        0    19083 2023-07-26 13:09:56.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_thumb.png
--rw-rw-rw-   0        0        0    89480 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_energy_yield_001.png
--rw-rw-rw-   0        0        0    35293 2023-07-26 13:10:17.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_energy_yield_thumb.png
--rw-rw-rw-   0        0        0   138205 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_001.png
--rw-rw-rw-   0        0        0    50200 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_002.png
--rw-rw-rw-   0        0        0    25448 2023-07-26 13:09:55.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_thumb.png
--rw-rw-rw-   0        0        0    47237 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_001.png
--rw-rw-rw-   0        0        0    47465 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_002.png
--rw-rw-rw-   0        0        0   133534 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_003.png
--rw-rw-rw-   0        0        0    54772 2023-07-26 13:09:51.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_thumb.png
--rw-rw-rw-   0        0        0    44667 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_2t_stc_001.png
--rw-rw-rw-   0        0        0    23041 2023-07-26 13:09:49.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_2t_stc_thumb.png
--rw-rw-rw-   0        0        0    39811 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_4t_stc_001.png
--rw-rw-rw-   0        0        0    18756 2023-07-26 13:09:49.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_4t_stc_thumb.png
--rw-rw-rw-   0        0        0   107962 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_ey_001.png
--rw-rw-rw-   0        0        0    46713 2023-07-26 13:11:03.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_ey_thumb.png
--rw-rw-rw-   0        0        0    43973 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_optim_bg_stc_001.png
--rw-rw-rw-   0        0        0    18056 2023-07-26 13:09:55.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_optim_bg_stc_thumb.png
--rw-rw-rw-   0        0        0    59111 2023-07-26 13:11:04.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_temp_vs_irrad_001.png
--rw-rw-rw-   0        0        0    37091 2023-07-26 13:09:50.000000 pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_temp_vs_irrad_thumb.png
-drwxrwxrwx   0        0        0        0 2023-07-26 16:00:33.094713 pv_tandem-0.1.0/docs/_build/html/_static/
--rw-rw-rw-   0        0        0    21404 2023-07-10 15:32:05.000000 pv_tandem-0.1.0/docs/_build/html/_static/broken_example.png
--rw-rw-rw-   0        0        0      286 2023-05-12 22:36:26.000000 pv_tandem-0.1.0/docs/_build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-05-12 22:36:26.000000 pv_tandem-0.1.0/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0     4315 2023-07-10 15:32:05.000000 pv_tandem-0.1.0/docs/_build/html/_static/no_image.png
--rw-rw-rw-   0        0        0       90 2023-05-12 22:36:26.000000 pv_tandem-0.1.0/docs/_build/html/_static/plus.png
--rw-rw-rw-   0        0        0     1929 2023-07-18 14:39:44.000000 pv_tandem-0.1.0/docs/_build/html/_static/tandem.png
-drwxrwxrwx   0        0        0        0 2023-07-26 16:00:33.102854 pv_tandem-0.1.0/docs/_static/
--rw-rw-rw-   0        0        0     1929 2023-07-18 14:39:44.000000 pv_tandem-0.1.0/docs/_static/tandem.png
--rw-rw-rw-   0        0        0      238 2023-05-22 15:34:10.000000 pv_tandem-0.1.0/docs/api.rst
--rw-rw-rw-   0        0        0       29 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/docs/authors.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 16:00:33.124603 pv_tandem-0.1.0/docs/auto_examples/
-drwxrwxrwx   0        0        0        0 2023-07-26 16:00:33.152661 pv_tandem-0.1.0/docs/auto_examples/images/
--rw-rw-rw-   0        0        0    48268 2023-07-26 13:09:55.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_bifacial_basics_001.png
--rw-rw-rw-   0        0        0    59501 2023-07-26 13:09:56.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_bifacial_basics_002.png
--rw-rw-rw-   0        0        0    70269 2023-07-26 13:09:56.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_bifacial_basics_003.png
--rw-rw-rw-   0        0        0    89480 2023-07-26 13:10:17.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_bifacial_energy_yield_001.png
--rw-rw-rw-   0        0        0   138205 2023-07-26 13:09:55.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_bifacial_irradiance_yield_001.png
--rw-rw-rw-   0        0        0    50200 2023-07-26 13:09:55.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_bifacial_irradiance_yield_002.png
--rw-rw-rw-   0        0        0    47237 2023-07-26 13:09:50.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_jph_from_spec_001.png
--rw-rw-rw-   0        0        0    47465 2023-07-26 13:09:51.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_jph_from_spec_002.png
--rw-rw-rw-   0        0        0   133534 2023-07-26 13:09:51.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_jph_from_spec_003.png
--rw-rw-rw-   0        0        0    44667 2023-07-26 13:09:49.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_tandem_2t_stc_001.png
--rw-rw-rw-   0        0        0    39811 2023-07-26 13:09:49.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_tandem_4t_stc_001.png
--rw-rw-rw-   0        0        0   107962 2023-07-26 13:11:03.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_tandem_ey_001.png
--rw-rw-rw-   0        0        0    43973 2023-07-26 13:09:55.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_tandem_optim_bg_stc_001.png
--rw-rw-rw-   0        0        0    59111 2023-07-26 13:09:50.000000 pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_temp_vs_irrad_001.png
-drwxrwxrwx   0        0        0        0 2023-07-26 16:00:33.164757 pv_tandem-0.1.0/docs/auto_examples/images/thumb/
--rw-rw-rw-   0        0        0    26794 2023-07-26 13:09:51.000000 pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_lambertw_num_testing_thumb.png
--rw-rw-rw-   0        0        0    19083 2023-07-26 13:09:56.000000 pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_bifacial_basics_thumb.png
--rw-rw-rw-   0        0        0    35293 2023-07-26 13:10:17.000000 pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_bifacial_energy_yield_thumb.png
--rw-rw-rw-   0        0        0    25448 2023-07-26 13:09:55.000000 pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_bifacial_irradiance_yield_thumb.png
--rw-rw-rw-   0        0        0    54772 2023-07-26 13:09:51.000000 pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_jph_from_spec_thumb.png
--rw-rw-rw-   0        0        0    23041 2023-07-26 13:09:49.000000 pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_tandem_2t_stc_thumb.png
--rw-rw-rw-   0        0        0    18756 2023-07-26 13:09:49.000000 pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_tandem_4t_stc_thumb.png
--rw-rw-rw-   0        0        0    46713 2023-07-26 13:11:03.000000 pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_tandem_ey_thumb.png
--rw-rw-rw-   0        0        0    18056 2023-07-26 13:09:55.000000 pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_tandem_optim_bg_stc_thumb.png
--rw-rw-rw-   0        0        0    37091 2023-07-26 13:09:50.000000 pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_temp_vs_irrad_thumb.png
--rw-rw-rw-   0        0        0     5099 2023-07-26 13:10:17.000000 pv_tandem-0.1.0/docs/auto_examples/index.rst
--rw-rw-rw-   0        0        0     4771 2023-07-26 13:09:51.000000 pv_tandem-0.1.0/docs/auto_examples/lambertw_num_testing.rst
--rw-rw-rw-   0        0        0     8101 2023-07-26 13:09:56.000000 pv_tandem-0.1.0/docs/auto_examples/plot_bifacial_basics.rst
--rw-rw-rw-   0        0        0     8349 2023-07-26 13:10:17.000000 pv_tandem-0.1.0/docs/auto_examples/plot_bifacial_energy_yield.rst
--rw-rw-rw-   0        0        0     4967 2023-07-26 13:09:55.000000 pv_tandem-0.1.0/docs/auto_examples/plot_bifacial_irradiance_yield.rst
--rw-rw-rw-   0        0        0     5767 2023-07-26 13:09:51.000000 pv_tandem-0.1.0/docs/auto_examples/plot_jph_from_spec.rst
--rw-rw-rw-   0        0        0     4023 2023-07-26 13:09:49.000000 pv_tandem-0.1.0/docs/auto_examples/plot_tandem_2t_stc.rst
--rw-rw-rw-   0        0        0     4026 2023-07-26 13:09:49.000000 pv_tandem-0.1.0/docs/auto_examples/plot_tandem_4t_stc.rst
--rw-rw-rw-   0        0        0     4890 2023-07-26 13:11:03.000000 pv_tandem-0.1.0/docs/auto_examples/plot_tandem_ey.rst
--rw-rw-rw-   0        0        0     5796 2023-07-26 13:09:55.000000 pv_tandem-0.1.0/docs/auto_examples/plot_tandem_optim_bg_stc.rst
--rw-rw-rw-   0        0        0     4735 2023-07-26 13:09:50.000000 pv_tandem-0.1.0/docs/auto_examples/plot_temp_vs_irrad.rst
--rw-rw-rw-   0        0        0     2870 2023-07-26 13:11:03.000000 pv_tandem-0.1.0/docs/auto_examples/sg_execution_times.rst
--rw-rw-rw-   0        0        0     5857 2023-07-18 14:47:57.000000 pv_tandem-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/docs/history.rst
--rw-rw-rw-   0        0        0      379 2023-07-18 09:21:10.000000 pv_tandem-0.1.0/docs/index.rst
--rw-rw-rw-   0        0        0     1189 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/docs/installation.rst
--rwxrwxrwx   0        0        0      807 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/docs/make.bat
--rw-rw-rw-   0        0        0     3429 2023-07-19 15:50:23.000000 pv_tandem-0.1.0/docs/model_basics.rst
--rw-rw-rw-   0        0        0       28 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/docs/readme.rst
--rw-rw-rw-   0        0        0       80 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 16:00:33.192526 pv_tandem-0.1.0/pv_tandem/
--rw-rw-rw-   0        0        0      358 2023-07-10 15:24:07.000000 pv_tandem-0.1.0/pv_tandem/__init__.py
--rw-rw-rw-   0        0        0    23820 2023-07-10 15:24:07.000000 pv_tandem-0.1.0/pv_tandem/bifacial_geo.py
--rw-rw-rw-   0        0        0     6012 2023-07-10 15:24:07.000000 pv_tandem-0.1.0/pv_tandem/bifacial_yield.py
--rw-rw-rw-   0        0        0     6710 2023-07-18 14:44:33.000000 pv_tandem-0.1.0/pv_tandem/electrical_models.py
--rw-rw-rw-   0        0        0     1778 2023-05-16 09:13:12.000000 pv_tandem-0.1.0/pv_tandem/irradiance_models.py
--rw-rw-rw-   0        0        0     1345 2023-05-10 13:08:33.000000 pv_tandem-0.1.0/pv_tandem/local_scripts.py
--rw-rw-rw-   0        0        0    33806 2023-07-18 09:21:10.000000 pv_tandem-0.1.0/pv_tandem/solarcell_models.py
--rw-rw-rw-   0        0        0     5838 2023-07-10 15:24:07.000000 pv_tandem-0.1.0/pv_tandem/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:00:33.205031 pv_tandem-0.1.0/pv_tandem.egg-info/
--rw-rw-rw-   0        0        0     2703 2023-07-26 16:00:32.000000 pv_tandem-0.1.0/pv_tandem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4688 2023-07-26 16:00:32.000000 pv_tandem-0.1.0/pv_tandem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 16:00:32.000000 pv_tandem-0.1.0/pv_tandem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-26 15:31:52.000000 pv_tandem-0.1.0/pv_tandem.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      301 2023-07-26 16:00:32.000000 pv_tandem-0.1.0/pv_tandem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-26 16:00:32.000000 pv_tandem-0.1.0/pv_tandem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      452 2023-07-26 16:00:33.212697 pv_tandem-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1755 2023-07-26 15:16:34.000000 pv_tandem-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:00:33.205031 pv_tandem-0.1.0/tests/
--rw-rw-rw-   0        0        0       40 2023-05-03 11:41:06.000000 pv_tandem-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1141 2023-05-09 09:22:31.000000 pv_tandem-0.1.0/tests/test_pv_tandem.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.173796 pv_tandem-0.1.1/
+-rw-rw-rw-   0        0        0      187 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3666 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1095 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3004 2023-08-02 16:05:02.174797 pv_tandem-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2034 2023-08-02 15:31:52.000000 pv_tandem-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:01.949178 pv_tandem-0.1.1/docs/
+-rw-rw-rw-   0        0        0      630 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:01.887133 pv_tandem-0.1.1/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:01.885999 pv_tandem-0.1.1/docs/_build/html/
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:01.884034 pv_tandem-0.1.1/docs/_build/html/_downloads/
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:01.951178 pv_tandem-0.1.1/docs/_build/html/_downloads/0686a03da72ef988337b900e8aa209e5/
+-rw-rw-rw-   0        0        0    48086 2023-08-02 15:32:37.000000 pv_tandem-0.1.1/docs/_build/html/_downloads/0686a03da72ef988337b900e8aa209e5/one-diode.hires.png
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:01.953178 pv_tandem-0.1.1/docs/_build/html/_downloads/ee2294afa81cddfca0cc7ca7c9fffed2/
+-rw-rw-rw-   0        0        0    14922 2023-08-02 15:32:37.000000 pv_tandem-0.1.1/docs/_build/html/_downloads/ee2294afa81cddfca0cc7ca7c9fffed2/one-diode.png
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.016929 pv_tandem-0.1.1/docs/_build/html/_images/
+-rw-rw-rw-   0        0        0    73339 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/_build/html/_images/irrad_vs_Jsc.png
+-rw-rw-rw-   0        0        0   599599 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/_build/html/_images/logo.png
+-rw-rw-rw-   0        0        0    14922 2023-08-02 15:32:37.000000 pv_tandem-0.1.1/docs/_build/html/_images/one-diode.png
+-rw-rw-rw-   0        0        0    48268 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_001.png
+-rw-rw-rw-   0        0        0    59501 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_002.png
+-rw-rw-rw-   0        0        0    70269 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_003.png
+-rw-rw-rw-   0        0        0    19083 2023-08-02 15:32:14.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_thumb.png
+-rw-rw-rw-   0        0        0    89480 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_energy_yield_001.png
+-rw-rw-rw-   0        0        0    35293 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_energy_yield_thumb.png
+-rw-rw-rw-   0        0        0   138205 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_001.png
+-rw-rw-rw-   0        0        0    50200 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_002.png
+-rw-rw-rw-   0        0        0    25448 2023-08-02 15:32:13.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_thumb.png
+-rw-rw-rw-   0        0        0    47237 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_001.png
+-rw-rw-rw-   0        0        0    47465 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_002.png
+-rw-rw-rw-   0        0        0   133534 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_003.png
+-rw-rw-rw-   0        0        0    54772 2023-08-02 15:32:09.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_thumb.png
+-rw-rw-rw-   0        0        0   110430 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_silicon_ey_001.png
+-rw-rw-rw-   0        0        0    48401 2023-08-02 15:32:14.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_silicon_ey_thumb.png
+-rw-rw-rw-   0        0        0    44667 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_2t_stc_001.png
+-rw-rw-rw-   0        0        0    23041 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_2t_stc_thumb.png
+-rw-rw-rw-   0        0        0    39811 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_4t_stc_001.png
+-rw-rw-rw-   0        0        0    18756 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_4t_stc_thumb.png
+-rw-rw-rw-   0        0        0   107962 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_ey_001.png
+-rw-rw-rw-   0        0        0    46713 2023-08-02 15:32:15.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_ey_thumb.png
+-rw-rw-rw-   0        0        0    43973 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_optim_bg_stc_001.png
+-rw-rw-rw-   0        0        0    18056 2023-08-02 15:32:37.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_optim_bg_stc_thumb.png
+-rw-rw-rw-   0        0        0    59111 2023-08-02 15:32:38.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_temp_vs_irrad_001.png
+-rw-rw-rw-   0        0        0    37091 2023-08-02 15:32:09.000000 pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_temp_vs_irrad_thumb.png
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.029300 pv_tandem-0.1.1/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0    21404 2023-07-10 15:32:05.000000 pv_tandem-0.1.1/docs/_build/html/_static/broken_example.png
+-rw-rw-rw-   0        0        0      286 2023-05-12 22:36:26.000000 pv_tandem-0.1.1/docs/_build/html/_static/file.png
+-rw-rw-rw-   0        0        0    73339 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/_build/html/_static/irrad_vs_Jsc.png
+-rw-rw-rw-   0        0        0       90 2023-05-12 22:36:26.000000 pv_tandem-0.1.1/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0     4315 2023-07-10 15:32:05.000000 pv_tandem-0.1.1/docs/_build/html/_static/no_image.png
+-rw-rw-rw-   0        0        0       90 2023-05-12 22:36:26.000000 pv_tandem-0.1.1/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0     2094 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/_build/html/_static/tandem.png
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:01.887356 pv_tandem-0.1.1/docs/_build/plot_directive/
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.033298 pv_tandem-0.1.1/docs/_build/plot_directive/pyplots/
+-rw-rw-rw-   0        0        0    48086 2023-08-02 15:32:37.000000 pv_tandem-0.1.1/docs/_build/plot_directive/pyplots/one-diode.hires.png
+-rw-rw-rw-   0        0        0    14922 2023-08-02 15:32:37.000000 pv_tandem-0.1.1/docs/_build/plot_directive/pyplots/one-diode.png
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.036641 pv_tandem-0.1.1/docs/_static/
+-rw-rw-rw-   0        0        0    73339 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/_static/irrad_vs_Jsc.png
+-rw-rw-rw-   0        0        0     2094 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/_static/tandem.png
+-rw-rw-rw-   0        0        0      238 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/api.rst
+-rw-rw-rw-   0        0        0       29 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/authors.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.038720 pv_tandem-0.1.1/docs/auto_examples/
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.046889 pv_tandem-0.1.1/docs/auto_examples/basics/
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.054923 pv_tandem-0.1.1/docs/auto_examples/basics/images/
+-rw-rw-rw-   0        0        0    47237 2023-08-02 15:32:09.000000 pv_tandem-0.1.1/docs/auto_examples/basics/images/sphx_glr_plot_jph_from_spec_001.png
+-rw-rw-rw-   0        0        0    47465 2023-08-02 15:32:09.000000 pv_tandem-0.1.1/docs/auto_examples/basics/images/sphx_glr_plot_jph_from_spec_002.png
+-rw-rw-rw-   0        0        0   133534 2023-08-02 15:32:09.000000 pv_tandem-0.1.1/docs/auto_examples/basics/images/sphx_glr_plot_jph_from_spec_003.png
+-rw-rw-rw-   0        0        0    59111 2023-08-02 15:32:09.000000 pv_tandem-0.1.1/docs/auto_examples/basics/images/sphx_glr_plot_temp_vs_irrad_001.png
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.058237 pv_tandem-0.1.1/docs/auto_examples/basics/images/thumb/
+-rw-rw-rw-   0        0        0    54772 2023-08-02 15:32:09.000000 pv_tandem-0.1.1/docs/auto_examples/basics/images/thumb/sphx_glr_plot_jph_from_spec_thumb.png
+-rw-rw-rw-   0        0        0    37091 2023-08-02 15:32:09.000000 pv_tandem-0.1.1/docs/auto_examples/basics/images/thumb/sphx_glr_plot_temp_vs_irrad_thumb.png
+-rw-rw-rw-   0        0        0     1158 2023-08-02 15:32:09.000000 pv_tandem-0.1.1/docs/auto_examples/basics/index.rst
+-rw-rw-rw-   0        0        0     5839 2023-08-02 15:32:09.000000 pv_tandem-0.1.1/docs/auto_examples/basics/plot_jph_from_spec.rst
+-rw-rw-rw-   0        0        0     4777 2023-08-02 15:32:09.000000 pv_tandem-0.1.1/docs/auto_examples/basics/plot_temp_vs_irrad.rst
+-rw-rw-rw-   0        0        0      735 2023-08-02 15:32:09.000000 pv_tandem-0.1.1/docs/auto_examples/basics/sg_execution_times.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.067101 pv_tandem-0.1.1/docs/auto_examples/bifacial/
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.076493 pv_tandem-0.1.1/docs/auto_examples/bifacial/images/
+-rw-rw-rw-   0        0        0    48268 2023-08-02 15:32:13.000000 pv_tandem-0.1.1/docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_001.png
+-rw-rw-rw-   0        0        0    59501 2023-08-02 15:32:14.000000 pv_tandem-0.1.1/docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_002.png
+-rw-rw-rw-   0        0        0    70269 2023-08-02 15:32:14.000000 pv_tandem-0.1.1/docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_003.png
+-rw-rw-rw-   0        0        0   138205 2023-08-02 15:32:13.000000 pv_tandem-0.1.1/docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_irradiance_yield_001.png
+-rw-rw-rw-   0        0        0    50200 2023-08-02 15:32:13.000000 pv_tandem-0.1.1/docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_irradiance_yield_002.png
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.080555 pv_tandem-0.1.1/docs/auto_examples/bifacial/images/thumb/
+-rw-rw-rw-   0        0        0    19083 2023-08-02 15:32:14.000000 pv_tandem-0.1.1/docs/auto_examples/bifacial/images/thumb/sphx_glr_plot_bifacial_basics_thumb.png
+-rw-rw-rw-   0        0        0    25448 2023-08-02 15:32:13.000000 pv_tandem-0.1.1/docs/auto_examples/bifacial/images/thumb/sphx_glr_plot_bifacial_irradiance_yield_thumb.png
+-rw-rw-rw-   0        0        0     1105 2023-08-02 15:32:14.000000 pv_tandem-0.1.1/docs/auto_examples/bifacial/index.rst
+-rw-rw-rw-   0        0        0     8191 2023-08-02 15:32:14.000000 pv_tandem-0.1.1/docs/auto_examples/bifacial/plot_bifacial_basics.rst
+-rw-rw-rw-   0        0        0     5040 2023-08-02 15:32:13.000000 pv_tandem-0.1.1/docs/auto_examples/bifacial/plot_bifacial_irradiance_yield.rst
+-rw-rw-rw-   0        0        0      869 2023-08-02 15:32:14.000000 pv_tandem-0.1.1/docs/auto_examples/bifacial/sg_execution_times.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.089778 pv_tandem-0.1.1/docs/auto_examples/energy_yield/
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.095738 pv_tandem-0.1.1/docs/auto_examples/energy_yield/images/
+-rw-rw-rw-   0        0        0    89480 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/auto_examples/energy_yield/images/sphx_glr_plot_bifacial_energy_yield_001.png
+-rw-rw-rw-   0        0        0   110430 2023-08-02 15:32:14.000000 pv_tandem-0.1.1/docs/auto_examples/energy_yield/images/sphx_glr_plot_silicon_ey_001.png
+-rw-rw-rw-   0        0        0   107962 2023-08-02 15:32:15.000000 pv_tandem-0.1.1/docs/auto_examples/energy_yield/images/sphx_glr_plot_tandem_ey_001.png
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.101006 pv_tandem-0.1.1/docs/auto_examples/energy_yield/images/thumb/
+-rw-rw-rw-   0        0        0    35293 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/auto_examples/energy_yield/images/thumb/sphx_glr_plot_bifacial_energy_yield_thumb.png
+-rw-rw-rw-   0        0        0    48401 2023-08-02 15:32:14.000000 pv_tandem-0.1.1/docs/auto_examples/energy_yield/images/thumb/sphx_glr_plot_silicon_ey_thumb.png
+-rw-rw-rw-   0        0        0    46713 2023-08-02 15:32:15.000000 pv_tandem-0.1.1/docs/auto_examples/energy_yield/images/thumb/sphx_glr_plot_tandem_ey_thumb.png
+-rw-rw-rw-   0        0        0     1591 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/auto_examples/energy_yield/index.rst
+-rw-rw-rw-   0        0        0     8431 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/auto_examples/energy_yield/plot_bifacial_energy_yield.rst
+-rw-rw-rw-   0        0        0     4978 2023-08-02 15:32:14.000000 pv_tandem-0.1.1/docs/auto_examples/energy_yield/plot_silicon_ey.rst
+-rw-rw-rw-   0        0        0     4971 2023-08-02 15:32:15.000000 pv_tandem-0.1.1/docs/auto_examples/energy_yield/plot_tandem_ey.rst
+-rw-rw-rw-   0        0        0     1125 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/auto_examples/energy_yield/sg_execution_times.rst
+-rw-rw-rw-   0        0        0     5599 2023-08-02 15:32:37.000000 pv_tandem-0.1.1/docs/auto_examples/index.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.110306 pv_tandem-0.1.1/docs/auto_examples/stc/
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.116458 pv_tandem-0.1.1/docs/auto_examples/stc/images/
+-rw-rw-rw-   0        0        0    44667 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/auto_examples/stc/images/sphx_glr_plot_tandem_2t_stc_001.png
+-rw-rw-rw-   0        0        0    39811 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/auto_examples/stc/images/sphx_glr_plot_tandem_4t_stc_001.png
+-rw-rw-rw-   0        0        0    43973 2023-08-02 15:32:37.000000 pv_tandem-0.1.1/docs/auto_examples/stc/images/sphx_glr_plot_tandem_optim_bg_stc_001.png
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.121742 pv_tandem-0.1.1/docs/auto_examples/stc/images/thumb/
+-rw-rw-rw-   0        0        0    23041 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/auto_examples/stc/images/thumb/sphx_glr_plot_tandem_2t_stc_thumb.png
+-rw-rw-rw-   0        0        0    18756 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/auto_examples/stc/images/thumb/sphx_glr_plot_tandem_4t_stc_thumb.png
+-rw-rw-rw-   0        0        0    18056 2023-08-02 15:32:37.000000 pv_tandem-0.1.1/docs/auto_examples/stc/images/thumb/sphx_glr_plot_tandem_optim_bg_stc_thumb.png
+-rw-rw-rw-   0        0        0     1490 2023-08-02 15:32:37.000000 pv_tandem-0.1.1/docs/auto_examples/stc/index.rst
+-rw-rw-rw-   0        0        0     4048 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/auto_examples/stc/plot_tandem_2t_stc.rst
+-rw-rw-rw-   0        0        0     4051 2023-08-02 15:32:36.000000 pv_tandem-0.1.1/docs/auto_examples/stc/plot_tandem_4t_stc.rst
+-rw-rw-rw-   0        0        0     5822 2023-08-02 15:32:37.000000 pv_tandem-0.1.1/docs/auto_examples/stc/plot_tandem_optim_bg_stc.rst
+-rw-rw-rw-   0        0        0     1016 2023-08-02 15:32:37.000000 pv_tandem-0.1.1/docs/auto_examples/stc/sg_execution_times.rst
+-rw-rw-rw-   0        0        0     5918 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/history.rst
+-rw-rw-rw-   0        0        0      936 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/index.rst
+-rwxrwxrwx   0        0        0      807 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/make.bat
+-rw-rw-rw-   0        0        0     7057 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/model_basics.rst
+-rw-rw-rw-   0        0        0     1067 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.150911 pv_tandem-0.1.1/pv_tandem/
+-rw-rw-rw-   0        0        0      358 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/pv_tandem/__init__.py
+-rw-rw-rw-   0        0        0    23820 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/pv_tandem/bifacial_geo.py
+-rw-rw-rw-   0        0        0     6012 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/pv_tandem/bifacial_yield.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.165309 pv_tandem-0.1.1/pv_tandem/data/
+-rw-rw-rw-   0        0        0    65546 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/pv_tandem/data/ASTMG173.csv
+-rw-rw-rw-   0        0        0     7023 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/pv_tandem/electrical_models.py
+-rw-rw-rw-   0        0        0     1778 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/pv_tandem/irradiance_models.py
+-rw-rw-rw-   0        0        0    33806 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/pv_tandem/solarcell_models.py
+-rw-rw-rw-   0        0        0     5838 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/pv_tandem/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.163309 pv_tandem-0.1.1/pv_tandem.egg-info/
+-rw-rw-rw-   0        0        0     3004 2023-08-02 16:05:01.000000 pv_tandem-0.1.1/pv_tandem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5798 2023-08-02 16:05:01.000000 pv_tandem-0.1.1/pv_tandem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 16:05:01.000000 pv_tandem-0.1.1/pv_tandem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 16:05:01.000000 pv_tandem-0.1.1/pv_tandem.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      320 2023-08-02 16:05:01.000000 pv_tandem-0.1.1/pv_tandem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-02 16:05:01.000000 pv_tandem-0.1.1/pv_tandem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      452 2023-08-02 16:05:02.175788 pv_tandem-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1832 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:05:02.171787 pv_tandem-0.1.1/tests/
+-rw-rw-rw-   0        0        0       40 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1141 2023-08-02 15:29:03.000000 pv_tandem-0.1.1/tests/test_pv_tandem.py
```

### Comparing `pv_tandem-0.1.0/CONTRIBUTING.rst` & `pv_tandem-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/LICENSE` & `pv_tandem-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/PKG-INFO` & `pv_tandem-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pv_tandem
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python toolbox for simulation and energy yield calculations of tandem solar cells.
 Home-page: https://github.com/nano-sippe/pv_tandem
 Author: Peter Tillmann
 Author-email: Peter.tillmann@helmholtz-berlin.de
 License: MIT license
 Keywords: pv_tandem
 Classifier: Development Status :: 3 - Alpha
@@ -51,17 +51,29 @@
 * Helping tools to process irradiance data for solar cell simulations
 * Electrical modeling with 1-diode model for single junction or tandem solar cells
 * Modeling of illumination in a large PV power plant for the front- and backside of the modules
 
 Where to get it
 ---------------
 
-The source code is hosted at GitHub at: https://github.com/nano-sippe/pv_tandem
+pv_tandem can easily be installed with pip:
 
-To install pv_tandem clone the project from github:
+.. code-block:: bash
+
+    pip install pv_tandem
+
+If you want to be able to directly run the examples you can install pv_tandems together with all nessesary libraries with
+
+.. code-block:: bash
+
+    pip install pv_tandem[doc]
+
+The source code is hosted at GitHub at: https://github.com/HZBSolarOptics/pv_tandem
+
+If you want to install from source clone the project from github:
 
 .. code-block:: bash
 
     git clone https://github.com/nano-sippe/pv_tandem
 
 Then change into the pv_tandem folder and install with pip
```

### Comparing `pv_tandem-0.1.0/README.rst` & `pv_tandem-0.1.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -26,17 +26,29 @@
 * Helping tools to process irradiance data for solar cell simulations
 * Electrical modeling with 1-diode model for single junction or tandem solar cells
 * Modeling of illumination in a large PV power plant for the front- and backside of the modules
 
 Where to get it
 ---------------
 
-The source code is hosted at GitHub at: https://github.com/nano-sippe/pv_tandem
+pv_tandem can easily be installed with pip:
 
-To install pv_tandem clone the project from github:
+.. code-block:: bash
+
+    pip install pv_tandem
+
+If you want to be able to directly run the examples you can install pv_tandems together with all nessesary libraries with
+
+.. code-block:: bash
+
+    pip install pv_tandem[doc]
+
+The source code is hosted at GitHub at: https://github.com/HZBSolarOptics/pv_tandem
+
+If you want to install from source clone the project from github:
 
 .. code-block:: bash
 
     git clone https://github.com/nano-sippe/pv_tandem
 
 Then change into the pv_tandem folder and install with pip
```

### Comparing `pv_tandem-0.1.0/docs/Makefile` & `pv_tandem-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_001.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_002.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_002.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_003.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_003.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_thumb.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_basics_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_energy_yield_001.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_energy_yield_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_energy_yield_thumb.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_energy_yield_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_001.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_002.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_002.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_thumb.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_001.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_002.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_002.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_003.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_003.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_thumb.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_jph_from_spec_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_2t_stc_001.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_2t_stc_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_2t_stc_thumb.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_2t_stc_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_4t_stc_001.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_4t_stc_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_4t_stc_thumb.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_4t_stc_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_ey_001.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_ey_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_ey_thumb.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_ey_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_optim_bg_stc_001.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_optim_bg_stc_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_tandem_optim_bg_stc_thumb.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_tandem_optim_bg_stc_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_temp_vs_irrad_001.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_temp_vs_irrad_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_images/sphx_glr_plot_temp_vs_irrad_thumb.png` & `pv_tandem-0.1.1/docs/_build/html/_images/sphx_glr_plot_temp_vs_irrad_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_static/broken_example.png` & `pv_tandem-0.1.1/docs/_build/html/_static/broken_example.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/_build/html/_static/no_image.png` & `pv_tandem-0.1.1/docs/_build/html/_static/no_image.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_bifacial_basics_001.png` & `pv_tandem-0.1.1/docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_bifacial_basics_002.png` & `pv_tandem-0.1.1/docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_002.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_bifacial_basics_003.png` & `pv_tandem-0.1.1/docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_003.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_bifacial_energy_yield_001.png` & `pv_tandem-0.1.1/docs/auto_examples/energy_yield/images/sphx_glr_plot_bifacial_energy_yield_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_bifacial_irradiance_yield_001.png` & `pv_tandem-0.1.1/docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_irradiance_yield_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_bifacial_irradiance_yield_002.png` & `pv_tandem-0.1.1/docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_irradiance_yield_002.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_jph_from_spec_001.png` & `pv_tandem-0.1.1/docs/auto_examples/basics/images/sphx_glr_plot_jph_from_spec_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_jph_from_spec_002.png` & `pv_tandem-0.1.1/docs/auto_examples/basics/images/sphx_glr_plot_jph_from_spec_002.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_jph_from_spec_003.png` & `pv_tandem-0.1.1/docs/auto_examples/basics/images/sphx_glr_plot_jph_from_spec_003.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_tandem_2t_stc_001.png` & `pv_tandem-0.1.1/docs/auto_examples/stc/images/sphx_glr_plot_tandem_2t_stc_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_tandem_4t_stc_001.png` & `pv_tandem-0.1.1/docs/auto_examples/stc/images/sphx_glr_plot_tandem_4t_stc_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_tandem_ey_001.png` & `pv_tandem-0.1.1/docs/auto_examples/energy_yield/images/sphx_glr_plot_tandem_ey_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_tandem_optim_bg_stc_001.png` & `pv_tandem-0.1.1/docs/auto_examples/stc/images/sphx_glr_plot_tandem_optim_bg_stc_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/sphx_glr_plot_temp_vs_irrad_001.png` & `pv_tandem-0.1.1/docs/auto_examples/basics/images/sphx_glr_plot_temp_vs_irrad_001.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_bifacial_basics_thumb.png` & `pv_tandem-0.1.1/docs/auto_examples/bifacial/images/thumb/sphx_glr_plot_bifacial_basics_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_bifacial_energy_yield_thumb.png` & `pv_tandem-0.1.1/docs/auto_examples/energy_yield/images/thumb/sphx_glr_plot_bifacial_energy_yield_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_bifacial_irradiance_yield_thumb.png` & `pv_tandem-0.1.1/docs/auto_examples/bifacial/images/thumb/sphx_glr_plot_bifacial_irradiance_yield_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_jph_from_spec_thumb.png` & `pv_tandem-0.1.1/docs/auto_examples/basics/images/thumb/sphx_glr_plot_jph_from_spec_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_tandem_2t_stc_thumb.png` & `pv_tandem-0.1.1/docs/auto_examples/stc/images/thumb/sphx_glr_plot_tandem_2t_stc_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_tandem_4t_stc_thumb.png` & `pv_tandem-0.1.1/docs/auto_examples/stc/images/thumb/sphx_glr_plot_tandem_4t_stc_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_tandem_ey_thumb.png` & `pv_tandem-0.1.1/docs/auto_examples/energy_yield/images/thumb/sphx_glr_plot_tandem_ey_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_tandem_optim_bg_stc_thumb.png` & `pv_tandem-0.1.1/docs/auto_examples/stc/images/thumb/sphx_glr_plot_tandem_optim_bg_stc_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/images/thumb/sphx_glr_plot_temp_vs_irrad_thumb.png` & `pv_tandem-0.1.1/docs/auto_examples/basics/images/thumb/sphx_glr_plot_temp_vs_irrad_thumb.png`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/docs/auto_examples/index.rst` & `pv_tandem-0.1.1/docs/auto_examples/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,208 +1,258 @@
 :orphan:
 
+.. _gallery:
+
 Gallery
-==================
+=======
 
 Below is a gallery of examples of how to use PV Tandem for solar cell simulations.
 
 
 .. raw:: html
 
     <div class="sphx-glr-thumbnails">
 
 
 .. raw:: html
 
-    <div class="sphx-glr-thumbcontainer" tooltip="Tandem Solar Cell under STC">
+    </div>
+
+Basic modeling examples
+-----------------------
+
+
+.. raw:: html
+
+    <div class="sphx-glr-thumbnails">
+
+
+.. raw:: html
+
+    <div class="sphx-glr-thumbcontainer" tooltip="Showing the effect of cell temperature and light intensity on Voc and FF">
 
 .. only:: html
 
-  .. image:: /auto_examples/images/thumb/sphx_glr_plot_tandem_2t_stc_thumb.png
+  .. image:: /auto_examples/basics/images/thumb/sphx_glr_plot_temp_vs_irrad_thumb.png
     :alt:
 
-  :ref:`sphx_glr_auto_examples_plot_tandem_2t_stc.py`
+  :ref:`sphx_glr_auto_examples_basics_plot_temp_vs_irrad.py`
 
 .. raw:: html
 
-      <div class="sphx-glr-thumbnail-title">Tandem Solar Cell under STC</div>
+      <div class="sphx-glr-thumbnail-title">Effect of temperature and intensity on solar cell</div>
     </div>
 
 
 .. raw:: html
 
-    <div class="sphx-glr-thumbcontainer" tooltip="Tandem Solar Cell under STC">
+    <div class="sphx-glr-thumbcontainer" tooltip="Modeling Photocurrent Density for Tandem Solar Cells">
 
 .. only:: html
 
-  .. image:: /auto_examples/images/thumb/sphx_glr_plot_tandem_4t_stc_thumb.png
+  .. image:: /auto_examples/basics/images/thumb/sphx_glr_plot_jph_from_spec_thumb.png
     :alt:
 
-  :ref:`sphx_glr_auto_examples_plot_tandem_4t_stc.py`
+  :ref:`sphx_glr_auto_examples_basics_plot_jph_from_spec.py`
 
 .. raw:: html
 
-      <div class="sphx-glr-thumbnail-title">Tandem Solar Cell under STC</div>
+      <div class="sphx-glr-thumbnail-title">Modeling Photocurrent Density for Tandem Solar Cells</div>
     </div>
 
 
 .. raw:: html
 
-    <div class="sphx-glr-thumbcontainer" tooltip="Showing the effect of cell temperature and light intensity on Voc and FF">
+    </div>
+
+Bifacial illumination
+---------------------
+
+
+.. raw:: html
+
+    <div class="sphx-glr-thumbnails">
+
+
+.. raw:: html
+
+    <div class="sphx-glr-thumbcontainer" tooltip="Bifacial Irradiance Yield">
 
 .. only:: html
 
-  .. image:: /auto_examples/images/thumb/sphx_glr_plot_temp_vs_irrad_thumb.png
+  .. image:: /auto_examples/bifacial/images/thumb/sphx_glr_plot_bifacial_irradiance_yield_thumb.png
     :alt:
 
-  :ref:`sphx_glr_auto_examples_plot_temp_vs_irrad.py`
+  :ref:`sphx_glr_auto_examples_bifacial_plot_bifacial_irradiance_yield.py`
 
 .. raw:: html
 
-      <div class="sphx-glr-thumbnail-title">Effect of temperature and intensity on solar cell</div>
+      <div class="sphx-glr-thumbnail-title">Bifacial Irradiance Yield</div>
     </div>
 
 
 .. raw:: html
 
-    <div class="sphx-glr-thumbcontainer" tooltip="Modeling Photocurrent Density for Tandem Solar Cells">
+    <div class="sphx-glr-thumbcontainer" tooltip="Basic examples of bifacial modeling">
 
 .. only:: html
 
-  .. image:: /auto_examples/images/thumb/sphx_glr_plot_jph_from_spec_thumb.png
+  .. image:: /auto_examples/bifacial/images/thumb/sphx_glr_plot_bifacial_basics_thumb.png
     :alt:
 
-  :ref:`sphx_glr_auto_examples_plot_jph_from_spec.py`
+  :ref:`sphx_glr_auto_examples_bifacial_plot_bifacial_basics.py`
 
 .. raw:: html
 
-      <div class="sphx-glr-thumbnail-title">Modeling Photocurrent Density for Tandem Solar Cells</div>
+      <div class="sphx-glr-thumbnail-title">Basic examples of bifacial modeling</div>
     </div>
 
 
 .. raw:: html
 
-    <div class="sphx-glr-thumbcontainer" tooltip="Energy Yield for Tandem Solar Cell">
+    </div>
+
+Energy yield calculations
+-------------------------
+
+
+.. raw:: html
+
+    <div class="sphx-glr-thumbnails">
+
+
+.. raw:: html
+
+    <div class="sphx-glr-thumbcontainer" tooltip="Energy Yield for Silicon Solar Cell">
 
 .. only:: html
 
-  .. image:: /auto_examples/images/thumb/sphx_glr_plot_tandem_ey_thumb.png
+  .. image:: /auto_examples/energy_yield/images/thumb/sphx_glr_plot_silicon_ey_thumb.png
     :alt:
 
-  :ref:`sphx_glr_auto_examples_plot_tandem_ey.py`
+  :ref:`sphx_glr_auto_examples_energy_yield_plot_silicon_ey.py`
 
 .. raw:: html
 
-      <div class="sphx-glr-thumbnail-title">Energy Yield for Tandem Solar Cell</div>
+      <div class="sphx-glr-thumbnail-title">Energy Yield for Silicon Solar Cell</div>
     </div>
 
 
 .. raw:: html
 
     <div class="sphx-glr-thumbcontainer" tooltip="Energy Yield for Tandem Solar Cell">
 
 .. only:: html
 
-  .. image:: /auto_examples/images/thumb/sphx_glr_lambertw_num_testing_thumb.png
+  .. image:: /auto_examples/energy_yield/images/thumb/sphx_glr_plot_tandem_ey_thumb.png
     :alt:
 
-  :ref:`sphx_glr_auto_examples_lambertw_num_testing.py`
+  :ref:`sphx_glr_auto_examples_energy_yield_plot_tandem_ey.py`
 
 .. raw:: html
 
       <div class="sphx-glr-thumbnail-title">Energy Yield for Tandem Solar Cell</div>
     </div>
 
 
 .. raw:: html
 
-    <div class="sphx-glr-thumbcontainer" tooltip="Bifacial Irradiance Yield">
+    <div class="sphx-glr-thumbcontainer" tooltip="Energy Yield for Bifacial Tandem Solar Cell">
 
 .. only:: html
 
-  .. image:: /auto_examples/images/thumb/sphx_glr_plot_bifacial_irradiance_yield_thumb.png
+  .. image:: /auto_examples/energy_yield/images/thumb/sphx_glr_plot_bifacial_energy_yield_thumb.png
     :alt:
 
-  :ref:`sphx_glr_auto_examples_plot_bifacial_irradiance_yield.py`
+  :ref:`sphx_glr_auto_examples_energy_yield_plot_bifacial_energy_yield.py`
+
+.. raw:: html
+
+      <div class="sphx-glr-thumbnail-title">Energy Yield for Bifacial Tandem Solar Cell</div>
+    </div>
+
 
 .. raw:: html
 
-      <div class="sphx-glr-thumbnail-title">Bifacial Irradiance Yield</div>
     </div>
 
+Modeling for standart test conditions (STC)
+-------------------------------------------
+
+
+.. raw:: html
+
+    <div class="sphx-glr-thumbnails">
+
 
 .. raw:: html
 
     <div class="sphx-glr-thumbcontainer" tooltip="Tandem Solar Cell under STC">
 
 .. only:: html
 
-  .. image:: /auto_examples/images/thumb/sphx_glr_plot_tandem_optim_bg_stc_thumb.png
+  .. image:: /auto_examples/stc/images/thumb/sphx_glr_plot_tandem_2t_stc_thumb.png
     :alt:
 
-  :ref:`sphx_glr_auto_examples_plot_tandem_optim_bg_stc.py`
+  :ref:`sphx_glr_auto_examples_stc_plot_tandem_2t_stc.py`
 
 .. raw:: html
 
       <div class="sphx-glr-thumbnail-title">Tandem Solar Cell under STC</div>
     </div>
 
 
 .. raw:: html
 
-    <div class="sphx-glr-thumbcontainer" tooltip="Basic examples of bifacial modeling">
+    <div class="sphx-glr-thumbcontainer" tooltip="Tandem Solar Cell under STC">
 
 .. only:: html
 
-  .. image:: /auto_examples/images/thumb/sphx_glr_plot_bifacial_basics_thumb.png
+  .. image:: /auto_examples/stc/images/thumb/sphx_glr_plot_tandem_4t_stc_thumb.png
     :alt:
 
-  :ref:`sphx_glr_auto_examples_plot_bifacial_basics.py`
+  :ref:`sphx_glr_auto_examples_stc_plot_tandem_4t_stc.py`
 
 .. raw:: html
 
-      <div class="sphx-glr-thumbnail-title">Basic examples of bifacial modeling</div>
+      <div class="sphx-glr-thumbnail-title">Tandem Solar Cell under STC</div>
     </div>
 
 
 .. raw:: html
 
-    <div class="sphx-glr-thumbcontainer" tooltip="Energy Yield for Bifacial Tandem Solar Cell">
+    <div class="sphx-glr-thumbcontainer" tooltip="Tandem Solar Cell under STC">
 
 .. only:: html
 
-  .. image:: /auto_examples/images/thumb/sphx_glr_plot_bifacial_energy_yield_thumb.png
+  .. image:: /auto_examples/stc/images/thumb/sphx_glr_plot_tandem_optim_bg_stc_thumb.png
     :alt:
 
-  :ref:`sphx_glr_auto_examples_plot_bifacial_energy_yield.py`
+  :ref:`sphx_glr_auto_examples_stc_plot_tandem_optim_bg_stc.py`
 
 .. raw:: html
 
-      <div class="sphx-glr-thumbnail-title">Energy Yield for Bifacial Tandem Solar Cell</div>
+      <div class="sphx-glr-thumbnail-title">Tandem Solar Cell under STC</div>
     </div>
 
 
 .. raw:: html
 
     </div>
 
 
 .. toctree::
    :hidden:
+   :includehidden:
+
 
-   /auto_examples/plot_tandem_2t_stc
-   /auto_examples/plot_tandem_4t_stc
-   /auto_examples/plot_temp_vs_irrad
-   /auto_examples/plot_jph_from_spec
-   /auto_examples/plot_tandem_ey
-   /auto_examples/lambertw_num_testing
-   /auto_examples/plot_bifacial_irradiance_yield
-   /auto_examples/plot_tandem_optim_bg_stc
-   /auto_examples/plot_bifacial_basics
-   /auto_examples/plot_bifacial_energy_yield
+   /auto_examples/basics/index.rst
+   /auto_examples/bifacial/index.rst
+   /auto_examples/energy_yield/index.rst
+   /auto_examples/stc/index.rst
 
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-gallery
 
     .. container:: sphx-glr-download sphx-glr-download-python
```

### Comparing `pv_tandem-0.1.0/docs/auto_examples/lambertw_num_testing.rst` & `pv_tandem-0.1.1/docs/auto_examples/energy_yield/plot_tandem_ey.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,93 @@
 
 .. DO NOT EDIT.
 .. THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY.
 .. TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE:
-.. "auto_examples\lambertw_num_testing.py"
+.. "auto_examples\energy_yield\plot_tandem_ey.py"
 .. LINE NUMBERS ARE GIVEN BELOW.
 
 .. only:: html
 
     .. note::
         :class: sphx-glr-download-link-note
 
-        :ref:`Go to the end <sphx_glr_download_auto_examples_lambertw_num_testing.py>`
+        :ref:`Go to the end <sphx_glr_download_auto_examples_energy_yield_plot_tandem_ey.py>`
         to download the full example code
 
 .. rst-class:: sphx-glr-example-title
 
-.. _sphx_glr_auto_examples_lambertw_num_testing.py:
+.. _sphx_glr_auto_examples_energy_yield_plot_tandem_ey.py:
 
 
 Energy Yield for Tandem Solar Cell
 ==================================
 Using spectral on-demand data from NREL and simulated EQE data from GENPRO4.
 
-.. GENERATED FROM PYTHON SOURCE LINES 10-20
+.. GENERATED FROM PYTHON SOURCE LINES 8-18
 
 This example shows how to model the performance of a tandem solar cell. It
 uses "spectral-on-demand" data from the NSRDB providded by NREL.
 For the absorptances of the subcells GENPRO4 simulated EQE curves are used
 originally createf for the following publication:
 Reference
 ----------
 .. [1] P. Tillmann, K. Jäger, A. Karsenti, L. Kreinin, C. Becker (2022)
    “Model-Chain Validation for Estimating the Energy Yield of Bifacial 
    Perovskite/Silicon Tandem Solar Cells,” Solar RRL 2200079, 
    DOI: 10.1002/solr.202200079
 
-.. GENERATED FROM PYTHON SOURCE LINES 22-24
+.. GENERATED FROM PYTHON SOURCE LINES 20-22
 
 First, we load the preprocessed spectral and meta-data (for temperature)
 The spectral data has to be converted from W/µm/m2 to W/nm/m2 (by deviding by 1000)
 
-.. GENERATED FROM PYTHON SOURCE LINES 24-43
+.. GENERATED FROM PYTHON SOURCE LINES 22-41
 
 .. code-block:: default
 
 
     import pandas as pd
     import numpy as np
     import matplotlib.pyplot as plt
     from pv_tandem import utils, solarcell_models
     import pvlib
 
     plt.rcParams['figure.dpi'] = 140
 
     spec_irrad_ts = pd.read_csv(
-        "./data/spec_poa_dallas_2020.csv", index_col=0, parse_dates=True
+        "../data/spec_poa_dallas_2020.csv", index_col=0, parse_dates=True
     )
     spec_irrad_ts.columns = spec_irrad_ts.columns.astype(float)
     spec_irrad_ts = spec_irrad_ts.clip(lower=0)/1000
 
     meta_ts = pd.read_csv(
-        "./data/meta_ts_dallas_2020.csv", index_col=0, parse_dates=True
+        "../data/meta_ts_dallas_2020.csv", index_col=0, parse_dates=True
     )
 
 
-.. GENERATED FROM PYTHON SOURCE LINES 44-49
+
+
+
+
+
+
+.. GENERATED FROM PYTHON SOURCE LINES 42-47
 
 Note that the airmass and zenith values do not exactly match the values in
 the technical report; this is because airmass is estimated from solar
 position and the solar position calculation in the technical report does not
 exactly match the one used here.  However, the differences are minor enough
 to not materially change the spectra.
 
-.. GENERATED FROM PYTHON SOURCE LINES 49-101
+.. GENERATED FROM PYTHON SOURCE LINES 47-89
 
 .. code-block:: default
 
 
-    eqe = pd.read_csv('./data/eqe_tandem_2t.csv', index_col=0)
+    eqe = pd.read_csv('../data/eqe_tandem_2t.csv', index_col=0)
 
     eqe = utils.interp_eqe_to_spec(eqe, spec_irrad_ts)
 
     electrical_parameters = {
         "Rsh": {"pero": 1000, "si": 3000},
         "RsTandem": 3,
         "j0": {"pero": 2.7e-18, "si": 1e-12},
@@ -98,63 +104,70 @@
                                              noct=45,
                                              module_efficiency=0.25)
 
 
     temperature = pd.DataFrame({'pero':temperature,
                                 'si':temperature})
 
-    tandem = solarcell_models.TandemSimulator(
+    tandem = solarcell_models.TandemSimulator2T(
         eqe=eqe,
         electrical_parameters=electrical_parameters,
         subcell_names=["pero", "si"],
     )
 
-    import time
-
-    start = time.time()
-
     power = tandem.calc_power(spec_irrad=spec_irrad_ts,
                               cell_temps=temperature)
 
-    stop = time.time()
-
-    runtime = stop-start
-
-    print(f'Runtime: {runtime}')
-
     power.index = spec_irrad_ts.index
 
     ax = (power.groupby(power.index.dayofyear).sum() * 10 / 1000).plot()
     ax.set_xlabel('Day of year')
     ax.set_ylabel('Daily yield (kWh/m2)')
 
     print(f"Yearly yield: {(power * 10 /1000).sum():.1f} kWh/m2")
     # %%
 
+
+.. image-sg:: /auto_examples/energy_yield/images/sphx_glr_plot_tandem_ey_001.png
+   :alt: plot tandem ey
+   :srcset: /auto_examples/energy_yield/images/sphx_glr_plot_tandem_ey_001.png
+   :class: sphx-glr-single-img
+
+
+.. rst-class:: sphx-glr-script-out
+
+ .. code-block:: none
+
+    Yearly yield: 516.7 kWh/m2
+
+
+
+
+
 .. rst-class:: sphx-glr-timing
 
-   **Total running time of the script:** ( 0 minutes  0.000 seconds)
+   **Total running time of the script:** ( 0 minutes  0.581 seconds)
 
 
-.. _sphx_glr_download_auto_examples_lambertw_num_testing.py:
+.. _sphx_glr_download_auto_examples_energy_yield_plot_tandem_ey.py:
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-example
 
 
 
 
     .. container:: sphx-glr-download sphx-glr-download-python
 
-      :download:`Download Python source code: lambertw_num_testing.py <lambertw_num_testing.py>`
+      :download:`Download Python source code: plot_tandem_ey.py <plot_tandem_ey.py>`
 
     .. container:: sphx-glr-download sphx-glr-download-jupyter
 
-      :download:`Download Jupyter notebook: lambertw_num_testing.ipynb <lambertw_num_testing.ipynb>`
+      :download:`Download Jupyter notebook: plot_tandem_ey.ipynb <plot_tandem_ey.ipynb>`
 
 
 .. only:: html
 
  .. rst-class:: sphx-glr-signature
 
     `Gallery generated by Sphinx-Gallery <https://sphinx-gallery.github.io>`_
```

### Comparing `pv_tandem-0.1.0/docs/auto_examples/plot_bifacial_basics.rst` & `pv_tandem-0.1.1/docs/auto_examples/bifacial/plot_bifacial_basics.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 .. DO NOT EDIT.
 .. THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY.
 .. TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE:
-.. "auto_examples\plot_bifacial_basics.py"
+.. "auto_examples\bifacial\plot_bifacial_basics.py"
 .. LINE NUMBERS ARE GIVEN BELOW.
 
 .. only:: html
 
     .. note::
         :class: sphx-glr-download-link-note
 
-        :ref:`Go to the end <sphx_glr_download_auto_examples_plot_bifacial_basics.py>`
+        :ref:`Go to the end <sphx_glr_download_auto_examples_bifacial_plot_bifacial_basics.py>`
         to download the full example code
 
 .. rst-class:: sphx-glr-example-title
 
-.. _sphx_glr_auto_examples_plot_bifacial_basics.py:
+.. _sphx_glr_auto_examples_bifacial_plot_bifacial_basics.py:
 
 
 Basic examples of bifacial modeling
 ===================================
 Showcasing basic examples for modeling of bifacial irradiance
 
 .. GENERATED FROM PYTHON SOURCE LINES 10-20
@@ -89,17 +89,17 @@
     ax.set_xlabel('Ground array position (-)')
 
     plt.show()
 
 
 
 
-.. image-sg:: /auto_examples/images/sphx_glr_plot_bifacial_basics_001.png
+.. image-sg:: /auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_001.png
    :alt: plot bifacial basics
-   :srcset: /auto_examples/images/sphx_glr_plot_bifacial_basics_001.png
+   :srcset: /auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_001.png
    :class: sphx-glr-single-img
 
 
 
 
 
 .. GENERATED FROM PYTHON SOURCE LINES 59-65
@@ -161,17 +161,17 @@
 
     fig.tight_layout()
     plt.show()
 
 
 
 
-.. image-sg:: /auto_examples/images/sphx_glr_plot_bifacial_basics_002.png
+.. image-sg:: /auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_002.png
    :alt: 20-06-2019, 23-09-2019, 20-11-2019
-   :srcset: /auto_examples/images/sphx_glr_plot_bifacial_basics_002.png
+   :srcset: /auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_002.png
    :class: sphx-glr-single-img
 
 
 .. rst-class:: sphx-glr-script-out
 
  .. code-block:: none
 
@@ -227,36 +227,36 @@
     ax1.set_ylabel('Irradiance fraction (%)')
     ax1.legend(legend_1)
     ax2.set_ylabel('Irradiance fraction (%)')
     ax2.set_xlabel('Position on module (m)')
     ax2.legend(legend_2)
 
 
-.. image-sg:: /auto_examples/images/sphx_glr_plot_bifacial_basics_003.png
+.. image-sg:: /auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_003.png
    :alt: plot bifacial basics
-   :srcset: /auto_examples/images/sphx_glr_plot_bifacial_basics_003.png
+   :srcset: /auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_003.png
    :class: sphx-glr-single-img
 
 
 .. rst-class:: sphx-glr-script-out
 
  .. code-block:: none
 
 
-    <matplotlib.legend.Legend object at 0x0000026E01B41B50>
+    <matplotlib.legend.Legend object at 0x0000026A44E11850>
 
 
 
 
 .. rst-class:: sphx-glr-timing
 
-   **Total running time of the script:** ( 0 minutes  0.559 seconds)
+   **Total running time of the script:** ( 0 minutes  0.566 seconds)
 
 
-.. _sphx_glr_download_auto_examples_plot_bifacial_basics.py:
+.. _sphx_glr_download_auto_examples_bifacial_plot_bifacial_basics.py:
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-example
```

### Comparing `pv_tandem-0.1.0/docs/auto_examples/plot_bifacial_energy_yield.rst` & `pv_tandem-0.1.1/docs/auto_examples/energy_yield/plot_bifacial_energy_yield.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 .. DO NOT EDIT.
 .. THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY.
 .. TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE:
-.. "auto_examples\plot_bifacial_energy_yield.py"
+.. "auto_examples\energy_yield\plot_bifacial_energy_yield.py"
 .. LINE NUMBERS ARE GIVEN BELOW.
 
 .. only:: html
 
     .. note::
         :class: sphx-glr-download-link-note
 
-        :ref:`Go to the end <sphx_glr_download_auto_examples_plot_bifacial_energy_yield.py>`
+        :ref:`Go to the end <sphx_glr_download_auto_examples_energy_yield_plot_bifacial_energy_yield.py>`
         to download the full example code
 
 .. rst-class:: sphx-glr-example-title
 
-.. _sphx_glr_auto_examples_plot_bifacial_energy_yield.py:
+.. _sphx_glr_auto_examples_energy_yield_plot_bifacial_energy_yield.py:
 
 
 Energy Yield for Bifacial Tandem Solar Cell
 ===========================================
 Using spectral on-demand data from NREL and simulated EQE data from GENPRO4.
 
 .. GENERATED FROM PYTHON SOURCE LINES 8-22
@@ -55,26 +55,26 @@
     import matplotlib.pyplot as plt
     import numpy as np
     import pvlib
     import pandas as pd
     import seaborn as sns
 
     spec_irrad_ts = pd.read_csv(
-        "./data/spec_poa_dallas_2020.csv", index_col=0, parse_dates=True
+        "../data/spec_poa_dallas_2020.csv", index_col=0, parse_dates=True
     )
 
     spec_irrad_ts.columns = spec_irrad_ts.columns.astype(float)
     # converting spectral data from W/µ/m² to W/nm/m²
     spec_irrad_ts = spec_irrad_ts.clip(lower=0) / 1000
 
-    eqe = pd.read_csv("./data/eqe_tandem_2t.csv", index_col=0)
+    eqe = pd.read_csv("../data/eqe_tandem_2t.csv", index_col=0)
     eqe = utils.interp_eqe_to_spec(eqe, spec_irrad_ts)
 
     meta_ts = pd.read_csv(
-        "./data/meta_ts_dallas_2020.csv", index_col=0, parse_dates=True
+        "../data/meta_ts_dallas_2020.csv", index_col=0, parse_dates=True
     )
 
     coord_dallas = dict(latitude=32.8, longitude=-96.8)
 
 
 
 
@@ -160,15 +160,15 @@
     P_max = P.max(axis=1)
     P_max = pd.Series(P_max, index=spec_irrad_ts.index)
 
 
     # A dataset with simulated eqe data for several different perovskite bandgaps is
     # loaded to scan the energy yield for the optimal bandgap
 
-    eqe_all_bgs = pd.read_csv("./data/eqe_tandem_all_bgs.csv")
+    eqe_all_bgs = pd.read_csv("../data/eqe_tandem_all_bgs.csv")
 
     P_stc = []
     energy_yield_bif = []
     energy_yield_mono = []
     j_ph = []
 
     for bandgap in eqe_all_bgs["bandgap"].sort_values().unique():
@@ -238,36 +238,36 @@
             "Energy yield monofacial",
             "Standart test conditions",
         ],
     )
 
 
 
-.. image-sg:: /auto_examples/images/sphx_glr_plot_bifacial_energy_yield_001.png
+.. image-sg:: /auto_examples/energy_yield/images/sphx_glr_plot_bifacial_energy_yield_001.png
    :alt: plot bifacial energy yield
-   :srcset: /auto_examples/images/sphx_glr_plot_bifacial_energy_yield_001.png
+   :srcset: /auto_examples/energy_yield/images/sphx_glr_plot_bifacial_energy_yield_001.png
    :class: sphx-glr-single-img
 
 
 .. rst-class:: sphx-glr-script-out
 
  .. code-block:: none
 
 
-    <matplotlib.legend.Legend object at 0x0000026E01B425D0>
+    <matplotlib.legend.Legend object at 0x0000026A44D7B210>
 
 
 
 
 .. rst-class:: sphx-glr-timing
 
-   **Total running time of the script:** ( 0 minutes  20.716 seconds)
+   **Total running time of the script:** ( 0 minutes  20.294 seconds)
 
 
-.. _sphx_glr_download_auto_examples_plot_bifacial_energy_yield.py:
+.. _sphx_glr_download_auto_examples_energy_yield_plot_bifacial_energy_yield.py:
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-example
```

### Comparing `pv_tandem-0.1.0/docs/auto_examples/plot_bifacial_irradiance_yield.rst` & `pv_tandem-0.1.1/docs/auto_examples/bifacial/plot_bifacial_irradiance_yield.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 .. DO NOT EDIT.
 .. THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY.
 .. TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE:
-.. "auto_examples\plot_bifacial_irradiance_yield.py"
+.. "auto_examples\bifacial\plot_bifacial_irradiance_yield.py"
 .. LINE NUMBERS ARE GIVEN BELOW.
 
 .. only:: html
 
     .. note::
         :class: sphx-glr-download-link-note
 
-        :ref:`Go to the end <sphx_glr_download_auto_examples_plot_bifacial_irradiance_yield.py>`
+        :ref:`Go to the end <sphx_glr_download_auto_examples_bifacial_plot_bifacial_irradiance_yield.py>`
         to download the full example code
 
 .. rst-class:: sphx-glr-example-title
 
-.. _sphx_glr_auto_examples_plot_bifacial_irradiance_yield.py:
+.. _sphx_glr_auto_examples_bifacial_plot_bifacial_irradiance_yield.py:
 
 
 Bifacial Irradiance Yield
 =========================
 Demonstrating the irradiance calculation on the front and backside over one year.
 
 .. GENERATED FROM PYTHON SOURCE LINES 6-9
@@ -55,15 +55,15 @@
     import matplotlib.pyplot as plt
     import numpy as np
     import pvlib
     import pandas as pd
     import seaborn as sns
 
     meta_ts = pd.read_csv(
-        "./data/meta_ts_dallas_2020.csv", index_col=0, parse_dates=True
+        "../data/meta_ts_dallas_2020.csv", index_col=0, parse_dates=True
     )
 
     coord_dallas = dict(latitude = 32.8, longitude = -96.8)
 
     solar_pos = pvlib.solarposition.get_solarposition(meta_ts.index, **coord_dallas)
 
     illumination_df = meta_ts
@@ -125,37 +125,37 @@
 
 
 .. rst-class:: sphx-glr-horizontal
 
 
     *
 
-      .. image-sg:: /auto_examples/images/sphx_glr_plot_bifacial_irradiance_yield_001.png
+      .. image-sg:: /auto_examples/bifacial/images/sphx_glr_plot_bifacial_irradiance_yield_001.png
          :alt: plot bifacial irradiance yield
-         :srcset: /auto_examples/images/sphx_glr_plot_bifacial_irradiance_yield_001.png
+         :srcset: /auto_examples/bifacial/images/sphx_glr_plot_bifacial_irradiance_yield_001.png
          :class: sphx-glr-multi-img
 
     *
 
-      .. image-sg:: /auto_examples/images/sphx_glr_plot_bifacial_irradiance_yield_002.png
+      .. image-sg:: /auto_examples/bifacial/images/sphx_glr_plot_bifacial_irradiance_yield_002.png
          :alt: Front, Back, Combined
-         :srcset: /auto_examples/images/sphx_glr_plot_bifacial_irradiance_yield_002.png
+         :srcset: /auto_examples/bifacial/images/sphx_glr_plot_bifacial_irradiance_yield_002.png
          :class: sphx-glr-multi-img
 
 
 
 
 
 
 .. rst-class:: sphx-glr-timing
 
-   **Total running time of the script:** ( 0 minutes  3.691 seconds)
+   **Total running time of the script:** ( 0 minutes  3.872 seconds)
 
 
-.. _sphx_glr_download_auto_examples_plot_bifacial_irradiance_yield.py:
+.. _sphx_glr_download_auto_examples_bifacial_plot_bifacial_irradiance_yield.py:
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-example
```

### Comparing `pv_tandem-0.1.0/docs/auto_examples/plot_jph_from_spec.rst` & `pv_tandem-0.1.1/docs/auto_examples/basics/plot_jph_from_spec.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 .. DO NOT EDIT.
 .. THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY.
 .. TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE:
-.. "auto_examples\plot_jph_from_spec.py"
+.. "auto_examples\basics\plot_jph_from_spec.py"
 .. LINE NUMBERS ARE GIVEN BELOW.
 
 .. only:: html
 
     .. note::
         :class: sphx-glr-download-link-note
 
-        :ref:`Go to the end <sphx_glr_download_auto_examples_plot_jph_from_spec.py>`
+        :ref:`Go to the end <sphx_glr_download_auto_examples_basics_plot_jph_from_spec.py>`
         to download the full example code
 
 .. rst-class:: sphx-glr-example-title
 
-.. _sphx_glr_auto_examples_plot_jph_from_spec.py:
+.. _sphx_glr_auto_examples_basics_plot_jph_from_spec.py:
 
 
 Modeling Photocurrent Density for Tandem Solar Cells
 ====================================================
 Using spectral on-demand data from NREL and simulated EQE data from GENPRO4.
 
 .. GENERATED FROM PYTHON SOURCE LINES 8-11
@@ -79,27 +79,27 @@
 has to be between 0 and 1.
 
 .. GENERATED FROM PYTHON SOURCE LINES 38-46
 
 .. code-block:: default
 
 
-    example_eqe = pd.read_csv("./data/eqe_tandem_2t.csv", index_col=0)
+    example_eqe = pd.read_csv("../data/eqe_tandem_2t.csv", index_col=0)
     ax = (example_eqe * 100).plot()
     ax.set_xlabel("Wavelength (nm)")
     ax.set_ylabel("Absorptance (%)")
     ax.legend(["Perovskite cell", "Silicon cell"], loc="lower right")
     plt.show()
 
 
 
 
-.. image-sg:: /auto_examples/images/sphx_glr_plot_jph_from_spec_001.png
+.. image-sg:: /auto_examples/basics/images/sphx_glr_plot_jph_from_spec_001.png
    :alt: plot jph from spec
-   :srcset: /auto_examples/images/sphx_glr_plot_jph_from_spec_001.png
+   :srcset: /auto_examples/basics/images/sphx_glr_plot_jph_from_spec_001.png
    :class: sphx-glr-single-img
 
 
 
 
 
 .. GENERATED FROM PYTHON SOURCE LINES 47-50
@@ -110,15 +110,15 @@
 
 .. GENERATED FROM PYTHON SOURCE LINES 50-59
 
 .. code-block:: default
 
 
     spec_irrad_ts = pd.read_csv(
-        "./data/spec_poa_dallas_2020.csv", index_col=0, parse_dates=True
+        "../data/spec_poa_dallas_2020.csv", index_col=0, parse_dates=True
     )
     spec_irrad_ts.columns = spec_irrad_ts.columns.astype(float)
     # converting to W/m²/nm from W/m²/µm and clipping negative values to zero
     spec_irrad_ts = spec_irrad_ts.clip(lower=0) / 1000
 
 
 
@@ -146,17 +146,17 @@
     ax.set_ylabel("Absorptance (%)")
     ax.legend(["Perovskite cell", "Silicon cell"], loc="lower right")
     plt.show()
 
 
 
 
-.. image-sg:: /auto_examples/images/sphx_glr_plot_jph_from_spec_002.png
+.. image-sg:: /auto_examples/basics/images/sphx_glr_plot_jph_from_spec_002.png
    :alt: plot jph from spec
-   :srcset: /auto_examples/images/sphx_glr_plot_jph_from_spec_002.png
+   :srcset: /auto_examples/basics/images/sphx_glr_plot_jph_from_spec_002.png
    :class: sphx-glr-single-img
 
 
 
 
 
 .. GENERATED FROM PYTHON SOURCE LINES 73-77
@@ -183,30 +183,30 @@
     ax.set_xlabel("Day of year")
     ax.set_ylabel("Daily generated Charge (MC/day)")
     ax.legend(["Perovskite cell", "Silicon cell"], loc="upper right")
     plt.show()
 
 
 
-.. image-sg:: /auto_examples/images/sphx_glr_plot_jph_from_spec_003.png
+.. image-sg:: /auto_examples/basics/images/sphx_glr_plot_jph_from_spec_003.png
    :alt: plot jph from spec
-   :srcset: /auto_examples/images/sphx_glr_plot_jph_from_spec_003.png
+   :srcset: /auto_examples/basics/images/sphx_glr_plot_jph_from_spec_003.png
    :class: sphx-glr-single-img
 
 
 
 
 
 
 .. rst-class:: sphx-glr-timing
 
-   **Total running time of the script:** ( 0 minutes  0.357 seconds)
+   **Total running time of the script:** ( 0 minutes  0.379 seconds)
 
 
-.. _sphx_glr_download_auto_examples_plot_jph_from_spec.py:
+.. _sphx_glr_download_auto_examples_basics_plot_jph_from_spec.py:
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-example
```

### Comparing `pv_tandem-0.1.0/docs/auto_examples/plot_tandem_2t_stc.rst` & `pv_tandem-0.1.1/docs/auto_examples/stc/plot_tandem_4t_stc.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 .. DO NOT EDIT.
 .. THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY.
 .. TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE:
-.. "auto_examples\plot_tandem_2t_stc.py"
+.. "auto_examples\stc\plot_tandem_4t_stc.py"
 .. LINE NUMBERS ARE GIVEN BELOW.
 
 .. only:: html
 
     .. note::
         :class: sphx-glr-download-link-note
 
-        :ref:`Go to the end <sphx_glr_download_auto_examples_plot_tandem_2t_stc.py>`
+        :ref:`Go to the end <sphx_glr_download_auto_examples_stc_plot_tandem_4t_stc.py>`
         to download the full example code
 
 .. rst-class:: sphx-glr-example-title
 
-.. _sphx_glr_auto_examples_plot_tandem_2t_stc.py:
+.. _sphx_glr_auto_examples_stc_plot_tandem_4t_stc.py:
 
 
 Tandem Solar Cell under STC
 ===========================
 Simulating the IV curve of a Tandem Solar Cell with a 1-Diode model.
 
 .. GENERATED FROM PYTHON SOURCE LINES 8-18
@@ -49,15 +49,15 @@
     import numpy as np
     import matplotlib.pyplot as plt
     from pv_tandem import utils, solarcell_models
     import pvlib
 
     plt.rcParams["figure.dpi"] = 140
 
-    eqe = pd.read_csv("./data/eqe_tandem_2t.csv", index_col=0)
+    eqe = pd.read_csv("../data/eqe_tandem_2t.csv", index_col=0)
 
 
 
 
 
 
 
@@ -67,84 +67,86 @@
 
 Note that the airmass and zenith values do not exactly match the values in
 the technical report; this is because airmass is estimated from solar
 position and the solar position calculation in the technical report does not
 exactly match the one used here.  However, the differences are minor enough
 to not materially change the spectra.
 
-.. GENERATED FROM PYTHON SOURCE LINES 40-72
+.. GENERATED FROM PYTHON SOURCE LINES 40-74
 
 .. code-block:: default
 
 
+
     electrical_parameters = {
         "Rsh": {"pero": 2000, "si": 5000},
-        "RsTandem": 3,
+        "Rs": {"pero":6, "si":2},
         "j0": {"pero": 2.7e-18, "si": 1e-12},
         "n": {"pero": 1.1, "si": 1},
         "Temp": {"pero": 25, "si": 25},
         "noct": {"pero": 48, "si": 48},
         "tcJsc": {"pero": 0.0002, "si": 0.00032},
         "tcVoc": {"pero": -0.002, "si": -0.0041},
     }
 
-    tandem = solarcell_models.TandemSimulator2T(
+    tandem = solarcell_models.TandemSimulator4T(
         eqe=eqe,
         electrical_parameters=electrical_parameters,
         subcell_names=["pero", "si"],
     )
 
     iv_stc = tandem.calc_IV_stc()
+
     fig, ax = plt.subplots()
 
     for subcell, iv in iv_stc.items():
         iv = iv[(iv > 0).shift(1, fill_value=True)]
         iv = iv.reset_index().set_index(subcell)
         iv.plot(ax=ax)
 
-    ax.legend(["Perovskite", "Silicon", "Tandem"])
+    ax.legend(["Perovskite", "Silicon"])
     ax.set_xlabel("Voltage (V)")
     ax.set_ylabel("Current density (mA/cm2)")
     ax.set_xlim(0)
     ax.set_ylim(0)
     plt.show()
 
 
 
-.. image-sg:: /auto_examples/images/sphx_glr_plot_tandem_2t_stc_001.png
-   :alt: plot tandem 2t stc
-   :srcset: /auto_examples/images/sphx_glr_plot_tandem_2t_stc_001.png
+.. image-sg:: /auto_examples/stc/images/sphx_glr_plot_tandem_4t_stc_001.png
+   :alt: plot tandem 4t stc
+   :srcset: /auto_examples/stc/images/sphx_glr_plot_tandem_4t_stc_001.png
    :class: sphx-glr-single-img
 
 
 
 
 
 
 .. rst-class:: sphx-glr-timing
 
-   **Total running time of the script:** ( 0 minutes  0.425 seconds)
+   **Total running time of the script:** ( 0 minutes  0.077 seconds)
 
 
-.. _sphx_glr_download_auto_examples_plot_tandem_2t_stc.py:
+.. _sphx_glr_download_auto_examples_stc_plot_tandem_4t_stc.py:
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-example
 
 
 
 
     .. container:: sphx-glr-download sphx-glr-download-python
 
-      :download:`Download Python source code: plot_tandem_2t_stc.py <plot_tandem_2t_stc.py>`
+      :download:`Download Python source code: plot_tandem_4t_stc.py <plot_tandem_4t_stc.py>`
 
     .. container:: sphx-glr-download sphx-glr-download-jupyter
 
-      :download:`Download Jupyter notebook: plot_tandem_2t_stc.ipynb <plot_tandem_2t_stc.ipynb>`
+      :download:`Download Jupyter notebook: plot_tandem_4t_stc.ipynb <plot_tandem_4t_stc.ipynb>`
 
 
 .. only:: html
 
  .. rst-class:: sphx-glr-signature
 
     `Gallery generated by Sphinx-Gallery <https://sphinx-gallery.github.io>`_
```

### Comparing `pv_tandem-0.1.0/docs/auto_examples/plot_tandem_4t_stc.rst` & `pv_tandem-0.1.1/docs/auto_examples/stc/plot_tandem_2t_stc.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 .. DO NOT EDIT.
 .. THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY.
 .. TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE:
-.. "auto_examples\plot_tandem_4t_stc.py"
+.. "auto_examples\stc\plot_tandem_2t_stc.py"
 .. LINE NUMBERS ARE GIVEN BELOW.
 
 .. only:: html
 
     .. note::
         :class: sphx-glr-download-link-note
 
-        :ref:`Go to the end <sphx_glr_download_auto_examples_plot_tandem_4t_stc.py>`
+        :ref:`Go to the end <sphx_glr_download_auto_examples_stc_plot_tandem_2t_stc.py>`
         to download the full example code
 
 .. rst-class:: sphx-glr-example-title
 
-.. _sphx_glr_auto_examples_plot_tandem_4t_stc.py:
+.. _sphx_glr_auto_examples_stc_plot_tandem_2t_stc.py:
 
 
 Tandem Solar Cell under STC
 ===========================
 Simulating the IV curve of a Tandem Solar Cell with a 1-Diode model.
 
 .. GENERATED FROM PYTHON SOURCE LINES 8-18
@@ -49,15 +49,15 @@
     import numpy as np
     import matplotlib.pyplot as plt
     from pv_tandem import utils, solarcell_models
     import pvlib
 
     plt.rcParams["figure.dpi"] = 140
 
-    eqe = pd.read_csv("./data/eqe_tandem_2t.csv", index_col=0)
+    eqe = pd.read_csv("../data/eqe_tandem_2t.csv", index_col=0)
 
 
 
 
 
 
 
@@ -67,86 +67,84 @@
 
 Note that the airmass and zenith values do not exactly match the values in
 the technical report; this is because airmass is estimated from solar
 position and the solar position calculation in the technical report does not
 exactly match the one used here.  However, the differences are minor enough
 to not materially change the spectra.
 
-.. GENERATED FROM PYTHON SOURCE LINES 40-74
+.. GENERATED FROM PYTHON SOURCE LINES 40-72
 
 .. code-block:: default
 
 
-
     electrical_parameters = {
         "Rsh": {"pero": 2000, "si": 5000},
-        "Rs": {"pero":6, "si":2},
+        "RsTandem": 3,
         "j0": {"pero": 2.7e-18, "si": 1e-12},
         "n": {"pero": 1.1, "si": 1},
         "Temp": {"pero": 25, "si": 25},
         "noct": {"pero": 48, "si": 48},
         "tcJsc": {"pero": 0.0002, "si": 0.00032},
         "tcVoc": {"pero": -0.002, "si": -0.0041},
     }
 
-    tandem = solarcell_models.TandemSimulator4T(
+    tandem = solarcell_models.TandemSimulator2T(
         eqe=eqe,
         electrical_parameters=electrical_parameters,
         subcell_names=["pero", "si"],
     )
 
     iv_stc = tandem.calc_IV_stc()
-
     fig, ax = plt.subplots()
 
     for subcell, iv in iv_stc.items():
         iv = iv[(iv > 0).shift(1, fill_value=True)]
         iv = iv.reset_index().set_index(subcell)
         iv.plot(ax=ax)
 
-    ax.legend(["Perovskite", "Silicon"])
+    ax.legend(["Perovskite", "Silicon", "Tandem"])
     ax.set_xlabel("Voltage (V)")
     ax.set_ylabel("Current density (mA/cm2)")
     ax.set_xlim(0)
     ax.set_ylim(0)
     plt.show()
 
 
 
-.. image-sg:: /auto_examples/images/sphx_glr_plot_tandem_4t_stc_001.png
-   :alt: plot tandem 4t stc
-   :srcset: /auto_examples/images/sphx_glr_plot_tandem_4t_stc_001.png
+.. image-sg:: /auto_examples/stc/images/sphx_glr_plot_tandem_2t_stc_001.png
+   :alt: plot tandem 2t stc
+   :srcset: /auto_examples/stc/images/sphx_glr_plot_tandem_2t_stc_001.png
    :class: sphx-glr-single-img
 
 
 
 
 
 
 .. rst-class:: sphx-glr-timing
 
-   **Total running time of the script:** ( 0 minutes  0.080 seconds)
+   **Total running time of the script:** ( 0 minutes  0.084 seconds)
 
 
-.. _sphx_glr_download_auto_examples_plot_tandem_4t_stc.py:
+.. _sphx_glr_download_auto_examples_stc_plot_tandem_2t_stc.py:
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-example
 
 
 
 
     .. container:: sphx-glr-download sphx-glr-download-python
 
-      :download:`Download Python source code: plot_tandem_4t_stc.py <plot_tandem_4t_stc.py>`
+      :download:`Download Python source code: plot_tandem_2t_stc.py <plot_tandem_2t_stc.py>`
 
     .. container:: sphx-glr-download sphx-glr-download-jupyter
 
-      :download:`Download Jupyter notebook: plot_tandem_4t_stc.ipynb <plot_tandem_4t_stc.ipynb>`
+      :download:`Download Jupyter notebook: plot_tandem_2t_stc.ipynb <plot_tandem_2t_stc.ipynb>`
 
 
 .. only:: html
 
  .. rst-class:: sphx-glr-signature
 
     `Gallery generated by Sphinx-Gallery <https://sphinx-gallery.github.io>`_
```

### Comparing `pv_tandem-0.1.0/docs/auto_examples/plot_tandem_ey.rst` & `pv_tandem-0.1.1/docs/auto_examples/basics/plot_temp_vs_irrad.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,173 +1,201 @@
 
 .. DO NOT EDIT.
 .. THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY.
 .. TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE:
-.. "auto_examples\plot_tandem_ey.py"
+.. "auto_examples\basics\plot_temp_vs_irrad.py"
 .. LINE NUMBERS ARE GIVEN BELOW.
 
 .. only:: html
 
     .. note::
         :class: sphx-glr-download-link-note
 
-        :ref:`Go to the end <sphx_glr_download_auto_examples_plot_tandem_ey.py>`
+        :ref:`Go to the end <sphx_glr_download_auto_examples_basics_plot_temp_vs_irrad.py>`
         to download the full example code
 
 .. rst-class:: sphx-glr-example-title
 
-.. _sphx_glr_auto_examples_plot_tandem_ey.py:
+.. _sphx_glr_auto_examples_basics_plot_temp_vs_irrad.py:
 
 
-Energy Yield for Tandem Solar Cell
-==================================
-Using spectral on-demand data from NREL and simulated EQE data from GENPRO4.
+Effect of temperature and intensity on solar cell 
+=================================================
 
-.. GENERATED FROM PYTHON SOURCE LINES 8-18
+Showing the effect of cell temperature and light intensity on Voc and FF
 
-This example shows how to model the performance of a tandem solar cell. It
-uses "spectral-on-demand" data from the NSRDB providded by NREL.
-For the absorptances of the subcells GENPRO4 simulated EQE curves are used
-originally createf for the following publication:
-Reference
-----------
-.. [1] P. Tillmann, K. Jäger, A. Karsenti, L. Kreinin, C. Becker (2022)
-   “Model-Chain Validation for Estimating the Energy Yield of Bifacial 
-   Perovskite/Silicon Tandem Solar Cells,” Solar RRL 2200079, 
-   DOI: 10.1002/solr.202200079
+.. GENERATED FROM PYTHON SOURCE LINES 11-16
 
-.. GENERATED FROM PYTHON SOURCE LINES 20-22
+This examples shows how to visulize the effects of the cell temperature and light
+intensity (irradiance) on the open circuit voltage (VoC) and fill factor (FF) of a single
+junction solar cell. This is done by defining a One-Diode model of a silicon solar
+cell and calculating the Voc and FF for a grid of irradiance levels and cell
+temperatures
 
-First, we load the preprocessed spectral and meta-data (for temperature)
-The spectral data has to be converted from W/µm/m2 to W/nm/m2 (by deviding by 1000)
-
-.. GENERATED FROM PYTHON SOURCE LINES 22-41
+.. GENERATED FROM PYTHON SOURCE LINES 16-23
 
 .. code-block:: default
 
 
     import pandas as pd
     import numpy as np
     import matplotlib.pyplot as plt
-    from pv_tandem import utils, solarcell_models
-    import pvlib
+    import seaborn as sns
+    from pv_tandem import electrical_models
+
+
+
+
+
+
+
+
+.. GENERATED FROM PYTHON SOURCE LINES 24-26
+
+After loading the nessesary python libraries, the diode model is defined with the temperature coefficents for Voc
+and Jsc, series and shunt resistance, ideality factor and dark saturation current.
 
-    plt.rcParams['figure.dpi'] = 140
+.. GENERATED FROM PYTHON SOURCE LINES 26-31
 
-    spec_irrad_ts = pd.read_csv(
-        "./data/spec_poa_dallas_2020.csv", index_col=0, parse_dates=True
+.. code-block:: default
+
+
+    one_diode = electrical_models.OneDiodeModel(
+        tcJsc=0.00032, tcVoc=-0.0041, R_shunt=2000, R_series=2, n=1, j0=1e-11
     )
-    spec_irrad_ts.columns = spec_irrad_ts.columns.astype(float)
-    spec_irrad_ts = spec_irrad_ts.clip(lower=0)/1000
 
-    meta_ts = pd.read_csv(
-        "./data/meta_ts_dallas_2020.csv", index_col=0, parse_dates=True
+
+
+
+
+
+
+
+.. GENERATED FROM PYTHON SOURCE LINES 32-34
+
+Then, data data grid of cell temperature (defined in °C) and irradiance (W/m2)
+is created as a pandas DataFrame.
+
+.. GENERATED FROM PYTHON SOURCE LINES 34-42
+
+.. code-block:: default
+
+
+    df = pd.DataFrame(
+        {
+            "temperature": np.repeat(np.arange(15, 76, 5), 10),
+            "irrad": np.tile(np.arange(100, 1100, 100), 13),
+        }
     )
 
 
 
 
 
 
 
 
-.. GENERATED FROM PYTHON SOURCE LINES 42-47
+.. GENERATED FROM PYTHON SOURCE LINES 43-45
 
-Note that the airmass and zenith values do not exactly match the values in
-the technical report; this is because airmass is estimated from solar
-position and the solar position calculation in the technical report does not
-exactly match the one used here.  However, the differences are minor enough
-to not materially change the spectra.
+The irradiance is transformed transformed into a short ciurcuit density (mA/cm2)
+assuming a generation of 40.6 mA/cm2 for a illumination of 1000 W/cm2. 
 
-.. GENERATED FROM PYTHON SOURCE LINES 47-89
+.. GENERATED FROM PYTHON SOURCE LINES 45-48
 
 .. code-block:: default
 
 
-    eqe = pd.read_csv('./data/eqe_tandem_2t.csv', index_col=0)
+    df["j_ph"] = df["irrad"] / 1000 * 40.6
+
+
+
 
-    eqe = utils.interp_eqe_to_spec(eqe, spec_irrad_ts)
 
-    electrical_parameters = {
-        "Rsh": {"pero": 1000, "si": 3000},
-        "RsTandem": 3,
-        "j0": {"pero": 2.7e-18, "si": 1e-12},
-        "n": {"pero": 1.1, "si": 1},
-        "Temp": {"pero": 25, "si": 25},
-        "noct": {"pero": 48, "si": 48},
-        "tcJsc": {"pero": 0.0002, "si": 0.00032},
-        "tcVoc": {"pero": -0.002, "si": -0.0041},
-    }
-
-    temperature = pvlib.temperature.noct_sam(spec_irrad_ts.sum(axis=1)*1.15,
-                                             meta_ts['Temperature'],
-                                             meta_ts['Wind Speed'],
-                                             noct=45,
-                                             module_efficiency=0.25)
-
-
-    temperature = pd.DataFrame({'pero':temperature,
-                                'si':temperature})
-
-    tandem = solarcell_models.TandemSimulator2T(
-        eqe=eqe,
-        electrical_parameters=electrical_parameters,
-        subcell_names=["pero", "si"],
-    )
 
-    power = tandem.calc_power(spec_irrad=spec_irrad_ts,
-                              cell_temps=temperature)
 
-    power.index = spec_irrad_ts.index
 
-    ax = (power.groupby(power.index.dayofyear).sum() * 10 / 1000).plot()
-    ax.set_xlabel('Day of year')
-    ax.set_ylabel('Daily yield (kWh/m2)')
+.. GENERATED FROM PYTHON SOURCE LINES 49-52
 
-    print(f"Yearly yield: {(power * 10 /1000).sum():.1f} kWh/m2")
-    # %%
+Short circuit current and temperature are fed into the diode model for the
+resulting IV parameters and Voc and FF are plotted as functions of irradiance
+and temperature.
+
+.. GENERATED FROM PYTHON SOURCE LINES 52-81
+
+.. code-block:: default
+
+
+    params = one_diode.calc_iv_params(df["j_ph"], df["temperature"])
+
+    df = pd.concat([df, params], axis=1)
+    df = df.set_index(["temperature", "irrad"])
+
+    v_oc = df["Voc"].unstack("irrad")
+    ff = df["FF"].unstack("irrad")
+
+    fig, (ax1, ax2) = plt.subplots(1, 2, sharey=True, figsize=(8, 5), dpi=150)
+
+    ax1.set_title("Open Circuit Voltage")
+    ax2.set_title("Fill Factor")
+
+    cs1 = ax1.contourf(v_oc.columns, v_oc.index, v_oc.values * 1e3, levels=15)
+    cs2 = ax2.contourf(ff.columns, ff.index, ff.values * 1e2, levels=15)
+    ax1.set_ylabel("Cell Temperature (°C)")
+    ax1.set_xlabel("Irradiance (W/m²)")
+    ax2.set_xlabel("Irradiance (W/m²)")
+
+    fig.colorbar(
+        cs1,
+        ax=ax1,
+        shrink=0.9,
+        orientation="horizontal",
+        label="Open Circuit Voltage (mV)",
+    )
+    fig.colorbar(
+        cs2, ax=ax2, shrink=0.9, orientation="horizontal", label="Fill Factor (%)"
+    )
 
 
-.. image-sg:: /auto_examples/images/sphx_glr_plot_tandem_ey_001.png
-   :alt: plot tandem ey
-   :srcset: /auto_examples/images/sphx_glr_plot_tandem_ey_001.png
+.. image-sg:: /auto_examples/basics/images/sphx_glr_plot_temp_vs_irrad_001.png
+   :alt: Open Circuit Voltage, Fill Factor
+   :srcset: /auto_examples/basics/images/sphx_glr_plot_temp_vs_irrad_001.png
    :class: sphx-glr-single-img
 
 
 .. rst-class:: sphx-glr-script-out
 
  .. code-block:: none
 
-    Yearly yield: 516.7 kWh/m2
 
+    <matplotlib.colorbar.Colorbar object at 0x0000026A49E2B850>
 
 
 
 
 .. rst-class:: sphx-glr-timing
 
-   **Total running time of the script:** ( 0 minutes  0.747 seconds)
+   **Total running time of the script:** ( 0 minutes  0.570 seconds)
 
 
-.. _sphx_glr_download_auto_examples_plot_tandem_ey.py:
+.. _sphx_glr_download_auto_examples_basics_plot_temp_vs_irrad.py:
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-example
 
 
 
 
     .. container:: sphx-glr-download sphx-glr-download-python
 
-      :download:`Download Python source code: plot_tandem_ey.py <plot_tandem_ey.py>`
+      :download:`Download Python source code: plot_temp_vs_irrad.py <plot_temp_vs_irrad.py>`
 
     .. container:: sphx-glr-download sphx-glr-download-jupyter
 
-      :download:`Download Jupyter notebook: plot_tandem_ey.ipynb <plot_tandem_ey.ipynb>`
+      :download:`Download Jupyter notebook: plot_temp_vs_irrad.ipynb <plot_temp_vs_irrad.ipynb>`
 
 
 .. only:: html
 
  .. rst-class:: sphx-glr-signature
 
     `Gallery generated by Sphinx-Gallery <https://sphinx-gallery.github.io>`_
```

### Comparing `pv_tandem-0.1.0/docs/auto_examples/plot_tandem_optim_bg_stc.rst` & `pv_tandem-0.1.1/docs/auto_examples/stc/plot_tandem_optim_bg_stc.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 .. DO NOT EDIT.
 .. THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY.
 .. TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE:
-.. "auto_examples\plot_tandem_optim_bg_stc.py"
+.. "auto_examples\stc\plot_tandem_optim_bg_stc.py"
 .. LINE NUMBERS ARE GIVEN BELOW.
 
 .. only:: html
 
     .. note::
         :class: sphx-glr-download-link-note
 
-        :ref:`Go to the end <sphx_glr_download_auto_examples_plot_tandem_optim_bg_stc.py>`
+        :ref:`Go to the end <sphx_glr_download_auto_examples_stc_plot_tandem_optim_bg_stc.py>`
         to download the full example code
 
 .. rst-class:: sphx-glr-example-title
 
-.. _sphx_glr_auto_examples_plot_tandem_optim_bg_stc.py:
+.. _sphx_glr_auto_examples_stc_plot_tandem_optim_bg_stc.py:
 
 
 Tandem Solar Cell under STC
 ===========================
 Simulating the IV curve of a Tandem Solar Cell with a 1-Diode model.
 
 .. GENERATED FROM PYTHON SOURCE LINES 8-18
@@ -49,15 +49,15 @@
     import numpy as np
     import matplotlib.pyplot as plt
     from pv_tandem import utils, solarcell_models
     import pvlib
 
     plt.rcParams["figure.dpi"] = 140
 
-    eqe = pd.read_csv("./data/eqe_tandem_2t.csv", index_col=0)
+    eqe = pd.read_csv("../data/eqe_tandem_2t.csv", index_col=0)
 
 
 
 
 
 
 
@@ -103,15 +103,15 @@
 
     tandem_4T = solarcell_models.TandemSimulator4T(
         eqe=eqe,
         electrical_parameters=electrical_parameters_4T,
         subcell_names=["pero", "si"],
     )
 
-    eqe_all_bgs = pd.read_csv('./data/eqe_tandem_all_bgs.csv')
+    eqe_all_bgs = pd.read_csv('../data/eqe_tandem_all_bgs.csv')
 
     eff_2T = []
     eff_4T = []
 
     bandgaps = eqe_all_bgs['bandgap'].sort_values().unique()
 
     for bandgap in bandgaps:
@@ -164,36 +164,36 @@
 
 
     # Combine the handles from both axes
 
     ax.legend(handles, ['2 Terminal', '4 Terminal'])
 
 
-.. image-sg:: /auto_examples/images/sphx_glr_plot_tandem_optim_bg_stc_001.png
+.. image-sg:: /auto_examples/stc/images/sphx_glr_plot_tandem_optim_bg_stc_001.png
    :alt: plot tandem optim bg stc
-   :srcset: /auto_examples/images/sphx_glr_plot_tandem_optim_bg_stc_001.png
+   :srcset: /auto_examples/stc/images/sphx_glr_plot_tandem_optim_bg_stc_001.png
    :class: sphx-glr-single-img
 
 
 .. rst-class:: sphx-glr-script-out
 
  .. code-block:: none
 
 
-    <matplotlib.legend.Legend object at 0x0000026E006F6AD0>
+    <matplotlib.legend.Legend object at 0x0000026A44E082D0>
 
 
 
 
 .. rst-class:: sphx-glr-timing
 
-   **Total running time of the script:** ( 0 minutes  0.388 seconds)
+   **Total running time of the script:** ( 0 minutes  0.395 seconds)
 
 
-.. _sphx_glr_download_auto_examples_plot_tandem_optim_bg_stc.py:
+.. _sphx_glr_download_auto_examples_stc_plot_tandem_optim_bg_stc.py:
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-example
```

### Comparing `pv_tandem-0.1.0/docs/auto_examples/plot_temp_vs_irrad.rst` & `pv_tandem-0.1.1/docs/auto_examples/energy_yield/plot_silicon_ey.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,201 +1,196 @@
 
 .. DO NOT EDIT.
 .. THIS FILE WAS AUTOMATICALLY GENERATED BY SPHINX-GALLERY.
 .. TO MAKE CHANGES, EDIT THE SOURCE PYTHON FILE:
-.. "auto_examples\plot_temp_vs_irrad.py"
+.. "auto_examples\energy_yield\plot_silicon_ey.py"
 .. LINE NUMBERS ARE GIVEN BELOW.
 
 .. only:: html
 
     .. note::
         :class: sphx-glr-download-link-note
 
-        :ref:`Go to the end <sphx_glr_download_auto_examples_plot_temp_vs_irrad.py>`
+        :ref:`Go to the end <sphx_glr_download_auto_examples_energy_yield_plot_silicon_ey.py>`
         to download the full example code
 
 .. rst-class:: sphx-glr-example-title
 
-.. _sphx_glr_auto_examples_plot_temp_vs_irrad.py:
+.. _sphx_glr_auto_examples_energy_yield_plot_silicon_ey.py:
 
 
-Effect of temperature and intensity on solar cell 
-=================================================
+Energy Yield for Silicon Solar Cell
+==================================
+Using non-spectral data from NREL
 
-Showing the effect of cell temperature and light intensity on Voc and FF
+.. GENERATED FROM PYTHON SOURCE LINES 8-14
 
-.. GENERATED FROM PYTHON SOURCE LINES 11-16
+This example shows how to model the performance of a single junction silicon
+solar cell. It uses irradiance data from the NSRDB providded by NREL. The
+irradiance data is part of the meta data of the sepctral on demand data product
+but can also be obtained from NSRDB as a seperate data product.
+For the absorptances of the cell it is assumed that the cell produces 39 mA/cm²
+short-circuit current density.
 
-This examples shows how to visulize the effects of the cell temperature and light
-intensity (irradiance) on the open circuit voltage (VoC) and fill factor (FF) of a single
-junction solar cell. This is done by defining a One-Diode model of a silicon solar
-cell and calculating the Voc and FF for a grid of irradiance levels and cell
-temperatures
+.. GENERATED FROM PYTHON SOURCE LINES 17-19
 
-.. GENERATED FROM PYTHON SOURCE LINES 16-23
+First, we load the required libraries and the preprocessed meta-data from spectral
+data for temperature and non-spectral irradiance data
+
+.. GENERATED FROM PYTHON SOURCE LINES 19-32
 
 .. code-block:: default
 
 
     import pandas as pd
     import numpy as np
     import matplotlib.pyplot as plt
-    import seaborn as sns
-    from pv_tandem import electrical_models
-
-
+    from pv_tandem.electrical_models import OneDiodeModel
+    import pvlib
 
+    plt.rcParams['figure.dpi'] = 140
 
+    meta_ts = pd.read_csv(
+        "../data/meta_ts_dallas_2020.csv", index_col=0, parse_dates=True
+    )
 
 
 
 
-.. GENERATED FROM PYTHON SOURCE LINES 24-26
 
-After loading the nessesary python libraries, the diode model is defined with the temperature coefficents for Voc
-and Jsc, series and shunt resistance, ideality factor and dark saturation current.
 
-.. GENERATED FROM PYTHON SOURCE LINES 26-31
 
-.. code-block:: default
 
+.. GENERATED FROM PYTHON SOURCE LINES 33-35
 
-    one_diode = electrical_models.OneDiodeModel(
-        tcJsc=0.00032, tcVoc=-0.0041, R_shunt=2000, R_series=2, n=1, j0=1e-11
-    )
+Next, we calculate the draction of DNI radiating on the tilted module plane 
+(with tilt angle 20 deg) and a fixed fraction of the DHI of 80 %
 
+.. GENERATED FROM PYTHON SOURCE LINES 35-55
 
+.. code-block:: default
 
 
+    # Convert angles from degrees to radians
+    solar_zenith = np.radians(meta_ts['Solar Zenith Angle'])
+    solar_azimuth = np.radians(meta_ts['Solar Azimuth Angle'])
+    tilt = np.radians(20)
+    plane_azimuth = np.radians(180)
 
+    # Calculate the cosine of the angle of incidence
+    cos_theta_i = np.cos(solar_zenith) * np.cos(tilt) + np.sin(solar_zenith) * np.sin(tilt) * np.cos(solar_azimuth - plane_azimuth)
 
+    # Calculate the DNI absorbed
+    dni_plane = meta_ts['DNI'] * cos_theta_i
 
+    # Make sure the absorbed DNI is not negative (i.e., the sun is behind the plane)
+    dni_plane[dni_plane < 0] = 0
 
-.. GENERATED FROM PYTHON SOURCE LINES 32-34
+    # assuming 80% of the DHI are reaching the 20° tilted module plane
 
-Then, data data grid of cell temperature (defined in °C) and irradiance (W/m2)
-is created as a pandas DataFrame.
+    irrad_plane = dni_plane + meta_ts['DHI'] * 0.8
 
-.. GENERATED FROM PYTHON SOURCE LINES 34-42
 
-.. code-block:: default
 
 
-    df = pd.DataFrame(
-        {
-            "temperature": np.repeat(np.arange(15, 76, 5), 10),
-            "irrad": np.tile(np.arange(100, 1100, 100), 13),
-        }
-    )
 
 
 
 
+.. GENERATED FROM PYTHON SOURCE LINES 56-58
 
+Next, we define the one-diode model of the solar cell and estiamte the cell
+temperature with the ross model of pvlib
 
+.. GENERATED FROM PYTHON SOURCE LINES 58-68
 
+.. code-block:: default
 
-.. GENERATED FROM PYTHON SOURCE LINES 43-45
 
-The irradiance is transformed transformed into a short ciurcuit density (mA/cm2)
-assuming a generation of 40.6 mA/cm2 for a illumination of 1000 W/cm2. 
+    one_diode = OneDiodeModel(
+        tcJsc=0.0003, tcVoc=-0.004, R_shunt=3000, R_series=1.5, n=1, j0=1e-12
+    )
 
-.. GENERATED FROM PYTHON SOURCE LINES 45-48
+    cell_temp = pvlib.temperature.ross(poa_global = irrad_plane,
+                                             temp_air = meta_ts['Temperature'],
+                                             noct=45
+                                             )
 
-.. code-block:: default
 
 
-    df["j_ph"] = df["irrad"] / 1000 * 40.6
 
 
 
 
 
+.. GENERATED FROM PYTHON SOURCE LINES 69-72
 
+Finally, the power output of the cell is calculated, assuming a linear relationship
+between irradaince and short circuit density, with Jsc of 39 mA/cm² for 1000
+Watts irradiance
 
+.. GENERATED FROM PYTHON SOURCE LINES 72-87
 
-.. GENERATED FROM PYTHON SOURCE LINES 49-52
+.. code-block:: default
 
-Short circuit current and temperature are fed into the diode model for the
-resulting IV parameters and Voc and FF are plotted as functions of irradiance
-and temperature.
 
-.. GENERATED FROM PYTHON SOURCE LINES 52-81
+    Jsc = irrad_plane/1000*39
 
-.. code-block:: default
+    iv_paras = one_diode.calc_iv_params(Jsc=Jsc, cell_temp = cell_temp)
 
+    power_max = iv_paras['Pmax']
 
-    params = one_diode.calc_iv_params(df["j_ph"], df["temperature"])
+    # Converting from W/cm² to kW/m²
 
-    df = pd.concat([df, params], axis=1)
-    df = df.set_index(["temperature", "irrad"])
+    power_max = power_max * 10 / 1000
 
-    v_oc = df["Voc"].unstack("irrad")
-    ff = df["FF"].unstack("irrad")
+    ax = power_max.groupby(power_max.index.dayofyear).sum().plot()
+    ax.set_xlabel('Day of year')
+    ax.set_ylabel('Daily yield (kWh/m2)')
 
-    fig, (ax1, ax2) = plt.subplots(1, 2, sharey=True, figsize=(8, 5), dpi=150)
-
-    ax1.set_title("Open Circuit Voltage")
-    ax2.set_title("Fill Factor")
-
-    cs1 = ax1.contourf(v_oc.columns, v_oc.index, v_oc.values * 1e3, levels=15)
-    cs2 = ax2.contourf(ff.columns, ff.index, ff.values * 1e2, levels=15)
-    ax1.set_ylabel("Cell Temperature (°C)")
-    ax1.set_xlabel("Irradiance (W/m²)")
-    ax2.set_xlabel("Irradiance (W/m²)")
-
-    fig.colorbar(
-        cs1,
-        ax=ax1,
-        shrink=0.9,
-        orientation="horizontal",
-        label="Open Circuit Voltage (mV)",
-    )
-    fig.colorbar(
-        cs2, ax=ax2, shrink=0.9, orientation="horizontal", label="Fill Factor (%)"
-    )
+    print(f"Yearly yield: {(power_max).sum():.1f} kWh/m2")
 
 
-.. image-sg:: /auto_examples/images/sphx_glr_plot_temp_vs_irrad_001.png
-   :alt: Open Circuit Voltage, Fill Factor
-   :srcset: /auto_examples/images/sphx_glr_plot_temp_vs_irrad_001.png
+.. image-sg:: /auto_examples/energy_yield/images/sphx_glr_plot_silicon_ey_001.png
+   :alt: plot silicon ey
+   :srcset: /auto_examples/energy_yield/images/sphx_glr_plot_silicon_ey_001.png
    :class: sphx-glr-single-img
 
 
 .. rst-class:: sphx-glr-script-out
 
  .. code-block:: none
 
+    Yearly yield: 394.4 kWh/m2
 
-    <matplotlib.colorbar.Colorbar object at 0x0000026E01561BD0>
 
 
 
 
 .. rst-class:: sphx-glr-timing
 
-   **Total running time of the script:** ( 0 minutes  0.858 seconds)
+   **Total running time of the script:** ( 0 minutes  0.212 seconds)
 
 
-.. _sphx_glr_download_auto_examples_plot_temp_vs_irrad.py:
+.. _sphx_glr_download_auto_examples_energy_yield_plot_silicon_ey.py:
 
 .. only:: html
 
   .. container:: sphx-glr-footer sphx-glr-footer-example
 
 
 
 
     .. container:: sphx-glr-download sphx-glr-download-python
 
-      :download:`Download Python source code: plot_temp_vs_irrad.py <plot_temp_vs_irrad.py>`
+      :download:`Download Python source code: plot_silicon_ey.py <plot_silicon_ey.py>`
 
     .. container:: sphx-glr-download sphx-glr-download-jupyter
 
-      :download:`Download Jupyter notebook: plot_temp_vs_irrad.ipynb <plot_temp_vs_irrad.ipynb>`
+      :download:`Download Jupyter notebook: plot_silicon_ey.ipynb <plot_silicon_ey.ipynb>`
 
 
 .. only:: html
 
  .. rst-class:: sphx-glr-signature
 
     `Gallery generated by Sphinx-Gallery <https://sphinx-gallery.github.io>`_
```

### Comparing `pv_tandem-0.1.0/docs/conf.py` & `pv_tandem-0.1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
+    "matplotlib.sphinxext.plot_directive",
     "sphinx.ext.mathjax",
     "sphinx.ext.autodoc",
     "sphinx.ext.viewcode",
     "sphinx.ext.intersphinx",
     "sphinx.ext.extlinks",
     "sphinx.ext.autosummary",
     "sphinx.ext.napoleon",
@@ -98,14 +99,16 @@
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
+numfig = True
+
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
```

### Comparing `pv_tandem-0.1.0/docs/make.bat` & `pv_tandem-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/pv_tandem/bifacial_geo.py` & `pv_tandem-0.1.1/pv_tandem/bifacial_geo.py`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/pv_tandem/bifacial_yield.py` & `pv_tandem-0.1.1/pv_tandem/bifacial_yield.py`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/pv_tandem/electrical_models.py` & `pv_tandem-0.1.1/pv_tandem/electrical_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,20 +124,27 @@
                 (
                     (Jsc / 1000 * self.R_shunt)[:, None]
                     - (j_arr / 1000 * (self.R_shunt + self.R_series)[:, None])
                 )
                 - (self.n * Vth)[:, None] * lambertwlog((lambw))
                 + (self.j0 / 1000 * self.R_shunt - Voc_rt + Voc)[:, None]
             )
-
-        return np.real(V)
+            
+        if hasattr(Jsc, "__len__"):
+            return np.real(V)
+        else:
+            return np.real(V)[0]
+            
 
     def calc_iv_params(self, Jsc, cell_temp, j_arr=np.linspace(0, 45, 451)):
 
+        index = None        
+
         if hasattr(Jsc, "values"):
+            index = Jsc.index
             Jsc = Jsc.values
 
         if hasattr(cell_temp, "values"):
             cell_temp = cell_temp.values
 
         V = self.calc_iv(Jsc, cell_temp, j_arr)
         P = V * j_arr
@@ -157,14 +164,19 @@
                 "Vmpp": Vmpp,
                 "Pmax": Pmax,
                 "FF": FF,
                 "Jsc": Jsc,
                 "Jmpp": Jmpp,
             }
         )
+        
+        # set index from Jsc if it was a pd.series
+        
+        if index is not None:
+            res.index = index
 
         return res
 
 
 if __name__ == "__main__":
 
     import matplotlib.pyplot as plt
```

### Comparing `pv_tandem-0.1.0/pv_tandem/irradiance_models.py` & `pv_tandem-0.1.1/pv_tandem/irradiance_models.py`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/pv_tandem/solarcell_models.py` & `pv_tandem-0.1.1/pv_tandem/solarcell_models.py`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/pv_tandem/utils.py` & `pv_tandem-0.1.1/pv_tandem/utils.py`

 * *Files identical despite different names*

### Comparing `pv_tandem-0.1.0/pv_tandem.egg-info/PKG-INFO` & `pv_tandem-0.1.1/pv_tandem.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pv-tandem
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python toolbox for simulation and energy yield calculations of tandem solar cells.
 Home-page: https://github.com/nano-sippe/pv_tandem
 Author: Peter Tillmann
 Author-email: Peter.tillmann@helmholtz-berlin.de
 License: MIT license
 Keywords: pv_tandem
 Classifier: Development Status :: 3 - Alpha
@@ -51,17 +51,29 @@
 * Helping tools to process irradiance data for solar cell simulations
 * Electrical modeling with 1-diode model for single junction or tandem solar cells
 * Modeling of illumination in a large PV power plant for the front- and backside of the modules
 
 Where to get it
 ---------------
 
-The source code is hosted at GitHub at: https://github.com/nano-sippe/pv_tandem
+pv_tandem can easily be installed with pip:
 
-To install pv_tandem clone the project from github:
+.. code-block:: bash
+
+    pip install pv_tandem
+
+If you want to be able to directly run the examples you can install pv_tandems together with all nessesary libraries with
+
+.. code-block:: bash
+
+    pip install pv_tandem[doc]
+
+The source code is hosted at GitHub at: https://github.com/HZBSolarOptics/pv_tandem
+
+If you want to install from source clone the project from github:
 
 .. code-block:: bash
 
     git clone https://github.com/nano-sippe/pv_tandem
 
 Then change into the pv_tandem folder and install with pip
```

### Comparing `pv_tandem-0.1.0/pv_tandem.egg-info/SOURCES.txt` & `pv_tandem-0.1.1/pv_tandem.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,95 +9,111 @@
 docs/Makefile
 docs/api.rst
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
-docs/installation.rst
 docs/make.bat
 docs/model_basics.rst
-docs/readme.rst
 docs/usage.rst
-docs/_build/html/_images/sphx_glr_lambertw_num_testing_thumb.png
+docs/_build/html/_downloads/0686a03da72ef988337b900e8aa209e5/one-diode.hires.png
+docs/_build/html/_downloads/ee2294afa81cddfca0cc7ca7c9fffed2/one-diode.png
+docs/_build/html/_images/irrad_vs_Jsc.png
+docs/_build/html/_images/logo.png
+docs/_build/html/_images/one-diode.png
 docs/_build/html/_images/sphx_glr_plot_bifacial_basics_001.png
 docs/_build/html/_images/sphx_glr_plot_bifacial_basics_002.png
 docs/_build/html/_images/sphx_glr_plot_bifacial_basics_003.png
 docs/_build/html/_images/sphx_glr_plot_bifacial_basics_thumb.png
 docs/_build/html/_images/sphx_glr_plot_bifacial_energy_yield_001.png
 docs/_build/html/_images/sphx_glr_plot_bifacial_energy_yield_thumb.png
 docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_001.png
 docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_002.png
 docs/_build/html/_images/sphx_glr_plot_bifacial_irradiance_yield_thumb.png
 docs/_build/html/_images/sphx_glr_plot_jph_from_spec_001.png
 docs/_build/html/_images/sphx_glr_plot_jph_from_spec_002.png
 docs/_build/html/_images/sphx_glr_plot_jph_from_spec_003.png
 docs/_build/html/_images/sphx_glr_plot_jph_from_spec_thumb.png
+docs/_build/html/_images/sphx_glr_plot_silicon_ey_001.png
+docs/_build/html/_images/sphx_glr_plot_silicon_ey_thumb.png
 docs/_build/html/_images/sphx_glr_plot_tandem_2t_stc_001.png
 docs/_build/html/_images/sphx_glr_plot_tandem_2t_stc_thumb.png
 docs/_build/html/_images/sphx_glr_plot_tandem_4t_stc_001.png
 docs/_build/html/_images/sphx_glr_plot_tandem_4t_stc_thumb.png
 docs/_build/html/_images/sphx_glr_plot_tandem_ey_001.png
 docs/_build/html/_images/sphx_glr_plot_tandem_ey_thumb.png
 docs/_build/html/_images/sphx_glr_plot_tandem_optim_bg_stc_001.png
 docs/_build/html/_images/sphx_glr_plot_tandem_optim_bg_stc_thumb.png
 docs/_build/html/_images/sphx_glr_plot_temp_vs_irrad_001.png
 docs/_build/html/_images/sphx_glr_plot_temp_vs_irrad_thumb.png
 docs/_build/html/_static/broken_example.png
 docs/_build/html/_static/file.png
+docs/_build/html/_static/irrad_vs_Jsc.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/no_image.png
 docs/_build/html/_static/plus.png
 docs/_build/html/_static/tandem.png
+docs/_build/plot_directive/pyplots/one-diode.hires.png
+docs/_build/plot_directive/pyplots/one-diode.png
+docs/_static/irrad_vs_Jsc.png
 docs/_static/tandem.png
 docs/auto_examples/index.rst
-docs/auto_examples/lambertw_num_testing.rst
-docs/auto_examples/plot_bifacial_basics.rst
-docs/auto_examples/plot_bifacial_energy_yield.rst
-docs/auto_examples/plot_bifacial_irradiance_yield.rst
-docs/auto_examples/plot_jph_from_spec.rst
-docs/auto_examples/plot_tandem_2t_stc.rst
-docs/auto_examples/plot_tandem_4t_stc.rst
-docs/auto_examples/plot_tandem_ey.rst
-docs/auto_examples/plot_tandem_optim_bg_stc.rst
-docs/auto_examples/plot_temp_vs_irrad.rst
-docs/auto_examples/sg_execution_times.rst
-docs/auto_examples/images/sphx_glr_plot_bifacial_basics_001.png
-docs/auto_examples/images/sphx_glr_plot_bifacial_basics_002.png
-docs/auto_examples/images/sphx_glr_plot_bifacial_basics_003.png
-docs/auto_examples/images/sphx_glr_plot_bifacial_energy_yield_001.png
-docs/auto_examples/images/sphx_glr_plot_bifacial_irradiance_yield_001.png
-docs/auto_examples/images/sphx_glr_plot_bifacial_irradiance_yield_002.png
-docs/auto_examples/images/sphx_glr_plot_jph_from_spec_001.png
-docs/auto_examples/images/sphx_glr_plot_jph_from_spec_002.png
-docs/auto_examples/images/sphx_glr_plot_jph_from_spec_003.png
-docs/auto_examples/images/sphx_glr_plot_tandem_2t_stc_001.png
-docs/auto_examples/images/sphx_glr_plot_tandem_4t_stc_001.png
-docs/auto_examples/images/sphx_glr_plot_tandem_ey_001.png
-docs/auto_examples/images/sphx_glr_plot_tandem_optim_bg_stc_001.png
-docs/auto_examples/images/sphx_glr_plot_temp_vs_irrad_001.png
-docs/auto_examples/images/thumb/sphx_glr_lambertw_num_testing_thumb.png
-docs/auto_examples/images/thumb/sphx_glr_plot_bifacial_basics_thumb.png
-docs/auto_examples/images/thumb/sphx_glr_plot_bifacial_energy_yield_thumb.png
-docs/auto_examples/images/thumb/sphx_glr_plot_bifacial_irradiance_yield_thumb.png
-docs/auto_examples/images/thumb/sphx_glr_plot_jph_from_spec_thumb.png
-docs/auto_examples/images/thumb/sphx_glr_plot_tandem_2t_stc_thumb.png
-docs/auto_examples/images/thumb/sphx_glr_plot_tandem_4t_stc_thumb.png
-docs/auto_examples/images/thumb/sphx_glr_plot_tandem_ey_thumb.png
-docs/auto_examples/images/thumb/sphx_glr_plot_tandem_optim_bg_stc_thumb.png
-docs/auto_examples/images/thumb/sphx_glr_plot_temp_vs_irrad_thumb.png
+docs/auto_examples/basics/index.rst
+docs/auto_examples/basics/plot_jph_from_spec.rst
+docs/auto_examples/basics/plot_temp_vs_irrad.rst
+docs/auto_examples/basics/sg_execution_times.rst
+docs/auto_examples/basics/images/sphx_glr_plot_jph_from_spec_001.png
+docs/auto_examples/basics/images/sphx_glr_plot_jph_from_spec_002.png
+docs/auto_examples/basics/images/sphx_glr_plot_jph_from_spec_003.png
+docs/auto_examples/basics/images/sphx_glr_plot_temp_vs_irrad_001.png
+docs/auto_examples/basics/images/thumb/sphx_glr_plot_jph_from_spec_thumb.png
+docs/auto_examples/basics/images/thumb/sphx_glr_plot_temp_vs_irrad_thumb.png
+docs/auto_examples/bifacial/index.rst
+docs/auto_examples/bifacial/plot_bifacial_basics.rst
+docs/auto_examples/bifacial/plot_bifacial_irradiance_yield.rst
+docs/auto_examples/bifacial/sg_execution_times.rst
+docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_001.png
+docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_002.png
+docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_basics_003.png
+docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_irradiance_yield_001.png
+docs/auto_examples/bifacial/images/sphx_glr_plot_bifacial_irradiance_yield_002.png
+docs/auto_examples/bifacial/images/thumb/sphx_glr_plot_bifacial_basics_thumb.png
+docs/auto_examples/bifacial/images/thumb/sphx_glr_plot_bifacial_irradiance_yield_thumb.png
+docs/auto_examples/energy_yield/index.rst
+docs/auto_examples/energy_yield/plot_bifacial_energy_yield.rst
+docs/auto_examples/energy_yield/plot_silicon_ey.rst
+docs/auto_examples/energy_yield/plot_tandem_ey.rst
+docs/auto_examples/energy_yield/sg_execution_times.rst
+docs/auto_examples/energy_yield/images/sphx_glr_plot_bifacial_energy_yield_001.png
+docs/auto_examples/energy_yield/images/sphx_glr_plot_silicon_ey_001.png
+docs/auto_examples/energy_yield/images/sphx_glr_plot_tandem_ey_001.png
+docs/auto_examples/energy_yield/images/thumb/sphx_glr_plot_bifacial_energy_yield_thumb.png
+docs/auto_examples/energy_yield/images/thumb/sphx_glr_plot_silicon_ey_thumb.png
+docs/auto_examples/energy_yield/images/thumb/sphx_glr_plot_tandem_ey_thumb.png
+docs/auto_examples/stc/index.rst
+docs/auto_examples/stc/plot_tandem_2t_stc.rst
+docs/auto_examples/stc/plot_tandem_4t_stc.rst
+docs/auto_examples/stc/plot_tandem_optim_bg_stc.rst
+docs/auto_examples/stc/sg_execution_times.rst
+docs/auto_examples/stc/images/sphx_glr_plot_tandem_2t_stc_001.png
+docs/auto_examples/stc/images/sphx_glr_plot_tandem_4t_stc_001.png
+docs/auto_examples/stc/images/sphx_glr_plot_tandem_optim_bg_stc_001.png
+docs/auto_examples/stc/images/thumb/sphx_glr_plot_tandem_2t_stc_thumb.png
+docs/auto_examples/stc/images/thumb/sphx_glr_plot_tandem_4t_stc_thumb.png
+docs/auto_examples/stc/images/thumb/sphx_glr_plot_tandem_optim_bg_stc_thumb.png
 pv_tandem/__init__.py
 pv_tandem/bifacial_geo.py
 pv_tandem/bifacial_yield.py
 pv_tandem/electrical_models.py
 pv_tandem/irradiance_models.py
-pv_tandem/local_scripts.py
 pv_tandem/solarcell_models.py
 pv_tandem/utils.py
 pv_tandem.egg-info/PKG-INFO
 pv_tandem.egg-info/SOURCES.txt
 pv_tandem.egg-info/dependency_links.txt
 pv_tandem.egg-info/not-zip-safe
 pv_tandem.egg-info/requires.txt
 pv_tandem.egg-info/top_level.txt
+pv_tandem/data/ASTMG173.csv
 tests/__init__.py
 tests/test_pv_tandem.py
```

### Comparing `pv_tandem-0.1.0/setup.py` & `pv_tandem-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-INSTALL_REQUIRES = ['pvlib >= 0.7.0']
+INSTALL_REQUIRES = ['pvlib >= 0.7.0', 'numpy', 'pandas', 'scipy']
 
 TESTS_REQUIRE = ['pytest>=3',]
 EXTRAS_REQUIRE = {
     'optional': ['netcdf4',],
     'doc': ['ipython', 'matplotlib', 'sphinx == 4.5.0',
             'pydata-sphinx-theme == 0.8.1', 'sphinx-gallery',
             'docutils == 0.15.2', 'seaborn', 'numpydoc'],
@@ -44,12 +44,13 @@
     tests_require=TESTS_REQUIRE,
     license="MIT license",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='pv_tandem',
     name='pv_tandem',
     packages=find_packages(include=['pv_tandem', 'pv_tandem.*']),
+    package_data={'pv_tandem': ['data/*.csv']},
     test_suite='tests',
     url='https://github.com/nano-sippe/pv_tandem',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

### Comparing `pv_tandem-0.1.0/tests/test_pv_tandem.py` & `pv_tandem-0.1.1/tests/test_pv_tandem.py`

 * *Files identical despite different names*

