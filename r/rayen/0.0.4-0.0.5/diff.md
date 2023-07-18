# Comparing `tmp/rayen-0.0.4.tar.gz` & `tmp/rayen-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayen-0.0.4.tar", last modified: Mon Jul 17 08:31:03 2023, max compression
+gzip compressed data, was "rayen-0.0.5.tar", last modified: Tue Jul 18 09:01:11 2023, max compression
```

## Comparing `rayen-0.0.4.tar` & `rayen-0.0.5.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.139711 rayen-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-17 08:30:40.000000 rayen-0.0.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.123710 rayen-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.123710 rayen-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-17 08:30:40.000000 rayen-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-17 08:30:40.000000 rayen-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-17 08:30:40.000000 rayen-0.0.4/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-17 08:30:40.000000 rayen-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-17 08:31:03.139711 rayen-0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.127710 rayen-0.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/cost_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/examples_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/first_figure.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/fixpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    18486 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.127710 rayen-0.0.4/examples/other/
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/other/FindGurobi.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    23976 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/other/derivation_equations.lyx
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/other/plot_examples_with_mayavi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/other/test_bug_logpcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/other/testing_sdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/other_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/requirements_examples.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.127710 rayen-0.0.4/examples/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.131710 rayen-0.0.4/examples/scripts/matlab/
--rw-r--r--   0 runner    (1001) docker     (123)    29620 2023-07-17 08:30:40.000000 rayen-0.0.4/examples/scripts/matlab/MyClampedUniformSpline.m
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/corridor_dim2.mat
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/corridor_dim3.mat
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/doSetup.m
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/getABVerticesgivenP1P2.m
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/getCorridorAndParamsSpline.m
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/handling_degenerate_cases.m
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/my_test.m
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/plotStuff.m
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/plot_eigenvalues.m
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/test_idea_ellipsoids.m
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/test_idea_equality_and_inequality.m
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/testing_accel_and_vel_costs.m
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/traj_planning_in_corridor.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.131710 rayen-0.0.4/examples/scripts/matlab/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.135711 rayen-0.0.4/examples/scripts/matlab/utils/breakyaxis/
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/breakyaxis/breakyaxis.m
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/breakyaxis/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/containsSymCasadi.m
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/convertMX2Matlab.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.135711 rayen-0.0.4/examples/scripts/matlab/utils/cprnd/
--rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/cprnd/chebycenter.m
--rwxr-xr-x   0 runner    (1001) docker     (123)     9987 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/cprnd/cprnd.m
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/cprnd/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/getAbLinearConstraints.m
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/getAb_Box2D.m
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/getAb_Box3D.m
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/getAllPqrQuadraticConstraints.m
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/getCoeffPolyCasadi.m
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/getIneqAndEqConstraintsFromOptiCasadi.m
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/getPandqandrOfQuadraticExpressionCasadi.m
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/getTCasadi.m
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/isMinusInfCasadi.m
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/isPlusInfCasadi.m
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/keepOnlyVerticesConvexHull.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.135711 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/CIELab_to_DIN99.m
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/CIELab_to_DIN99o.m
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23968 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor.m
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor_demo.m
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor_doc.m
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor_view.m
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/sRGB_to_CIELab.m
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/sRGB_to_OKLab.m
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/sRGB_to_OSAUCS.m
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/test_CIELab.m
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/test_DIN99x.m
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/test_OKLab.m
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/test_OSAUCS.m
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/testfun_mdc.m
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/plot2dConvHullAndVertices.m
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/plot3dConvHullAndVertices.m
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/plotConvexHullOfPoints.m
--rw-r--r--   0 runner    (1001) docker     (123)    15776 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/plotregion.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.135711 rayen-0.0.4/examples/scripts/matlab/utils/polytopes/
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/polytopes/addBounds.m
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/polytopes/intersectionHull.m
--rw-r--r--   0 runner    (1001) docker     (123)    15372 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/polytopes/lcon2vert.m
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/polytopes/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/polytopes/qlcon2vert.m
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/polytopes/separateBounds.m
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/polytopes/unionHull.m
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/polytopes/vert2lcon.m
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/randInInterval.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.135711 rayen-0.0.4/examples/scripts/matlab/utils/samplePoints/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/samplePoints/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/samplePoints/samplePoints.m
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/uniformSampleInUnitBall.m
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/matlab/utils/uniformSampleInUnitSphere.m
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/merge_all_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/plot_losses_vs_time.m
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/plot_time_results.m
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/plot_trajectories_RAYEN.m
--rwxr-xr-x   0 runner    (1001) docker     (123)     4188 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/time_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/scripts/train.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/test_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-07-17 08:30:41.000000 rayen-0.0.4/examples/utils_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.139711 rayen-0.0.4/imgs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-17 08:30:41.000000 rayen-0.0.4/imgs/diamond.svg
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-17 08:30:41.000000 rayen-0.0.4/imgs/green-tick.png
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 08:30:41.000000 rayen-0.0.4/imgs/rayen.png
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 08:30:41.000000 rayen-0.0.4/imgs/rayen_equations.png
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-17 08:30:41.000000 rayen-0.0.4/imgs/rayen_rays.png
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-17 08:30:41.000000 rayen-0.0.4/imgs/red_cross.svg
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-17 08:30:41.000000 rayen-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.139711 rayen-0.0.4/rayen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:30:41.000000 rayen-0.0.4/rayen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-07-17 08:30:41.000000 rayen-0.0.4/rayen/constraint_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-07-17 08:30:41.000000 rayen-0.0.4/rayen/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-07-17 08:30:41.000000 rayen-0.0.4/rayen/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:31:03.139711 rayen-0.0.4/rayen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-17 08:31:03.000000 rayen-0.0.4/rayen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-17 08:31:03.000000 rayen-0.0.4/rayen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:31:03.000000 rayen-0.0.4/rayen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-17 08:31:03.000000 rayen-0.0.4/rayen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:31:03.000000 rayen-0.0.4/rayen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-07-17 08:30:41.000000 rayen-0.0.4/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:31:03.139711 rayen-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.484894 rayen-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-18 09:00:57.000000 rayen-0.0.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.468893 rayen-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.472893 rayen-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-18 09:00:57.000000 rayen-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-18 09:00:57.000000 rayen-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-18 09:00:57.000000 rayen-0.0.5/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-18 09:00:57.000000 rayen-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-18 09:01:11.484894 rayen-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.472893 rayen-0.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/cost_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/examples_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/first_figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/fixpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18486 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.472893 rayen-0.0.5/examples/other/
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/other/FindGurobi.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    23976 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/other/derivation_equations.lyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/other/plot_examples_with_mayavi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/other/test_bug_logpcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/other/testing_sdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/other_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/requirements_examples.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.472893 rayen-0.0.5/examples/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.476893 rayen-0.0.5/examples/scripts/matlab/
+-rw-r--r--   0 runner    (1001) docker     (123)    29620 2023-07-18 09:00:57.000000 rayen-0.0.5/examples/scripts/matlab/MyClampedUniformSpline.m
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/corridor_dim2.mat
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/corridor_dim3.mat
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/doSetup.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/getABVerticesgivenP1P2.m
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/getCorridorAndParamsSpline.m
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/handling_degenerate_cases.m
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/my_test.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/plotStuff.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/plot_eigenvalues.m
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/test_idea_ellipsoids.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/test_idea_equality_and_inequality.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/testing_accel_and_vel_costs.m
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/traj_planning_in_corridor.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.476893 rayen-0.0.5/examples/scripts/matlab/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.476893 rayen-0.0.5/examples/scripts/matlab/utils/breakyaxis/
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/breakyaxis/breakyaxis.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/breakyaxis/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/containsSymCasadi.m
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/convertMX2Matlab.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.476893 rayen-0.0.5/examples/scripts/matlab/utils/cprnd/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/cprnd/chebycenter.m
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9987 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/cprnd/cprnd.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/cprnd/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/getAbLinearConstraints.m
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/getAb_Box2D.m
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/getAb_Box3D.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/getAllPqrQuadraticConstraints.m
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/getCoeffPolyCasadi.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/getIneqAndEqConstraintsFromOptiCasadi.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/getPandqandrOfQuadraticExpressionCasadi.m
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/getTCasadi.m
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/isMinusInfCasadi.m
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/isPlusInfCasadi.m
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/keepOnlyVerticesConvexHull.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.480893 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/CIELab_to_DIN99.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/CIELab_to_DIN99o.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23968 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor_demo.m
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor_doc.m
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor_view.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/sRGB_to_CIELab.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/sRGB_to_OKLab.m
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/sRGB_to_OSAUCS.m
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/test_CIELab.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/test_DIN99x.m
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/test_OKLab.m
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/test_OSAUCS.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/testfun_mdc.m
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/plot2dConvHullAndVertices.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/plot3dConvHullAndVertices.m
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/plotConvexHullOfPoints.m
+-rw-r--r--   0 runner    (1001) docker     (123)    15776 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/plotregion.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.480893 rayen-0.0.5/examples/scripts/matlab/utils/polytopes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/polytopes/addBounds.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/polytopes/intersectionHull.m
+-rw-r--r--   0 runner    (1001) docker     (123)    15372 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/polytopes/lcon2vert.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/polytopes/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/polytopes/qlcon2vert.m
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/polytopes/separateBounds.m
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/polytopes/unionHull.m
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/polytopes/vert2lcon.m
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/randInInterval.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.480893 rayen-0.0.5/examples/scripts/matlab/utils/samplePoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/samplePoints/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/samplePoints/samplePoints.m
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/uniformSampleInUnitBall.m
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/matlab/utils/uniformSampleInUnitSphere.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/merge_all_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/plot_losses_vs_time.m
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/plot_time_results.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/plot_trajectories_RAYEN.m
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4188 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/time_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/scripts/train.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/test_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-07-18 09:00:58.000000 rayen-0.0.5/examples/utils_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.480893 rayen-0.0.5/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-18 09:00:58.000000 rayen-0.0.5/imgs/diamond.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-18 09:00:58.000000 rayen-0.0.5/imgs/green-tick.png
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-18 09:00:58.000000 rayen-0.0.5/imgs/rayen.png
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-18 09:00:58.000000 rayen-0.0.5/imgs/rayen_equations.png
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-18 09:00:58.000000 rayen-0.0.5/imgs/rayen_rays.png
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-18 09:00:58.000000 rayen-0.0.5/imgs/red_cross.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-18 09:00:58.000000 rayen-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.480893 rayen-0.0.5/rayen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:00:58.000000 rayen-0.0.5/rayen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20384 2023-07-18 09:00:58.000000 rayen-0.0.5/rayen/constraint_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18396 2023-07-18 09:00:58.000000 rayen-0.0.5/rayen/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-07-18 09:00:58.000000 rayen-0.0.5/rayen/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:01:11.484894 rayen-0.0.5/rayen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-18 09:01:11.000000 rayen-0.0.5/rayen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-18 09:01:11.000000 rayen-0.0.5/rayen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:01:11.000000 rayen-0.0.5/rayen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-18 09:01:11.000000 rayen-0.0.5/rayen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 09:01:11.000000 rayen-0.0.5/rayen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-07-18 09:00:58.000000 rayen-0.0.5/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:01:11.484894 rayen-0.0.5/setup.cfg
```

### Comparing `rayen-0.0.4/.github/workflows/python-publish.yml` & `rayen-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/.gitignore` & `rayen-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/LICENSE` & `rayen-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/PKG-INFO` & `rayen-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayen
-Version: 0.0.4
+Version: 0.0.5
 Summary: Imposition of Hard Convex Constraints on Neural Networks
 Author-email: Jesus Tordesillas <jtordesillas@ethz.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Robotic Systems Lab - Legged Robotics at ETH Zürich
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `rayen-0.0.4/examples/cost_computer.py` & `rayen-0.0.5/examples/cost_computer.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/create_dataset.py` & `rayen-0.0.5/examples/create_dataset.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/early_stopping.py` & `rayen-0.0.5/examples/early_stopping.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/examples_sets.py` & `rayen-0.0.5/examples/examples_sets.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/first_figure.py` & `rayen-0.0.5/examples/first_figure.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/main.py` & `rayen-0.0.5/examples/main.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/other/FindGurobi.cmake` & `rayen-0.0.5/examples/other/FindGurobi.cmake`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/other/derivation_equations.lyx` & `rayen-0.0.5/examples/other/derivation_equations.lyx`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/other/plot_examples_with_mayavi.py` & `rayen-0.0.5/examples/other/plot_examples_with_mayavi.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/other/test_bug_logpcg.py` & `rayen-0.0.5/examples/other/test_bug_logpcg.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/other/testing_sdp.py` & `rayen-0.0.5/examples/other/testing_sdp.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/other_utils.py` & `rayen-0.0.5/examples/other_utils.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/MyClampedUniformSpline.m` & `rayen-0.0.5/examples/scripts/matlab/MyClampedUniformSpline.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/doSetup.m` & `rayen-0.0.5/examples/scripts/matlab/doSetup.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/getABVerticesgivenP1P2.m` & `rayen-0.0.5/examples/scripts/matlab/getABVerticesgivenP1P2.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/getCorridorAndParamsSpline.m` & `rayen-0.0.5/examples/scripts/matlab/getCorridorAndParamsSpline.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/handling_degenerate_cases.m` & `rayen-0.0.5/examples/scripts/matlab/handling_degenerate_cases.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/my_test.m` & `rayen-0.0.5/examples/scripts/matlab/my_test.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/plotStuff.m` & `rayen-0.0.5/examples/scripts/matlab/plotStuff.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/plot_eigenvalues.m` & `rayen-0.0.5/examples/scripts/matlab/plot_eigenvalues.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/test_idea_ellipsoids.m` & `rayen-0.0.5/examples/scripts/matlab/test_idea_ellipsoids.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/test_idea_equality_and_inequality.m` & `rayen-0.0.5/examples/scripts/matlab/test_idea_equality_and_inequality.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/testing_accel_and_vel_costs.m` & `rayen-0.0.5/examples/scripts/matlab/testing_accel_and_vel_costs.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/traj_planning_in_corridor.m` & `rayen-0.0.5/examples/scripts/matlab/traj_planning_in_corridor.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/breakyaxis/breakyaxis.m` & `rayen-0.0.5/examples/scripts/matlab/utils/breakyaxis/breakyaxis.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/breakyaxis/license.txt` & `rayen-0.0.5/examples/scripts/matlab/utils/breakyaxis/license.txt`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/convertMX2Matlab.m` & `rayen-0.0.5/examples/scripts/matlab/utils/convertMX2Matlab.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/cprnd/cprnd.m` & `rayen-0.0.5/examples/scripts/matlab/utils/cprnd/cprnd.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/cprnd/license.txt` & `rayen-0.0.5/examples/scripts/matlab/utils/cprnd/license.txt`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/getAbLinearConstraints.m` & `rayen-0.0.5/examples/scripts/matlab/utils/getAbLinearConstraints.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/getAb_Box2D.m` & `rayen-0.0.5/examples/scripts/matlab/utils/getAb_Box2D.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/getAb_Box3D.m` & `rayen-0.0.5/examples/scripts/matlab/utils/getAb_Box3D.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/getAllPqrQuadraticConstraints.m` & `rayen-0.0.5/examples/scripts/matlab/utils/getAllPqrQuadraticConstraints.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/getCoeffPolyCasadi.m` & `rayen-0.0.5/examples/scripts/matlab/utils/getCoeffPolyCasadi.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/getIneqAndEqConstraintsFromOptiCasadi.m` & `rayen-0.0.5/examples/scripts/matlab/utils/getIneqAndEqConstraintsFromOptiCasadi.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/getPandqandrOfQuadraticExpressionCasadi.m` & `rayen-0.0.5/examples/scripts/matlab/utils/getPandqandrOfQuadraticExpressionCasadi.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/CIELab_to_DIN99.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/CIELab_to_DIN99.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/CIELab_to_DIN99o.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/CIELab_to_DIN99o.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/license.txt` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/license.txt`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor_demo.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor_demo.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor_doc.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor_doc.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor_view.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/maxdistcolor_view.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/sRGB_to_CIELab.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/sRGB_to_CIELab.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/sRGB_to_OKLab.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/sRGB_to_OKLab.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/sRGB_to_OSAUCS.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/sRGB_to_OSAUCS.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/test_CIELab.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/test_CIELab.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/test_DIN99x.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/test_DIN99x.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/test_OKLab.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/test_OKLab.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/test_OSAUCS.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/test_OSAUCS.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/maxdistcolor/testfun_mdc.m` & `rayen-0.0.5/examples/scripts/matlab/utils/maxdistcolor/testfun_mdc.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/plot3dConvHullAndVertices.m` & `rayen-0.0.5/examples/scripts/matlab/utils/plot3dConvHullAndVertices.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/plotConvexHullOfPoints.m` & `rayen-0.0.5/examples/scripts/matlab/utils/plotConvexHullOfPoints.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/plotregion.m` & `rayen-0.0.5/examples/scripts/matlab/utils/plotregion.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/polytopes/addBounds.m` & `rayen-0.0.5/examples/scripts/matlab/utils/polytopes/addBounds.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/polytopes/intersectionHull.m` & `rayen-0.0.5/examples/scripts/matlab/utils/polytopes/intersectionHull.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/polytopes/lcon2vert.m` & `rayen-0.0.5/examples/scripts/matlab/utils/polytopes/lcon2vert.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/polytopes/license.txt` & `rayen-0.0.5/examples/scripts/matlab/utils/polytopes/license.txt`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/polytopes/qlcon2vert.m` & `rayen-0.0.5/examples/scripts/matlab/utils/polytopes/qlcon2vert.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/polytopes/separateBounds.m` & `rayen-0.0.5/examples/scripts/matlab/utils/polytopes/separateBounds.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/polytopes/unionHull.m` & `rayen-0.0.5/examples/scripts/matlab/utils/polytopes/unionHull.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/polytopes/vert2lcon.m` & `rayen-0.0.5/examples/scripts/matlab/utils/polytopes/vert2lcon.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/samplePoints/license.txt` & `rayen-0.0.5/examples/scripts/matlab/utils/samplePoints/license.txt`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/samplePoints/samplePoints.m` & `rayen-0.0.5/examples/scripts/matlab/utils/samplePoints/samplePoints.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/uniformSampleInUnitBall.m` & `rayen-0.0.5/examples/scripts/matlab/utils/uniformSampleInUnitBall.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/matlab/utils/uniformSampleInUnitSphere.m` & `rayen-0.0.5/examples/scripts/matlab/utils/uniformSampleInUnitSphere.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/merge_all_results.py` & `rayen-0.0.5/examples/scripts/merge_all_results.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/plot_losses_vs_time.m` & `rayen-0.0.5/examples/scripts/plot_losses_vs_time.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/plot_time_results.m` & `rayen-0.0.5/examples/scripts/plot_time_results.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/plot_trajectories_RAYEN.m` & `rayen-0.0.5/examples/scripts/plot_trajectories_RAYEN.m`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/run.sh` & `rayen-0.0.5/examples/scripts/run.sh`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/time_analysis.py` & `rayen-0.0.5/examples/scripts/time_analysis.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/scripts/train.yaml` & `rayen-0.0.5/examples/scripts/train.yaml`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/test_layer.py` & `rayen-0.0.5/examples/test_layer.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/examples/utils_examples.py` & `rayen-0.0.5/examples/utils_examples.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/pyproject.toml` & `rayen-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "rayen"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Jesus Tordesillas", email="jtordesillas@ethz.ch" },
 ]
 description = "Imposition of Hard Convex Constraints on Neural Networks"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -30,8 +30,8 @@
 license = {file = "LICENSE"}
 
 [project.urls]
 "Homepage" = "https://github.com/leggedrobotics/rayen"
 "Bug Tracker" = "https://github.com/leggedrobotics/rayen/issues"
 
 [tool.setuptools]
-py-modules = []
+packages = ["rayen"]
```

### Comparing `rayen-0.0.4/rayen/constraint_module.py` & `rayen-0.0.5/rayen/constraint_module.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/rayen/constraints.py` & `rayen-0.0.5/rayen/constraints.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/rayen/utils.py` & `rayen-0.0.5/rayen/utils.py`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/rayen.egg-info/PKG-INFO` & `rayen-0.0.5/rayen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayen
-Version: 0.0.4
+Version: 0.0.5
 Summary: Imposition of Hard Convex Constraints on Neural Networks
 Author-email: Jesus Tordesillas <jtordesillas@ethz.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Robotic Systems Lab - Legged Robotics at ETH Zürich
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `rayen-0.0.4/rayen.egg-info/SOURCES.txt` & `rayen-0.0.5/rayen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rayen-0.0.4/readme.md` & `rayen-0.0.5/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RAYEN: Imposition of Hard Convex Constraints on Neural Networks #
 
-Paper: Coming soon....
+Paper: [http://arxiv.org/abs/2307.08336](http://arxiv.org/abs/2307.08336)
 
 This framework allows you to impose convex constraints on the output or latent variable of a Neural Network.
 ![](./imgs/rayen.png)
 
 ![](./imgs/rayen_equations.png)
 
 
@@ -16,19 +16,14 @@
 pip install --upgrade pip
 ```
 
 Then, you simply need to do:
 
 
 ```bash
-pip install rayen
-```
-
-If you want to do an editable install, you can also do:
-```bash
 git clone https://github.com/leggedrobotics/rayen.git
 cd rayen && pip install -e .
 ```
 
 # Usage
 
 A minimal example is as follows:
@@ -116,15 +111,15 @@
 git submodule init && git submodule update --init --recursive
 pip install -r examples/requirements_examples.txt
 ```
 
 These are the most important files in the `examples` folder:
 * **`test_layer.py`**: This file imposes many different constraints using all the methods shown above. It will create plots similar to the one shown at the beginning of this repo 
 * **`time_analysis.py`**: This file obtains the computation time of RAYEN when applied to many different constraints. 
-* **`run.h`**: This file will train the networks for all the algorithms used in the paper, and then evaluate them using the testing sets. Depending on the computer to use, this can take ~1 day to run. The datasets that this file uses are stored in the files `corridor_dim2.mat` (Optimization 1 of the paper, which is for a 2D scenario) and `corridor_dim3.mat` (Optimization 2 of the paper, which is for a 3D scenario). These files were generated running the file `traj_planning_in_corridor.m`. This Matlab files requires Casadi (and its interface with Gurobi) to be installed. You can do this using the instructions below
+* **`run.sh`**: This file will train the networks for all the algorithms used in the paper, and then evaluate them using the testing sets. Depending on the computer to use, this can take ~1 day to run. The datasets that this file uses are stored in the files `corridor_dim2.mat` (Optimization 1 of the paper, which is for a 2D scenario) and `corridor_dim3.mat` (Optimization 2 of the paper, which is for a 3D scenario). These files were generated running the file `traj_planning_in_corridor.m`. These Matlab files requires Casadi (and its interface with Gurobi) to be installed. You can do this using the instructions below
 
 Some of these examples use (or can use) [Gurobi Optimizer](https://www.gurobi.com/products/gurobi-optimizer/). Once installed (following the instructions in the previous link) you can test the installation typing `gurobi.sh` in the terminal. You will also need this package:
 ```
 pip install gurobipy
 ```
 
 <details>
@@ -163,15 +158,15 @@
 ```
 </details>
 
 
 <details>
   <summary> <b>Publishing to PyPI</b></summary>
 
-More info [here](https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/)
+More info [here](https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/). See also the file `python-publish.yml`
 
 First change the `version` line in `pyproject.toml`  to X.X.X. Then do the following:
 ```bash
 git add pyproject.toml && git commit -m "updated version" && git tag vX.X.X
 git push origin master vX.X.X
 
 ```
```

