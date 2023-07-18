# Comparing `tmp/spotPython-0.6.1.tar.gz` & `tmp/spotPython-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotPython-0.6.1.tar", last modified: Sun Jul 16 22:12:58 2023, max compression
+gzip compressed data, was "spotPython-0.6.3.tar", last modified: Mon Jul 17 22:32:25 2023, max compression
```

## Comparing `spotPython-0.6.1.tar` & `spotPython-0.6.3.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.525274 spotPython-0.6.1/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.469378 spotPython-0.6.1/.github/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.473697 spotPython-0.6.1/.github/workflows/
--rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.6.1/.github/workflows/test.yml
--rw-r--r--   0 bartz      (501) staff       (20)    17867 2023-07-04 14:15:14.000000 spotPython-0.6.1/.gitignore
--rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 22:04:43.000000 spotPython-0.6.1/.nojekyll
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.483348 spotPython-0.6.1/Figures.d/
--rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.6.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.6.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.6.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
--rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.6.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.6.1/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.6.1/LICENSE.txt
--rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-20 20:35:14.000000 spotPython-0.6.1/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     7578 2023-07-16 22:12:58.525100 spotPython-0.6.1/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     6808 2023-06-08 16:18:46.000000 spotPython-0.6.1/README.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.484444 spotPython-0.6.1/docs/
--rw-r--r--   0 bartz      (501) staff       (20)    46499 2022-10-31 16:48:05.000000 spotPython-0.6.1/docs/about.md
--rw-r--r--   0 bartz      (501) staff       (20)       49 2023-07-12 23:09:54.000000 spotPython-0.6.1/docs/download.md
--rw-r--r--   0 bartz      (501) staff       (20)      802 2023-07-16 08:32:11.000000 spotPython-0.6.1/docs/examples.md
--rw-r--r--   0 bartz      (501) staff       (20)      947 2022-10-31 16:48:05.000000 spotPython-0.6.1/docs/gen_ref_pages.py
--rw-r--r--   0 bartz      (501) staff       (20)      350 2023-07-14 22:03:54.000000 spotPython-0.6.1/docs/hyperparameter-tuning-cookbook.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.484671 spotPython-0.6.1/docs/images/
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2022-10-31 16:48:05.000000 spotPython-0.6.1/docs/images/favicon.png
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2022-10-31 16:48:05.000000 spotPython-0.6.1/docs/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)      392 2023-07-15 18:25:23.000000 spotPython-0.6.1/docs/index.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.485339 spotPython-0.6.1/img/
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2023-07-13 05:52:18.000000 spotPython-0.6.1/img/favicon.png
--rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-27 21:03:27.000000 spotPython-0.6.1/img/spotLogo.png
--rwxr-xr-x   0 bartz      (501) staff       (20)      146 2023-07-15 09:35:47.000000 spotPython-0.6.1/makeSpot.sh
--rw-r--r--   0 bartz      (501) staff       (20)     1487 2023-07-15 23:01:11.000000 spotPython-0.6.1/mkdocs.yml
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.487480 spotPython-0.6.1/notebooks/
--rw-r--r--   0 bartz      (501) staff       (20)    64826 2023-07-15 20:49:26.000000 spotPython-0.6.1/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
--rw-r--r--   0 bartz      (501) staff       (20)   953519 2023-07-04 14:15:14.000000 spotPython-0.6.1/notebooks/31_spot_lightning_csv.ipynb
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.469837 spotPython-0.6.1/notebooks/data/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.487759 spotPython-0.6.1/notebooks/data/torch/
--rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.6.1/notebooks/data/torch/model_spot_trained.pt
--rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.6.1/notebooks/data.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.504998 spotPython-0.6.1/notebooks/figures/
--rw-r--r--   0 bartz      (501) staff       (20)   114797 2023-06-07 17:28:19.000000 spotPython-0.6.1/notebooks/figures/12-torch_p040025_1min_5init_2023-06-07_19-09-30_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)   117891 2023-06-08 12:22:25.000000 spotPython-0.6.1/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    35435 2023-06-08 12:22:25.000000 spotPython-0.6.1/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    41877 2023-06-08 12:22:25.000000 spotPython-0.6.1/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   117933 2023-06-07 11:49:47.000000 spotPython-0.6.1/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    29392 2023-06-07 11:04:53.000000 spotPython-0.6.1/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   770688 2023-06-07 11:10:20.000000 spotPython-0.6.1/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_01.png
--rw-r--r--   0 bartz      (501) staff       (20)   305679 2023-06-07 11:11:28.000000 spotPython-0.6.1/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_02.png
--rw-r--r--   0 bartz      (501) staff       (20)    34252 2023-06-24 19:48:27.000000 spotPython-0.6.1/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    44029 2023-06-24 19:48:27.000000 spotPython-0.6.1/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
--rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
--rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   121376 2023-05-28 06:32:18.000000 spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png
--rw-r--r--   0 bartz      (501) staff       (20)   116976 2023-06-07 05:09:22.000000 spotPython-0.6.1/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_contour_0_3.png
--rw-r--r--   0 bartz      (501) staff       (20)    28703 2023-06-06 21:13:57.000000 spotPython-0.6.1/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_importance.png
--rw-r--r--   0 bartz      (501) staff       (20)   161701 2023-06-07 06:30:18.000000 spotPython-0.6.1/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_parallel.png
--rw-r--r--   0 bartz      (501) staff       (20)    41471 2023-06-06 21:13:56.000000 spotPython-0.6.1/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_progress.png
--rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.6.1/notebooks/figures/spotModel.graffle
--rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.6.1/notebooks/figures/spotModel.pdf
--rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.6.1/notebooks/figures/spotModel.png
--rw-r--r--   0 bartz      (501) staff       (20)   434803 2023-06-07 06:48:45.000000 spotPython-0.6.1/notebooks/figures/tensorboard_0.png
--rw-r--r--   0 bartz      (501) staff       (20)   145933 2023-06-07 06:46:35.000000 spotPython-0.6.1/notebooks/figures/tensorboard_1.png
--rw-r--r--   0 bartz      (501) staff       (20)   751199 2023-06-07 06:51:03.000000 spotPython-0.6.1/notebooks/figures/tensorboard_hdparams.png
--rw-r--r--   0 bartz      (501) staff       (20)  2025087 2023-06-07 06:53:15.000000 spotPython-0.6.1/notebooks/figures/tensorboard_parallel.png
--rw-r--r--   0 bartz      (501) staff       (20)     1545 2023-07-15 22:08:54.000000 spotPython-0.6.1/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2023-07-16 22:12:58.525319 spotPython-0.6.1/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.470081 spotPython-0.6.1/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.506354 spotPython-0.6.1/src/spotPython/
--rw-r--r--   0 bartz      (501) staff       (20)      194 2023-07-16 22:12:58.000000 spotPython-0.6.1/src/spotPython/_version.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.507130 spotPython-0.6.1/src/spotPython/budget/
--rw-r--r--   0 bartz      (501) staff       (20)     3475 2023-07-14 22:29:47.000000 spotPython-0.6.1/src/spotPython/budget/ocba.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.507874 spotPython-0.6.1/src/spotPython/build/
--rw-r--r--   0 bartz      (501) staff       (20)    55706 2023-07-15 17:45:05.000000 spotPython-0.6.1/src/spotPython/build/kriging.py
--rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.6.1/src/spotPython/build/surrogates.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.510513 spotPython-0.6.1/src/spotPython/data/
--rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-20 20:18:46.000000 spotPython-0.6.1/src/spotPython/data/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)    13563 2023-04-20 20:17:18.000000 spotPython-0.6.1/src/spotPython/data/base.py
--rw-r--r--   0 bartz      (501) staff       (20)     3907 2023-06-28 17:48:55.000000 spotPython-0.6.1/src/spotPython/data/light_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      333 2023-06-24 18:51:10.000000 spotPython-0.6.1/src/spotPython/data/light_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-30 15:26:52.000000 spotPython-0.6.1/src/spotPython/data/sklearn_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      333 2023-04-20 20:14:06.000000 spotPython-0.6.1/src/spotPython/data/sklearn_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)     9208 2023-06-06 20:04:52.000000 spotPython-0.6.1/src/spotPython/data/torch_hyper_dict.json
--rw-r--r--   0 bartz      (501) staff       (20)      329 2023-04-26 18:22:38.000000 spotPython-0.6.1/src/spotPython/data/torch_hyper_dict.py
--rw-r--r--   0 bartz      (501) staff       (20)      459 2023-05-28 07:19:43.000000 spotPython-0.6.1/src/spotPython/data/torchdata.py
--rw-r--r--   0 bartz      (501) staff       (20)     2214 2023-06-17 21:19:39.000000 spotPython-0.6.1/src/spotPython/data/vbdp.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.511835 spotPython-0.6.1/src/spotPython/design/
--rw-r--r--   0 bartz      (501) staff       (20)      375 2023-02-02 22:52:12.000000 spotPython-0.6.1/src/spotPython/design/designs.py
--rw-r--r--   0 bartz      (501) staff       (20)      341 2023-02-02 22:52:12.000000 spotPython-0.6.1/src/spotPython/design/factorial.py
--rw-r--r--   0 bartz      (501) staff       (20)     2156 2023-04-23 08:24:45.000000 spotPython-0.6.1/src/spotPython/design/spacefilling.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.512841 spotPython-0.6.1/src/spotPython/fun/
--rw-r--r--   0 bartz      (501) staff       (20)     2729 2023-07-02 15:50:20.000000 spotPython-0.6.1/src/spotPython/fun/hyperlight.py
--rw-r--r--   0 bartz      (501) staff       (20)     3914 2023-06-24 19:02:26.000000 spotPython-0.6.1/src/spotPython/fun/hypersklearn.py
--rw-r--r--   0 bartz      (501) staff       (20)     5911 2023-07-06 20:04:22.000000 spotPython-0.6.1/src/spotPython/fun/hypertorch.py
--rw-r--r--   0 bartz      (501) staff       (20)    26824 2023-07-15 21:02:46.000000 spotPython-0.6.1/src/spotPython/fun/objectivefunctions.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.513616 spotPython-0.6.1/src/spotPython/hyperparameters/
--rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-25 16:36:59.000000 spotPython-0.6.1/src/spotPython/hyperparameters/categorical.py
--rw-r--r--   0 bartz      (501) staff       (20)     4212 2023-07-08 16:34:18.000000 spotPython-0.6.1/src/spotPython/hyperparameters/optimizer.py
--rw-r--r--   0 bartz      (501) staff       (20)    33682 2023-07-15 21:11:28.000000 spotPython-0.6.1/src/spotPython/hyperparameters/values.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.515627 spotPython-0.6.1/src/spotPython/light/
--rw-r--r--   0 bartz      (501) staff       (20)     2426 2023-07-03 21:15:52.000000 spotPython-0.6.1/src/spotPython/light/crossvalidationdatamodule.py
--rw-r--r--   0 bartz      (501) staff       (20)     1433 2023-07-02 14:10:14.000000 spotPython-0.6.1/src/spotPython/light/csvdatamodule.py
--rw-r--r--   0 bartz      (501) staff       (20)     1380 2023-06-25 16:06:47.000000 spotPython-0.6.1/src/spotPython/light/csvdataset.py
--rw-r--r--   0 bartz      (501) staff       (20)     2103 2023-06-25 16:06:47.000000 spotPython-0.6.1/src/spotPython/light/litmodel.py
--rw-r--r--   0 bartz      (501) staff       (20)     1659 2023-06-25 16:06:47.000000 spotPython-0.6.1/src/spotPython/light/mnistdatamodule.py
--rw-r--r--   0 bartz      (501) staff       (20)     3979 2023-07-02 14:27:11.000000 spotPython-0.6.1/src/spotPython/light/netlightbase.py
--rw-r--r--   0 bartz      (501) staff       (20)     7195 2023-07-07 16:41:58.000000 spotPython-0.6.1/src/spotPython/light/traintest.py
--rw-r--r--   0 bartz      (501) staff       (20)      255 2023-07-02 17:23:44.000000 spotPython-0.6.1/src/spotPython/light/utils.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.516082 spotPython-0.6.1/src/spotPython/plot/
--rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-05-29 06:13:03.000000 spotPython-0.6.1/src/spotPython/plot/contour.py
--rw-r--r--   0 bartz      (501) staff       (20)     5949 2023-07-15 21:05:52.000000 spotPython-0.6.1/src/spotPython/plot/validation.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.516382 spotPython-0.6.1/src/spotPython/sklearn/
--rw-r--r--   0 bartz      (501) staff       (20)     3715 2023-06-07 16:26:19.000000 spotPython-0.6.1/src/spotPython/sklearn/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.516641 spotPython-0.6.1/src/spotPython/spot/
--rw-r--r--   0 bartz      (501) staff       (20)    39594 2023-07-15 20:52:28.000000 spotPython-0.6.1/src/spotPython/spot/spot.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.519183 spotPython-0.6.1/src/spotPython/torch/
--rw-r--r--   0 bartz      (501) staff       (20)     1018 2023-06-23 13:29:53.000000 spotPython-0.6.1/src/spotPython/torch/activation.py
--rw-r--r--   0 bartz      (501) staff       (20)      517 2023-05-31 19:01:06.000000 spotPython-0.6.1/src/spotPython/torch/dataframedataset.py
--rw-r--r--   0 bartz      (501) staff       (20)      692 2023-06-27 22:26:23.000000 spotPython-0.6.1/src/spotPython/torch/initialization.py
--rw-r--r--   0 bartz      (501) staff       (20)     4570 2023-07-15 20:49:35.000000 spotPython-0.6.1/src/spotPython/torch/mapk.py
--rw-r--r--   0 bartz      (501) staff       (20)     1012 2023-05-27 19:17:19.000000 spotPython-0.6.1/src/spotPython/torch/netcifar10.py
--rw-r--r--   0 bartz      (501) staff       (20)      425 2023-05-27 19:21:33.000000 spotPython-0.6.1/src/spotPython/torch/netcore.py
--rw-r--r--   0 bartz      (501) staff       (20)      803 2023-05-27 19:17:19.000000 spotPython-0.6.1/src/spotPython/torch/netfashionMNIST.py
--rw-r--r--   0 bartz      (501) staff       (20)     1071 2023-06-06 19:59:34.000000 spotPython-0.6.1/src/spotPython/torch/netregression.py
--rw-r--r--   0 bartz      (501) staff       (20)     1565 2023-06-01 18:55:33.000000 spotPython-0.6.1/src/spotPython/torch/netvbdp.py
--rw-r--r--   0 bartz      (501) staff       (20)    14987 2023-06-20 05:35:32.000000 spotPython-0.6.1/src/spotPython/torch/traintest.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.521682 spotPython-0.6.1/src/spotPython/utils/
--rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-09 20:33:54.000000 spotPython-0.6.1/src/spotPython/utils/aggregate.py
--rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.6.1/src/spotPython/utils/classes.py
--rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-13 18:33:36.000000 spotPython-0.6.1/src/spotPython/utils/compare.py
--rw-r--r--   0 bartz      (501) staff       (20)     3764 2023-07-15 20:51:00.000000 spotPython-0.6.1/src/spotPython/utils/convert.py
--rw-r--r--   0 bartz      (501) staff       (20)      628 2023-07-15 21:01:58.000000 spotPython-0.6.1/src/spotPython/utils/device.py
--rw-r--r--   0 bartz      (501) staff       (20)     9289 2023-07-15 20:33:18.000000 spotPython-0.6.1/src/spotPython/utils/eda.py
--rw-r--r--   0 bartz      (501) staff       (20)     3299 2023-07-15 20:40:43.000000 spotPython-0.6.1/src/spotPython/utils/file.py
--rw-r--r--   0 bartz      (501) staff       (20)     5846 2023-07-15 20:53:33.000000 spotPython-0.6.1/src/spotPython/utils/init.py
--rw-r--r--   0 bartz      (501) staff       (20)     5028 2023-05-30 21:09:07.000000 spotPython-0.6.1/src/spotPython/utils/metrics.py
--rw-r--r--   0 bartz      (501) staff       (20)      912 2023-06-01 22:37:01.000000 spotPython-0.6.1/src/spotPython/utils/progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-13 18:43:38.000000 spotPython-0.6.1/src/spotPython/utils/repair.py
--rw-r--r--   0 bartz      (501) staff       (20)     6826 2023-07-15 20:54:18.000000 spotPython-0.6.1/src/spotPython/utils/transform.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.507018 spotPython-0.6.1/src/spotPython.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     7578 2023-07-16 22:12:58.000000 spotPython-0.6.1/src/spotPython.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     8144 2023-07-16 22:12:58.000000 spotPython-0.6.1/src/spotPython.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2023-07-16 22:12:58.000000 spotPython-0.6.1/src/spotPython.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)      196 2023-07-16 22:12:58.000000 spotPython-0.6.1/src/spotPython.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)       11 2023-07-16 22:12:58.000000 spotPython-0.6.1/src/spotPython.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-16 22:12:58.524842 spotPython-0.6.1/test/
--rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_aggregate_mean_var.py
--rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-09 19:57:56.000000 spotPython-0.6.1/test/test_build_Psi.py
--rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-09 19:58:12.000000 spotPython-0.6.1/test/test_build_U.py
--rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_build_psi_vec.py
--rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_evaluate_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_evaluate_new_solutions.py
--rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-09 19:58:51.000000 spotPython-0.6.1/test/test_extract_from_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_generate_design.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_infill.py
--rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_nat_to_cod.py
--rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_nat_to_cod_init.py
--rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_ocba.py
--rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_repair_non_numeric.py
--rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_set_de_bounds.py
--rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_show_progress.py
--rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_suggest_new_X.py
--rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.6.1/test/test_update_surrogate.py
--rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 10:19:58.000000 spotPython-0.6.1/tox.ini
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.153115 spotPython-0.6.3/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.124396 spotPython-0.6.3/.github/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.127966 spotPython-0.6.3/.github/workflows/
+-rw-r--r--   0 bartz      (501) staff       (20)      557 2023-02-02 20:30:23.000000 spotPython-0.6.3/.github/workflows/test.yml
+-rw-r--r--   0 bartz      (501) staff       (20)    17867 2023-07-04 14:15:14.000000 spotPython-0.6.3/.gitignore
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2023-05-18 22:04:43.000000 spotPython-0.6.3/.nojekyll
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.133333 spotPython-0.6.3/Figures.d/
+-rw-r--r--   0 bartz      (501) staff       (20)    21113 2023-04-26 21:03:04.000000 spotPython-0.6.3/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     5878 2023-04-26 21:03:04.000000 spotPython-0.6.3/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6563 2023-04-26 21:03:04.000000 spotPython-0.6.3/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    26562 2023-04-26 22:09:11.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8850 2023-04-26 22:09:11.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6569 2023-04-26 22:09:11.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20478 2023-04-28 06:03:36.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    20590 2023-04-28 06:03:36.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23054 2023-04-28 06:03:36.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22138 2023-04-28 06:03:36.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21534 2023-04-28 06:03:36.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22805 2023-04-28 06:03:36.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22098 2023-04-28 06:03:36.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23275 2023-04-28 06:03:36.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21965 2023-04-28 06:03:36.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22913 2023-04-28 06:03:36.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9680 2023-04-28 06:03:36.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     6536 2023-04-28 06:03:36.000000 spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21132 2023-05-08 04:46:15.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21651 2023-05-08 04:46:16.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22154 2023-05-08 04:46:18.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    21347 2023-05-08 04:46:19.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22265 2023-05-08 04:46:20.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22056 2023-05-08 04:46:21.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22224 2023-05-08 04:46:22.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23950 2023-05-08 04:46:23.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23161 2023-05-08 04:46:24.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22297 2023-05-08 04:46:25.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     9681 2023-05-08 04:37:14.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8189 2023-05-08 04:37:14.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    22759 2023-05-07 21:33:09.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24775 2023-05-07 21:33:09.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    23126 2023-05-07 21:33:10.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     8905 2023-05-07 21:23:58.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)     7635 2023-05-07 21:23:58.000000 spotPython-0.6.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    24695 2023-05-06 06:36:55.000000 spotPython-0.6.3/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    34523 2023-02-01 14:33:52.000000 spotPython-0.6.3/LICENSE.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       71 2023-04-20 20:35:14.000000 spotPython-0.6.3/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     7578 2023-07-17 22:32:25.152947 spotPython-0.6.3/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     6808 2023-06-08 16:18:46.000000 spotPython-0.6.3/README.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.134139 spotPython-0.6.3/docs/
+-rw-r--r--   0 bartz      (501) staff       (20)    46499 2022-10-31 16:48:05.000000 spotPython-0.6.3/docs/about.md
+-rw-r--r--   0 bartz      (501) staff       (20)       49 2023-07-12 23:09:54.000000 spotPython-0.6.3/docs/download.md
+-rw-r--r--   0 bartz      (501) staff       (20)      802 2023-07-16 08:32:11.000000 spotPython-0.6.3/docs/examples.md
+-rw-r--r--   0 bartz      (501) staff       (20)      947 2022-10-31 16:48:05.000000 spotPython-0.6.3/docs/gen_ref_pages.py
+-rw-r--r--   0 bartz      (501) staff       (20)      350 2023-07-14 22:03:54.000000 spotPython-0.6.3/docs/hyperparameter-tuning-cookbook.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.134448 spotPython-0.6.3/docs/images/
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2022-10-31 16:48:05.000000 spotPython-0.6.3/docs/images/favicon.png
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2022-10-31 16:48:05.000000 spotPython-0.6.3/docs/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)      392 2023-07-15 18:25:23.000000 spotPython-0.6.3/docs/index.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.134681 spotPython-0.6.3/img/
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2023-07-13 05:52:18.000000 spotPython-0.6.3/img/favicon.png
+-rw-r--r--   0 bartz      (501) staff       (20)    67674 2023-05-27 21:03:27.000000 spotPython-0.6.3/img/spotLogo.png
+-rwxr-xr-x   0 bartz      (501) staff       (20)      146 2023-07-15 09:35:47.000000 spotPython-0.6.3/makeSpot.sh
+-rw-r--r--   0 bartz      (501) staff       (20)     1487 2023-07-15 23:01:11.000000 spotPython-0.6.3/mkdocs.yml
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.135574 spotPython-0.6.3/notebooks/
+-rw-r--r--   0 bartz      (501) staff       (20)    64826 2023-07-15 20:49:26.000000 spotPython-0.6.3/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb
+-rw-r--r--   0 bartz      (501) staff       (20)   953519 2023-07-04 14:15:14.000000 spotPython-0.6.3/notebooks/31_spot_lightning_csv.ipynb
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.124916 spotPython-0.6.3/notebooks/data/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.135693 spotPython-0.6.3/notebooks/data/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)    77195 2023-05-14 08:03:00.000000 spotPython-0.6.3/notebooks/data/torch/model_spot_trained.pt
+-rw-r--r--   0 bartz      (501) staff       (20)      359 2023-03-21 18:40:04.000000 spotPython-0.6.3/notebooks/data.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.141799 spotPython-0.6.3/notebooks/figures/
+-rw-r--r--   0 bartz      (501) staff       (20)   114797 2023-06-07 17:28:19.000000 spotPython-0.6.3/notebooks/figures/12-torch_p040025_1min_5init_2023-06-07_19-09-30_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)   117891 2023-06-08 12:22:25.000000 spotPython-0.6.3/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    35435 2023-06-08 12:22:25.000000 spotPython-0.6.3/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    41877 2023-06-08 12:22:25.000000 spotPython-0.6.3/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   117933 2023-06-07 11:49:47.000000 spotPython-0.6.3/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    29392 2023-06-07 11:04:53.000000 spotPython-0.6.3/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   770688 2023-06-07 11:10:20.000000 spotPython-0.6.3/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_01.png
+-rw-r--r--   0 bartz      (501) staff       (20)   305679 2023-06-07 11:11:28.000000 spotPython-0.6.3/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_02.png
+-rw-r--r--   0 bartz      (501) staff       (20)    34252 2023-06-24 19:48:27.000000 spotPython-0.6.3/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    44029 2023-06-24 19:48:27.000000 spotPython-0.6.3/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)    88272 2023-05-26 10:05:04.000000 spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84164 2023-05-26 10:04:55.000000 spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    93300 2023-05-26 10:04:39.000000 spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    84900 2023-05-26 10:04:25.000000 spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    94821 2023-05-26 10:04:11.000000 spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    92856 2023-05-26 10:03:52.000000 spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png
+-rw-r--r--   0 bartz      (501) staff       (20)    21443 2023-05-26 10:02:53.000000 spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)    26414 2023-05-26 10:02:27.000000 spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   121376 2023-05-28 06:32:18.000000 spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png
+-rw-r--r--   0 bartz      (501) staff       (20)   116976 2023-06-07 05:09:22.000000 spotPython-0.6.3/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_contour_0_3.png
+-rw-r--r--   0 bartz      (501) staff       (20)    28703 2023-06-06 21:13:57.000000 spotPython-0.6.3/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_importance.png
+-rw-r--r--   0 bartz      (501) staff       (20)   161701 2023-06-07 06:30:18.000000 spotPython-0.6.3/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_parallel.png
+-rw-r--r--   0 bartz      (501) staff       (20)    41471 2023-06-06 21:13:56.000000 spotPython-0.6.3/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)   115822 2023-02-01 14:33:52.000000 spotPython-0.6.3/notebooks/figures/spotModel.graffle
+-rw-r--r--   0 bartz      (501) staff       (20)    26289 2023-02-01 14:33:52.000000 spotPython-0.6.3/notebooks/figures/spotModel.pdf
+-rw-r--r--   0 bartz      (501) staff       (20)    64603 2023-02-01 14:33:52.000000 spotPython-0.6.3/notebooks/figures/spotModel.png
+-rw-r--r--   0 bartz      (501) staff       (20)   434803 2023-06-07 06:48:45.000000 spotPython-0.6.3/notebooks/figures/tensorboard_0.png
+-rw-r--r--   0 bartz      (501) staff       (20)   145933 2023-06-07 06:46:35.000000 spotPython-0.6.3/notebooks/figures/tensorboard_1.png
+-rw-r--r--   0 bartz      (501) staff       (20)   751199 2023-06-07 06:51:03.000000 spotPython-0.6.3/notebooks/figures/tensorboard_hdparams.png
+-rw-r--r--   0 bartz      (501) staff       (20)  2025087 2023-06-07 06:53:15.000000 spotPython-0.6.3/notebooks/figures/tensorboard_parallel.png
+-rw-r--r--   0 bartz      (501) staff       (20)     1545 2023-07-17 19:42:28.000000 spotPython-0.6.3/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2023-07-17 22:32:25.153159 spotPython-0.6.3/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.125189 spotPython-0.6.3/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.142902 spotPython-0.6.3/src/spotPython/
+-rw-r--r--   0 bartz      (501) staff       (20)      214 2023-07-17 22:32:25.000000 spotPython-0.6.3/src/spotPython/_version.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.143634 spotPython-0.6.3/src/spotPython/budget/
+-rw-r--r--   0 bartz      (501) staff       (20)     3475 2023-07-14 22:29:47.000000 spotPython-0.6.3/src/spotPython/budget/ocba.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.143881 spotPython-0.6.3/src/spotPython/build/
+-rw-r--r--   0 bartz      (501) staff       (20)    55706 2023-07-15 17:45:05.000000 spotPython-0.6.3/src/spotPython/build/kriging.py
+-rw-r--r--   0 bartz      (501) staff       (20)      342 2023-02-02 22:52:12.000000 spotPython-0.6.3/src/spotPython/build/surrogates.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.145074 spotPython-0.6.3/src/spotPython/data/
+-rw-r--r--   0 bartz      (501) staff       (20)      317 2023-04-20 20:18:46.000000 spotPython-0.6.3/src/spotPython/data/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)    23267 2023-07-17 19:56:10.000000 spotPython-0.6.3/src/spotPython/data/base.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3907 2023-06-28 17:48:55.000000 spotPython-0.6.3/src/spotPython/data/light_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)     1036 2023-07-17 20:01:02.000000 spotPython-0.6.3/src/spotPython/data/light_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)    20975 2023-05-30 15:26:52.000000 spotPython-0.6.3/src/spotPython/data/sklearn_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)     1282 2023-07-17 20:05:39.000000 spotPython-0.6.3/src/spotPython/data/sklearn_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)     9208 2023-06-06 20:04:52.000000 spotPython-0.6.3/src/spotPython/data/torch_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)     1262 2023-07-17 20:07:25.000000 spotPython-0.6.3/src/spotPython/data/torch_hyper_dict.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1471 2023-07-17 20:09:39.000000 spotPython-0.6.3/src/spotPython/data/torchdata.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2912 2023-07-17 20:14:22.000000 spotPython-0.6.3/src/spotPython/data/vbdp.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.145411 spotPython-0.6.3/src/spotPython/design/
+-rw-r--r--   0 bartz      (501) staff       (20)     1223 2023-07-17 22:31:41.000000 spotPython-0.6.3/src/spotPython/design/designs.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1234 2023-07-17 20:32:50.000000 spotPython-0.6.3/src/spotPython/design/factorial.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2213 2023-07-17 22:32:14.000000 spotPython-0.6.3/src/spotPython/design/spacefilling.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.145920 spotPython-0.6.3/src/spotPython/fun/
+-rw-r--r--   0 bartz      (501) staff       (20)     4541 2023-07-17 20:41:35.000000 spotPython-0.6.3/src/spotPython/fun/hyperlight.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6325 2023-07-17 20:50:55.000000 spotPython-0.6.3/src/spotPython/fun/hypersklearn.py
+-rw-r--r--   0 bartz      (501) staff       (20)     7435 2023-07-17 20:59:08.000000 spotPython-0.6.3/src/spotPython/fun/hypertorch.py
+-rw-r--r--   0 bartz      (501) staff       (20)    26824 2023-07-15 21:02:46.000000 spotPython-0.6.3/src/spotPython/fun/objectivefunctions.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.146287 spotPython-0.6.3/src/spotPython/hyperparameters/
+-rw-r--r--   0 bartz      (501) staff       (20)     4851 2023-03-25 16:36:59.000000 spotPython-0.6.3/src/spotPython/hyperparameters/categorical.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5113 2023-07-17 21:02:24.000000 spotPython-0.6.3/src/spotPython/hyperparameters/optimizer.py
+-rw-r--r--   0 bartz      (501) staff       (20)    34602 2023-07-17 21:26:45.000000 spotPython-0.6.3/src/spotPython/hyperparameters/values.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.147408 spotPython-0.6.3/src/spotPython/light/
+-rw-r--r--   0 bartz      (501) staff       (20)     4898 2023-07-17 21:33:45.000000 spotPython-0.6.3/src/spotPython/light/crossvalidationdatamodule.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4128 2023-07-17 21:38:58.000000 spotPython-0.6.3/src/spotPython/light/csvdatamodule.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3313 2023-07-17 21:43:36.000000 spotPython-0.6.3/src/spotPython/light/csvdataset.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5546 2023-07-17 21:54:43.000000 spotPython-0.6.3/src/spotPython/light/litmodel.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1659 2023-06-25 16:06:47.000000 spotPython-0.6.3/src/spotPython/light/mnistdatamodule.py
+-rw-r--r--   0 bartz      (501) staff       (20)    12050 2023-07-17 22:12:28.000000 spotPython-0.6.3/src/spotPython/light/netlightbase.py
+-rw-r--r--   0 bartz      (501) staff       (20)    11131 2023-07-17 22:21:29.000000 spotPython-0.6.3/src/spotPython/light/traintest.py
+-rw-r--r--   0 bartz      (501) staff       (20)      255 2023-07-02 17:23:44.000000 spotPython-0.6.3/src/spotPython/light/utils.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.147771 spotPython-0.6.3/src/spotPython/plot/
+-rw-r--r--   0 bartz      (501) staff       (20)     1707 2023-05-29 06:13:03.000000 spotPython-0.6.3/src/spotPython/plot/contour.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5949 2023-07-15 21:05:52.000000 spotPython-0.6.3/src/spotPython/plot/validation.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.147922 spotPython-0.6.3/src/spotPython/sklearn/
+-rw-r--r--   0 bartz      (501) staff       (20)     3715 2023-06-07 16:26:19.000000 spotPython-0.6.3/src/spotPython/sklearn/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.148059 spotPython-0.6.3/src/spotPython/spot/
+-rw-r--r--   0 bartz      (501) staff       (20)    39594 2023-07-15 20:52:28.000000 spotPython-0.6.3/src/spotPython/spot/spot.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.149275 spotPython-0.6.3/src/spotPython/torch/
+-rw-r--r--   0 bartz      (501) staff       (20)     1018 2023-06-23 13:29:53.000000 spotPython-0.6.3/src/spotPython/torch/activation.py
+-rw-r--r--   0 bartz      (501) staff       (20)      517 2023-05-31 19:01:06.000000 spotPython-0.6.3/src/spotPython/torch/dataframedataset.py
+-rw-r--r--   0 bartz      (501) staff       (20)      692 2023-06-27 22:26:23.000000 spotPython-0.6.3/src/spotPython/torch/initialization.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4570 2023-07-15 20:49:35.000000 spotPython-0.6.3/src/spotPython/torch/mapk.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1012 2023-05-27 19:17:19.000000 spotPython-0.6.3/src/spotPython/torch/netcifar10.py
+-rw-r--r--   0 bartz      (501) staff       (20)      425 2023-05-27 19:21:33.000000 spotPython-0.6.3/src/spotPython/torch/netcore.py
+-rw-r--r--   0 bartz      (501) staff       (20)      803 2023-05-27 19:17:19.000000 spotPython-0.6.3/src/spotPython/torch/netfashionMNIST.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1071 2023-06-06 19:59:34.000000 spotPython-0.6.3/src/spotPython/torch/netregression.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1565 2023-06-01 18:55:33.000000 spotPython-0.6.3/src/spotPython/torch/netvbdp.py
+-rw-r--r--   0 bartz      (501) staff       (20)    14987 2023-06-20 05:35:32.000000 spotPython-0.6.3/src/spotPython/torch/traintest.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.150689 spotPython-0.6.3/src/spotPython/utils/
+-rw-r--r--   0 bartz      (501) staff       (20)     2003 2023-04-09 20:33:54.000000 spotPython-0.6.3/src/spotPython/utils/aggregate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      498 2023-05-12 15:45:09.000000 spotPython-0.6.3/src/spotPython/utils/classes.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1162 2023-04-13 18:33:36.000000 spotPython-0.6.3/src/spotPython/utils/compare.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3764 2023-07-15 20:51:00.000000 spotPython-0.6.3/src/spotPython/utils/convert.py
+-rw-r--r--   0 bartz      (501) staff       (20)      628 2023-07-15 21:01:58.000000 spotPython-0.6.3/src/spotPython/utils/device.py
+-rw-r--r--   0 bartz      (501) staff       (20)     9289 2023-07-15 20:33:18.000000 spotPython-0.6.3/src/spotPython/utils/eda.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3299 2023-07-15 20:40:43.000000 spotPython-0.6.3/src/spotPython/utils/file.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5846 2023-07-15 20:53:33.000000 spotPython-0.6.3/src/spotPython/utils/init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5028 2023-05-30 21:09:07.000000 spotPython-0.6.3/src/spotPython/utils/metrics.py
+-rw-r--r--   0 bartz      (501) staff       (20)      912 2023-06-01 22:37:01.000000 spotPython-0.6.3/src/spotPython/utils/progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1379 2023-04-13 18:43:38.000000 spotPython-0.6.3/src/spotPython/utils/repair.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6826 2023-07-15 20:54:18.000000 spotPython-0.6.3/src/spotPython/utils/transform.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.143508 spotPython-0.6.3/src/spotPython.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     7578 2023-07-17 22:32:25.000000 spotPython-0.6.3/src/spotPython.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     8144 2023-07-17 22:32:25.000000 spotPython-0.6.3/src/spotPython.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2023-07-17 22:32:25.000000 spotPython-0.6.3/src/spotPython.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)      196 2023-07-17 22:32:25.000000 spotPython-0.6.3/src/spotPython.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       11 2023-07-17 22:32:25.000000 spotPython-0.6.3/src/spotPython.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-07-17 22:32:25.152735 spotPython-0.6.3/test/
+-rw-r--r--   0 bartz      (501) staff       (20)      873 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_aggregate_mean_var.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4546 2023-04-09 19:57:56.000000 spotPython-0.6.3/test/test_build_Psi.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4511 2023-04-09 19:58:12.000000 spotPython-0.6.3/test/test_build_U.py
+-rw-r--r--   0 bartz      (501) staff       (20)      797 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_build_psi_vec.py
+-rw-r--r--   0 bartz      (501) staff       (20)      917 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_evaluate_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1319 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_evaluate_new_solutions.py
+-rw-r--r--   0 bartz      (501) staff       (20)    10337 2023-04-09 19:58:51.000000 spotPython-0.6.3/test/test_extract_from_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2263 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_generate_design.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_infill.py
+-rw-r--r--   0 bartz      (501) staff       (20)      643 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_nat_to_cod.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1330 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_nat_to_cod_init.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1603 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_ocba.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1208 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_repair_non_numeric.py
+-rw-r--r--   0 bartz      (501) staff       (20)     4887 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_set_de_bounds.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2223 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_show_progress.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1131 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_suggest_new_X.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1765 2023-02-01 14:33:52.000000 spotPython-0.6.3/test/test_update_surrogate.py
+-rw-r--r--   0 bartz      (501) staff       (20)      130 2023-05-19 10:19:58.000000 spotPython-0.6.3/tox.ini
```

### Comparing `spotPython-0.6.1/.github/workflows/test.yml` & `spotPython-0.6.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/.gitignore` & `spotPython-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf` & `spotPython-0.6.3/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf` & `spotPython-0.6.3/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf` & `spotPython-0.6.3/Figures.d/11-torch_p040025_1min_3init_2023-04-26_22-37-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_1min_3init_2023-04-26_22-57-45_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf` & `spotPython-0.6.3/Figures.d/11-torch_s7cfd16_360min_10init_2023-04-27_07-25-12_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_1.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_0_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_1_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_2_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_contour_3_4.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_360min_20init_2023-05-07_23-36-22_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_2.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_1_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_importance.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf` & `spotPython-0.6.3/Figures.d/12-torch_p040025_60min_20init_2023-05-07_21-33-26_progress.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf` & `spotPython-0.6.3/Figures.d/13-torch_s7cfd16_600min_20init_2023-05-05_18-52-19_contour_2_3.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/LICENSE.txt` & `spotPython-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/PKG-INFO` & `spotPython-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.6.1
+Version: 0.6.3
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.6.1/README.md` & `spotPython-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/docs/about.md` & `spotPython-0.6.3/docs/about.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/docs/examples.md` & `spotPython-0.6.3/docs/examples.md`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/docs/gen_ref_pages.py` & `spotPython-0.6.3/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/docs/images/favicon.png` & `spotPython-0.6.3/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/docs/images/spotlogo.png` & `spotPython-0.6.3/docs/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/img/favicon.png` & `spotPython-0.6.3/img/favicon.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/img/spotLogo.png` & `spotPython-0.6.3/img/spotLogo.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/mkdocs.yml` & `spotPython-0.6.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb` & `spotPython-0.6.3/notebooks/14_spot_ray_hpt_torch_cifar10.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/31_spot_lightning_csv.ipynb` & `spotPython-0.6.3/notebooks/31_spot_lightning_csv.ipynb`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/data/torch/model_spot_trained.pt` & `spotPython-0.6.3/notebooks/data/torch/model_spot_trained.pt`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/12-torch_p040025_1min_5init_2023-06-07_19-09-30_contour_0_1.png` & `spotPython-0.6.3/notebooks/figures/12-torch_p040025_1min_5init_2023-06-07_19-09-30_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_contour_0_1.png` & `spotPython-0.6.3/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_importance.png` & `spotPython-0.6.3/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_progress.png` & `spotPython-0.6.3/notebooks/figures/14-torch_maans05_60min_20init_2023-06-08_10-52-59_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_contour_0_1.png` & `spotPython-0.6.3/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_progress.png` & `spotPython-0.6.3/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_01.png` & `spotPython-0.6.3/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_01.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_02.png` & `spotPython-0.6.3/notebooks/figures/14-torch_p040025_10min_5init_2023-06-07_12-41-06_tensorboard_02.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_importance.png` & `spotPython-0.6.3/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_progress.png` & `spotPython-0.6.3/notebooks/figures/29-torch_bartz09_1min_5init_2023-06-24_21-45-17_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png` & `spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png` & `spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png` & `spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_0_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png` & `spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png` & `spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_1_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png` & `spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_contour_3_4.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png` & `spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png` & `spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_10init_2023-05-19_16-34-33_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png` & `spotPython-0.6.3/notebooks/figures/figures14-torch_maans03_60min_20init_2023-05-27_23-10-01_parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_contour_0_3.png` & `spotPython-0.6.3/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_contour_0_3.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_importance.png` & `spotPython-0.6.3/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_importance.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_parallel.png` & `spotPython-0.6.3/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_progress.png` & `spotPython-0.6.3/notebooks/figures/figures24-torch_bartz09_10min_20init_2023-06-06_22-50-23_progress.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/spotModel.graffle` & `spotPython-0.6.3/notebooks/figures/spotModel.graffle`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/spotModel.pdf` & `spotPython-0.6.3/notebooks/figures/spotModel.pdf`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/spotModel.png` & `spotPython-0.6.3/notebooks/figures/spotModel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/tensorboard_0.png` & `spotPython-0.6.3/notebooks/figures/tensorboard_0.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/tensorboard_1.png` & `spotPython-0.6.3/notebooks/figures/tensorboard_1.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/tensorboard_hdparams.png` & `spotPython-0.6.3/notebooks/figures/tensorboard_hdparams.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/notebooks/figures/tensorboard_parallel.png` & `spotPython-0.6.3/notebooks/figures/tensorboard_parallel.png`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/pyproject.toml` & `spotPython-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools>=61.0",
   "setuptools_scm[toml]"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotPython"
-version = "0.6.1"
+version = "0.6.3"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotPython - Sequential Parameter Optimization in Python"
 readme = "README.md"
 license = { text="AGPL-3.0-or-later" }
 requires-python = ">=3.10"
```

### Comparing `spotPython-0.6.1/src/spotPython/budget/ocba.py` & `spotPython-0.6.3/src/spotPython/budget/ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/build/kriging.py` & `spotPython-0.6.3/src/spotPython/build/kriging.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/data/light_hyper_dict.json` & `spotPython-0.6.3/src/spotPython/data/light_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/data/sklearn_hyper_dict.json` & `spotPython-0.6.3/src/spotPython/data/sklearn_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/data/torch_hyper_dict.json` & `spotPython-0.6.3/src/spotPython/data/torch_hyper_dict.json`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/data/vbdp.py` & `spotPython-0.6.3/src/spotPython/data/vbdp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,80 @@
 # Purpose: Functions for the VBDP project
 
 
-def cluster_features(X):
-    """Clusters the features of a dataframe based on similarity
+import pandas as pd
+from sklearn.cluster import AffinityPropagation
+from sklearn.metrics.pairwise import manhattan_distances
+
+
+def cluster_features(X: pd.DataFrame) -> pd.DataFrame:
+    """Clusters the features of a dataframe based on similarity.
+
+    This function takes a dataframe with features and clusters them based on similarity.
+    The resulting dataframe contains the original features as well as new features representing the clusters.
 
     Args:
-        X (pd.DataFrame): dataframe with features
+        X (pd.DataFrame): A dataframe with features.
+
     Returns:
-        X (pd.DataFrame): dataframe with new features
+        (pd.DataFrame): A dataframe with the original features and new cluster features.
+
     Examples:
         >>> df = pd.DataFrame({"a": [True, False, True], "b": [True, True, False], "c": [False, False, True]})
         >>> df
             a      b      c
         0  True   True  False
         1 False   True  False
         2  True  False   True
         >>> cluster_features(df)
-            a      b      c  cluster
-        0  True   True  False       0
-        1 False   True  False       1
-        2  True  False   True        2
+            a      b      c  c_0  c_1  c_2  c_3
+        0  True   True  False    0    0    0    0
+        1 False   True  False    0    0    0    0
+        2  True  False   True    0    0    0    0
     """
     c_0 = X.columns[X.columns.str.contains("pain")]
     c_1 = X.columns[X.columns.str.contains("inflammation")]
     c_2 = X.columns[X.columns.str.contains("bleed")]
     c_3 = X.columns[X.columns.str.contains("skin")]
     X["c_0"] = X[c_0].sum(axis=1)
     X["c_1"] = X[c_1].sum(axis=1)
     X["c_2"] = X[c_2].sum(axis=1)
     X["c_3"] = X[c_3].sum(axis=1)
     return X
 
 
-def affinity_propagation_features(X):
-    """Clusters the features of a dataframe using Affinity Propagation
+def affinity_propagation_features(X: pd.DataFrame) -> pd.DataFrame:
+    """Clusters the features of a dataframe using Affinity Propagation.
+
+    This function takes a dataframe with features and clusters them using the
+    Affinity Propagation algorithm. The resulting dataframe contains the original
+    features as well as a new feature representing the cluster labels.
 
     Args:
-        X (pd.DataFrame): dataframe with features
+        X (pd.DataFrame):
+            A dataframe with features.
+
     Returns:
-        X (pd.DataFrame): dataframe with new features
+        (pd.DataFrame):
+            A dataframe with the original features and a new cluster feature.
+
     Examples:
         >>> df = pd.DataFrame({"a": [True, False, True], "b": [True, True, False], "c": [False, False, True]})
         >>> df
             a      b      c
         0  True   True   False
         1  False  True   False
         2  True   False  True
         >>> affinity_propagation_features(df)
+        Estimated number of clusters: 3
             a      b      c  cluster
         0  True   True   False       0
         1  False  True   False       1
         2  True   False  True        2
     """
-    from sklearn.cluster import AffinityPropagation
-    from sklearn.metrics.pairwise import manhattan_distances
-
     D = manhattan_distances(X)
     af = AffinityPropagation(random_state=0, affinity="precomputed").fit(D)
     cluster_centers_indices = af.cluster_centers_indices_
     n_clusters_ = len(cluster_centers_indices)
     print("Estimated number of clusters: %d" % n_clusters_)
     X["cluster"] = af.labels_
     return X
```

### Comparing `spotPython-0.6.1/src/spotPython/design/spacefilling.py` & `spotPython-0.6.3/src/spotPython/design/spacefilling.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from spotPython.utils.transform import scale
 from typing import Optional, Union
 
 from .designs import designs
 
 
 class spacefilling(designs):
-    def __init__(self, k=2, seed=123):
+    def __init__(self, k: int = 2, seed: int = 123) -> None:
         """
         Spacefilling design class
 
         Args:
             k (int, optional): number of design variables (dimensions). Defaults to 2.
             seed (int, optional): random seed. Defaults to 123.
         """
@@ -29,34 +29,35 @@
     ) -> ndarray:
         """
         Latin hypercube sampling based on scipy.
 
         Args:
             n (int): number of samples
             repeats (int): number of repeats (replicates)
-            lower (int, optional): lower bound. Defaults to 0.
-            upper (int, optional): upper bound. Defaults to 1.
+            lower (int or float, optional): lower bound. Defaults to 0.
+            upper (int or float, optional): upper bound. Defaults to 1.
 
         Returns:
-            (numpy.ndarray): Latin hypercube design.
-        Examples:
+            (ndarray): Latin hypercube design.
+
+        Example:
             >>> from spotPython.design.spacefilling import spacefilling
-                import numpy as np
-                lhd = spacefilling(k=2, seed=123)
-                lhd.scipy_lhd(n=5, repeats=2, lower=np.array([0,0]), upper=np.array([1,1]))
-                array([[0.66352963, 0.5892358 ],
-                [0.66352963, 0.5892358 ],
-                [0.55592803, 0.96312564],
-                [0.55592803, 0.96312564],
-                [0.16481882, 0.0375811 ],
-                [0.16481882, 0.0375811 ],
-                [0.215331  , 0.34468512],
-                [0.215331  , 0.34468512],
-                [0.83604909, 0.62202146],
-                [0.83604909, 0.62202146]])
+            >>> import numpy as np
+            >>> lhd = spacefilling(k=2, seed=123)
+            >>> lhd.scipy_lhd(n=5, repeats=2, lower=np.array([0,0]), upper=np.array([1,1]))
+            array([[0.66352963, 0.5892358 ],
+                   [0.66352963, 0.5892358 ],
+                   [0.55592803, 0.96312564],
+                   [0.55592803, 0.96312564],
+                   [0.16481882, 0.0375811 ],
+                   [0.16481882, 0.0375811 ],
+                   [0.215331  , 0.34468512],
+                   [0.215331  , 0.34468512],
+                   [0.83604909, 0.62202146],
+                   [0.83604909, 0.62202146]])
         """
         if lower is None:
             lower = zeros(self.k)
         if upper is None:
             upper = ones(self.k)
         sample = self.sampler.random(n=n)
         des = scale(sample, lower, upper)
```

### Comparing `spotPython-0.6.1/src/spotPython/fun/hypersklearn.py` & `spotPython-0.6.3/src/spotPython/fun/hyperlight.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,129 @@
-from numpy.random import default_rng
+import logging
 import numpy as np
+from numpy.random import default_rng
 from numpy import array
-from sklearn.pipeline import make_pipeline
-
-from spotPython.hyperparameters.values import assign_values
+from spotPython.light.traintest import train_model
 from spotPython.hyperparameters.values import (
+    assign_values,
     generate_one_config_from_var_dict,
 )
 
-from spotPython.sklearn.traintest import evaluate_cv, evaluate_model_oob, evaluate_hold_out
-
-# from spotPython.utils.eda import generate_config_id
-
-import logging
-from sklearn.metrics import mean_absolute_error
-
 logger = logging.getLogger(__name__)
-# configure the handler and formatter as needed
 py_handler = logging.FileHandler(f"{__name__}.log", mode="w")
 py_formatter = logging.Formatter("%(name)s %(asctime)s %(levelname)s %(message)s")
-# add formatter to the handler
 py_handler.setFormatter(py_formatter)
-# add handler to the logger
 logger.addHandler(py_handler)
 
 
-class HyperSklearn:
+class HyperLight:
     """
-    Hyperparameter Tuning for Sklearn.
+    Hyperparameter Tuning for Lightning 2.
 
     Args:
-        seed (int): seed.
-            See [Numpy Random Sampling](https://numpy.org/doc/stable/reference/random/index.html#random-quick-start)
+        seed (int): seed for the random number generator. See Numpy Random Sampling.
+        log_level (int): log level for the logger.
 
+    Attributes:
+        seed (int): seed for the random number generator.
+        rng (Generator): random number generator.
+        fun_control (dict): dictionary containing control parameters for the hyperparameter tuning.
+        log_level (int): log level for the logger.
+
+    Example:
+        >>> hyper_light = HyperLight(seed=126, log_level=50)
+        >>> print(hyper_light.seed)
+        126
     """
 
-    def __init__(self, seed=126, log_level=50):
+    def __init__(self, seed: int = 126, log_level: int = 50) -> None:
         self.seed = seed
         self.rng = default_rng(seed=self.seed)
         self.fun_control = {
             "seed": None,
             "data": None,
             "step": 10_000,
             "horizon": None,
             "grace_period": None,
             "metric_river": None,
-            "metric_sklearn": mean_absolute_error,
+            "metric_sklearn": None,
             "weights": array([1, 0, 0]),
             "weight_coeff": 0.0,
             "log_level": log_level,
             "var_name": [],
             "var_type": [],
-            "prep_model": None,
-            "predict_proba": False,
         }
         self.log_level = self.fun_control["log_level"]
         logger.setLevel(self.log_level)
         logger.info(f"Starting the logger at level {self.log_level} for module {__name__}:")
 
-    def check_X_shape(self, X):
+    def check_X_shape(self, X: np.ndarray) -> np.ndarray:
+        """
+        Checks the shape of the input array X and raises an exception if it is not valid.
+
+        Args:
+            X (np.ndarray):
+                input array.
+
+        Returns:
+            np.ndarray:
+                input array with valid shape.
+
+        Raises:
+            Exception:
+                if the shape of the input array is not valid.
+
+        Example:
+            >>> hyper_light = HyperLight(seed=126, log_level=50)
+            >>> X = np.array([[1, 2], [3, 4]])
+            >>> hyper_light.check_X_shape(X)
+            array([[1, 2],
+                   [3, 4]])
+        """
         try:
             X.shape[1]
         except ValueError:
             X = np.array([X])
         if X.shape[1] != len(self.fun_control["var_name"]):
-            raise Exception
-
-    def get_sklearn_df_eval_preds(self, model):
-        try:
-            df_eval, df_preds = self.evaluate_model(model, self.fun_control)
-        except Exception as err:
-            print(f"Error in get_sklearn_df_eval_preds(). Call to evaluate_model failed. {err=}, {type(err)=}")
-            print("Setting df_eval and df.preds to np.nan")
-            df_eval = np.nan
-            df_preds = np.nan
-        return df_eval, df_preds
+            raise Exception("Invalid shape of input array X.")
+        return X
 
-    def fun_sklearn(self, X, fun_control=None):
+    def fun(self, X: np.ndarray, fun_control: dict = None) -> np.ndarray:
+        """
+        Evaluates the function for the given input array X and control parameters.
+
+        Args:
+            X (np.ndarray):
+                input array.
+            fun_control (dict):
+                dictionary containing control parameters for the hyperparameter tuning.
+
+        Returns:
+            (np.ndarray):
+                array containing the evaluation results.
+
+        Example:
+            >>> hyper_light = HyperLight(seed=126, log_level=50)
+            >>> X = np.array([[1, 2], [3, 4]])
+            >>> fun_control = {"weights": np.array([1, 0, 0])}
+            >>> hyper_light.fun(X, fun_control)
+            array([nan, nan])
+        """
         z_res = np.array([], dtype=float)
-        self.fun_control.update(fun_control)
+        if fun_control is not None:
+            self.fun_control.update(fun_control)
         self.check_X_shape(X)
         var_dict = assign_values(X, self.fun_control["var_name"])
+        # type information and transformations are considered in generate_one_config_from_var_dict:
         for config in generate_one_config_from_var_dict(var_dict, self.fun_control):
+            logger.debug(f"\nconfig: {config}")
+            # extract parameters like epochs, batch_size, lr, etc. from config
             # config_id = generate_config_id(config)
-            if self.fun_control["prep_model"] is not None:
-                model = make_pipeline(self.fun_control["prep_model"], self.fun_control["core_model"](**config))
-            else:
-                model = self.fun_control["core_model"](**config)
             try:
-                eval_type = fun_control["eval"]
-                if eval_type == "eval_oob_score":
-                    df_eval, _ = evaluate_model_oob(model, self.fun_control)
-                elif eval_type == "train_cv":
-                    df_eval, _ = evaluate_cv(model, self.fun_control)
-                else:  # eval_type == "train_hold_out":
-                    df_eval, _ = evaluate_hold_out(model, self.fun_control)
+                df_eval = train_model(config, self.fun_control)
             except Exception as err:
-                print(f"Error in fun_sklearn(). Call to evaluate_model failed. {err=}, {type(err)=}")
-                print("Setting df_eval to np.nan")
+                logger.error(f"Error in fun(). Call to train_model failed. {err=}, {type(err)=}")
+                logger.error("Setting df_eval to np.nan")
                 df_eval = np.nan
-            z_res = np.append(z_res, fun_control["weights"] * df_eval)
+            z_val = self.fun_control["weights"] * df_eval
+            z_res = np.append(z_res, z_val)
         return z_res
```

### Comparing `spotPython-0.6.1/src/spotPython/fun/objectivefunctions.py` & `spotPython-0.6.3/src/spotPython/fun/objectivefunctions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/hyperparameters/categorical.py` & `spotPython-0.6.3/src/spotPython/hyperparameters/categorical.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/hyperparameters/optimizer.py` & `spotPython-0.6.3/src/spotPython/hyperparameters/optimizer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,38 @@
 import torch.optim
+from typing import Any, Union
 
 
-def optimizer_handler(optimizer_name: str, params, lr_mult=1.0, **kwargs):
+def optimizer_handler(
+    optimizer_name: str, params: Union[list, torch.Tensor], lr_mult: float = 1.0, **kwargs: Any
+) -> torch.optim.Optimizer:
+    """Returns an instance of the specified optimizer.
+
+    Args:
+        optimizer_name (str): The name of the optimizer to use.
+        params (list or torch.Tensor): The parameters to optimize.
+        lr_mult (float, optional): A multiplier for the learning rate. Defaults to 1.0.
+        **kwargs: Additional keyword arguments for the optimizer.
+
+    Returns:
+        (torch.optim.Optimizer):
+            An instance of the specified optimizer.
+
+    Examples:
+        >>> model = torch.nn.Linear(10, 1)
+        >>> optimizer = optimizer_handler("Adadelta", model.parameters(), lr_mult=0.5)
+        >>> print(optimizer)
+        Adadelta (
+            Parameter Group 0
+                eps: 1e-06
+                lr: 0.5
+                rho: 0.9
+                weight_decay: 0
+        )
+    """
     if optimizer_name == "Adadelta":
         return torch.optim.Adadelta(
             params,
             lr=lr_mult * 1.0,
             rho=0.9,
             eps=1e-06,
             weight_decay=0,
```

### Comparing `spotPython-0.6.1/src/spotPython/hyperparameters/values.py` & `spotPython-0.6.3/src/spotPython/hyperparameters/values.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,128 +1,123 @@
 import numpy as np
 import copy
 import json
 from sklearn.pipeline import make_pipeline
 from river import compose
-from typing import Union, List
+from typing import Union, List, Dict, Generator, Any
 
 from spotPython.utils.convert import class_for_name
 from spotPython.utils.transform import transform_hyper_parameter_values
 
 
-def generate_one_config_from_var_dict(var_dict, fun_control) -> dict:
+def generate_one_config_from_var_dict(
+    var_dict: Dict[str, np.ndarray], fun_control: Dict[str, Union[List[str], str]]
+) -> Generator[Dict[str, Union[int, float]], None, None]:
     """Generate one configuration from a dictionary of variables (as a generator).
-    This function takes a dictionary of variables as input arguments and returns a dictionary
-    with the values from the arrays in the dictionary.
+
+    This function takes a dictionary of variables as input arguments and returns a generator
+    that yields dictionaries with the values from the arrays in the input dictionary.
 
     Args:
-        var_dict (dict):
-            A dictionary where keys are variable names and values are numpy arrays.
-        fun_control (dict):
-            A dictionary which (at least) has an entry with the following key:
-            "var_type": A list of variable types. If the entry is not "num" the corresponding
+        var_dict (dict): A dictionary where keys are variable names and values are numpy arrays.
+        fun_control (dict): A dictionary which (at least) has an entry with the following key:
+            "var_type" (list): A list of variable types. If the entry is not "num" the corresponding
             value will be converted to the type "int".
 
     Returns:
-        (dict):
-            A dictionary with the values from the arrays in the dictionary.
+        Generator[dict]: A generator that yields dictionaries with the values from the arrays in the input dictionary.
 
     Examples:
         >>> import numpy as np
         >>> from spotPython.utils.prepare import generate_one_config_from_var_dict
         >>> var_dict = {'a': np.array([1, 3, 5]), 'b': np.array([2, 4, 6])}
         >>> fun_control = {"var_type": ["int", "num"]}
-        >>> generate_one_config_from_var_dict(var_dict, fun_control)
-        {'a': 1, 'b': 2}
+        >>> list(generate_one_config_from_var_dict(var_dict, fun_control))
+        [{'a': 1, 'b': 2}, {'a': 3, 'b': 4}, {'a': 5, 'b': 6}]
     """
     for values in iterate_dict_values(var_dict):
         values = convert_keys(values, fun_control["var_type"])
         values = get_dict_with_levels_and_types(fun_control=fun_control, v=values)
         values = transform_hyper_parameter_values(fun_control=fun_control, hyper_parameter_values=values)
         yield values
 
 
-def return_conf_list_from_var_dict(var_dict: dict, fun_control: dict) -> list:
-    """This function takes a dictionary of variables and a dictionary of function control.
-    It performs similar steps as generate_one_config_from_var_dict()
-    but returns a list of dictionaries of hyper parameter values.
-    Args:
-        var_dict (dict):
-            A dictionary of variables.
-        fun_control (dict):
-            A dictionary of function control.
+def return_conf_list_from_var_dict(
+    var_dict: Dict[str, np.ndarray], fun_control: Dict[str, Union[List[str], str]]
+) -> List[Dict[str, Union[int, float]]]:
+    """Return a list of configurations from a dictionary of variables.
+
+    This function takes a dictionary of variables and a dictionary of function control as input arguments.
+    It performs similar steps as generate_one_config_from_var_dict() but returns a list of dictionaries
+    of hyper parameter values.
+
+    Args:
+        var_dict (dict): A dictionary where keys are variable names and values are numpy arrays.
+        fun_control (dict): A dictionary which (at least) has an entry with the following key:
+            "var_type" (list): A list of variable types. If the entry is not "num" the corresponding
+            value will be converted to the type "int".
+
     Returns:
-        (list):
-            A list of dictionaries of hyper parameter values. Transformations are applied to the values.
+        list: A list of dictionaries of hyper parameter values. Transformations are applied to the values.
+
     Examples:
         >>> import numpy as np
         >>> from spotPython.utils.prepare import return_conf_list_from_var_dict
-            var_dict = {'a': np.array([1]),
-                        'b': np.array([2])}
-            fun_control = {'var_type': ['int', 'int']}
-            return_conf_list_from_var_dict(var_dict, fun_control)
-            var_dict = {'a': np.array([1, 3, 5]), 'b': np.array([2, 4, 6])}
-            fun_control = {'var_type': ['int', 'int']}
-            return_conf_list_from_var_dict(var_dict, fun_control)
-            {'a': [1, 3, 5], 'b': [2, 4, 6]}
-
+        >>> var_dict = {'a': np.array([1, 3, 5]), 'b': np.array([2, 4, 6])}
+        >>> fun_control = {'var_type': ['int', 'int']}
+        >>> return_conf_list_from_var_dict(var_dict, fun_control)
+        [{'a': 1, 'b': 2}, {'a': 3, 'b': 4}, {'a': 5, 'b': 6}]
     """
     conf_list = []
     for values in generate_one_config_from_var_dict(var_dict, fun_control):
         conf_list.append(values)
     return conf_list
 
 
-def iterate_dict_values(var_dict: dict):
-    """
-    This function takes a dictionary of variables as input arguments and returns an iterator that
-    yields the values from the arrays in the dictionary.
+def iterate_dict_values(var_dict: Dict[str, np.ndarray]) -> Generator[Dict[str, Union[int, float]], None, None]:
+    """Iterate over the values of a dictionary of variables.
 
-    Parameters:
-        var_dict (dict):
-            A dictionary where keys are variable names and values are numpy arrays.
+    This function takes a dictionary of variables as input arguments and returns a generator that
+    yields dictionaries with the values from the arrays in the input dictionary.
+
+    Args:
+        var_dict (dict): A dictionary where keys are variable names and values are numpy arrays.
 
     Returns:
-        iterator (generator):
-            An iterator that yields the values from the arrays in the dictionary.
+        Generator[dict]:
+            A generator that yields dictionaries with the values from the arrays in the input dictionary.
 
     Examples:
         >>> import numpy as np
         >>> from spotPython.utils.prepare import iterate_dict_values
         >>> var_dict = {'a': np.array([1, 3, 5]), 'b': np.array([2, 4, 6])}
-        >>> for values in iterate_dict_values(var_dict):
-        ...     print(values)
-        {'a': 1, 'b': 2}
-        {'a': 3, 'b': 4}
-        {'a': 5, 'b': 6}
+        >>> list(iterate_dict_values(var_dict))
+        [{'a': 1, 'b': 2}, {'a': 3, 'b': 4}, {'a': 5, 'b': 6}]
     """
     n = len(next(iter(var_dict.values())))
     for i in range(n):
         yield {key: value[i] for key, value in var_dict.items()}
 
 
-def convert_keys(d: dict, var_type: list):
-    """
-    Convert values in a dictionary to integers based on a list of variable types.
+def convert_keys(d: Dict[str, Union[int, float, str]], var_type: List[str]) -> Dict[str, Union[int, float]]:
+    """Convert values in a dictionary to integers based on a list of variable types.
 
     This function takes a dictionary `d` and a list of variable types `var_type` as arguments.
     For each key in the dictionary,
     if the corresponding entry in `var_type` is not equal to `"num"`,
     the value associated with that key is converted to an integer.
 
     Args:
-        d (dict):
-            The input dictionary.
+        d (dict): The input dictionary.
         var_type (list):
             A list of variable types. If the entry is not `"num"` the corresponding
             value will be converted to the type `"int"`.
 
     Returns:
-        (dict):
-            The modified dictionary with values converted to integers based on `var_type`.
+        dict: The modified dictionary with values converted to integers based on `var_type`.
 
     Examples:
         >>> from spotPython.utils.prepare import convert_keys
         >>> d = {'a': '1.1', 'b': '2', 'c': '3.1'}
         >>> var_type = ["int", "num", "int"]
         >>> convert_keys(d, var_type)
         {'a': 1, 'b': '2', 'c': 3}
@@ -130,95 +125,101 @@
     keys = list(d.keys())
     for i in range(len(keys)):
         if var_type[i] not in ["num", "float"]:
             d[keys[i]] = int(d[keys[i]])
     return d
 
 
-def get_dict_with_levels_and_types(fun_control, v) -> dict:
+def get_dict_with_levels_and_types(fun_control: Dict[str, Any], v: Dict[str, Any]) -> Dict[str, Any]:
     """Get dictionary with levels and types.
+
     The function maps the numerical output of the hyperparameter optimization to the corresponding levels
     of the hyperparameter needed by the core model, i.e., the tuned algorithm.
     The function takes the dictionaries fun_control and v and returns a new dictionary with the same keys as v
     but with the values of the levels of the keys from fun_control.
     If the key value in the dictionary is 0, it takes the first value from the list,
     if it is 1, it takes the second and so on.
     If a key is not in fun_control, it takes the key from v.
     If the core_model_parameter_type value is instance, it returns the class of the value from the module
     via getattr("class", value).
-    For example,
-    if fun_control = {"HoeffdingTreeRegressor":{
-        "leaf_prediction": {
-            "levels": ["mean", "model", "adaptive"],
-            "type": "factor",
-            "default": "mean",
-            "core_model_parameter_type": "str"},
-        "leaf_model": {
-            "levels": ["linear_model.LinearRegression", "linear_model.PARegressor", "linear_model.Perceptron"],
-            "type": "factor",
-            "default": "LinearRegression",
-            "core_model_parameter_type": "instance"},
-            "splitter": {"levels": ["EBSTSplitter", "TEBSTSplitter", "QOSplitter"],
-            "type": "factor",
-            "default": "EBSTSplitter", "core_model_parameter_type": "instance()"},
-        "binary_split": {
-            "levels": [0, 1],
-            "type": "factor",
-            "default": 0,
-            "core_model_parameter_type": "bool"},
-        "stop_mem_management": {
-            "levels": [0, 1],
-            "type": "factor",
-            "default": 0,
-            "core_model_parameter_type": "bool"}}}
-        and
-        v = {'grace_period': 200,
+
+    Args:
+        fun_control (Dict[str, Any]): A dictionary containing information about the core model hyperparameters.
+        v (Dict[str, Any]): A dictionary containing the numerical output of the hyperparameter optimization.
+
+    Returns:
+        Dict[str, Any]:
+            A new dictionary with the same keys as v but with the values of the levels of the keys from fun_control.
+
+    Examples:
+        >>> fun_control = {
+        ...     "core_model_hyper_dict": {
+        ...         "leaf_prediction": {
+        ...             "levels": ["mean", "model", "adaptive"],
+        ...             "type": "factor",
+        ...             "default": "mean",
+        ...             "core_model_parameter_type": "str"
+        ...         },
+        ...         "leaf_model": {
+        ...             "levels": [
+        ...                 "linear_model.LinearRegression",
+        ...                 "linear_model.PARegressor",
+        ...                 "linear_model.Perceptron"
+        ...             ],
+        ...             "type": "factor",
+        ...             "default": "LinearRegression",
+        ...             "core_model_parameter_type": "instance"
+        ...         },
+        ...         "splitter": {
+        ...             "levels": ["EBSTSplitter", "TEBSTSplitter", "QOSplitter"],
+        ...             "type": "factor",
+        ...             "default": "EBSTSplitter",
+        ...             "core_model_parameter_type": "instance()"
+        ...         },
+        ...         "binary_split": {
+        ...             "levels": [0, 1],
+        ...             "type": "factor",
+        ...             "default": 0,
+        ...             "core_model_parameter_type": "bool"
+        ...         },
+        ...         "stop_mem_management": {
+        ...             "levels": [0, 1],
+        ...             "type": "factor",
+        ...             "default": 0,
+        ...             "core_model_parameter_type": "bool"
+        ...         }
+        ...     }
+        ... }
+        >>> v = {
+        ...     'grace_period': 200,
+        ...     'max_depth': 10,
+        ...     'delta': 1e-07,
+        ...     'tau': 0.05,
+        ...     'leaf_prediction': 0,
+        ...     'leaf_model': 0,
+        ...     'model_selector_decay': 0.95,
+        ...     'splitter': 1,
+        ...     'min_samples_split': 9,
+        ...     'binary_split': 0,
+        ...     'max_size': 500.0
+        ... }
+        >>> get_dict_with_levels_and_types(fun_control, v)
+        {
+            'grace_period': 200,
             'max_depth': 10,
             'delta': 1e-07,
             'tau': 0.05,
-            'leaf_prediction': 0,
-            'leaf_model': 0,
+            'leaf_prediction': 'mean',
+            'leaf_model': linear_model.LinearRegression,
             'model_selector_decay': 0.95,
-            'splitter': 1,
+            'splitter': TEBSTSplitter,
             'min_samples_split': 9,
-            'binary_split': 0,
-            'max_size': 500.0}
-        then the function returns
-        {'grace_period': 200,
-        'max_depth': 10,
-        'delta': 1e-07,
-        'tau': 0.05,
-        'leaf_prediction': 'mean',
-        'leaf_model': linear_model.LinearRegression,
-        'model_selector_decay': 0.95,
-        'splitter': 'TEBSTSplitter',
-        'min_samples_split': 9,
-        'binary_split': 0,
-        'max_size': 500.0}.
-
-    Args:
-        fun_control (dict):
-            dictionary with levels and types
-        v (dict):
-            dictionary with values
-
-    Returns:
-        new_dict (dict):
-            dictionary with levels and types
-
-    Examples:
-        >>> from spotPython.utils.prepare import get_dict_with_levels_and_types
-            fun_control = {"HoeffdingTreeRegressor":{
-                "leaf_prediction": {"levels": ["mean", "model", "adaptive"],
-                                    "type": "factor",
-                                    "default": "mean",
-                                    "core_model_parameter_type": "str"}}}
-            v = {"leaf_prediction": 0}
-            get_dict_with_levels_and_types(fun_control, v)
-            {"leaf_prediction": "mean"}
+            'binary_split': False,
+            'max_size': 500.0
+        }
     """
     d = fun_control["core_model_hyper_dict"]
     new_dict = {}
     for key, value in v.items():
         if key in d and d[key]["type"] == "factor":
             if d[key]["core_model_parameter_type"] == "instance":
                 if "class_name" in d[key]:
@@ -238,15 +239,15 @@
 
 
 def assign_values(X: np.array, var_list: list) -> dict:
     """
     This function takes an np.array X and a list of variable names as input arguments
     and returns a dictionary where the keys are the variable names and the values are assigned from X.
 
-    Parameters:
+    Args:
         X (np.array):
             A 2D numpy array where each column represents a variable.
         var_list (list):
             A list of strings representing variable names.
 
     Returns:
         dict:
```

### Comparing `spotPython-0.6.1/src/spotPython/light/crossvalidationdatamodule.py` & `spotPython-0.6.3/src/spotPython/light/mnistdatamodule.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,42 @@
 import lightning as L
-from torch.utils.data import DataLoader, Subset
-from typing import Optional
-from spotPython.light.csvdataset import CSVDataset
-from sklearn.model_selection import KFold
-from torch.utils.data import Dataset
-
-
-class CrossValidationDataModule(L.LightningDataModule):
-    def __init__(
-        self,
-        batch_size=64,
-        k: int = 1,
-        split_seed: int = 42,
-        num_splits: int = 10,
-        DATASET_PATH: str = "./data",
-        num_workers: int = 0,
-        pin_memory: bool = False,
-    ):
+from torch.utils.data import DataLoader, random_split
+from torchvision import transforms
+from torchvision.datasets import MNIST
+
+
+class MNISTDataModule(L.LightningDataModule):
+    def __init__(self, batch_size, data_dir: str = "./data", num_workers: int = 0):
         super().__init__()
         self.batch_size = batch_size
-        self.DATASET_PATH = DATASET_PATH
+        self.data_dir = data_dir
         self.num_workers = num_workers
-        self.k = k
-        self.split_seed = split_seed
-        self.num_splits = num_splits
-        self.pin_memory = pin_memory
-        self.save_hyperparameters(logger=False)
-        assert 0 <= self.k < self.num_splits, "incorrect fold number"
-
-        # no data transformations
-        self.transforms = None
-
-        self.data_train: Optional[Dataset] = None
-        self.data_val: Optional[Dataset] = None
+        self.transform = transforms.Compose(
+            [
+                transforms.ToTensor(),
+                transforms.Normalize((0.1307,), (0.3081,)),
+            ]
+        )
 
     def prepare_data(self):
         # download
-        pass
+        MNIST(self.data_dir, train=True, download=True)
+        MNIST(self.data_dir, train=False, download=True)
 
     def setup(self, stage=None):
-        if not self.data_train and not self.data_val:
-            dataset_full = CSVDataset(csv_file="./data/VBDP/train.csv", train=True)
-            kf = KFold(n_splits=self.hparams.num_splits, shuffle=True, random_state=self.hparams.split_seed)
-            all_splits = [k for k in kf.split(dataset_full)]
-            train_indexes, val_indexes = all_splits[self.hparams.k]
-            train_indexes, val_indexes = train_indexes.tolist(), val_indexes.tolist()
-            self.data_train = Subset(dataset_full, train_indexes)
-            print(f"Train Dataset Size: {len(self.data_train)}")
-            self.data_val = Subset(dataset_full, val_indexes)
-            print(f"Val Dataset Size: {len(self.data_val)}")
+        # Assign train/val datasets for use in dataloaders
+        if stage == "fit" or stage is None:
+            mnist_full = MNIST(self.data_dir, train=True, transform=self.transform)
+            self.mnist_train, self.mnist_val = random_split(mnist_full, [55000, 5000])
+
+        # Assign test dataset for use in dataloader(s)
+        if stage == "test" or stage is None:
+            self.mnist_test = MNIST(self.data_dir, train=False, transform=self.transform)
 
     def train_dataloader(self):
-        return DataLoader(
-            dataset=self.data_train,
-            batch_size=self.hparams.batch_size,
-            num_workers=self.hparams.num_workers,
-            pin_memory=self.hparams.pin_memory,
-            shuffle=True,
-        )
+        return DataLoader(self.mnist_train, batch_size=self.batch_size, num_workers=self.num_workers)
 
     def val_dataloader(self):
-        return DataLoader(
-            dataset=self.data_val,
-            batch_size=self.hparams.batch_size,
-            num_workers=self.hparams.num_workers,
-            pin_memory=self.hparams.pin_memory,
-        )
+        return DataLoader(self.mnist_val, batch_size=self.batch_size, num_workers=self.num_workers)
+
+    def test_dataloader(self):
+        return DataLoader(self.mnist_test, batch_size=self.batch_size, num_workers=self.num_workers)
```

### Comparing `spotPython-0.6.1/src/spotPython/plot/contour.py` & `spotPython-0.6.3/src/spotPython/plot/contour.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/plot/validation.py` & `spotPython-0.6.3/src/spotPython/plot/validation.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/sklearn/traintest.py` & `spotPython-0.6.3/src/spotPython/sklearn/traintest.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/spot/spot.py` & `spotPython-0.6.3/src/spotPython/spot/spot.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/torch/activation.py` & `spotPython-0.6.3/src/spotPython/torch/activation.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/torch/dataframedataset.py` & `spotPython-0.6.3/src/spotPython/torch/dataframedataset.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/torch/initialization.py` & `spotPython-0.6.3/src/spotPython/torch/initialization.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/torch/mapk.py` & `spotPython-0.6.3/src/spotPython/torch/mapk.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/torch/netcifar10.py` & `spotPython-0.6.3/src/spotPython/torch/netcifar10.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/torch/netfashionMNIST.py` & `spotPython-0.6.3/src/spotPython/torch/netfashionMNIST.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/torch/netregression.py` & `spotPython-0.6.3/src/spotPython/torch/netregression.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/torch/netvbdp.py` & `spotPython-0.6.3/src/spotPython/torch/netvbdp.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/torch/traintest.py` & `spotPython-0.6.3/src/spotPython/torch/traintest.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/utils/aggregate.py` & `spotPython-0.6.3/src/spotPython/utils/aggregate.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/utils/compare.py` & `spotPython-0.6.3/src/spotPython/utils/compare.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/utils/convert.py` & `spotPython-0.6.3/src/spotPython/utils/convert.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/utils/device.py` & `spotPython-0.6.3/src/spotPython/utils/device.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/utils/eda.py` & `spotPython-0.6.3/src/spotPython/utils/eda.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/utils/file.py` & `spotPython-0.6.3/src/spotPython/utils/file.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/utils/init.py` & `spotPython-0.6.3/src/spotPython/utils/init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/utils/metrics.py` & `spotPython-0.6.3/src/spotPython/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/utils/progress.py` & `spotPython-0.6.3/src/spotPython/utils/progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/utils/repair.py` & `spotPython-0.6.3/src/spotPython/utils/repair.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython/utils/transform.py` & `spotPython-0.6.3/src/spotPython/utils/transform.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/src/spotPython.egg-info/PKG-INFO` & `spotPython-0.6.3/src/spotPython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotPython
-Version: 0.6.1
+Version: 0.6.3
 Summary: spotPython - Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
 Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotPython/issues
 Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotPython
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `spotPython-0.6.1/src/spotPython.egg-info/SOURCES.txt` & `spotPython-0.6.3/src/spotPython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_aggregate_mean_var.py` & `spotPython-0.6.3/test/test_aggregate_mean_var.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_build_Psi.py` & `spotPython-0.6.3/test/test_build_Psi.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_build_U.py` & `spotPython-0.6.3/test/test_build_U.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_build_psi_vec.py` & `spotPython-0.6.3/test/test_build_psi_vec.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_evaluate_new_X.py` & `spotPython-0.6.3/test/test_evaluate_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_evaluate_new_solutions.py` & `spotPython-0.6.3/test/test_evaluate_new_solutions.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_extract_from_bounds.py` & `spotPython-0.6.3/test/test_extract_from_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_generate_design.py` & `spotPython-0.6.3/test/test_generate_design.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_infill.py` & `spotPython-0.6.3/test/test_infill.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_nat_to_cod.py` & `spotPython-0.6.3/test/test_nat_to_cod.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_nat_to_cod_init.py` & `spotPython-0.6.3/test/test_nat_to_cod_init.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_ocba.py` & `spotPython-0.6.3/test/test_ocba.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_repair_non_numeric.py` & `spotPython-0.6.3/test/test_repair_non_numeric.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_set_de_bounds.py` & `spotPython-0.6.3/test/test_set_de_bounds.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_show_progress.py` & `spotPython-0.6.3/test/test_show_progress.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_suggest_new_X.py` & `spotPython-0.6.3/test/test_suggest_new_X.py`

 * *Files identical despite different names*

### Comparing `spotPython-0.6.1/test/test_update_surrogate.py` & `spotPython-0.6.3/test/test_update_surrogate.py`

 * *Files identical despite different names*

