# Comparing `tmp/picca-7.2.0.tar.gz` & `tmp/picca-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picca-7.2.0.tar", last modified: Tue Jul 18 07:19:34 2023, max compression
+gzip compressed data, was "picca-8.0.0.tar", last modified: Wed Aug  2 08:40:33 2023, max compression
```

## Comparing `picca-7.2.0.tar` & `picca-8.0.0.tar`

### file list

```diff
@@ -1,215 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.230544 picca-7.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-18 07:19:16.000000 picca-7.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-18 07:19:34.230544 picca-7.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-18 07:19:16.000000 picca-7.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.194542 picca-7.2.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_Pk1D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_Pk1D_postprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_cf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_cf1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_cf_angl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_co.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_coadd_zint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_compute_fvoigt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_compute_pk_pksb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_convert_transmission.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_delta_extraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_dmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12239 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_export.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_export_co.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_export_cross_covariance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_metal_dmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_metal_xdmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_nersc_submit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_pk2fits.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_plot_pk1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_reduce_spall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_wick.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_xcf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12022 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_xcf1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_xcf_angl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_xdmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_xwick.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.190541 picca-7.2.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.198542 picca-7.2.0/py/picca/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bal_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.206542 picca-7.2.0/py/picca/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.206542 picca-7.2.0/py/picca/bin/old/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43689 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/old/picca_deltas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/old/picca_fitter2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/old/picca_fitter2_control.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/old/picca_fitter2_control_mpi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_Pk1D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_Pk1D_postprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_cf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_cf1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_cf_angl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_co.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_coadd_zint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_compute_fvoigt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_compute_pk_pksb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_convert_transmission.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_delta_extraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_dmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12239 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_export.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_export_co.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_export_cross_covariance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_metal_dmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_metal_xdmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_nersc_submit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_pk2fits.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_plot_pk1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_reduce_spall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_wick.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_xcf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12022 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_xcf1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_xcf_angl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_xdmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_xwick.py
--rw-r--r--   0 runner    (1001) docker     (123)    64077 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/cf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/co.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    51080 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.210543 picca-7.2.0/py/picca/delta_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.210543 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    25713 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    27062 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.210543 picca-7.2.0/py/picca/delta_extraction/corrections/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/corrections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/corrections/calibration_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/corrections/dust_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/corrections/ivar_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/corrections/optical_depth_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)    22238 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.214543 picca-7.2.0/py/picca/delta_extraction/data_catalogues/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data_catalogues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data_catalogues/desi_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data_catalogues/desi_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data_catalogues/sdss_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.214543 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29855 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.218543 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/
--rw-r--r--   0 runner    (1001) docker     (123)    98923 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_0.8.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    26124 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    28890 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    20204 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.218543 picca-7.2.0/py/picca/delta_extraction/least_squares/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/least_squares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/mask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.218543 picca-7.2.0/py/picca/delta_extraction/masks/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/masks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/masks/absorber_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/masks/bal_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/masks/dla_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/masks/lines_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/quasar_catalogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.218543 picca-7.2.0/py/picca/delta_extraction/quasar_catalogues/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/quasar_catalogues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/rejection_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.218543 picca-7.2.0/py/picca/delta_extraction/rejection_logs/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/rejection_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/utils_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/dla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.222544 picca-7.2.0/py/picca/fitter2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/chi2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/control_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6784 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/effective-bins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.190541 picca-7.2.0/py/picca/fitter2/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.222544 picca-7.2.0/py/picca/fitter2/models/DR16_blind_test_large/
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.222544 picca-7.2.0/py/picca/fitter2/models/DR16_blind_test_small/
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.222544 picca-7.2.0/py/picca/fitter2/models/DR9LyaMocks/
--rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.222544 picca-7.2.0/py/picca/fitter2/models/Planck18/
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/Planck18/Planck18_z_2.406.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.226544 picca-7.2.0/py/picca/fitter2/models/PlanckDR12/
--rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.226544 picca-7.2.0/py/picca/fitter2/models/PlanckDR16/
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/myGamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16465 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/pk.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/priors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/xi.py
--rw-r--r--   0 runner    (1001) docker     (123)    64892 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.226544 picca-7.2.0/py/picca/pk1d/
--rw-r--r--   0 runner    (1001) docker     (123)    19994 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/pk1d/compute_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    38897 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/pk1d/postproc_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/pk1d/prep_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/pk1d/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/prep_del.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/raw_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.226544 picca-7.2.0/py/picca/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.230544 picca-7.2.0/py/picca/tests/delta_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/tests/delta_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/tests/delta_extraction/abstract_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    88977 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/tests/delta_extraction/astronomical_object_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/tests/delta_extraction/config_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/tests/delta_extraction/correction_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    63846 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/delta_extraction/data_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    81524 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/delta_extraction/expected_flux_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    31381 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/delta_extraction/mask_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/delta_extraction/scripts_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/delta_extraction/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.230544 picca-7.2.0/py/picca/tests/old/
--rw-r--r--   0 runner    (1001) docker     (123)    17429 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/old/test_1_deltas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/old/test_4_fitter2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/test_2_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    42559 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/test_3_cor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16216 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/wedgize.py
--rw-r--r--   0 runner    (1001) docker     (123)    40690 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/xcf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.198542 picca-7.2.0/py/picca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-18 07:19:34.000000 picca-7.2.0/py/picca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-18 07:19:34.000000 picca-7.2.0/py/picca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:19:34.000000 picca-7.2.0/py/picca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-18 07:19:34.000000 picca-7.2.0/py/picca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 07:19:34.000000 picca-7.2.0/py/picca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-18 07:19:19.000000 picca-7.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:19:34.230544 picca-7.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-18 07:19:19.000000 picca-7.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.976513 picca-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-08-02 08:40:18.000000 picca-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-08-02 08:40:33.972512 picca-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-08-02 08:40:18.000000 picca-8.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.944512 picca-8.0.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_Pk1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_Pk1D_postprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_cf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_cf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_cf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_coadd_zint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_compute_fvoigt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_compute_pk_pksb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_convert_transmission.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_delta_extraction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12609 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_export.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_export_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_export_cross_covariance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_metal_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_metal_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_nersc_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_pk2fits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_plot_pk1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_reduce_spall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_wick.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_xcf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12022 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_xcf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_xcf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-08-02 08:40:18.000000 picca-8.0.0/bin/picca_xwick.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.936512 picca-8.0.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.948512 picca-8.0.0/py/picca/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.956512 picca-8.0.0/py/picca/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_Pk1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_Pk1D_postprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_cf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_cf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_cf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_coadd_zint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_compute_fvoigt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_compute_pk_pksb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_convert_transmission.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_delta_extraction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12609 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_export.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_export_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_export_cross_covariance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_metal_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_metal_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_nersc_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_pk2fits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_plot_pk1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_reduce_spall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_wick.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_xcf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12022 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_xcf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_xcf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/bin/picca_xwick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64077 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/co.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24636 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.960512 picca-8.0.0/py/picca/delta_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.960512 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25713 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27062 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.960512 picca-8.0.0/py/picca/delta_extraction/corrections/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/corrections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/corrections/calibration_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/corrections/dust_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/corrections/ivar_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/corrections/optical_depth_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22238 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.964512 picca-8.0.0/py/picca/delta_extraction/data_catalogues/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data_catalogues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data_catalogues/desi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data_catalogues/desi_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/data_catalogues/sdss_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.964512 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29855 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.968512 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/
+-rw-r--r--   0 runner    (1001) docker     (123)    98923 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_0.8.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    26124 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    28890 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    20204 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/expected_fluxes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.968512 picca-8.0.0/py/picca/delta_extraction/least_squares/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/least_squares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.968512 picca-8.0.0/py/picca/delta_extraction/masks/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/masks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/masks/absorber_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/masks/bal_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/masks/dla_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/masks/lines_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/quasar_catalogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.968512 picca-8.0.0/py/picca/delta_extraction/quasar_catalogues/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/quasar_catalogues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/rejection_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.968512 picca-8.0.0/py/picca/delta_extraction/rejection_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/rejection_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/delta_extraction/utils_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17281 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.972512 picca-8.0.0/py/picca/pk1d/
+-rw-r--r--   0 runner    (1001) docker     (123)    19994 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/pk1d/compute_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38897 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/pk1d/postproc_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/pk1d/prep_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/pk1d/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/prep_del.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/raw_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.972512 picca-8.0.0/py/picca/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.972512 picca-8.0.0/py/picca/tests/delta_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/tests/delta_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/tests/delta_extraction/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88977 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/tests/delta_extraction/astronomical_object_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/tests/delta_extraction/config_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-08-02 08:40:18.000000 picca-8.0.0/py/picca/tests/delta_extraction/correction_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63846 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/delta_extraction/data_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81524 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/delta_extraction/expected_flux_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31381 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/delta_extraction/mask_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/delta_extraction/scripts_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/delta_extraction/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/test_2_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42559 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/test_3_cor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17426 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/wedgize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40690 2023-08-02 08:40:20.000000 picca-8.0.0/py/picca/xcf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:40:33.948512 picca-8.0.0/py/picca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-08-02 08:40:33.000000 picca-8.0.0/py/picca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-08-02 08:40:33.000000 picca-8.0.0/py/picca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 08:40:33.000000 picca-8.0.0/py/picca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-02 08:40:33.000000 picca-8.0.0/py/picca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 08:40:33.000000 picca-8.0.0/py/picca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 08:40:20.000000 picca-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 08:40:33.976513 picca-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-02 08:40:20.000000 picca-8.0.0/setup.py
```

### Comparing `picca-7.2.0/LICENSE` & `picca-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/PKG-INFO` & `picca-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picca
-Version: 7.2.0
+Version: 8.0.0
 Summary: Package for Igm Cosmological-Correlations Analyses
 Home-page: https://github.com/igmhub/picca
 Author: Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols, Michael Walther, the DESI Lya forest picca topical group, et al
 Author-email: iprafols@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `picca-7.2.0/README.md` & `picca-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_Pk1D.py` & `picca-8.0.0/bin/picca_Pk1D.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_Pk1D_postprocess.py` & `picca-8.0.0/bin/picca_Pk1D_postprocess.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_cf.py` & `picca-8.0.0/bin/picca_cf.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_cf1d.py` & `picca-8.0.0/bin/picca_cf1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_cf_angl.py` & `picca-8.0.0/bin/picca_cf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_co.py` & `picca-8.0.0/bin/picca_co.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_coadd_zint.py` & `picca-8.0.0/bin/picca_coadd_zint.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_compute_fvoigt.py` & `picca-8.0.0/bin/picca_compute_fvoigt.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_compute_pk_pksb.py` & `picca-8.0.0/bin/picca_compute_pk_pksb.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_convert_transmission.py` & `picca-8.0.0/bin/picca_convert_transmission.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_delta_extraction.py` & `picca-8.0.0/bin/picca_delta_extraction.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_dmat.py` & `picca-8.0.0/bin/picca_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_export.py` & `picca-8.0.0/bin/picca_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,19 @@
         help='Remove a correlation from shuffling the distribution of los')
 
     parser.add_argument(
         '--do-not-smooth-cov',
         action='store_true',
         default=False,
         help='Do not smooth the covariance matrix')
+    parser.add_argument(
+        '--smooth-per-r-par',
+        action='store_true',
+        default=False,
+        help='Consider different correlation coefficients per r_par')
 
     parser.add_argument(
         '--blind-corr-type',
         default=None,
         choices=['lyaxlya', 'lyaxlyb', 'qsoxlya', 'qsoxlyb'],
         help='Type of correlation. Required to apply blinding in DESI')
 
@@ -145,20 +150,23 @@
         var = np.diagonal(covariance)
         covariance = correlation * np.sqrt(var * var[:, None])
     else:
         delta_r_par = (r_par_max - r_par_min) / num_bins_r_par
         delta_r_trans = (r_trans_max - 0.) / num_bins_r_trans
         if not args.do_not_smooth_cov:
             userprint("INFO: The covariance will be smoothed")
+            if args.smooth_per_r_par :
+                userprint("INFO: with different correlation coefficients per r_par")
             covariance = smooth_cov(xi,
                                     weights,
                                     r_par,
                                     r_trans,
                                     delta_r_trans=delta_r_trans,
-                                    delta_r_par=delta_r_par)
+                                    delta_r_par=delta_r_par,
+                                    per_r_par=args.smooth_per_r_par)
         else:
             userprint("INFO: The covariance will not be smoothed")
             covariance = compute_cov(xi, weights)
 
     xi = (xi * weights).sum(axis=0)
     weights = weights.sum(axis=0)
     w = weights > 0
```

### Comparing `picca-7.2.0/bin/picca_export_co.py` & `picca-8.0.0/bin/picca_export_co.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_export_cross_covariance.py` & `picca-8.0.0/bin/picca_export_cross_covariance.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_metal_dmat.py` & `picca-8.0.0/bin/picca_metal_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_metal_xdmat.py` & `picca-8.0.0/bin/picca_metal_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_nersc_submit.py` & `picca-8.0.0/bin/picca_nersc_submit.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_pk2fits.py` & `picca-8.0.0/bin/picca_pk2fits.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_plot_pk1d.py` & `picca-8.0.0/bin/picca_plot_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_reduce_spall.py` & `picca-8.0.0/bin/picca_reduce_spall.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_wick.py` & `picca-8.0.0/bin/picca_wick.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_xcf.py` & `picca-8.0.0/bin/picca_xcf.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_xcf1d.py` & `picca-8.0.0/bin/picca_xcf1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_xcf_angl.py` & `picca-8.0.0/bin/picca_xcf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_xdmat.py` & `picca-8.0.0/bin/picca_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/bin/picca_xwick.py` & `picca-8.0.0/bin/picca_xwick.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_Pk1D.py` & `picca-8.0.0/py/picca/bin/picca_Pk1D.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_Pk1D_postprocess.py` & `picca-8.0.0/py/picca/bin/picca_Pk1D_postprocess.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_cf.py` & `picca-8.0.0/py/picca/bin/picca_cf.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_cf1d.py` & `picca-8.0.0/py/picca/bin/picca_cf1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_cf_angl.py` & `picca-8.0.0/py/picca/bin/picca_cf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_co.py` & `picca-8.0.0/py/picca/bin/picca_co.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_coadd_zint.py` & `picca-8.0.0/py/picca/bin/picca_coadd_zint.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_compute_fvoigt.py` & `picca-8.0.0/py/picca/bin/picca_compute_fvoigt.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_compute_pk_pksb.py` & `picca-8.0.0/py/picca/bin/picca_compute_pk_pksb.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_convert_transmission.py` & `picca-8.0.0/py/picca/bin/picca_convert_transmission.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_delta_extraction.py` & `picca-8.0.0/py/picca/bin/picca_delta_extraction.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_dmat.py` & `picca-8.0.0/py/picca/bin/picca_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_export.py` & `picca-8.0.0/py/picca/bin/picca_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,19 @@
         help='Remove a correlation from shuffling the distribution of los')
 
     parser.add_argument(
         '--do-not-smooth-cov',
         action='store_true',
         default=False,
         help='Do not smooth the covariance matrix')
+    parser.add_argument(
+        '--smooth-per-r-par',
+        action='store_true',
+        default=False,
+        help='Consider different correlation coefficients per r_par')
 
     parser.add_argument(
         '--blind-corr-type',
         default=None,
         choices=['lyaxlya', 'lyaxlyb', 'qsoxlya', 'qsoxlyb'],
         help='Type of correlation. Required to apply blinding in DESI')
 
@@ -145,20 +150,23 @@
         var = np.diagonal(covariance)
         covariance = correlation * np.sqrt(var * var[:, None])
     else:
         delta_r_par = (r_par_max - r_par_min) / num_bins_r_par
         delta_r_trans = (r_trans_max - 0.) / num_bins_r_trans
         if not args.do_not_smooth_cov:
             userprint("INFO: The covariance will be smoothed")
+            if args.smooth_per_r_par :
+                userprint("INFO: with different correlation coefficients per r_par")
             covariance = smooth_cov(xi,
                                     weights,
                                     r_par,
                                     r_trans,
                                     delta_r_trans=delta_r_trans,
-                                    delta_r_par=delta_r_par)
+                                    delta_r_par=delta_r_par,
+                                    per_r_par=args.smooth_per_r_par)
         else:
             userprint("INFO: The covariance will not be smoothed")
             covariance = compute_cov(xi, weights)
 
     xi = (xi * weights).sum(axis=0)
     weights = weights.sum(axis=0)
     w = weights > 0
```

### Comparing `picca-7.2.0/py/picca/bin/picca_export_co.py` & `picca-8.0.0/py/picca/bin/picca_export_co.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_export_cross_covariance.py` & `picca-8.0.0/py/picca/bin/picca_export_cross_covariance.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_metal_dmat.py` & `picca-8.0.0/py/picca/bin/picca_metal_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_metal_xdmat.py` & `picca-8.0.0/py/picca/bin/picca_metal_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_nersc_submit.py` & `picca-8.0.0/py/picca/bin/picca_nersc_submit.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_pk2fits.py` & `picca-8.0.0/py/picca/bin/picca_pk2fits.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_plot_pk1d.py` & `picca-8.0.0/py/picca/bin/picca_plot_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_reduce_spall.py` & `picca-8.0.0/py/picca/bin/picca_reduce_spall.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_wick.py` & `picca-8.0.0/py/picca/bin/picca_wick.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_xcf.py` & `picca-8.0.0/py/picca/bin/picca_xcf.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_xcf1d.py` & `picca-8.0.0/py/picca/bin/picca_xcf1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_xcf_angl.py` & `picca-8.0.0/py/picca/bin/picca_xcf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_xdmat.py` & `picca-8.0.0/py/picca/bin/picca_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/bin/picca_xwick.py` & `picca-8.0.0/py/picca/bin/picca_xwick.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/cf.py` & `picca-8.0.0/py/picca/cf.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/co.py` & `picca-8.0.0/py/picca/co.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/constants.py` & `picca-8.0.0/py/picca/constants.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/converters.py` & `picca-8.0.0/py/picca/converters.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/astronomical_object.py` & `picca-8.0.0/py/picca/delta_extraction/astronomical_object.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py` & `picca-8.0.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py` & `picca-8.0.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/astronomical_objects/forest.py` & `picca-8.0.0/py/picca/delta_extraction/astronomical_objects/forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py` & `picca-8.0.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py` & `picca-8.0.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py` & `picca-8.0.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/config.py` & `picca-8.0.0/py/picca/delta_extraction/config.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/correction.py` & `picca-8.0.0/py/picca/delta_extraction/correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/corrections/calibration_correction.py` & `picca-8.0.0/py/picca/delta_extraction/corrections/calibration_correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/corrections/dust_correction.py` & `picca-8.0.0/py/picca/delta_extraction/corrections/dust_correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/corrections/ivar_correction.py` & `picca-8.0.0/py/picca/delta_extraction/corrections/ivar_correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/corrections/optical_depth_correction.py` & `picca-8.0.0/py/picca/delta_extraction/corrections/optical_depth_correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/data.py` & `picca-8.0.0/py/picca/delta_extraction/data.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/data_catalogues/desi_data.py` & `picca-8.0.0/py/picca/delta_extraction/data_catalogues/desi_data.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py` & `picca-8.0.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/data_catalogues/desi_tile.py` & `picca-8.0.0/py/picca/delta_extraction/data_catalogues/desi_tile.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py` & `picca-8.0.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/data_catalogues/sdss_data.py` & `picca-8.0.0/py/picca/delta_extraction/data_catalogues/sdss_data.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/errors.py` & `picca-8.0.0/py/picca/delta_extraction/errors.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_flux.py` & `picca-8.0.0/py/picca/delta_extraction/expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_0.8.fits.gz` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_0.8.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/utils.py` & `picca-8.0.0/py/picca/delta_extraction/expected_fluxes/utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py` & `picca-8.0.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py` & `picca-8.0.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/mask.py` & `picca-8.0.0/py/picca/delta_extraction/mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/masks/absorber_mask.py` & `picca-8.0.0/py/picca/delta_extraction/masks/absorber_mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/masks/bal_mask.py` & `picca-8.0.0/py/picca/delta_extraction/masks/bal_mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/masks/dla_mask.py` & `picca-8.0.0/py/picca/delta_extraction/masks/dla_mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/masks/lines_mask.py` & `picca-8.0.0/py/picca/delta_extraction/masks/lines_mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/quasar_catalogue.py` & `picca-8.0.0/py/picca/delta_extraction/quasar_catalogue.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py` & `picca-8.0.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py` & `picca-8.0.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/rejection_log.py` & `picca-8.0.0/py/picca/delta_extraction/rejection_log.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py` & `picca-8.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py` & `picca-8.0.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/survey.py` & `picca-8.0.0/py/picca/delta_extraction/survey.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/utils.py` & `picca-8.0.0/py/picca/delta_extraction/utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/delta_extraction/utils_pk1d.py` & `picca-8.0.0/py/picca/delta_extraction/utils_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/pk1d/compute_pk1d.py` & `picca-8.0.0/py/picca/pk1d/compute_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/pk1d/postproc_pk1d.py` & `picca-8.0.0/py/picca/pk1d/postproc_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/pk1d/prep_pk1d.py` & `picca-8.0.0/py/picca/pk1d/prep_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/pk1d/utils.py` & `picca-8.0.0/py/picca/pk1d/utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/raw_io.py` & `picca-8.0.0/py/picca/raw_io.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/tests/delta_extraction/abstract_test.py` & `picca-8.0.0/py/picca/tests/delta_extraction/abstract_test.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/tests/delta_extraction/astronomical_object_tests.py` & `picca-8.0.0/py/picca/tests/delta_extraction/astronomical_object_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/tests/delta_extraction/config_tests.py` & `picca-8.0.0/py/picca/tests/delta_extraction/config_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/tests/delta_extraction/correction_tests.py` & `picca-8.0.0/py/picca/tests/delta_extraction/correction_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/tests/delta_extraction/data_tests.py` & `picca-8.0.0/py/picca/tests/delta_extraction/data_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/tests/delta_extraction/expected_flux_tests.py` & `picca-8.0.0/py/picca/tests/delta_extraction/expected_flux_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/tests/delta_extraction/mask_tests.py` & `picca-8.0.0/py/picca/tests/delta_extraction/mask_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py` & `picca-8.0.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/tests/delta_extraction/scripts_tests.py` & `picca-8.0.0/py/picca/tests/delta_extraction/scripts_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/tests/delta_extraction/test_utils.py` & `picca-8.0.0/py/picca/tests/delta_extraction/test_utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/tests/test_2_pk1d.py` & `picca-8.0.0/py/picca/tests/test_2_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/tests/test_3_cor.py` & `picca-8.0.0/py/picca/tests/test_3_cor.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/tests/test_helpers.py` & `picca-8.0.0/py/picca/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/utils.py` & `picca-8.0.0/py/picca/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,15 +60,16 @@
 
 def smooth_cov(xi,
                weights,
                r_par,
                r_trans,
                delta_r_trans=4.0,
                delta_r_par=4.0,
-               covariance=None):
+               covariance=None,
+               per_r_par=False):
     """Smoothes the covariance matrix
 
     Args:
         xi: array of floats
             Correlation function measburement in each helpix
         weights: array of floats
             Weights on the correlation function measurement
@@ -79,14 +80,16 @@
         delta_r_trans: float - default: 4.0
             Variation of the transverse distance between two pixels
         delta_r_par: float - default: 4.0
             Variation of the transverse distance between two pixels
         covariance: array of floats or None - defautl: None
             Covariance matrix. If None, it will be computed using the
             subsampling technique
+        per_r_par: if true, average the correlation coef per
+                  (r_par,delta_r_par,delta_r_trans)
 
     Returns:
         The smooth covariance matrix. If data is not correct, then print a
         warning and return the unsmoothed covariance matrix
     """
     if covariance is None:
         covariance = compute_cov(xi, weights)
@@ -103,38 +106,56 @@
     correlation_smooth = np.zeros([num_bins, num_bins])
 
     # add together the correlation from bins with similar separations in
     # parallel and perpendicular distances
     sum_correlation = {}
     counts_correlation = {}
     for index in range(num_bins):
+        if per_r_par :
+            index_r_par = int(r_par[index]/delta_r_par)
         userprint("\rsmoothing {}".format(index), end="")
         for index2 in range(index + 1, num_bins):
             index_delta_r_par = round(
                 abs(r_par[index2] - r_par[index]) / delta_r_par)
             index_delta_r_trans = round(
                 abs(r_trans[index] - r_trans[index2]) / delta_r_trans)
-            if (index_delta_r_par, index_delta_r_trans) not in sum_correlation:
-                sum_correlation[(index_delta_r_par, index_delta_r_trans)] = 0.
-                counts_correlation[(index_delta_r_par, index_delta_r_trans)] = 0
-
-            sum_correlation[(index_delta_r_par,
-                             index_delta_r_trans)] += correlation[index, index2]
-            counts_correlation[(index_delta_r_par, index_delta_r_trans)] += 1
+            if per_r_par :
+                if (index_r_par, index_delta_r_par, index_delta_r_trans) not in sum_correlation:
+                    sum_correlation[(index_r_par, index_delta_r_par, index_delta_r_trans)] = 0.
+                    counts_correlation[(index_r_par, index_delta_r_par, index_delta_r_trans)] = 0
+
+                sum_correlation[(index_r_par, index_delta_r_par,
+                                 index_delta_r_trans)] += correlation[index, index2]
+                counts_correlation[(index_r_par, index_delta_r_par, index_delta_r_trans)] += 1
+            else :
+                if (index_delta_r_par, index_delta_r_trans) not in sum_correlation:
+                    sum_correlation[(index_delta_r_par, index_delta_r_trans)] = 0.
+                    counts_correlation[(index_delta_r_par, index_delta_r_trans)] = 0
+
+                sum_correlation[(index_delta_r_par,
+                                 index_delta_r_trans)] += correlation[index, index2]
+                counts_correlation[(index_delta_r_par, index_delta_r_trans)] += 1
 
     for index in range(num_bins):
         correlation_smooth[index, index] = 1.
+        if per_r_par :
+            index_r_par = int(r_par[index]/delta_r_par)
         for index2 in range(index + 1, num_bins):
             index_delta_r_par = round(
                 abs(r_par[index2] - r_par[index]) / delta_r_par)
             index_delta_r_trans = round(
                 abs(r_trans[index] - r_trans[index2]) / delta_r_trans)
-            correlation_smooth[index, index2] = (
-                sum_correlation[(index_delta_r_par, index_delta_r_trans)] /
-                counts_correlation[(index_delta_r_par, index_delta_r_trans)])
+            if per_r_par :
+                correlation_smooth[index, index2] = (
+                    sum_correlation[(index_r_par, index_delta_r_par, index_delta_r_trans)] /
+                    counts_correlation[(index_r_par , index_delta_r_par, index_delta_r_trans)])
+            else :
+                correlation_smooth[index, index2] = (
+                    sum_correlation[(index_delta_r_par, index_delta_r_trans)] /
+                    counts_correlation[(index_delta_r_par, index_delta_r_trans)])
             correlation_smooth[index2, index] = correlation_smooth[index,
                                                                    index2]
 
     userprint("\n")
     covariance_smooth = correlation_smooth * np.sqrt(var * var[:, None])
     return covariance_smooth
 
@@ -466,8 +487,7 @@
         curve[iopir] = interpolate.splev(x[iopir], tck)
 
     #Now apply extinction correction to input flux vector
     curve *= ebv
     corr = 1. / (10.**(0.4 * curve))
 
     return corr
-
```

### Comparing `picca-7.2.0/py/picca/wedgize.py` & `picca-8.0.0/py/picca/wedgize.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca/xcf.py` & `picca-8.0.0/py/picca/xcf.py`

 * *Files identical despite different names*

### Comparing `picca-7.2.0/py/picca.egg-info/PKG-INFO` & `picca-8.0.0/py/picca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picca
-Version: 7.2.0
+Version: 8.0.0
 Summary: Package for Igm Cosmological-Correlations Analyses
 Home-page: https://github.com/igmhub/picca
 Author: Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols, Michael Walther, the DESI Lya forest picca topical group, et al
 Author-email: iprafols@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `picca-7.2.0/py/picca.egg-info/SOURCES.txt` & `picca-8.0.0/py/picca.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -27,21 +27,19 @@
 bin/picca_xcf.py
 bin/picca_xcf1d.py
 bin/picca_xcf_angl.py
 bin/picca_xdmat.py
 bin/picca_xwick.py
 py/picca/__init__.py
 py/picca/_version.py
-py/picca/bal_tools.py
 py/picca/cf.py
 py/picca/co.py
 py/picca/constants.py
 py/picca/converters.py
 py/picca/data.py
-py/picca/dla.py
 py/picca/io.py
 py/picca/prep_del.py
 py/picca/raw_io.py
 py/picca/utils.py
 py/picca/wedgize.py
 py/picca/xcf.py
 py/picca.egg-info/PKG-INFO
@@ -73,18 +71,14 @@
 py/picca/bin/picca_reduce_spall.py
 py/picca/bin/picca_wick.py
 py/picca/bin/picca_xcf.py
 py/picca/bin/picca_xcf1d.py
 py/picca/bin/picca_xcf_angl.py
 py/picca/bin/picca_xdmat.py
 py/picca/bin/picca_xwick.py
-py/picca/bin/old/picca_deltas.py
-py/picca/bin/old/picca_fitter2.py
-py/picca/bin/old/picca_fitter2_control.py
-py/picca/bin/old/picca_fitter2_control_mpi.py
 py/picca/delta_extraction/__init__.py
 py/picca/delta_extraction/astronomical_object.py
 py/picca/delta_extraction/config.py
 py/picca/delta_extraction/correction.py
 py/picca/delta_extraction/data.py
 py/picca/delta_extraction/errors.py
 py/picca/delta_extraction/expected_flux.py
@@ -137,34 +131,14 @@
 py/picca/delta_extraction/masks/lines_mask.py
 py/picca/delta_extraction/quasar_catalogues/__init__.py
 py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py
 py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py
 py/picca/delta_extraction/rejection_logs/__init__.py
 py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py
 py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py
-py/picca/fitter2/__init__.py
-py/picca/fitter2/chi2.py
-py/picca/fitter2/control.py
-py/picca/fitter2/control_mpi.py
-py/picca/fitter2/data.py
-py/picca/fitter2/effective-bins.py
-py/picca/fitter2/myGamma.py
-py/picca/fitter2/parser.py
-py/picca/fitter2/pk.py
-py/picca/fitter2/priors.py
-py/picca/fitter2/sampler.py
-py/picca/fitter2/utils.py
-py/picca/fitter2/xi.py
-py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits
-py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits
-py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits
-py/picca/fitter2/models/Planck18/Planck18_z_2.406.fits
-py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits
-py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits
-py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits
 py/picca/pk1d/compute_pk1d.py
 py/picca/pk1d/postproc_pk1d.py
 py/picca/pk1d/prep_pk1d.py
 py/picca/pk1d/utils.py
 py/picca/tests/__init__.py
 py/picca/tests/test_2_pk1d.py
 py/picca/tests/test_3_cor.py
@@ -175,10 +149,8 @@
 py/picca/tests/delta_extraction/config_tests.py
 py/picca/tests/delta_extraction/correction_tests.py
 py/picca/tests/delta_extraction/data_tests.py
 py/picca/tests/delta_extraction/expected_flux_tests.py
 py/picca/tests/delta_extraction/mask_tests.py
 py/picca/tests/delta_extraction/quasar_catalogue_tests.py
 py/picca/tests/delta_extraction/scripts_tests.py
-py/picca/tests/delta_extraction/test_utils.py
-py/picca/tests/old/test_1_deltas.py
-py/picca/tests/old/test_4_fitter2.py
+py/picca/tests/delta_extraction/test_utils.py
```

### Comparing `picca-7.2.0/setup.py` & `picca-8.0.0/setup.py`

 * *Files identical despite different names*

