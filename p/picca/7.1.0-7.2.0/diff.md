# Comparing `tmp/picca-7.1.0.tar.gz` & `tmp/picca-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picca-7.1.0.tar", last modified: Wed Jul 12 15:20:10 2023, max compression
+gzip compressed data, was "picca-7.2.0.tar", last modified: Tue Jul 18 07:19:34 2023, max compression
```

## Comparing `picca-7.1.0.tar` & `picca-7.2.0.tar`

### file list

```diff
@@ -1,214 +1,215 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.729496 picca-7.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-12 15:19:58.000000 picca-7.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-12 15:20:10.729496 picca-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-12 15:19:58.000000 picca-7.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.709495 picca-7.1.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_Pk1D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_Pk1D_postprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_cf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_cf1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_cf_angl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_co.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_coadd_zint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_compute_fvoigt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_compute_pk_pksb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_convert_transmission.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_delta_extraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_dmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12239 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_export.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_export_co.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_export_cross_covariance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_metal_dmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_metal_xdmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_nersc_submit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_pk2fits.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_plot_pk1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_reduce_spall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_wick.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_xcf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12008 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_xcf1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_xcf_angl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_xdmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-07-12 15:19:58.000000 picca-7.1.0/bin/picca_xwick.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.705495 picca-7.1.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.713495 picca-7.1.0/py/picca/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bal_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.717496 picca-7.1.0/py/picca/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.717496 picca-7.1.0/py/picca/bin/old/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43689 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/old/picca_deltas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/old/picca_fitter2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/old/picca_fitter2_control.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/old/picca_fitter2_control_mpi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_Pk1D.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_Pk1D_postprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_cf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_cf1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_cf_angl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_co.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_coadd_zint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_compute_fvoigt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_compute_pk_pksb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_convert_transmission.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_delta_extraction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_dmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12239 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_export.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_export_co.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_export_cross_covariance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_metal_dmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_metal_xdmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_nersc_submit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_pk2fits.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_plot_pk1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_reduce_spall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_wick.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_xcf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12008 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_xcf1d.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_xcf_angl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_xdmat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/bin/picca_xwick.py
--rw-r--r--   0 runner    (1001) docker     (123)    64077 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/cf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/co.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    51080 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.717496 picca-7.1.0/py/picca/delta_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.717496 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    25713 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)    27062 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/corrections/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/corrections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/corrections/calibration_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/corrections/dust_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/corrections/ivar_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/corrections/optical_depth_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)    22238 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/data_catalogues/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data_catalogues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data_catalogues/desi_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data_catalogues/desi_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/data_catalogues/sdss_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30238 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/
--rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    15906 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz
--rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/expected_fluxes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/least_squares/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/least_squares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/mask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/masks/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/masks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/masks/absorber_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/masks/bal_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/masks/dla_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/masks/lines_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/quasar_catalogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/quasar_catalogues/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/quasar_catalogues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/rejection_log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.721495 picca-7.1.0/py/picca/delta_extraction/rejection_logs/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/rejection_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/delta_extraction/utils_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/dla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/chi2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/control_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6784 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/effective-bins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.705495 picca-7.1.0/py/picca/fitter2/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/models/DR16_blind_test_large/
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/models/DR16_blind_test_small/
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/models/DR9LyaMocks/
--rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/models/Planck18/
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/Planck18/Planck18_z_2.406.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/models/PlanckDR12/
--rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/fitter2/models/PlanckDR16/
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/myGamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16465 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/pk.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/priors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/fitter2/xi.py
--rw-r--r--   0 runner    (1001) docker     (123)    64892 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/pk1d/
--rw-r--r--   0 runner    (1001) docker     (123)    19994 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/pk1d/compute_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    38897 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/pk1d/postproc_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/pk1d/prep_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/pk1d/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/prep_del.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/raw_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.725495 picca-7.1.0/py/picca/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-12 15:19:58.000000 picca-7.1.0/py/picca/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.729496 picca-7.1.0/py/picca/tests/delta_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-12 15:19:59.000000 picca-7.1.0/py/picca/tests/delta_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-12 15:19:59.000000 picca-7.1.0/py/picca/tests/delta_extraction/abstract_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    88977 2023-07-12 15:19:59.000000 picca-7.1.0/py/picca/tests/delta_extraction/astronomical_object_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-07-12 15:19:59.000000 picca-7.1.0/py/picca/tests/delta_extraction/config_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-07-12 15:19:59.000000 picca-7.1.0/py/picca/tests/delta_extraction/correction_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    63846 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/delta_extraction/data_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    81274 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/delta_extraction/expected_flux_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    31381 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/delta_extraction/mask_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/delta_extraction/scripts_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/delta_extraction/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.729496 picca-7.1.0/py/picca/tests/old/
--rw-r--r--   0 runner    (1001) docker     (123)    17429 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/old/test_1_deltas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/old/test_4_fitter2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/test_2_pk1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    42559 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/test_3_cor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16216 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/wedgize.py
--rw-r--r--   0 runner    (1001) docker     (123)    40856 2023-07-12 15:20:01.000000 picca-7.1.0/py/picca/xcf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:20:10.713495 picca-7.1.0/py/picca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-12 15:20:10.000000 picca-7.1.0/py/picca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-07-12 15:20:10.000000 picca-7.1.0/py/picca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:20:10.000000 picca-7.1.0/py/picca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-12 15:20:10.000000 picca-7.1.0/py/picca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 15:20:10.000000 picca-7.1.0/py/picca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-12 15:20:01.000000 picca-7.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:20:10.729496 picca-7.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-12 15:20:01.000000 picca-7.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.230544 picca-7.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-18 07:19:16.000000 picca-7.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-18 07:19:34.230544 picca-7.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-18 07:19:16.000000 picca-7.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.194542 picca-7.2.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_Pk1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_Pk1D_postprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_cf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_cf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_cf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_coadd_zint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_compute_fvoigt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_compute_pk_pksb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_convert_transmission.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_delta_extraction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12239 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_export.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_export_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_export_cross_covariance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_metal_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_metal_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_nersc_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_pk2fits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_plot_pk1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_reduce_spall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_wick.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_xcf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12022 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_xcf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_xcf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-07-18 07:19:16.000000 picca-7.2.0/bin/picca_xwick.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.190541 picca-7.2.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.198542 picca-7.2.0/py/picca/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bal_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.206542 picca-7.2.0/py/picca/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.206542 picca-7.2.0/py/picca/bin/old/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43689 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/old/picca_deltas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/old/picca_fitter2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/old/picca_fitter2_control.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      614 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/old/picca_fitter2_control_mpi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24135 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_Pk1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10849 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_Pk1D_postprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16058 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_cf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11731 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_cf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11265 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_cf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12071 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14263 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_coadd_zint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9312 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_compute_fvoigt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5833 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_compute_pk_pksb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3480 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_convert_transmission.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_delta_extraction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15850 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12239 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_export.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14187 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_export_co.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_export_cross_covariance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19846 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_metal_dmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18174 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_metal_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27530 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_nersc_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2201 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_pk2fits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5870 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_plot_pk1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_reduce_spall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19061 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_wick.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16708 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_xcf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12022 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_xcf1d.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13810 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_xcf_angl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15413 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_xdmat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17951 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/bin/picca_xwick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64077 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/co.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51080 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.210543 picca-7.2.0/py/picca/delta_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.210543 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25713 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27062 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.210543 picca-7.2.0/py/picca/delta_extraction/corrections/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/corrections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/corrections/calibration_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/corrections/dust_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/corrections/ivar_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/corrections/optical_depth_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22238 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.214543 picca-7.2.0/py/picca/delta_extraction/data_catalogues/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data_catalogues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data_catalogues/desi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data_catalogues/desi_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/data_catalogues/sdss_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16433 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.214543 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29855 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.218543 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/
+-rw-r--r--   0 runner    (1001) docker     (123)    98923 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_0.8.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    35125 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    26124 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    28890 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    20204 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/expected_fluxes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.218543 picca-7.2.0/py/picca/delta_extraction/least_squares/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/least_squares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/mask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.218543 picca-7.2.0/py/picca/delta_extraction/masks/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/masks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/masks/absorber_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/masks/bal_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/masks/dla_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/masks/lines_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/quasar_catalogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.218543 picca-7.2.0/py/picca/delta_extraction/quasar_catalogues/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/quasar_catalogues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/rejection_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.218543 picca-7.2.0/py/picca/delta_extraction/rejection_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/rejection_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/delta_extraction/utils_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/dla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.222544 picca-7.2.0/py/picca/fitter2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/chi2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/control_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6784 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/effective-bins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.190541 picca-7.2.0/py/picca/fitter2/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.222544 picca-7.2.0/py/picca/fitter2/models/DR16_blind_test_large/
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.222544 picca-7.2.0/py/picca/fitter2/models/DR16_blind_test_small/
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.222544 picca-7.2.0/py/picca/fitter2/models/DR9LyaMocks/
+-rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.222544 picca-7.2.0/py/picca/fitter2/models/Planck18/
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/Planck18/Planck18_z_2.406.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.226544 picca-7.2.0/py/picca/fitter2/models/PlanckDR12/
+-rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.226544 picca-7.2.0/py/picca/fitter2/models/PlanckDR16/
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/myGamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16465 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/fitter2/xi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64892 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.226544 picca-7.2.0/py/picca/pk1d/
+-rw-r--r--   0 runner    (1001) docker     (123)    19994 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/pk1d/compute_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38897 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/pk1d/postproc_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/pk1d/prep_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/pk1d/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13939 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/prep_del.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/raw_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.226544 picca-7.2.0/py/picca/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.230544 picca-7.2.0/py/picca/tests/delta_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/tests/delta_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/tests/delta_extraction/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88977 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/tests/delta_extraction/astronomical_object_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/tests/delta_extraction/config_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-07-18 07:19:16.000000 picca-7.2.0/py/picca/tests/delta_extraction/correction_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63846 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/delta_extraction/data_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81524 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/delta_extraction/expected_flux_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31381 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/delta_extraction/mask_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6230 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/delta_extraction/scripts_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/delta_extraction/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.230544 picca-7.2.0/py/picca/tests/old/
+-rw-r--r--   0 runner    (1001) docker     (123)    17429 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/old/test_1_deltas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/old/test_4_fitter2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/test_2_pk1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42559 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/test_3_cor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16216 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/wedgize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40690 2023-07-18 07:19:19.000000 picca-7.2.0/py/picca/xcf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:19:34.198542 picca-7.2.0/py/picca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-18 07:19:34.000000 picca-7.2.0/py/picca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-07-18 07:19:34.000000 picca-7.2.0/py/picca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:19:34.000000 picca-7.2.0/py/picca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-18 07:19:34.000000 picca-7.2.0/py/picca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 07:19:34.000000 picca-7.2.0/py/picca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-18 07:19:19.000000 picca-7.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:19:34.230544 picca-7.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-18 07:19:19.000000 picca-7.2.0/setup.py
```

### Comparing `picca-7.1.0/LICENSE` & `picca-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/PKG-INFO` & `picca-7.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picca
-Version: 7.1.0
+Version: 7.2.0
 Summary: Package for Igm Cosmological-Correlations Analyses
 Home-page: https://github.com/igmhub/picca
 Author: Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols, Michael Walther, the DESI Lya forest picca topical group, et al
 Author-email: iprafols@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `picca-7.1.0/README.md` & `picca-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_Pk1D.py` & `picca-7.2.0/bin/picca_Pk1D.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_Pk1D_postprocess.py` & `picca-7.2.0/bin/picca_Pk1D_postprocess.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_cf.py` & `picca-7.2.0/bin/picca_cf.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_cf1d.py` & `picca-7.2.0/bin/picca_cf1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_cf_angl.py` & `picca-7.2.0/bin/picca_cf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_co.py` & `picca-7.2.0/bin/picca_co.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_coadd_zint.py` & `picca-7.2.0/bin/picca_coadd_zint.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_compute_fvoigt.py` & `picca-7.2.0/bin/picca_compute_fvoigt.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_compute_pk_pksb.py` & `picca-7.2.0/bin/picca_compute_pk_pksb.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_convert_transmission.py` & `picca-7.2.0/bin/picca_convert_transmission.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_delta_extraction.py` & `picca-7.2.0/bin/picca_delta_extraction.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_dmat.py` & `picca-7.2.0/bin/picca_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_export.py` & `picca-7.2.0/bin/picca_export.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_export_co.py` & `picca-7.2.0/bin/picca_export_co.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_export_cross_covariance.py` & `picca-7.2.0/bin/picca_export_cross_covariance.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_metal_dmat.py` & `picca-7.2.0/bin/picca_metal_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_metal_xdmat.py` & `picca-7.2.0/bin/picca_metal_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_nersc_submit.py` & `picca-7.2.0/bin/picca_nersc_submit.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_pk2fits.py` & `picca-7.2.0/bin/picca_pk2fits.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_plot_pk1d.py` & `picca-7.2.0/bin/picca_plot_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_reduce_spall.py` & `picca-7.2.0/bin/picca_reduce_spall.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_wick.py` & `picca-7.2.0/bin/picca_wick.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_xcf.py` & `picca-7.2.0/bin/picca_xcf.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_xcf1d.py` & `picca-7.2.0/bin/picca_xcf1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     # setup variables in module xcf
     xcf.r_par_min = args.wr_min
     xcf.r_par_max = args.wr_max
     xcf.r_trans_max = 1.e-6
     xcf.z_cut_min = args.z_cut_min
     xcf.z_cut_max = args.z_cut_max
     xcf.num_bins_r_par = args.np
-    xcf.nt = 1
+    xcf.num_bins_r_trans = 1
     xcf.nside = args.nside
     xcf.ang_correlation = True
 
     lambda_abs = constants.ABSORBER_IGM[args.lambda_abs]
 
     ### Read deltas
     data, num_data, z_min, z_max = io.read_deltas(args.in_dir,
```

### Comparing `picca-7.1.0/bin/picca_xcf_angl.py` & `picca-7.2.0/bin/picca_xcf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_xdmat.py` & `picca-7.2.0/bin/picca_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/bin/picca_xwick.py` & `picca-7.2.0/bin/picca_xwick.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bal_tools.py` & `picca-7.2.0/py/picca/bal_tools.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/old/picca_deltas.py` & `picca-7.2.0/py/picca/bin/old/picca_deltas.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/old/picca_fitter2.py` & `picca-7.2.0/py/picca/bin/old/picca_fitter2.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/old/picca_fitter2_control.py` & `picca-7.2.0/py/picca/bin/old/picca_fitter2_control.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/old/picca_fitter2_control_mpi.py` & `picca-7.2.0/py/picca/bin/old/picca_fitter2_control_mpi.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_Pk1D.py` & `picca-7.2.0/py/picca/bin/picca_Pk1D.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_Pk1D_postprocess.py` & `picca-7.2.0/py/picca/bin/picca_Pk1D_postprocess.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_cf.py` & `picca-7.2.0/py/picca/bin/picca_cf.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_cf1d.py` & `picca-7.2.0/py/picca/bin/picca_cf1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_cf_angl.py` & `picca-7.2.0/py/picca/bin/picca_cf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_co.py` & `picca-7.2.0/py/picca/bin/picca_co.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_coadd_zint.py` & `picca-7.2.0/py/picca/bin/picca_coadd_zint.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_compute_fvoigt.py` & `picca-7.2.0/py/picca/bin/picca_compute_fvoigt.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_compute_pk_pksb.py` & `picca-7.2.0/py/picca/bin/picca_compute_pk_pksb.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_convert_transmission.py` & `picca-7.2.0/py/picca/bin/picca_convert_transmission.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_delta_extraction.py` & `picca-7.2.0/py/picca/bin/picca_delta_extraction.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_dmat.py` & `picca-7.2.0/py/picca/bin/picca_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_export.py` & `picca-7.2.0/py/picca/bin/picca_export.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_export_co.py` & `picca-7.2.0/py/picca/bin/picca_export_co.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_export_cross_covariance.py` & `picca-7.2.0/py/picca/bin/picca_export_cross_covariance.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_metal_dmat.py` & `picca-7.2.0/py/picca/bin/picca_metal_dmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_metal_xdmat.py` & `picca-7.2.0/py/picca/bin/picca_metal_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_nersc_submit.py` & `picca-7.2.0/py/picca/bin/picca_nersc_submit.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_pk2fits.py` & `picca-7.2.0/py/picca/bin/picca_pk2fits.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_plot_pk1d.py` & `picca-7.2.0/py/picca/bin/picca_plot_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_reduce_spall.py` & `picca-7.2.0/py/picca/bin/picca_reduce_spall.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_wick.py` & `picca-7.2.0/py/picca/bin/picca_wick.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_xcf.py` & `picca-7.2.0/py/picca/bin/picca_xcf.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_xcf1d.py` & `picca-7.2.0/py/picca/bin/picca_xcf1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
     # setup variables in module xcf
     xcf.r_par_min = args.wr_min
     xcf.r_par_max = args.wr_max
     xcf.r_trans_max = 1.e-6
     xcf.z_cut_min = args.z_cut_min
     xcf.z_cut_max = args.z_cut_max
     xcf.num_bins_r_par = args.np
-    xcf.nt = 1
+    xcf.num_bins_r_trans = 1
     xcf.nside = args.nside
     xcf.ang_correlation = True
 
     lambda_abs = constants.ABSORBER_IGM[args.lambda_abs]
 
     ### Read deltas
     data, num_data, z_min, z_max = io.read_deltas(args.in_dir,
```

### Comparing `picca-7.1.0/py/picca/bin/picca_xcf_angl.py` & `picca-7.2.0/py/picca/bin/picca_xcf_angl.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_xdmat.py` & `picca-7.2.0/py/picca/bin/picca_xdmat.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/bin/picca_xwick.py` & `picca-7.2.0/py/picca/bin/picca_xwick.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/cf.py` & `picca-7.2.0/py/picca/cf.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/co.py` & `picca-7.2.0/py/picca/co.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/constants.py` & `picca-7.2.0/py/picca/constants.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/converters.py` & `picca-7.2.0/py/picca/converters.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/data.py` & `picca-7.2.0/py/picca/data.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/astronomical_object.py` & `picca-7.2.0/py/picca/delta_extraction/astronomical_object.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py` & `picca-7.2.0/py/picca/delta_extraction/astronomical_objects/desi_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py` & `picca-7.2.0/py/picca/delta_extraction/astronomical_objects/desi_pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/astronomical_objects/forest.py` & `picca-7.2.0/py/picca/delta_extraction/astronomical_objects/forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py` & `picca-7.2.0/py/picca/delta_extraction/astronomical_objects/pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py` & `picca-7.2.0/py/picca/delta_extraction/astronomical_objects/sdss_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py` & `picca-7.2.0/py/picca/delta_extraction/astronomical_objects/sdss_pk1d_forest.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/config.py` & `picca-7.2.0/py/picca/delta_extraction/config.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/correction.py` & `picca-7.2.0/py/picca/delta_extraction/correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/corrections/calibration_correction.py` & `picca-7.2.0/py/picca/delta_extraction/corrections/calibration_correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/corrections/dust_correction.py` & `picca-7.2.0/py/picca/delta_extraction/corrections/dust_correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/corrections/ivar_correction.py` & `picca-7.2.0/py/picca/delta_extraction/corrections/ivar_correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/corrections/optical_depth_correction.py` & `picca-7.2.0/py/picca/delta_extraction/corrections/optical_depth_correction.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/data.py` & `picca-7.2.0/py/picca/delta_extraction/data.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/data_catalogues/desi_data.py` & `picca-7.2.0/py/picca/delta_extraction/data_catalogues/desi_data.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py` & `picca-7.2.0/py/picca/delta_extraction/data_catalogues/desi_healpix.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/data_catalogues/desi_tile.py` & `picca-7.2.0/py/picca/delta_extraction/data_catalogues/desi_tile.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,18 +193,22 @@
             return {}, 0
 
         fibermap = hdul['FIBERMAP'].read()
 
         ra = fibermap['TARGET_RA']
         dec = fibermap['TARGET_DEC']
         tile_spec = fibermap['TILEID'][0]
-        if "cumulative" in self.input_directory:
-            night_spec = int(filename.split('thru')[-1].split('.')[0])
-        else:
-            night_spec = int(filename.split('-')[-1].split('.')[0])
+        try:
+            if "cumulative" in self.input_directory:
+                night_spec = int(filename.split('thru')[-1].split('.')[0])
+            else:
+                night_spec = int(filename.split('-')[-1].split('.')[0])
+        except ValueError:
+            self.logger.warning(f"In file {filename}, error reading night. Ignoring file")
+            return {}, 0
 
         colors = ['B', 'R', 'Z']
         ra = np.radians(ra)
         dec = np.radians(dec)
 
         petal_spec = fibermap['PETAL_LOC'][0]
 
@@ -217,15 +221,15 @@
                 spec['IVAR'] = (hdul[f'{color}_IVAR'].read() *
                                 (hdul[f'{color}_MASK'].read() == 0))
                 if self.analysis_type == "PK 1D":
                     if f"{color}_RESOLUTION" in hdul:
                         spec["RESO"] = hdul[f"{color}_RESOLUTION"].read()
                     else:
                         raise DataError(
-                            "Error while reading {color} band from "
+                            f"Error while reading {color} band from "
                             "{filename}. Analysis type is  'PK 1D', "
                             "but file does not contain HDU "
                             f"'{color}_RESOLUTION' ")
                 w = np.isnan(spec['FLUX']) | np.isnan(spec['IVAR'])
                 for key in ['FLUX', 'IVAR']:
                     spec[key][w] = 0.
                 spectrographs_data[color] = spec
```

### Comparing `picca-7.1.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py` & `picca-7.2.0/py/picca/delta_extraction/data_catalogues/desisim_mocks.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/data_catalogues/sdss_data.py` & `picca-7.2.0/py/picca/delta_extraction/data_catalogues/sdss_data.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/errors.py` & `picca-7.2.0/py/picca/delta_extraction/errors.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/expected_flux.py` & `picca-7.2.0/py/picca/delta_extraction/expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py` & `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_expected_flux.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
         "num iterations": 5,
         "min num qso in fit": 100,
         "order": 1,
         "use constant weight": False,
         "use ivar as weight": False,
     })
 
-FUDGE_FIT_START = FUDGE_REF
-ETA_FIT_START = 1.
-VAR_LSS_FIT_START = 0.1
+FUDGE_DEFAULT = 0
+ETA_DEFAULT = 1.
+VAR_LSS_DEFAULT = 0.1
 
 
 class Dr16ExpectedFlux(ExpectedFlux):
     """Class to the expected flux as done in the DR16 SDSS analysys
     The mean expected flux is calculated iteratively as explained in
     du Mas des Bourboux et al. (2020)
 
@@ -200,54 +200,54 @@
         if self.use_ivar_as_weight:
             eta = np.ones(self.num_bins_variance)
         # if use_constant_weight is set, we fix eta=0, var_lss=1, and fudge=0
         elif self.use_constant_weight:
             eta = np.zeros(self.num_bins_variance)
         # normal initialization, starting values eta=1, var_lss=0.2 , and fudge=0
         else:
-            eta = np.ones(self.num_bins_variance)
+            eta = np.zeros(self.num_bins_variance) + ETA_DEFAULT
             # this bit is what is actually freeing eta for the fit
             self.fit_variance_functions.append("eta")
 
         self.get_eta = interp1d(self.log_lambda_var_func_grid,
                                 eta,
                                 fill_value='extrapolate',
-                                kind='nearest')
+                                kind='cubic')
 
     def _initialize_get_fudge(self):
         """Initialiaze function get_fudge"""
         # if use_ivar_as_weight is set, we fix eta=1, var_lss=0 and fudge=0
         # if use_constant_weight is set, we fix eta=0, var_lss=1, and fudge=0
         # normal initialization, starting values eta=1, var_lss=0.2 , and fudge=0
         if not self.use_ivar_as_weight and not self.use_constant_weight:
             # this bit is what is actually freeing fudge for the fit
             self.fit_variance_functions.append("fudge")
-        fudge = np.zeros(self.num_bins_variance)
+        fudge = np.zeros(self.num_bins_variance) + FUDGE_DEFAULT
         self.get_fudge = interp1d(self.log_lambda_var_func_grid,
                                   fudge,
                                   fill_value='extrapolate',
-                                  kind='nearest')
+                                  kind='cubic')
 
     def _initialize_get_var_lss(self):
         """Initialiaze function get_var_lss"""
         # if use_ivar_as_weight is set, we fix eta=1, var_lss=0 and fudge=0
         if self.use_ivar_as_weight:
             var_lss = np.zeros(self.num_bins_variance)
         # if use_constant_weight is set, we fix eta=0, var_lss=1, and fudge=0
         elif self.use_constant_weight:
             var_lss = np.ones(self.num_bins_variance)
         # normal initialization, starting values eta=1, var_lss=0.2 , and fudge=0
         else:
-            var_lss = np.zeros(self.num_bins_variance) + 0.2
+            var_lss = np.zeros(self.num_bins_variance) + VAR_LSS_DEFAULT
             # this bit is what is actually freeing var_lss for the fit
             self.fit_variance_functions.append("var_lss")
         self.get_var_lss = interp1d(self.log_lambda_var_func_grid,
                                     var_lss,
                                     fill_value='extrapolate',
-                                    kind='nearest')
+                                    kind='cubic')
 
     def _initialize_variance_functions(self):
         """Initialize variance functions
         The initialized arrays are:
         - self.get_eta
         - self.get_fudge
         - self.get_num_pixels
@@ -525,26 +525,17 @@
         A list of Forest from which to compute the deltas.
 
         Raise
         -----
         ExpectedFluxError if wavelength solution is not valid
         """
         # initialize arrays
-        if "eta" in self.fit_variance_functions:
-            eta = np.zeros(self.num_bins_variance) + ETA_FIT_START
-        else:
-            eta = self.get_eta(self.log_lambda_var_func_grid)
-        if "var_lss" in self.fit_variance_functions:
-            var_lss = np.zeros(self.num_bins_variance) + VAR_LSS_FIT_START
-        else:
-            var_lss = self.get_var_lss(self.log_lambda_var_func_grid)
-        if "fudge" in self.fit_variance_functions:
-            fudge = np.zeros(self.num_bins_variance) + FUDGE_FIT_START
-        else:
-            fudge = self.get_fudge(self.log_lambda_var_func_grid)
+        eta = self.get_eta(self.log_lambda_var_func_grid)
+        var_lss = self.get_var_lss(self.log_lambda_var_func_grid)
+        fudge = self.get_fudge(self.log_lambda_var_func_grid)
         num_pixels = np.zeros(self.num_bins_variance)
         valid_fit = np.zeros(self.num_bins_variance)
 
         chi2_in_bin = np.zeros(self.num_bins_variance)
 
         # initialize the fitter class
         leasts_squares = LeastsSquaresVarStats(
@@ -583,17 +574,17 @@
             if minimizer.valid:
                 minimizer.hesse()
                 eta[index] = minimizer.values["eta"]
                 var_lss[index] = minimizer.values["var_lss"]
                 fudge[index] = minimizer.values["fudge"] * FUDGE_REF
                 valid_fit[index] = True
             else:
-                eta[index] = 1.
-                var_lss[index] = 0.1
-                fudge[index] = 1. * FUDGE_REF
+                eta[index] = ETA_DEFAULT
+                var_lss[index] = VAR_LSS_DEFAULT
+                fudge[index] = FUDGE_DEFAULT
                 valid_fit[index] = False
             num_pixels[index] = leasts_squares.get_num_pixels()
             chi2_in_bin[index] = minimizer.fval
 
             self.logger.progress(
                 f" {self.log_lambda_var_func_grid[index]:.3e} "
                 f"{eta[index]:.2e} {var_lss[index]:.2e} {fudge[index]:.2e} "
@@ -601,23 +592,23 @@
             )
 
         w = num_pixels > 0
 
         self.get_eta = interp1d(self.log_lambda_var_func_grid[w],
                                 eta[w],
                                 fill_value="extrapolate",
-                                kind="nearest")
+                                kind="cubic")
         self.get_var_lss = interp1d(self.log_lambda_var_func_grid[w],
                                     var_lss[w],
                                     fill_value="extrapolate",
-                                    kind="nearest")
+                                    kind="cubic")
         self.get_fudge = interp1d(self.log_lambda_var_func_grid[w],
                                   fudge[w],
                                   fill_value="extrapolate",
-                                  kind="nearest")
+                                  kind="cubic")
         self.get_num_pixels = interp1d(self.log_lambda_var_func_grid[w],
                                        num_pixels[w],
                                        fill_value="extrapolate",
                                        kind="nearest")
         self.get_valid_fit = interp1d(self.log_lambda_var_func_grid[w],
                                       valid_fit[w],
                                       fill_value="extrapolate",
```

### Comparing `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py` & `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_expected_flux.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,21 +62,21 @@
         # initialize eta factor
         if self.eta_value.endswith(".fits") or self.eta_value.endswith(
                 ".fits.gz"):
             hdu = fitsio.FITS(self.eta_value)["VAR_FUNC"]
             self.get_eta = interp1d(hdu["LOGLAM"].read(),
                                     hdu["ETA"].read(),
                                     fill_value='extrapolate',
-                                    kind='nearest')
+                                    kind='cubic')
         else:
             eta = np.ones(self.num_bins_variance) * float(self.eta_value)
             self.get_eta = interp1d(self.log_lambda_var_func_grid,
                                     eta,
                                     fill_value='extrapolate',
-                                    kind='nearest')
+                                    kind='cubic')
         # note that for eta to be fitted, we need to include it to
         # self.fit_variance_functions:
         # self.fit_variance_functions.append("eta")
         # since we do not do it here, eta is fixed
 
     def __parse_config(self, config):
         """Parse the configuration options
```

### Comparing `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py` & `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py` & `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py` & `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py` & `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,21 +62,21 @@
         # initialize fudge factor
         if self.fudge_value.endswith(".fits") or self.fudge_value.endswith(
                 ".fits.gz"):
             hdu = fitsio.FITS(self.fudge_value)["VAR_FUNC"]
             self.get_fudge = interp1d(hdu["LOGLAM"].read(),
                                       hdu["FUDGE"].read(),
                                       fill_value='extrapolate',
-                                      kind='nearest')
+                                      kind='cubic')
         else:
             fudge = np.ones(self.num_bins_variance) * float(self.fudge_value)
             self.get_fudge = interp1d(self.log_lambda_var_func_grid,
                                       fudge,
                                       fill_value='extrapolate',
-                                      kind='nearest')
+                                      kind='cubic')
         # note that for fudge to be fitted, we need to include it to
         # self.fit_variance_functions:
         # self.fit_variance_functions.append("fudge")
         # since we do not do it here, fudge is fixed
 
     def __parse_config(self, config):
         """Parse the configuration options
```

### Comparing `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py` & `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,22 +62,22 @@
         # initialize fudge factor
         if self.var_lss_value.endswith(".fits") or self.var_lss_value.endswith(
                 ".fits.gz"):
             hdu = fitsio.FITS(self.var_lss_value)["VAR_FUNC"]
             self.get_var_lss = interp1d(hdu["LOGLAM"].read(),
                                         hdu["VAR_LSS"].read(),
                                         fill_value='extrapolate',
-                                        kind='nearest')
+                                        kind='cubic')
         else:
             var_lss = np.ones(self.num_bins_variance) * float(
                 self.var_lss_value)
             self.get_var_lss = interp1d(self.log_lambda_var_func_grid,
                                         var_lss,
                                         fill_value='extrapolate',
-                                        kind='nearest')
+                                        kind='cubic')
         # note that for var_lss to be fitted, we need to include it to
         # self.fit_variance_functions:
         # self.fit_variance_functions.append("var_lss")
         # since we do not do it here, var_lss is fixed
 
     def __parse_config(self, config):
         """Parse the configuration options
```

### Comparing `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py` & `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py` & `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/true_continuum.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     "force stack delta to zero"
 ])
 
 defaults = update_default_options(defaults, {
     "raw statistics file": "",
     "use constant weight": False,
     "force stack delta to zero": False,
-    "use splines": False,
-    "recompute var lss": True
+    "use splines": True,
+    "recompute var lss": False
 })
 
 IN_NSIDE = 16
 
 
 class TrueContinuum(ExpectedFlux):
     """Class to compute the expected flux using the true unabsorbed contiuum
@@ -75,15 +75,14 @@
     for the final results.
 
     num_bins_variance: int
     Number of bins to be used to compute variance functions and statistics as
     a function of wavelength.
     """
 
-
     def __init__(self, config):
         """Initialize class instance.
 
         Arguments
         ---------
         config: configparser.SectionProxy
         Parsed options to initialize class
@@ -166,14 +165,18 @@
         """
         forests = self.read_all_true_continua(forests)
 
         # the might be some small changes in the var_lss compared to the read
         # values due to some smoothing of the forests
         # thus, we recompute it from the actual deltas
         if self.recompute_varlss:
+            self.logger.warning(
+                'Asked for var lss recomputation, which can lead to unwanted '
+                'effects, and biased correlations. For more details see '
+                'https://github.com/igmhub/picca/issues/1009.')
             self.compute_var_lss(forests)
             # note that this does not change the output deltas but might slightly
             # affect the mean continuum so we have to compute it after updating
             # var_lss
         self.compute_mean_cont(forests)
 
         self.compute_delta_stack(forests)
@@ -391,14 +394,20 @@
             filename = resource_filename(
                 'picca', 'delta_extraction') + '/expected_fluxes/raw_stats/'
             if Forest.wave_solution == "log":
                 filename += 'colore_v9_lya_log.fits.gz'
             elif Forest.wave_solution == "lin" and np.isclose(
                     10**Forest.log_lambda_grid[1] -
                     10**Forest.log_lambda_grid[0],
+                    0.8,
+                    rtol=0.1):
+                filename += 'colore_v9_lya_lin_0.8.fits.gz'
+            elif Forest.wave_solution == "lin" and np.isclose(
+                    10**Forest.log_lambda_grid[1] -
+                    10**Forest.log_lambda_grid[0],
                     2.4,
                     rtol=0.1):
                 filename += 'colore_v9_lya_lin_2.4.fits.gz'
             elif Forest.wave_solution == "lin" and np.isclose(
                     10**Forest.log_lambda_grid[1] -
                     10**Forest.log_lambda_grid[0],
                     3.2,
@@ -466,20 +475,20 @@
             'L_MIN', lambda_min, atol, is_rawfile_consistent, err_msg)
         # Check maximum lambda
         atol = (10**Forest.log_lambda_grid[-1] - 10**Forest.log_lambda_grid[-2])/2
         is_rawfile_consistent, err_msg = _check_header_consistency(
             'L_MAX', lambda_max, atol, is_rawfile_consistent, err_msg)
         # Check minimum rest-frame lambda
         atol = (10**Forest.log_lambda_rest_frame_grid[1]
-              - 10**Forest.log_lambda_rest_frame_grid[0])/2
+                - 10**Forest.log_lambda_rest_frame_grid[0])/2
         is_rawfile_consistent, err_msg = _check_header_consistency(
             'LR_MIN', lambda_rest_min, atol, is_rawfile_consistent, err_msg)
         # Check maximum rest-frame lambda
         atol = (10**Forest.log_lambda_rest_frame_grid[-1]
-              - 10**Forest.log_lambda_rest_frame_grid[-2])/2
+                - 10**Forest.log_lambda_rest_frame_grid[-2])/2
         is_rawfile_consistent, err_msg = _check_header_consistency(
             'LR_MAX', lambda_rest_max, atol, is_rawfile_consistent, err_msg)
 
         if not is_rawfile_consistent:
             raise ExpectedFluxError(err_msg)
 
         if self.use_splines:
@@ -490,20 +499,20 @@
             mean_flux = fits_data['MEANFLUX']
 
         var_lss = flux_variance / mean_flux**2
 
         self.get_var_lss = interp1d(log_lambda,
                                     var_lss,
                                     fill_value='extrapolate',
-                                    kind='nearest')
+                                    kind='cubic')
 
         self.get_mean_flux = interp1d(log_lambda,
                                       mean_flux,
                                       fill_value='extrapolate',
-                                      kind='nearest')
+                                      kind='cubic')
 
     def compute_var_lss(self, forests):
         """Compute var lss from delta variance by substracting
         the pipeline variance from it
 
         Arguments
         ---------
@@ -523,8 +532,8 @@
             counts[log_lambda_bins] += 1
 
         w = counts > 0
         var_lss[w] /= counts[w]
         self.get_var_lss = interp1d(Forest.log_lambda_grid[w],
                                     var_lss[w],
                                     fill_value='extrapolate',
-                                    kind='nearest')
+                                    kind='cubic')
```

### Comparing `picca-7.1.0/py/picca/delta_extraction/expected_fluxes/utils.py` & `picca-7.2.0/py/picca/delta_extraction/expected_fluxes/utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py` & `picca-7.2.0/py/picca/delta_extraction/least_squares/least_squares_cont_model.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py` & `picca-7.2.0/py/picca/delta_extraction/least_squares/least_squares_var_stats.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/mask.py` & `picca-7.2.0/py/picca/delta_extraction/mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/masks/absorber_mask.py` & `picca-7.2.0/py/picca/delta_extraction/masks/absorber_mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/masks/bal_mask.py` & `picca-7.2.0/py/picca/delta_extraction/masks/bal_mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/masks/dla_mask.py` & `picca-7.2.0/py/picca/delta_extraction/masks/dla_mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/masks/lines_mask.py` & `picca-7.2.0/py/picca/delta_extraction/masks/lines_mask.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/quasar_catalogue.py` & `picca-7.2.0/py/picca/delta_extraction/quasar_catalogue.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py` & `picca-7.2.0/py/picca/delta_extraction/quasar_catalogues/desi_quasar_catalogue.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py` & `picca-7.2.0/py/picca/delta_extraction/quasar_catalogues/drq_catalogue.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/rejection_log.py` & `picca-7.2.0/py/picca/delta_extraction/rejection_log.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py` & `picca-7.2.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_image.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py` & `picca-7.2.0/py/picca/delta_extraction/rejection_logs/rejection_log_from_table.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/survey.py` & `picca-7.2.0/py/picca/delta_extraction/survey.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/utils.py` & `picca-7.2.0/py/picca/delta_extraction/utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/delta_extraction/utils_pk1d.py` & `picca-7.2.0/py/picca/delta_extraction/utils_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/dla.py` & `picca-7.2.0/py/picca/dla.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/chi2.py` & `picca-7.2.0/py/picca/fitter2/chi2.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/control.py` & `picca-7.2.0/py/picca/fitter2/control.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/control_mpi.py` & `picca-7.2.0/py/picca/fitter2/control_mpi.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/data.py` & `picca-7.2.0/py/picca/fitter2/data.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/effective-bins.py` & `picca-7.2.0/py/picca/fitter2/effective-bins.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits` & `picca-7.2.0/py/picca/fitter2/models/DR16_blind_test_large/DR16_blind_test_large.fits`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits` & `picca-7.2.0/py/picca/fitter2/models/DR16_blind_test_small/DR16_blind_test_small.fits`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits` & `picca-7.2.0/py/picca/fitter2/models/DR9LyaMocks/DR9LyaMocks.fits`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/models/Planck18/Planck18_z_2.406.fits` & `picca-7.2.0/py/picca/fitter2/models/Planck18/Planck18_z_2.406.fits`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits` & `picca-7.2.0/py/picca/fitter2/models/PlanckDR12/PlanckDR12.fits`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits` & `picca-7.2.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16.fits`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits` & `picca-7.2.0/py/picca/fitter2/models/PlanckDR16/PlanckDR16_z_2.334.fits`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/myGamma.py` & `picca-7.2.0/py/picca/fitter2/myGamma.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/parser.py` & `picca-7.2.0/py/picca/fitter2/parser.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/pk.py` & `picca-7.2.0/py/picca/fitter2/pk.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/priors.py` & `picca-7.2.0/py/picca/fitter2/priors.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/sampler.py` & `picca-7.2.0/py/picca/fitter2/sampler.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/utils.py` & `picca-7.2.0/py/picca/fitter2/utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/fitter2/xi.py` & `picca-7.2.0/py/picca/fitter2/xi.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/io.py` & `picca-7.2.0/py/picca/io.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/pk1d/compute_pk1d.py` & `picca-7.2.0/py/picca/pk1d/compute_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/pk1d/postproc_pk1d.py` & `picca-7.2.0/py/picca/pk1d/postproc_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/pk1d/prep_pk1d.py` & `picca-7.2.0/py/picca/pk1d/prep_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/pk1d/utils.py` & `picca-7.2.0/py/picca/pk1d/utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/prep_del.py` & `picca-7.2.0/py/picca/prep_del.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/raw_io.py` & `picca-7.2.0/py/picca/raw_io.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/delta_extraction/abstract_test.py` & `picca-7.2.0/py/picca/tests/delta_extraction/abstract_test.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/delta_extraction/astronomical_object_tests.py` & `picca-7.2.0/py/picca/tests/delta_extraction/astronomical_object_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/delta_extraction/config_tests.py` & `picca-7.2.0/py/picca/tests/delta_extraction/config_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/delta_extraction/correction_tests.py` & `picca-7.2.0/py/picca/tests/delta_extraction/correction_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/delta_extraction/data_tests.py` & `picca-7.2.0/py/picca/tests/delta_extraction/data_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/delta_extraction/expected_flux_tests.py` & `picca-7.2.0/py/picca/tests/delta_extraction/expected_flux_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1538,15 +1538,15 @@
         # compare var_lss data with obtained results
         var_lss = expected_flux.get_var_lss(expectations["log_lambda"])
         if not np.allclose(var_lss, expectations["var_lss"]):
             print(f"\nOriginal file: {test_file}")
             print(f"New file: {out_file}")
             print("Difference found in var_lss")
             print(f"result test are_close result-test")
-            for i1, i2 in zip(mean_cont, expectations["var_lss"]):
+            for i1, i2 in zip(var_lss, expectations["var_lss"]):
                 print(i1, i2, np.isclose(i1, i2), i1-i2)
         self.assertTrue(np.allclose(var_lss, expectations["var_lss"]))
 
         # compare mean_flux data with obtained results
         mean_flux = expected_flux.get_mean_flux(expectations["log_lambda"])
         if not np.allclose(mean_flux, expectations["mean_flux"]):
             print(f"\nOriginal file: {test_file}")
@@ -1601,26 +1601,26 @@
         # compare var_lss data with obtained results
         var_lss = expected_flux.get_var_lss(expectations["log_lambda"])
         if not np.allclose(var_lss, expectations["var_lss"]):
             print(f"\nOriginal file: {test_file}")
             print(f"New file: {out_file}")
             print("Difference found in var_lss")
             print(f"result test are_close result-test")
-            for i1, i2 in zip(mean_cont, expectations["var_lss"]):
+            for i1, i2 in zip(var_lss, expectations["var_lss"]):
                 print(i1, i2, np.isclose(i1, i2), i1-i2)
         self.assertTrue(np.allclose(var_lss, expectations["var_lss"]))
 
         # compare mean_flux data with obtained results
         mean_flux = expected_flux.get_mean_flux(expectations["log_lambda"])
         if not np.allclose(mean_flux, expectations["mean_flux"]):
             print(f"\nOriginal file: {test_file}")
             print(f"New file: {out_file}")
             print("Difference found in mean_flux")
             print(f"result test are_close result-test")
-            for i1, i2 in zip(mean_cont, expectations["mean_flux"]):
+            for i1, i2 in zip(mean_flux, expectations["mean_flux"]):
                 print(i1, i2, np.isclose(i1, i2), i1-i2)
         self.assertTrue(np.allclose(mean_flux, expectations["mean_flux"]))
 
     def test_true_continuum_read_true_continuum_lin(self):
         """Test reading true continuum from mocks for linear wavelength solution"""
         setup_forest("lin", pixel_step=2.4)
 
@@ -1817,15 +1817,22 @@
 
         # compute the forest continua
         data.forests = expected_flux.read_all_true_continua(data.forests)
 
         # run populate_los_ids
         expected_flux.populate_los_ids(data.forests)
 
+        
+
+        for i, key in enumerate(("mean expected flux", "weights", "continuum")):
+            out_file = f"{THIS_DIR}/results/los_ids_{i}.txt"
+            np.savetxt(out_file,expected_flux.los_ids[59152][key])
+
         for i, key in enumerate(("mean expected flux", "weights", "continuum")):
+            test_file = f"{test_folder}/los_ids_{i}.txt"
             self.assertTrue(np.allclose(
                 expected_flux.los_ids[59152][key],
-                np.loadtxt(f"{test_folder}/los_ids_{i}.txt")
+                np.loadtxt(test_file)
             ))
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `picca-7.1.0/py/picca/tests/delta_extraction/mask_tests.py` & `picca-7.2.0/py/picca/tests/delta_extraction/mask_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py` & `picca-7.2.0/py/picca/tests/delta_extraction/quasar_catalogue_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/delta_extraction/scripts_tests.py` & `picca-7.2.0/py/picca/tests/delta_extraction/scripts_tests.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/delta_extraction/test_utils.py` & `picca-7.2.0/py/picca/tests/delta_extraction/test_utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/old/test_1_deltas.py` & `picca-7.2.0/py/picca/tests/old/test_1_deltas.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/old/test_4_fitter2.py` & `picca-7.2.0/py/picca/tests/old/test_4_fitter2.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/test_2_pk1d.py` & `picca-7.2.0/py/picca/tests/test_2_pk1d.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/test_3_cor.py` & `picca-7.2.0/py/picca/tests/test_3_cor.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/tests/test_helpers.py` & `picca-7.2.0/py/picca/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/utils.py` & `picca-7.2.0/py/picca/utils.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/wedgize.py` & `picca-7.2.0/py/picca/wedgize.py`

 * *Files identical despite different names*

### Comparing `picca-7.1.0/py/picca/xcf.py` & `picca-7.2.0/py/picca/xcf.py`

 * *Files 1% similar despite different names*

```diff
@@ -860,46 +860,43 @@
     """
     xi_1d = np.zeros(num_bins_r_par)
     weights1d = np.zeros(num_bins_r_par)
     r_par1d = np.zeros(num_bins_r_par)
     z1d = np.zeros(num_bins_r_par)
     num_pairs1d = np.zeros(num_bins_r_par, dtype=np.int64)
 
+    # not used only defined so that we can run compute_xi_forest_pairs_fast
+    r_trans1d = np.zeros(num_bins_r_par)
+
     for healpix in healpixs:
         for delta in data[healpix]:
 
             neighbours = [
                 obj for obj in objs[healpix] if obj.thingid == delta.thingid
             ]
             if len(neighbours) == 0:
                 continue
 
             z_qso = [obj.z_qso for obj in neighbours]
             weights_qso = [obj.weights for obj in neighbours]
             lambda_qso = [10.**obj.log_lambda for obj in neighbours]
             ang = np.zeros(len(lambda_qso))
 
-            (rebin_weight, rebin_xi, rebin_r_par, _, rebin_z,
-             rebin_num_pairs) = compute_xi_forest_pairs_fast(
+            compute_xi_forest_pairs_fast(
                  delta.z, 10.**delta.log_lambda, 10.**delta.log_lambda,
                  delta.weights, delta.delta, z_qso, lambda_qso, lambda_qso,
-                 weights_qso, ang)
-
-            xi_1d[:rebin_xi.size] += rebin_xi
-            weights1d[:rebin_weight.size] += rebin_weight
-            r_par1d[:rebin_r_par.size] += rebin_r_par
-            z1d[:rebin_z.size] += rebin_z
-            num_pairs1d[:rebin_num_pairs.size] += rebin_num_pairs.astype(int)
+                 weights_qso, ang, weights1d, xi_1d, r_par1d, r_trans1d, z1d,
+                 num_pairs1d)
 
     w = weights1d > 0.
     xi_1d[w] /= weights1d[w]
     r_par1d[w] /= weights1d[w]
-    z[w] /= weights1d[w]
+    z1d[w] /= weights1d[w]
 
-    return weights1d, xi_1d, r_par1d, z, num_pairs1d
+    return weights1d, xi_1d, r_par1d, z1d, num_pairs1d
 
 
 @njit
 def compute_wickT1234_pairs(ang, r_comov1, r_comov2, z1, z2, weights1, weights2,
                             weighted_xi_1d_1, weights_wick, num_pairs_wick, t1,
                             t2, t3, t4):
     """
```

### Comparing `picca-7.1.0/py/picca.egg-info/PKG-INFO` & `picca-7.2.0/py/picca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picca
-Version: 7.1.0
+Version: 7.2.0
 Summary: Package for Igm Cosmological-Correlations Analyses
 Home-page: https://github.com/igmhub/picca
 Author: Nicolas Busca, Helion du Mas des Bourboux, Ignasi Pérez-Ràfols, Michael Walther, the DESI Lya forest picca topical group, et al
 Author-email: iprafols@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `picca-7.1.0/py/picca.egg-info/SOURCES.txt` & `picca-7.2.0/py/picca.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_expected_flux.py
 py/picca/delta_extraction/expected_fluxes/dr16_fixed_eta_varlss_fudge_expected_flux.py
 py/picca/delta_extraction/expected_fluxes/dr16_fixed_fudge_expected_flux.py
 py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_expected_flux.py
 py/picca/delta_extraction/expected_fluxes/dr16_fixed_varlss_fudge_expected_flux.py
 py/picca/delta_extraction/expected_fluxes/true_continuum.py
 py/picca/delta_extraction/expected_fluxes/utils.py
+py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_0.8.fits.gz
 py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_2.4.fits.gz
 py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_lin_3.2.fits.gz
 py/picca/delta_extraction/expected_fluxes/raw_stats/colore_v9_lya_log.fits.gz
 py/picca/delta_extraction/least_squares/__init__.py
 py/picca/delta_extraction/least_squares/least_squares_cont_model.py
 py/picca/delta_extraction/least_squares/least_squares_var_stats.py
 py/picca/delta_extraction/masks/__init__.py
```

### Comparing `picca-7.1.0/setup.py` & `picca-7.2.0/setup.py`

 * *Files identical despite different names*

