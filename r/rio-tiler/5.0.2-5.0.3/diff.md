# Comparing `tmp/rio_tiler-5.0.2.tar.gz` & `tmp/rio_tiler-5.0.3.tar.gz`

## Comparing `rio_tiler-5.0.2.tar` & `rio_tiler-5.0.3.tar`

### file list

```diff
@@ -1,197 +1,197 @@
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/__init__.py
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/colormap.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/constants.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/errors.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/expression.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/logger.py
--rw-r--r--   0        0        0    25504 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/models.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/profiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/py.typed
--rw-r--r--   0        0        0    20985 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/reader.py
--rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/tasks.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/types.py
--rw-r--r--   0        0        0    21907 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/utils.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/accent.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/accent_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/afmhot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/afmhot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/autumn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/autumn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/binary.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/binary_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/blues.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/blues_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/bone.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/bone_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/brbg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/brbg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/brg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/brg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/bugn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/bugn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/bupu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/bupu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/bwr.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/bwr_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/cfastie.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/cividis.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/cividis_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/cmrmap.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/cmrmap_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/cool.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/cool_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/coolwarm.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/coolwarm_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/copper.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/copper_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/cubehelix.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/cubehelix_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/dark2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/dark2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/flag.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/flag_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_earth.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_earth_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_gray.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_gray_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_heat.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_heat_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_ncar.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_ncar_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_rainbow.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_rainbow_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_stern.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_stern_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_yarg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gist_yarg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gnbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gnbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gnuplot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gnuplot2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gnuplot2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gnuplot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gray.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/gray_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/greens.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/greens_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/greys.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/greys_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/hot.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/hot_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/hsv.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/hsv_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/inferno.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/inferno_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/jet.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/jet_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/magma.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/magma_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/nipy_spectral.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/nipy_spectral_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/ocean.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/ocean_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/oranges.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/oranges_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/orrd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/orrd_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/paired.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/paired_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/pastel1.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/pastel1_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/pastel2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/pastel2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/pink.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/pink_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/piyg.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/piyg_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/plasma.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/plasma_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/prgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/prgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/prism.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/prism_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/pubu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/pubu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/pubugn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/pubugn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/puor.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/puor_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/purd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/purd_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/purples.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/purples_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/rainbow.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/rainbow_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/rdbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/rdbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/rdgy.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/rdgy_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/rdpu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/rdpu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/rdylbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/rdylbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/rdylgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/rdylgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/reds.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/reds_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/rplumbo.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/schwarzwald.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/seismic.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/seismic_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/set1.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/set1_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/set2.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/set2_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/set3.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/set3_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/spectral.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/spectral_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/spring.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/spring_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/summer.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/summer_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/tab10.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/tab10_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/tab20.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/tab20_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/tab20b.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/tab20b_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/tab20c.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/tab20c_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/terrain.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/terrain_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/twilight.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/twilight_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/twilight_shifted.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/twilight_shifted_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/viridis.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/viridis_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/winter.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/winter_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/wistia.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/wistia_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/ylgn.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/ylgn_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/ylgnbu.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/ylgnbu_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/ylorbr.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/ylorbr_r.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/ylorrd.npy
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/cmap_data/ylorrd_r.npy
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/io/__init__.py
--rw-r--r--   0        0        0    44738 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/io/base.py
--rw-r--r--   0        0        0    31879 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/io/rasterio.py
--rw-r--r--   0        0        0    10091 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/io/stac.py
--rw-r--r--   0        0        0    16046 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/io/xarray.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/mosaic/__init__.py
--rw-r--r--   0        0        0     8111 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/mosaic/reader.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/mosaic/methods/__init__.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/mosaic/methods/base.py
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/rio_tiler/mosaic/methods/defaults.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/.gitignore
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/AUTHORS.txt
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/LICENSE
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/README.md
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/pyproject.toml
--rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 rio_tiler-5.0.2/PKG-INFO
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/__init__.py
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/colormap.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/constants.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/errors.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/expression.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/logger.py
+-rw-r--r--   0        0        0    25874 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/models.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/profiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/py.typed
+-rw-r--r--   0        0        0    21013 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/reader.py
+-rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/tasks.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/types.py
+-rw-r--r--   0        0        0    21907 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/utils.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/accent.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/accent_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/afmhot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/afmhot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/autumn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/autumn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/binary.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/binary_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/blues.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/blues_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bone.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bone_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/brbg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/brbg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/brg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/brg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bugn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bugn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bupu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bupu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bwr.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/bwr_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cfastie.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cividis.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cividis_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cmrmap.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cmrmap_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cool.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cool_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/coolwarm.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/coolwarm_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/copper.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/copper_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cubehelix.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/cubehelix_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/dark2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/dark2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/flag.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/flag_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_earth.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_earth_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_gray.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_gray_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_heat.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_heat_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_ncar.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_ncar_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_rainbow.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_rainbow_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_stern.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_stern_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_yarg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gist_yarg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gnbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gnbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gray.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/gray_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/greens.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/greens_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/greys.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/greys_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/hot.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/hot_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/hsv.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/hsv_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/inferno.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/inferno_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/jet.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/jet_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/magma.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/magma_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/nipy_spectral.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/nipy_spectral_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ocean.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ocean_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/oranges.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/oranges_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/orrd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/orrd_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/paired.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/paired_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pastel1.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pastel1_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pastel2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pastel2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pink.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pink_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/piyg.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/piyg_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/plasma.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/plasma_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/prgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/prgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/prism.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/prism_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pubu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pubu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pubugn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/pubugn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/puor.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/puor_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/purd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/purd_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/purples.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/purples_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rainbow.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rainbow_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdgy.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdgy_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdpu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdpu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdylbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdylbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdylgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rdylgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/reds.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/reds_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/rplumbo.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/schwarzwald.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/seismic.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/seismic_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/set1.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/set1_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/set2.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/set2_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/set3.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/set3_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/spectral.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/spectral_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/spring.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/spring_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/summer.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/summer_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab10.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab10_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab20.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab20_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab20b.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab20b_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab20c.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/tab20c_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/terrain.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/terrain_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/twilight.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/twilight_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/twilight_shifted.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/twilight_shifted_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/viridis.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/viridis_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/winter.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/winter_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/wistia.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/wistia_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylgn.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylgn_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylgnbu.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylgnbu_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylorbr.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylorbr_r.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylorrd.npy
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/cmap_data/ylorrd_r.npy
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/io/__init__.py
+-rw-r--r--   0        0        0    44738 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/io/base.py
+-rw-r--r--   0        0        0    32170 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/io/rasterio.py
+-rw-r--r--   0        0        0    10091 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/io/stac.py
+-rw-r--r--   0        0        0    16046 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/io/xarray.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/mosaic/__init__.py
+-rw-r--r--   0        0        0     8111 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/mosaic/reader.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/mosaic/methods/__init__.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/mosaic/methods/base.py
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/rio_tiler/mosaic/methods/defaults.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/.gitignore
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/AUTHORS.txt
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/LICENSE
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/README.md
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/pyproject.toml
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 rio_tiler-5.0.3/PKG-INFO
```

### Comparing `rio_tiler-5.0.2/rio_tiler/colormap.py` & `rio_tiler-5.0.3/rio_tiler/colormap.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/errors.py` & `rio_tiler-5.0.3/rio_tiler/errors.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/expression.py` & `rio_tiler-5.0.3/rio_tiler/expression.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/models.py` & `rio_tiler-5.0.3/rio_tiler/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from color_operations import parse_operations, scale_dtype, to_math_type
 from pydantic import BaseModel
 from rasterio import windows
 from rasterio.coords import BoundingBox
 from rasterio.crs import CRS
 from rasterio.dtypes import dtype_ranges
 from rasterio.enums import ColorInterp
+from rasterio.errors import NotGeoreferencedWarning
 from rasterio.io import MemoryFile
 from rasterio.plot import reshape_as_image
 from rasterio.transform import from_bounds
 
 from rio_tiler.colormap import apply_cmap
 from rio_tiler.errors import InvalidDatatypeWarning, InvalidPointDataError
 from rio_tiler.expression import apply_expression, get_expression_blocks
@@ -389,48 +390,54 @@
     def from_bytes(cls, data: bytes) -> "ImageData":
         """Create ImageData from bytes.
 
         Args:
             data (bytes): raster dataset as bytes.
 
         """
-        with MemoryFile(data) as m:
-            with m.open() as dataset:
-                indexes = non_alpha_indexes(dataset)
-                if ColorInterp.alpha in dataset.colorinterp:
-                    alpha_idx = dataset.colorinterp.index(ColorInterp.alpha) + 1
-                    idx = tuple(indexes) + (alpha_idx,)
-                    array = dataset.read(indexes=idx)
-
-                    mask = ~array[-1].astype("bool")
-                    array = numpy.ma.MaskedArray(array[0:-1])
-                    array.mask = mask
-
-                else:
-                    array = dataset.read(indexes=indexes, masked=True)
-
-                stats = []
-                for ix in indexes:
-                    tags = dataset.tags(ix)
-                    if all(
-                        stat in tags
-                        for stat in ["STATISTICS_MINIMUM", "STATISTICS_MAXIMUM"]
-                    ):
-                        stat_min = float(tags.get("STATISTICS_MINIMUM"))
-                        stat_max = float(tags.get("STATISTICS_MAXIMUM"))
-                        stats.append((stat_min, stat_max))
-
-                dataset_statistics = stats if len(stats) == len(indexes) else None
-
-                return cls(
-                    array,
-                    crs=dataset.crs,
-                    bounds=dataset.bounds,
-                    dataset_statistics=dataset_statistics,
-                )
+        with warnings.catch_warnings():
+            warnings.filterwarnings(
+                "ignore",
+                category=NotGeoreferencedWarning,
+                module="rasterio",
+            )
+            with MemoryFile(data) as m:
+                with m.open() as dataset:
+                    indexes = non_alpha_indexes(dataset)
+                    if ColorInterp.alpha in dataset.colorinterp:
+                        alpha_idx = dataset.colorinterp.index(ColorInterp.alpha) + 1
+                        idx = tuple(indexes) + (alpha_idx,)
+                        array = dataset.read(indexes=idx)
+
+                        mask = ~array[-1].astype("bool")
+                        array = numpy.ma.MaskedArray(array[0:-1])
+                        array.mask = mask
+
+                    else:
+                        array = dataset.read(indexes=indexes, masked=True)
+
+                    stats = []
+                    for ix in indexes:
+                        tags = dataset.tags(ix)
+                        if all(
+                            stat in tags
+                            for stat in ["STATISTICS_MINIMUM", "STATISTICS_MAXIMUM"]
+                        ):
+                            stat_min = float(tags.get("STATISTICS_MINIMUM"))
+                            stat_max = float(tags.get("STATISTICS_MAXIMUM"))
+                            stats.append((stat_min, stat_max))
+
+                    dataset_statistics = stats if len(stats) == len(indexes) else None
+
+                    return cls(
+                        array,
+                        crs=dataset.crs,
+                        bounds=dataset.bounds,
+                        dataset_statistics=dataset_statistics,
+                    )
 
     @classmethod
     def create_from_list(cls, data: Sequence["ImageData"]) -> "ImageData":
         """Create ImageData from a sequence of ImageData objects.
 
         Args:
             data (sequence): sequence of ImageData.
```

### Comparing `rio_tiler-5.0.2/rio_tiler/profiles.py` & `rio_tiler-5.0.3/rio_tiler/profiles.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/reader.py` & `rio_tiler-5.0.3/rio_tiler/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -543,14 +543,14 @@
             window=windows.Window(row_off=row, col_off=col, width=1, height=1),
             resampling_method=resampling_method,
             force_binary_mask=force_binary_mask,
             unscale=unscale,
             post_process=post_process,
         )
 
-    return PointData(
-        img.array[:, 0, 0],
-        coordinates=coordinates,
-        crs=coord_crs,
-        band_names=img.band_names,
-        metadata=dataset.tags(),
-    )
+        return PointData(
+            img.array[:, 0, 0],
+            coordinates=coordinates,
+            crs=coord_crs,
+            band_names=img.band_names,
+            metadata=dataset.tags(),
+        )
```

### Comparing `rio_tiler-5.0.2/rio_tiler/tasks.py` & `rio_tiler-5.0.3/rio_tiler/tasks.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/types.py` & `rio_tiler-5.0.3/rio_tiler/types.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/utils.py` & `rio_tiler-5.0.3/rio_tiler/utils.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/__init__.py` & `rio_tiler-5.0.3/rio_tiler/cmap_data/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/accent.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/accent.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/accent_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/accent_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/afmhot.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/afmhot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/afmhot_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/afmhot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/autumn.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/autumn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/autumn_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/autumn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/binary.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/binary.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/binary_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/binary_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/blues.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/blues.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/blues_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/blues_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/bone.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/bone.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/bone_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/bone_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/brbg.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/brbg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/brbg_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/brbg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/brg.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/brg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/brg_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/brg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/bugn.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/bugn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/bugn_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/bugn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/bupu.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/bupu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/bupu_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/bupu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/bwr.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/bwr.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/bwr_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/bwr_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/cfastie.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/cfastie.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/cividis.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/cividis.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/cividis_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/cividis_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/cmrmap.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/cmrmap.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/cmrmap_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/cmrmap_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/cool.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/cool.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/cool_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/cool_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/coolwarm.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/coolwarm.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/coolwarm_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/coolwarm_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/copper.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/copper.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/copper_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/copper_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/cubehelix.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/cubehelix.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/cubehelix_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/cubehelix_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/dark2.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/dark2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/dark2_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/dark2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/flag.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/flag.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/flag_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/flag_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_earth.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_earth.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_earth_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_earth_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_gray.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_gray.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_gray_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_gray_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_heat.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_heat.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_heat_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_heat_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_ncar.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_ncar.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_ncar_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_ncar_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_rainbow.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_rainbow.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_rainbow_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_rainbow_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_stern.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_stern.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_stern_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_stern_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_yarg.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_yarg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gist_yarg_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gist_yarg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gnbu.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gnbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gnbu_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gnbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gnuplot.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gnuplot2.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gnuplot2_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gnuplot_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gnuplot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gray.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gray.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/gray_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/gray_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/greens.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/greens.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/greens_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/greens_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/greys.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/greys.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/greys_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/greys_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/hot.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/hot.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/hot_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/hot_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/hsv.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/hsv.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/hsv_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/hsv_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/inferno.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/inferno.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/inferno_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/inferno_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/jet.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/jet.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/jet_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/jet_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/magma.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/magma.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/magma_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/magma_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/nipy_spectral.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/nipy_spectral.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/nipy_spectral_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/nipy_spectral_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/ocean.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/ocean.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/ocean_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/ocean_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/oranges.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/oranges.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/oranges_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/oranges_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/orrd.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/orrd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/orrd_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/orrd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/paired.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/paired.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/paired_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/paired_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/pastel1.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/pastel1.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/pastel1_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/pastel1_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/pastel2.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/pastel2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/pastel2_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/pastel2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/pink.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/pink.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/pink_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/pink_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/piyg.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/piyg.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/piyg_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/piyg_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/plasma.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/plasma.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/plasma_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/plasma_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/prgn.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/prgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/prgn_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/prgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/prism.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/prism.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/prism_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/prism_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/pubu.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/pubu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/pubu_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/pubu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/pubugn.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/pubugn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/pubugn_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/pubugn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/puor.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/puor.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/puor_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/puor_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/purd.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/purd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/purd_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/purd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/purples.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/purples.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/purples_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/purples_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/rainbow.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/rainbow.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/rainbow_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/rainbow_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/rdbu.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/rdbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/rdbu_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/rdbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/rdgy.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/rdgy.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/rdgy_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/rdgy_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/rdpu.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/rdpu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/rdpu_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/rdpu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/rdylbu.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/rdylbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/rdylbu_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/rdylbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/rdylgn.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/rdylgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/rdylgn_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/rdylgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/reds.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/reds.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/reds_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/reds_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/rplumbo.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/rplumbo.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/schwarzwald.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/schwarzwald.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/seismic.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/seismic.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/seismic_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/seismic_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/set1.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/set1.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/set1_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/set1_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/set2.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/set2.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/set2_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/set2_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/set3.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/set3.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/set3_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/set3_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/spectral.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/spectral.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/spectral_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/spectral_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/spring.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/spring.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/spring_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/spring_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/summer.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/summer.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/summer_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/summer_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/tab10.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/tab10.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/tab10_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/tab10_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/tab20.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/tab20.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/tab20_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/tab20_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/tab20b.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/tab20b.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/tab20b_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/tab20b_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/tab20c.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/tab20c.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/tab20c_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/tab20c_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/terrain.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/terrain.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/terrain_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/terrain_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/twilight.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/twilight.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/twilight_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/twilight_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/twilight_shifted.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/twilight_shifted.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/twilight_shifted_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/twilight_shifted_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/viridis.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/viridis.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/viridis_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/viridis_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/winter.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/winter.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/winter_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/winter_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/wistia.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/wistia.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/wistia_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/wistia_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/ylgn.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/ylgn.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/ylgn_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/ylgn_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/ylgnbu.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/ylgnbu.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/ylgnbu_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/ylgnbu_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/ylorbr.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/ylorbr.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/ylorbr_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/ylorbr_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/ylorrd.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/ylorrd.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/cmap_data/ylorrd_r.npy` & `rio_tiler-5.0.3/rio_tiler/cmap_data/ylorrd_r.npy`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/io/base.py` & `rio_tiler-5.0.3/rio_tiler/io/base.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/io/rasterio.py` & `rio_tiler-5.0.3/rio_tiler/io/rasterio.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import numpy
 import rasterio
 from affine import Affine
 from morecantile import BoundingBox, Coords, Tile, TileMatrixSet
 from morecantile.utils import _parse_tile_arg
 from rasterio import transform
 from rasterio.crs import CRS
+from rasterio.errors import NotGeoreferencedWarning
 from rasterio.features import bounds as featureBounds
 from rasterio.features import geometry_mask, rasterize
 from rasterio.io import DatasetReader, DatasetWriter, MemoryFile
 from rasterio.rio.overview import get_maximum_overview_level
 from rasterio.transform import from_bounds as transform_from_bounds
 from rasterio.vrt import WarpedVRT
 from rasterio.warp import calculate_default_transform, transform_geom
@@ -559,23 +560,30 @@
             buffer=buffer,
             **kwargs,
         )
 
         if dst_crs != shape_crs:
             shape = transform_geom(shape_crs, dst_crs, shape)
 
-        cutline_mask = rasterize(
-            [shape],
-            out_shape=(img.height, img.width),
-            transform=img.transform,
-            all_touched=True,  # Necesary for matching masks at different resolutions
-            default_value=0,
-            fill=1,
-            dtype="uint8",
-        ).astype("bool")
+        with warnings.catch_warnings():
+            warnings.filterwarnings(
+                "ignore",
+                category=NotGeoreferencedWarning,
+                module="rasterio",
+            )
+            cutline_mask = rasterize(
+                [shape],
+                out_shape=(img.height, img.width),
+                transform=img.transform,
+                all_touched=True,  # Necesary for matching masks at different resolutions
+                default_value=0,
+                fill=1,
+                dtype="uint8",
+            ).astype("bool")
+
         img.cutline_mask = cutline_mask
         img.array.mask = numpy.where(~cutline_mask, img.array.mask, True)
 
         return img
 
     def read(
         self,
```

### Comparing `rio_tiler-5.0.2/rio_tiler/io/stac.py` & `rio_tiler-5.0.3/rio_tiler/io/stac.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/io/xarray.py` & `rio_tiler-5.0.3/rio_tiler/io/xarray.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/mosaic/reader.py` & `rio_tiler-5.0.3/rio_tiler/mosaic/reader.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/mosaic/methods/__init__.py` & `rio_tiler-5.0.3/rio_tiler/mosaic/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/mosaic/methods/base.py` & `rio_tiler-5.0.3/rio_tiler/mosaic/methods/base.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/rio_tiler/mosaic/methods/defaults.py` & `rio_tiler-5.0.3/rio_tiler/mosaic/methods/defaults.py`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/.gitignore` & `rio_tiler-5.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/LICENSE` & `rio_tiler-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/README.md` & `rio_tiler-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/pyproject.toml` & `rio_tiler-5.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rio_tiler-5.0.2/PKG-INFO` & `rio_tiler-5.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-tiler
-Version: 5.0.2
+Version: 5.0.3
 Summary: User friendly Rasterio plugin to read raster datasets.
 Project-URL: Homepage, https://cogeotiff.github.io/rio-tiler/
 Project-URL: Documentation, https://cogeotiff.github.io/rio-tiler/
 Project-URL: Issues, https://github.com/cogeotiff/rio-tiler/issues
 Project-URL: Source, https://github.com/cogeotiff/rio-tiler
 Project-URL: Changelog, https://cogeotiff.github.io/rio-tiler/release-notes/
 Author-email: Vincent Sarago <vincent@developmentseed.com>
```

