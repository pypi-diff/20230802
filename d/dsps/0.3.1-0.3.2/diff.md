# Comparing `tmp/dsps-0.3.1.tar.gz` & `tmp/dsps-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsps-0.3.1.tar", last modified: Tue May  2 12:41:49 2023, max compression
+gzip compressed data, was "dsps-0.3.2.tar", last modified: Wed Aug  2 02:34:12 2023, max compression
```

## Comparing `dsps-0.3.1.tar` & `dsps-0.3.2.tar`

### file list

```diff
@@ -1,185 +1,187 @@
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.495882 dsps-0.3.1/
--rw-r--r--   0 aphearin   (501) staff       (20)       90 2022-09-09 13:28:37.000000 dsps-0.3.1/.coveragerc
--rw-r--r--   0 aphearin   (501) staff       (20)      110 2023-05-02 12:28:29.000000 dsps-0.3.1/.git_archival.txt
--rw-r--r--   0 aphearin   (501) staff       (20)       31 2023-05-02 12:28:29.000000 dsps-0.3.1/.gitattributes
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.381044 dsps-0.3.1/.github/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.395648 dsps-0.3.1/.github/workflows/
--rw-r--r--   0 aphearin   (501) staff       (20)     1089 2023-04-29 18:27:09.000000 dsps-0.3.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 aphearin   (501) staff       (20)     1150 2023-04-29 18:27:09.000000 dsps-0.3.1/.github/workflows/tests.yml
--rw-r--r--   0 aphearin   (501) staff       (20)     1489 2023-04-29 18:27:09.000000 dsps-0.3.1/.gitignore
--rw-r--r--   0 aphearin   (501) staff       (20)      212 2023-04-29 18:27:09.000000 dsps-0.3.1/.readthedocs.yml
--rw-r--r--   0 aphearin   (501) staff       (20)      898 2023-05-02 12:30:25.000000 dsps-0.3.1/CHANGES.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     1521 2023-04-29 18:27:09.000000 dsps-0.3.1/LICENSE.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     4101 2023-05-02 12:41:49.495378 dsps-0.3.1/PKG-INFO
--rw-r--r--   0 aphearin   (501) staff       (20)     1998 2023-05-02 12:41:32.000000 dsps-0.3.1/README.md
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.397039 dsps-0.3.1/docs/
--rw-r--r--   0 aphearin   (501) staff       (20)      638 2023-04-29 18:27:09.000000 dsps-0.3.1/docs/Makefile
--rw-r--r--   0 aphearin   (501) staff       (20)      804 2023-04-29 18:27:09.000000 dsps-0.3.1/docs/make.bat
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.404430 dsps-0.3.1/docs/source/
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.405058 dsps-0.3.1/docs/source/_static/
--rw-r--r--   0 aphearin   (501) staff       (20)   129468 2023-04-29 18:27:09.000000 dsps-0.3.1/docs/source/_static/fake_ssp_seds.png
--rw-r--r--   0 aphearin   (501) staff       (20)     1241 2023-04-29 18:27:09.000000 dsps-0.3.1/docs/source/citation.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     1039 2023-04-29 18:27:09.000000 dsps-0.3.1/docs/source/conf.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2171 2023-04-29 18:27:09.000000 dsps-0.3.1/docs/source/custom_ssps.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     2044 2023-04-29 18:27:09.000000 dsps-0.3.1/docs/source/dsps_data_config.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     9494 2023-04-29 18:27:09.000000 dsps-0.3.1/docs/source/dsps_quickstart.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)     1062 2023-04-29 18:27:09.000000 dsps-0.3.1/docs/source/index.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      804 2023-05-01 20:53:07.000000 dsps-0.3.1/docs/source/installation.rst
--rw-r--r--   0 aphearin   (501) staff       (20)     1454 2023-04-29 18:27:09.000000 dsps-0.3.1/docs/source/quickstart.rst
--rw-r--r--   0 aphearin   (501) staff       (20)      309 2023-04-29 18:27:09.000000 dsps-0.3.1/docs/source/reference.rst
--rw-r--r--   0 aphearin   (501) staff       (20)       62 2023-04-29 18:27:09.000000 dsps-0.3.1/docs/source/requirements.txt
--rw-r--r--   0 aphearin   (501) staff       (20)      127 2023-04-29 18:27:09.000000 dsps-0.3.1/docs/source/tutorials.rst
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.407964 dsps-0.3.1/dsps/
--rw-r--r--   0 aphearin   (501) staff       (20)      173 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)       22 2023-05-02 12:41:49.000000 dsps-0.3.1/dsps/_version.py
--rw-r--r--   0 aphearin   (501) staff       (20)      186 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/constants.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.412317 dsps-0.3.1/dsps/cosmology/
--rw-r--r--   0 aphearin   (501) staff       (20)      146 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/cosmology/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)      198 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/cosmology/defaults.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6618 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/cosmology/flat_wcdm.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.415034 dsps-0.3.1/dsps/cosmology/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/cosmology/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5975 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/cosmology/tests/test_flat_wcdm.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.415791 dsps-0.3.1/dsps/data/
--rw-r--r--   0 aphearin   (501) staff       (20)     2349 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/data/README.txt
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.419193 dsps-0.3.1/dsps/data_loaders/
--rw-r--r--   0 aphearin   (501) staff       (20)      250 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/data_loaders/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1165 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/data_loaders/defaults.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2564 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/data_loaders/load_filter_data.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2252 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/data_loaders/load_ssp_data.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3412 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/data_loaders/retrieve_fake_fsps_data.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2097 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/data_loaders/retrieve_fsps_data.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.421193 dsps-0.3.1/dsps/data_loaders/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/data_loaders/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1707 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/data_loaders/tests/test_load_filter_data.py
--rw-r--r--   0 aphearin   (501) staff       (20)      797 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/data_loaders/tests/test_load_ssp_data.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1042 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/data_loaders/tests/test_retrieve_fake_fsps_data.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.422149 dsps-0.3.1/dsps/data_loaders/tests/testing_data/
--rw-r--r--   0 aphearin   (501) staff       (20)    53768 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/data_loaders/tests/testing_data/ssp_plaw_data_c0.txt
--rw-r--r--   0 aphearin   (501) staff       (20)    53390 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/data_loaders/tests/testing_data/ssp_plaw_data_c1.txt
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.423822 dsps-0.3.1/dsps/dust/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)    12142 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/att_curves.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.425792 dsps-0.3.1/dsps/dust/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5152 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/test_att_curves.py
--rw-r--r--   0 aphearin   (501) staff       (20)      983 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/test_utils.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.437806 dsps-0.3.1/dsps/dust/tests/testing_data/
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/calzetti_2000_attenuation.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/calzetti_2000_k_lambda.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/calzetti_2000_wavelength_microns.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/leitherer_2002_attenuation.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/leitherer_2002_k_lambda.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/leitherer_2002_wavelength_microns.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2558 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_attenuation1.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2554 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_attenuation2.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2555 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_attenuation3.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2558 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_k_lambda1.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2554 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_k_lambda2.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2555 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_k_lambda3.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_wavelength_microns.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2554 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/salim_2018_attenuation1.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2556 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/salim_2018_attenuation2.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2554 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/salim_2018_k_lambda1.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2556 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/salim_2018_k_lambda2.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/tests/testing_data/salim_2018_wavelength_microns.txt
--rw-r--r--   0 aphearin   (501) staff       (20)      704 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/dust/utils.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.439653 dsps-0.3.1/dsps/em_lines/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/em_lines/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1699 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/em_lines/equivalent_width.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.440955 dsps-0.3.1/dsps/em_lines/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/em_lines/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1131 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/em_lines/tests/test_equivalent_width.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.442016 dsps-0.3.1/dsps/experimental/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/experimental/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3161 2023-05-01 17:12:20.000000 dsps-0.3.1/dsps/experimental/diffburst.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.443483 dsps-0.3.1/dsps/experimental/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/experimental/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5178 2023-05-01 17:12:20.000000 dsps-0.3.1/dsps/experimental/tests/test_diffburst.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.445464 dsps-0.3.1/dsps/imf/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1463 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/remnant_mass.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1822 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/surviving_mstar.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.446962 dsps-0.3.1/dsps/imf/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2830 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/tests/test_remnant_mass.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1917 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/tests/test_surviving_mstar.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.454541 dsps-0.3.1/dsps/imf/tests/testing_data/
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/tests/testing_data/chabrier_mstar_surviving.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/tests/testing_data/chabrier_mstar_surviving_norem.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/tests/testing_data/kroupa_mstar_surviving.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/tests/testing_data/kroupa_mstar_surviving_norem.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/tests/testing_data/lg_ages_mstar_surviving.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/tests/testing_data/salpeter_mstar_surviving.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/tests/testing_data/salpeter_mstar_surviving_norem.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/tests/testing_data/van_dokkum_mstar_surviving.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/imf/tests/testing_data/van_dokkum_mstar_surviving_norem.txt
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.455677 dsps-0.3.1/dsps/metallicity/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/metallicity/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3962 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/metallicity/mzr.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.456949 dsps-0.3.1/dsps/metallicity/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/metallicity/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)      842 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/metallicity/tests/test_mzr.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.460904 dsps-0.3.1/dsps/metallicity/tests/testing_data/
--rw-r--r--   0 aphearin   (501) staff       (20)      612 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/metallicity/tests/testing_data/galazzi_etal05_mzr.dat
--rw-r--r--   0 aphearin   (501) staff       (20)     1340 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/metallicity/tests/testing_data/kirby_etal13_mzr.dat
--rw-r--r--   0 aphearin   (501) staff       (20)      613 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/metallicity/tests/testing_data/kudritzki_etal16_mzr.dat
--rw-r--r--   0 aphearin   (501) staff       (20)     1010 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/metallicity/tests/testing_data/maiolino_etal18_mzr.dat
--rw-r--r--   0 aphearin   (501) staff       (20)      257 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/metallicity/tests/testing_data/trussler_etal20_mzr_all_centrals_sdss_dr7.dat
--rw-r--r--   0 aphearin   (501) staff       (20)      259 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/metallicity/tests/testing_data/trussler_etal20_mzr_all_sats_sdss_dr7.dat
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.463762 dsps-0.3.1/dsps/photometry/
--rw-r--r--   0 aphearin   (501) staff       (20)       57 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/photometry/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3312 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/photometry/photometry_kernels.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3030 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/photometry/photpop.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.465778 dsps-0.3.1/dsps/photometry/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/photometry/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2566 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/photometry/tests/test_photometry_kernels.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1646 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/photometry/tests/test_photpop.py
--rw-r--r--   0 aphearin   (501) staff       (20)     1449 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/photometry/utils.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.468880 dsps-0.3.1/dsps/sed/
--rw-r--r--   0 aphearin   (501) staff       (20)      147 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/sed/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3624 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/sed/metallicity_weights.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4386 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/sed/ssp_weights.py
--rw-r--r--   0 aphearin   (501) staff       (20)     5636 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/sed/stellar_age_weights.py
--rw-r--r--   0 aphearin   (501) staff       (20)     6139 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/sed/stellar_sed.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.471751 dsps-0.3.1/dsps/sed/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/sed/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     3222 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/sed/tests/test_csp_sed.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2130 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/sed/tests/test_metallicity_weights.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2994 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/sed/tests/test_ssp_weights.py
--rw-r--r--   0 aphearin   (501) staff       (20)     2957 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/sed/tests/test_stellar_age_weights.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.473008 dsps-0.3.1/dsps/tests/
--rw-r--r--   0 aphearin   (501) staff       (20)        0 2021-10-25 22:41:03.000000 dsps-0.3.1/dsps/tests/__init__.py
--rw-r--r--   0 aphearin   (501) staff       (20)     4234 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/tests/test_utils.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.484521 dsps-0.3.1/dsps/tests/testing_data/
--rw-r--r--   0 aphearin   (501) staff       (20)      328 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/tests/testing_data/fsps_lsst_mags_zobs.npy
--rw-r--r--   0 aphearin   (501) staff       (20)      792 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/tests/testing_data/fsps_lsst_mags_zobs_imet_20_iage_5.npy
--rw-r--r--   0 aphearin   (501) staff       (20)      792 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/tests/testing_data/fsps_lsst_mags_zobs_imet_2_iage_90.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    15832 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/tests/testing_data/fsps_ssp_imet_20_iage_5.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    15832 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/tests/testing_data/fsps_ssp_imet_2_iage_90.npy
--rw-r--r--   0 aphearin   (501) staff       (20)     3799 2021-10-26 18:12:12.000000 dsps-0.3.1/dsps/tests/testing_data/lgageray_myr.txt
--rw-r--r--   0 aphearin   (501) staff       (20)    14576 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/tests/testing_data/lsst_g_transmission.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    12688 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/tests/testing_data/lsst_i_transmission.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    13648 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/tests/testing_data/lsst_r_transmission.npy
--rw-r--r--   0 aphearin   (501) staff       (20)     7216 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/tests/testing_data/lsst_u_transmission.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    15376 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/tests/testing_data/lsst_y_transmission.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    10976 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/tests/testing_data/lsst_z_transmission.npy
--rw-r--r--   0 aphearin   (501) staff       (20)    53768 2021-11-08 14:32:51.000000 dsps-0.3.1/dsps/tests/testing_data/ssp_plaw_data_c0.txt
--rw-r--r--   0 aphearin   (501) staff       (20)    53390 2021-11-08 14:32:51.000000 dsps-0.3.1/dsps/tests/testing_data/ssp_plaw_data_c1.txt
--rw-r--r--   0 aphearin   (501) staff       (20)     5458 2023-04-29 18:27:09.000000 dsps-0.3.1/dsps/utils.py
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.410716 dsps-0.3.1/dsps.egg-info/
--rw-r--r--   0 aphearin   (501) staff       (20)     4101 2023-05-02 12:41:49.000000 dsps-0.3.1/dsps.egg-info/PKG-INFO
--rw-r--r--   0 aphearin   (501) staff       (20)     5668 2023-05-02 12:41:49.000000 dsps-0.3.1/dsps.egg-info/SOURCES.txt
--rw-r--r--   0 aphearin   (501) staff       (20)        1 2023-05-02 12:41:49.000000 dsps-0.3.1/dsps.egg-info/dependency_links.txt
--rw-r--r--   0 aphearin   (501) staff       (20)       15 2023-05-02 12:41:49.000000 dsps-0.3.1/dsps.egg-info/requires.txt
--rw-r--r--   0 aphearin   (501) staff       (20)       16 2023-05-02 12:41:49.000000 dsps-0.3.1/dsps.egg-info/top_level.txt
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.487683 dsps-0.3.1/notebooks/
--rw-r--r--   0 aphearin   (501) staff       (20)    72997 2021-11-17 23:25:46.000000 dsps-0.3.1/notebooks/tabulate_mstar_surviving_different_imfs.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)    70225 2021-10-27 11:32:35.000000 dsps-0.3.1/notebooks/validate_dsps_attenuation.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)     1222 2023-04-29 18:27:09.000000 dsps-0.3.1/pyproject.toml
--rw-r--r--   0 aphearin   (501) staff       (20)       14 2023-04-29 18:27:09.000000 dsps-0.3.1/requirements.txt
-drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-05-02 12:41:49.491245 dsps-0.3.1/scripts/
--rw-r--r--   0 aphearin   (501) staff       (20)    23049 2023-04-29 18:27:09.000000 dsps-0.3.1/scripts/generate_fsps_photometry_validation_data.ipynb
--rw-r--r--   0 aphearin   (501) staff       (20)      436 2023-04-29 18:27:09.000000 dsps-0.3.1/scripts/write_fsps_data_to_disk.py
--rw-r--r--   0 aphearin   (501) staff       (20)       38 2023-05-02 12:41:49.496044 dsps-0.3.1/setup.cfg
--rw-r--r--   0 aphearin   (501) staff       (20)       38 2023-04-29 18:27:09.000000 dsps-0.3.1/setup.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.385777 dsps-0.3.2/
+-rw-r--r--   0 aphearin   (501) staff       (20)       90 2022-09-09 13:28:37.000000 dsps-0.3.2/.coveragerc
+-rw-r--r--   0 aphearin   (501) staff       (20)      110 2023-05-03 20:18:18.000000 dsps-0.3.2/.git_archival.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)       31 2023-05-03 20:18:18.000000 dsps-0.3.2/.gitattributes
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.361889 dsps-0.3.2/.github/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.366016 dsps-0.3.2/.github/workflows/
+-rw-r--r--   0 aphearin   (501) staff       (20)     1089 2023-04-29 18:27:09.000000 dsps-0.3.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 aphearin   (501) staff       (20)     1150 2023-04-29 18:27:09.000000 dsps-0.3.2/.github/workflows/tests.yml
+-rw-r--r--   0 aphearin   (501) staff       (20)     1489 2023-04-29 18:27:09.000000 dsps-0.3.2/.gitignore
+-rw-r--r--   0 aphearin   (501) staff       (20)      212 2023-05-03 20:18:18.000000 dsps-0.3.2/.readthedocs.yml
+-rw-r--r--   0 aphearin   (501) staff       (20)     1071 2023-08-02 02:28:43.000000 dsps-0.3.2/CHANGES.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1521 2023-04-29 18:27:09.000000 dsps-0.3.2/LICENSE.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     4099 2023-08-02 02:34:12.385639 dsps-0.3.2/PKG-INFO
+-rw-r--r--   0 aphearin   (501) staff       (20)     1996 2023-05-10 19:07:23.000000 dsps-0.3.2/README.md
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.366377 dsps-0.3.2/docs/
+-rw-r--r--   0 aphearin   (501) staff       (20)      638 2023-04-29 18:27:09.000000 dsps-0.3.2/docs/Makefile
+-rw-r--r--   0 aphearin   (501) staff       (20)      804 2023-04-29 18:27:09.000000 dsps-0.3.2/docs/make.bat
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.367980 dsps-0.3.2/docs/source/
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.368108 dsps-0.3.2/docs/source/_static/
+-rw-r--r--   0 aphearin   (501) staff       (20)   129468 2023-04-29 18:27:09.000000 dsps-0.3.2/docs/source/_static/fake_ssp_seds.png
+-rw-r--r--   0 aphearin   (501) staff       (20)     1241 2023-04-29 18:27:09.000000 dsps-0.3.2/docs/source/citation.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1039 2023-04-29 18:27:09.000000 dsps-0.3.2/docs/source/conf.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2171 2023-05-03 20:18:18.000000 dsps-0.3.2/docs/source/custom_ssps.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     2044 2023-05-03 20:18:18.000000 dsps-0.3.2/docs/source/dsps_data_config.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     9494 2023-05-03 20:18:18.000000 dsps-0.3.2/docs/source/dsps_quickstart.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)     1062 2023-04-29 18:27:09.000000 dsps-0.3.2/docs/source/index.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      804 2023-05-03 20:18:18.000000 dsps-0.3.2/docs/source/installation.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)     1454 2023-05-03 20:18:18.000000 dsps-0.3.2/docs/source/quickstart.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)      309 2023-04-29 18:27:09.000000 dsps-0.3.2/docs/source/reference.rst
+-rw-r--r--   0 aphearin   (501) staff       (20)       62 2023-04-29 18:27:09.000000 dsps-0.3.2/docs/source/requirements.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)      127 2023-04-29 18:27:09.000000 dsps-0.3.2/docs/source/tutorials.rst
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.369135 dsps-0.3.2/dsps/
+-rw-r--r--   0 aphearin   (501) staff       (20)      173 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)       22 2023-08-02 02:34:12.000000 dsps-0.3.2/dsps/_version.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      186 2023-05-23 21:14:09.000000 dsps-0.3.2/dsps/constants.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.370013 dsps-0.3.2/dsps/cosmology/
+-rw-r--r--   0 aphearin   (501) staff       (20)      146 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/cosmology/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      198 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/cosmology/defaults.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6618 2023-05-23 21:14:09.000000 dsps-0.3.2/dsps/cosmology/flat_wcdm.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.370319 dsps-0.3.2/dsps/cosmology/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/cosmology/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5975 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/cosmology/tests/test_flat_wcdm.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.370539 dsps-0.3.2/dsps/data/
+-rw-r--r--   0 aphearin   (501) staff       (20)     2552 2023-05-10 19:47:34.000000 dsps-0.3.2/dsps/data/README.txt
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.371218 dsps-0.3.2/dsps/data_loaders/
+-rw-r--r--   0 aphearin   (501) staff       (20)      250 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/data_loaders/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1165 2023-05-03 20:18:18.000000 dsps-0.3.2/dsps/data_loaders/defaults.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2564 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/data_loaders/load_filter_data.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2252 2023-05-03 20:18:18.000000 dsps-0.3.2/dsps/data_loaders/load_ssp_data.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3416 2023-05-23 21:14:09.000000 dsps-0.3.2/dsps/data_loaders/retrieve_fake_fsps_data.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2460 2023-08-02 02:27:01.000000 dsps-0.3.2/dsps/data_loaders/retrieve_fsps_data.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.371635 dsps-0.3.2/dsps/data_loaders/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/data_loaders/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1707 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/data_loaders/tests/test_load_filter_data.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      797 2023-05-10 19:07:18.000000 dsps-0.3.2/dsps/data_loaders/tests/test_load_ssp_data.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1042 2023-05-03 20:18:18.000000 dsps-0.3.2/dsps/data_loaders/tests/test_retrieve_fake_fsps_data.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.371878 dsps-0.3.2/dsps/data_loaders/tests/testing_data/
+-rw-r--r--   0 aphearin   (501) staff       (20)    53768 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/data_loaders/tests/testing_data/ssp_plaw_data_c0.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)    53390 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/data_loaders/tests/testing_data/ssp_plaw_data_c1.txt
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.372584 dsps-0.3.2/dsps/dust/
+-rw-r--r--   0 aphearin   (501) staff       (20)       48 2023-06-01 17:10:30.000000 dsps-0.3.2/dsps/dust/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)    12142 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/att_curves.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3215 2023-06-01 17:10:30.000000 dsps-0.3.2/dsps/dust/blackbody.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.373132 dsps-0.3.2/dsps/dust/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5152 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/test_att_curves.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3379 2023-06-01 17:10:30.000000 dsps-0.3.2/dsps/dust/tests/test_blackbody.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      983 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/test_utils.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.375089 dsps-0.3.2/dsps/dust/tests/testing_data/
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/calzetti_2000_attenuation.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/calzetti_2000_k_lambda.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/calzetti_2000_wavelength_microns.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/leitherer_2002_attenuation.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/leitherer_2002_k_lambda.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/leitherer_2002_wavelength_microns.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2558 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_attenuation1.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2554 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_attenuation2.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2555 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_attenuation3.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2558 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_k_lambda1.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2554 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_k_lambda2.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2555 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_k_lambda3.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_wavelength_microns.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2554 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/salim_2018_attenuation1.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2556 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/salim_2018_attenuation2.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2554 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/salim_2018_k_lambda1.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2556 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/salim_2018_k_lambda2.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2500 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/tests/testing_data/salim_2018_wavelength_microns.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)      704 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/dust/utils.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.375264 dsps-0.3.2/dsps/em_lines/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/em_lines/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1699 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/em_lines/equivalent_width.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.375545 dsps-0.3.2/dsps/em_lines/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/em_lines/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1131 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/em_lines/tests/test_equivalent_width.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.375798 dsps-0.3.2/dsps/experimental/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/experimental/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3161 2023-05-03 20:18:18.000000 dsps-0.3.2/dsps/experimental/diffburst.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.376001 dsps-0.3.2/dsps/experimental/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/experimental/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5178 2023-05-03 20:18:18.000000 dsps-0.3.2/dsps/experimental/tests/test_diffburst.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.376319 dsps-0.3.2/dsps/imf/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1463 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/remnant_mass.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1822 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/surviving_mstar.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.376645 dsps-0.3.2/dsps/imf/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2830 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/tests/test_remnant_mass.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1917 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/tests/test_surviving_mstar.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.377540 dsps-0.3.2/dsps/imf/tests/testing_data/
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/tests/testing_data/chabrier_mstar_surviving.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/tests/testing_data/chabrier_mstar_surviving_norem.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/tests/testing_data/kroupa_mstar_surviving.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/tests/testing_data/kroupa_mstar_surviving_norem.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/tests/testing_data/lg_ages_mstar_surviving.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/tests/testing_data/salpeter_mstar_surviving.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/tests/testing_data/salpeter_mstar_surviving_norem.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/tests/testing_data/van_dokkum_mstar_surviving.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     2350 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/imf/tests/testing_data/van_dokkum_mstar_surviving_norem.txt
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.377709 dsps-0.3.2/dsps/metallicity/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/metallicity/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3962 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/metallicity/mzr.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.377912 dsps-0.3.2/dsps/metallicity/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/metallicity/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)      842 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/metallicity/tests/test_mzr.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.378800 dsps-0.3.2/dsps/metallicity/tests/testing_data/
+-rw-r--r--   0 aphearin   (501) staff       (20)      612 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/metallicity/tests/testing_data/galazzi_etal05_mzr.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)     1340 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/metallicity/tests/testing_data/kirby_etal13_mzr.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)      613 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/metallicity/tests/testing_data/kudritzki_etal16_mzr.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)     1010 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/metallicity/tests/testing_data/maiolino_etal18_mzr.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)      257 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/metallicity/tests/testing_data/trussler_etal20_mzr_all_centrals_sdss_dr7.dat
+-rw-r--r--   0 aphearin   (501) staff       (20)      259 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/metallicity/tests/testing_data/trussler_etal20_mzr_all_sats_sdss_dr7.dat
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.379252 dsps-0.3.2/dsps/photometry/
+-rw-r--r--   0 aphearin   (501) staff       (20)       57 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/photometry/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3312 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/photometry/photometry_kernels.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3030 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/photometry/photpop.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.379559 dsps-0.3.2/dsps/photometry/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/photometry/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2566 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/photometry/tests/test_photometry_kernels.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1646 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/photometry/tests/test_photpop.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     1449 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/photometry/utils.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.380183 dsps-0.3.2/dsps/sed/
+-rw-r--r--   0 aphearin   (501) staff       (20)      147 2023-05-23 21:14:09.000000 dsps-0.3.2/dsps/sed/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3624 2023-05-03 20:18:18.000000 dsps-0.3.2/dsps/sed/metallicity_weights.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4386 2023-05-03 20:18:18.000000 dsps-0.3.2/dsps/sed/ssp_weights.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     5636 2023-05-03 20:18:18.000000 dsps-0.3.2/dsps/sed/stellar_age_weights.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     6139 2023-05-23 21:14:09.000000 dsps-0.3.2/dsps/sed/stellar_sed.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.380820 dsps-0.3.2/dsps/sed/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/sed/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     3222 2023-05-03 20:18:18.000000 dsps-0.3.2/dsps/sed/tests/test_csp_sed.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2130 2023-05-03 20:18:18.000000 dsps-0.3.2/dsps/sed/tests/test_metallicity_weights.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2994 2023-05-03 20:18:18.000000 dsps-0.3.2/dsps/sed/tests/test_ssp_weights.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     2957 2023-05-03 20:18:18.000000 dsps-0.3.2/dsps/sed/tests/test_stellar_age_weights.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.381022 dsps-0.3.2/dsps/tests/
+-rw-r--r--   0 aphearin   (501) staff       (20)        0 2021-10-25 22:41:03.000000 dsps-0.3.2/dsps/tests/__init__.py
+-rw-r--r--   0 aphearin   (501) staff       (20)     4234 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/tests/test_utils.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.383008 dsps-0.3.2/dsps/tests/testing_data/
+-rw-r--r--   0 aphearin   (501) staff       (20)      328 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/tests/testing_data/fsps_lsst_mags_zobs.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)      792 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/tests/testing_data/fsps_lsst_mags_zobs_imet_20_iage_5.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)      792 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/tests/testing_data/fsps_lsst_mags_zobs_imet_2_iage_90.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    15832 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/tests/testing_data/fsps_ssp_imet_20_iage_5.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    15832 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/tests/testing_data/fsps_ssp_imet_2_iage_90.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)     3799 2021-10-26 18:12:12.000000 dsps-0.3.2/dsps/tests/testing_data/lgageray_myr.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)    14576 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/tests/testing_data/lsst_g_transmission.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    12688 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/tests/testing_data/lsst_i_transmission.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    13648 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/tests/testing_data/lsst_r_transmission.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)     7216 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/tests/testing_data/lsst_u_transmission.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    15376 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/tests/testing_data/lsst_y_transmission.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    10976 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/tests/testing_data/lsst_z_transmission.npy
+-rw-r--r--   0 aphearin   (501) staff       (20)    53768 2021-11-08 14:32:51.000000 dsps-0.3.2/dsps/tests/testing_data/ssp_plaw_data_c0.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)    53390 2021-11-08 14:32:51.000000 dsps-0.3.2/dsps/tests/testing_data/ssp_plaw_data_c1.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)     5458 2023-04-29 18:27:09.000000 dsps-0.3.2/dsps/utils.py
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.369668 dsps-0.3.2/dsps.egg-info/
+-rw-r--r--   0 aphearin   (501) staff       (20)     4099 2023-08-02 02:34:12.000000 dsps-0.3.2/dsps.egg-info/PKG-INFO
+-rw-r--r--   0 aphearin   (501) staff       (20)     5725 2023-08-02 02:34:12.000000 dsps-0.3.2/dsps.egg-info/SOURCES.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)        1 2023-08-02 02:34:12.000000 dsps-0.3.2/dsps.egg-info/dependency_links.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)       15 2023-08-02 02:34:12.000000 dsps-0.3.2/dsps.egg-info/requires.txt
+-rw-r--r--   0 aphearin   (501) staff       (20)       10 2023-08-02 02:34:12.000000 dsps-0.3.2/dsps.egg-info/top_level.txt
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.383442 dsps-0.3.2/notebooks/
+-rw-r--r--   0 aphearin   (501) staff       (20)    72997 2021-11-17 23:25:46.000000 dsps-0.3.2/notebooks/tabulate_mstar_surviving_different_imfs.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)    70225 2021-10-27 11:32:35.000000 dsps-0.3.2/notebooks/validate_dsps_attenuation.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)     1222 2023-04-29 18:27:09.000000 dsps-0.3.2/pyproject.toml
+-rw-r--r--   0 aphearin   (501) staff       (20)       14 2023-04-29 18:27:09.000000 dsps-0.3.2/requirements.txt
+drwxr-xr-x   0 aphearin   (501) staff       (20)        0 2023-08-02 02:34:12.385439 dsps-0.3.2/scripts/
+-rw-r--r--   0 aphearin   (501) staff       (20)    23049 2023-04-29 18:27:09.000000 dsps-0.3.2/scripts/generate_fsps_photometry_validation_data.ipynb
+-rw-r--r--   0 aphearin   (501) staff       (20)      436 2023-04-29 18:27:09.000000 dsps-0.3.2/scripts/write_fsps_data_to_disk.py
+-rw-r--r--   0 aphearin   (501) staff       (20)       38 2023-08-02 02:34:12.385809 dsps-0.3.2/setup.cfg
+-rw-r--r--   0 aphearin   (501) staff       (20)       38 2023-04-29 18:27:09.000000 dsps-0.3.2/setup.py
```

### Comparing `dsps-0.3.1/.github/workflows/publish-to-pypi.yml` & `dsps-0.3.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/.github/workflows/tests.yml` & `dsps-0.3.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/.gitignore` & `dsps-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/CHANGES.rst` & `dsps-0.3.2/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.3.2 (2023-08-01)
+-------------------
+- Fix bug leading to edge case in which FSPS is assumed to be installed and configured (https://github.com/ArgonneCPAC/dsps/pull/68)
+
 0.3.1 (2023-05-02)
 -------------------
 - Include .git_archival.txt and .gitattributes to help with versioning (https://github.com/ArgonneCPAC/dsps/pull/61)
 
 0.3.0 (2023-05-01)
 -------------------
 - Package DSPS using pyproject.toml (https://github.com/ArgonneCPAC/dsps/pull/43)
```

### Comparing `dsps-0.3.1/LICENSE.rst` & `dsps-0.3.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/PKG-INFO` & `dsps-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsps
-Version: 0.3.1
+Version: 0.3.2
 Summary: Differentiable Stellar Population Synthesis
 Author-email: Andrew Hearin <ahearin@anl.gov>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Andrew Hearin
         All rights reserved.
         
@@ -42,15 +42,15 @@
 # dsps
 [![tests](https://github.com/ArgonneCPAC/dsps/actions/workflows/tests.yml/badge.svg)](https://github.com/ArgonneCPAC/dsps/actions/workflows/tests.yml)
 
 Differentiable Stellar Population Synthesis
 
 ## Installation
 
-The latest release of DSPS is v0.3.0, which is now available for pip installation:
+The latest release of DSPS is v0.3, which is now available for pip installation:
 ```
 $ pip install dsps
 ```
 
 Alternatively, the latest release is also available on conda-forge:
 ```
 $ conda install -c conda-forge dsps
```

### Comparing `dsps-0.3.1/README.md` & `dsps-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # dsps
 [![tests](https://github.com/ArgonneCPAC/dsps/actions/workflows/tests.yml/badge.svg)](https://github.com/ArgonneCPAC/dsps/actions/workflows/tests.yml)
 
 Differentiable Stellar Population Synthesis
 
 ## Installation
 
-The latest release of DSPS is v0.3.0, which is now available for pip installation:
+The latest release of DSPS is v0.3, which is now available for pip installation:
 ```
 $ pip install dsps
 ```
 
 Alternatively, the latest release is also available on conda-forge:
 ```
 $ conda install -c conda-forge dsps
```

### Comparing `dsps-0.3.1/docs/Makefile` & `dsps-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/docs/make.bat` & `dsps-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/docs/source/_static/fake_ssp_seds.png` & `dsps-0.3.2/docs/source/_static/fake_ssp_seds.png`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/docs/source/citation.rst` & `dsps-0.3.2/docs/source/citation.rst`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/docs/source/conf.py` & `dsps-0.3.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/docs/source/custom_ssps.rst` & `dsps-0.3.2/docs/source/custom_ssps.rst`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/docs/source/dsps_data_config.rst` & `dsps-0.3.2/docs/source/dsps_data_config.rst`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/docs/source/dsps_quickstart.ipynb` & `dsps-0.3.2/docs/source/dsps_quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/docs/source/index.rst` & `dsps-0.3.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/docs/source/installation.rst` & `dsps-0.3.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/docs/source/quickstart.rst` & `dsps-0.3.2/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/cosmology/flat_wcdm.py` & `dsps-0.3.2/dsps/cosmology/flat_wcdm.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/cosmology/tests/test_flat_wcdm.py` & `dsps-0.3.2/dsps/cosmology/tests/test_flat_wcdm.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/data/README.txt` & `dsps-0.3.2/dsps/data/README.txt`

 * *Files 5% similar despite different names*

```diff
@@ -48,7 +48,13 @@
 
 >>> from dsps.data_loaders import load_transmission_curve
 >>> trans_curve = load_transmission_curve("/path/to/dsps/data/lsst_r*")
 
 If you have set the DSPS_DRN environment variable to your default data location,
 then you will need to store transmission curves in the DSPS_DRN/filters subdirectory.
 See the Quickstart Guide on dsps.readthedocs.io for more information.
+
+
+Alternate SSP data
+------------------
+The ssp_data_continuum_fsps_v3.2_lgmet_age.h5 file was run with the add_neb_emission 
+keyword set to False, so these SSPs can be treated as stellar continuum SSPs.
```

### Comparing `dsps-0.3.1/dsps/data_loaders/defaults.py` & `dsps-0.3.2/dsps/data_loaders/defaults.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/data_loaders/load_filter_data.py` & `dsps-0.3.2/dsps/data_loaders/load_filter_data.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/data_loaders/load_ssp_data.py` & `dsps-0.3.2/dsps/data_loaders/load_ssp_data.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/data_loaders/retrieve_fake_fsps_data.py` & `dsps-0.3.2/dsps/data_loaders/retrieve_fake_fsps_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 """
 import numpy as np
-from scipy.stats import norm
+from jax.scipy.stats import norm
 import os
 from .defaults import SSPData
 
 
 _THIS_DRNAME = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `dsps-0.3.1/dsps/data_loaders/retrieve_fsps_data.py` & `dsps-0.3.2/dsps/data_loaders/retrieve_fsps_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 """Use python-fsps to retrieve a block of Simple Stellar Population (SSP) data"""
 import numpy as np
 
 try:
     import fsps
 
     HAS_FSPS = True
-except ImportError:
+except (ImportError, RuntimeError):
     HAS_FSPS = False
 
 from .load_ssp_data import SSPData
 
 
-def retrieve_ssp_data_from_fsps():
+def retrieve_ssp_data_from_fsps(add_neb_emission=True, **kwargs):
     """Use python-fsps to populate arrays and matrices of data
     for the default simple stellar populations (SSPs) in the shapes expected by DSPS
 
+    Parameters
+    ----------
+    add_neb_emission : bool, optional
+        Argument passed to fsps.StellarPopulation. Default is True.
+
+    kwargs : optional
+        Any keyword arguments passed to the retrieve_ssp_data_from_fsps function will be
+        passed on to fsps.StellarPopulation.
+
     Returns
     -------
     ssp_lgmet : ndarray of shape (n_met, )
         Array of log10(Z) of the SSP templates
         where dimensionless Z is the mass fraction of elements heavier than He
 
     ssp_lg_age_gyr : ndarray of shape (n_ages, )
@@ -48,15 +57,15 @@
     ssp_lgmet = np.log10(sp.zlegend)
     nzmet = ssp_lgmet.size
     ssp_lg_age_gyr = sp.log_age - 9.0
     spectrum_collector = []
     for zmet_indx in range(1, ssp_lgmet.size + 1):
         print("...retrieving zmet = {0} of {1}".format(zmet_indx, nzmet))
         sp = fsps.StellarPopulation(
-            zcontinuous=0, zmet=zmet_indx, add_neb_emission=True
+            zcontinuous=0, zmet=zmet_indx, add_neb_emission=add_neb_emission, **kwargs
         )
         _wave, _fluxes = sp.get_spectrum()
         spectrum_collector.append(_fluxes)
     ssp_wave = np.array(_wave)
     ssp_flux = np.array(spectrum_collector)
 
     return SSPData(ssp_lgmet, ssp_lg_age_gyr, ssp_wave, ssp_flux)
```

### Comparing `dsps-0.3.1/dsps/data_loaders/tests/test_load_filter_data.py` & `dsps-0.3.2/dsps/data_loaders/tests/test_load_filter_data.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/data_loaders/tests/test_load_ssp_data.py` & `dsps-0.3.2/dsps/data_loaders/tests/test_load_ssp_data.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/data_loaders/tests/test_retrieve_fake_fsps_data.py` & `dsps-0.3.2/dsps/data_loaders/tests/test_retrieve_fake_fsps_data.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/data_loaders/tests/testing_data/ssp_plaw_data_c0.txt` & `dsps-0.3.2/dsps/data_loaders/tests/testing_data/ssp_plaw_data_c0.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/data_loaders/tests/testing_data/ssp_plaw_data_c1.txt` & `dsps-0.3.2/dsps/data_loaders/tests/testing_data/ssp_plaw_data_c1.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/att_curves.py` & `dsps-0.3.2/dsps/dust/att_curves.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/test_att_curves.py` & `dsps-0.3.2/dsps/dust/tests/test_att_curves.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/test_utils.py` & `dsps-0.3.2/dsps/dust/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/calzetti_2000_attenuation.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/calzetti_2000_attenuation.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/calzetti_2000_k_lambda.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/calzetti_2000_k_lambda.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/calzetti_2000_wavelength_microns.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/calzetti_2000_wavelength_microns.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/leitherer_2002_attenuation.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/leitherer_2002_attenuation.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/leitherer_2002_k_lambda.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/leitherer_2002_k_lambda.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/leitherer_2002_wavelength_microns.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/leitherer_2002_wavelength_microns.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_attenuation1.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_attenuation1.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_attenuation2.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_attenuation2.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_attenuation3.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_attenuation3.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_k_lambda1.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_k_lambda1.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_k_lambda2.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_k_lambda2.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_k_lambda3.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_k_lambda3.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/noll_2009_wavelength_microns.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/noll_2009_wavelength_microns.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/salim_2018_attenuation1.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/salim_2018_attenuation1.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/salim_2018_attenuation2.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/salim_2018_attenuation2.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/salim_2018_k_lambda1.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/salim_2018_k_lambda1.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/salim_2018_k_lambda2.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/salim_2018_k_lambda2.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/tests/testing_data/salim_2018_wavelength_microns.txt` & `dsps-0.3.2/dsps/dust/tests/testing_data/salim_2018_wavelength_microns.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/dust/utils.py` & `dsps-0.3.2/dsps/dust/utils.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/em_lines/equivalent_width.py` & `dsps-0.3.2/dsps/em_lines/equivalent_width.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/em_lines/tests/test_equivalent_width.py` & `dsps-0.3.2/dsps/em_lines/tests/test_equivalent_width.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/experimental/diffburst.py` & `dsps-0.3.2/dsps/experimental/diffburst.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/experimental/tests/test_diffburst.py` & `dsps-0.3.2/dsps/experimental/tests/test_diffburst.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/imf/remnant_mass.py` & `dsps-0.3.2/dsps/imf/remnant_mass.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/imf/surviving_mstar.py` & `dsps-0.3.2/dsps/imf/surviving_mstar.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/imf/tests/test_remnant_mass.py` & `dsps-0.3.2/dsps/imf/tests/test_remnant_mass.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/imf/tests/test_surviving_mstar.py` & `dsps-0.3.2/dsps/imf/tests/test_surviving_mstar.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/imf/tests/testing_data/chabrier_mstar_surviving.txt` & `dsps-0.3.2/dsps/imf/tests/testing_data/chabrier_mstar_surviving.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/imf/tests/testing_data/chabrier_mstar_surviving_norem.txt` & `dsps-0.3.2/dsps/imf/tests/testing_data/chabrier_mstar_surviving_norem.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/imf/tests/testing_data/kroupa_mstar_surviving.txt` & `dsps-0.3.2/dsps/imf/tests/testing_data/kroupa_mstar_surviving.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/imf/tests/testing_data/kroupa_mstar_surviving_norem.txt` & `dsps-0.3.2/dsps/imf/tests/testing_data/kroupa_mstar_surviving_norem.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/imf/tests/testing_data/lg_ages_mstar_surviving.txt` & `dsps-0.3.2/dsps/imf/tests/testing_data/lg_ages_mstar_surviving.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/imf/tests/testing_data/salpeter_mstar_surviving.txt` & `dsps-0.3.2/dsps/imf/tests/testing_data/salpeter_mstar_surviving.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/imf/tests/testing_data/salpeter_mstar_surviving_norem.txt` & `dsps-0.3.2/dsps/imf/tests/testing_data/salpeter_mstar_surviving_norem.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/imf/tests/testing_data/van_dokkum_mstar_surviving.txt` & `dsps-0.3.2/dsps/imf/tests/testing_data/van_dokkum_mstar_surviving.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/imf/tests/testing_data/van_dokkum_mstar_surviving_norem.txt` & `dsps-0.3.2/dsps/imf/tests/testing_data/van_dokkum_mstar_surviving_norem.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/metallicity/mzr.py` & `dsps-0.3.2/dsps/metallicity/mzr.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/metallicity/tests/test_mzr.py` & `dsps-0.3.2/dsps/metallicity/tests/test_mzr.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/metallicity/tests/testing_data/galazzi_etal05_mzr.dat` & `dsps-0.3.2/dsps/metallicity/tests/testing_data/galazzi_etal05_mzr.dat`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/metallicity/tests/testing_data/kirby_etal13_mzr.dat` & `dsps-0.3.2/dsps/metallicity/tests/testing_data/kirby_etal13_mzr.dat`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/metallicity/tests/testing_data/kudritzki_etal16_mzr.dat` & `dsps-0.3.2/dsps/metallicity/tests/testing_data/kudritzki_etal16_mzr.dat`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/metallicity/tests/testing_data/maiolino_etal18_mzr.dat` & `dsps-0.3.2/dsps/metallicity/tests/testing_data/maiolino_etal18_mzr.dat`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/photometry/photometry_kernels.py` & `dsps-0.3.2/dsps/photometry/photometry_kernels.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/photometry/photpop.py` & `dsps-0.3.2/dsps/photometry/photpop.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/photometry/tests/test_photometry_kernels.py` & `dsps-0.3.2/dsps/photometry/tests/test_photometry_kernels.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/photometry/tests/test_photpop.py` & `dsps-0.3.2/dsps/photometry/tests/test_photpop.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/photometry/utils.py` & `dsps-0.3.2/dsps/photometry/utils.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/sed/metallicity_weights.py` & `dsps-0.3.2/dsps/sed/metallicity_weights.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/sed/ssp_weights.py` & `dsps-0.3.2/dsps/sed/ssp_weights.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/sed/stellar_age_weights.py` & `dsps-0.3.2/dsps/sed/stellar_age_weights.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/sed/stellar_sed.py` & `dsps-0.3.2/dsps/sed/stellar_sed.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/sed/tests/test_csp_sed.py` & `dsps-0.3.2/dsps/sed/tests/test_csp_sed.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/sed/tests/test_metallicity_weights.py` & `dsps-0.3.2/dsps/sed/tests/test_metallicity_weights.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/sed/tests/test_ssp_weights.py` & `dsps-0.3.2/dsps/sed/tests/test_ssp_weights.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/sed/tests/test_stellar_age_weights.py` & `dsps-0.3.2/dsps/sed/tests/test_stellar_age_weights.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/test_utils.py` & `dsps-0.3.2/dsps/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/testing_data/fsps_lsst_mags_zobs_imet_20_iage_5.npy` & `dsps-0.3.2/dsps/tests/testing_data/fsps_lsst_mags_zobs_imet_20_iage_5.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/testing_data/fsps_lsst_mags_zobs_imet_2_iage_90.npy` & `dsps-0.3.2/dsps/tests/testing_data/fsps_lsst_mags_zobs_imet_2_iage_90.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/testing_data/fsps_ssp_imet_20_iage_5.npy` & `dsps-0.3.2/dsps/tests/testing_data/fsps_ssp_imet_20_iage_5.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/testing_data/fsps_ssp_imet_2_iage_90.npy` & `dsps-0.3.2/dsps/tests/testing_data/fsps_ssp_imet_2_iage_90.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/testing_data/lgageray_myr.txt` & `dsps-0.3.2/dsps/tests/testing_data/lgageray_myr.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/testing_data/lsst_g_transmission.npy` & `dsps-0.3.2/dsps/tests/testing_data/lsst_g_transmission.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/testing_data/lsst_i_transmission.npy` & `dsps-0.3.2/dsps/tests/testing_data/lsst_i_transmission.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/testing_data/lsst_r_transmission.npy` & `dsps-0.3.2/dsps/tests/testing_data/lsst_r_transmission.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/testing_data/lsst_u_transmission.npy` & `dsps-0.3.2/dsps/tests/testing_data/lsst_u_transmission.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/testing_data/lsst_y_transmission.npy` & `dsps-0.3.2/dsps/tests/testing_data/lsst_y_transmission.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/testing_data/lsst_z_transmission.npy` & `dsps-0.3.2/dsps/tests/testing_data/lsst_z_transmission.npy`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/testing_data/ssp_plaw_data_c0.txt` & `dsps-0.3.2/dsps/tests/testing_data/ssp_plaw_data_c0.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/tests/testing_data/ssp_plaw_data_c1.txt` & `dsps-0.3.2/dsps/tests/testing_data/ssp_plaw_data_c1.txt`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps/utils.py` & `dsps-0.3.2/dsps/utils.py`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/dsps.egg-info/PKG-INFO` & `dsps-0.3.2/dsps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsps
-Version: 0.3.1
+Version: 0.3.2
 Summary: Differentiable Stellar Population Synthesis
 Author-email: Andrew Hearin <ahearin@anl.gov>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Andrew Hearin
         All rights reserved.
         
@@ -42,15 +42,15 @@
 # dsps
 [![tests](https://github.com/ArgonneCPAC/dsps/actions/workflows/tests.yml/badge.svg)](https://github.com/ArgonneCPAC/dsps/actions/workflows/tests.yml)
 
 Differentiable Stellar Population Synthesis
 
 ## Installation
 
-The latest release of DSPS is v0.3.0, which is now available for pip installation:
+The latest release of DSPS is v0.3, which is now available for pip installation:
 ```
 $ pip install dsps
 ```
 
 Alternatively, the latest release is also available on conda-forge:
 ```
 $ conda install -c conda-forge dsps
```

### Comparing `dsps-0.3.1/dsps.egg-info/SOURCES.txt` & `dsps-0.3.2/dsps.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,19 @@
 dsps/data_loaders/tests/test_load_filter_data.py
 dsps/data_loaders/tests/test_load_ssp_data.py
 dsps/data_loaders/tests/test_retrieve_fake_fsps_data.py
 dsps/data_loaders/tests/testing_data/ssp_plaw_data_c0.txt
 dsps/data_loaders/tests/testing_data/ssp_plaw_data_c1.txt
 dsps/dust/__init__.py
 dsps/dust/att_curves.py
+dsps/dust/blackbody.py
 dsps/dust/utils.py
 dsps/dust/tests/__init__.py
 dsps/dust/tests/test_att_curves.py
+dsps/dust/tests/test_blackbody.py
 dsps/dust/tests/test_utils.py
 dsps/dust/tests/testing_data/calzetti_2000_attenuation.txt
 dsps/dust/tests/testing_data/calzetti_2000_k_lambda.txt
 dsps/dust/tests/testing_data/calzetti_2000_wavelength_microns.txt
 dsps/dust/tests/testing_data/leitherer_2002_attenuation.txt
 dsps/dust/tests/testing_data/leitherer_2002_k_lambda.txt
 dsps/dust/tests/testing_data/leitherer_2002_wavelength_microns.txt
```

### Comparing `dsps-0.3.1/notebooks/tabulate_mstar_surviving_different_imfs.ipynb` & `dsps-0.3.2/notebooks/tabulate_mstar_surviving_different_imfs.ipynb`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/notebooks/validate_dsps_attenuation.ipynb` & `dsps-0.3.2/notebooks/validate_dsps_attenuation.ipynb`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/pyproject.toml` & `dsps-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsps-0.3.1/scripts/generate_fsps_photometry_validation_data.ipynb` & `dsps-0.3.2/scripts/generate_fsps_photometry_validation_data.ipynb`

 * *Files identical despite different names*

