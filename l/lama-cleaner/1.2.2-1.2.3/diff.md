# Comparing `tmp/lama-cleaner-1.2.2.tar.gz` & `tmp/lama-cleaner-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama-cleaner-1.2.2.tar", last modified: Sun Jul  9 04:20:13 2023, max compression
+gzip compressed data, was "lama-cleaner-1.2.3.tar", last modified: Tue Jul 18 13:44:58 2023, max compression
```

## Comparing `lama-cleaner-1.2.2.tar` & `lama-cleaner-1.2.3.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.387716 lama-cleaner-1.2.2/
--rw-r--r--   0 cwq        (501) staff       (20)    11357 2023-02-05 13:09:10.000000 lama-cleaner-1.2.2/LICENSE
--rw-r--r--   0 cwq        (501) staff       (20)     4273 2023-07-09 04:20:13.387603 lama-cleaner-1.2.2/PKG-INFO
--rw-r--r--   0 cwq        (501) staff       (20)     3544 2023-06-17 14:05:39.000000 lama-cleaner-1.2.2/README.md
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.350082 lama-cleaner-1.2.2/lama_cleaner/
--rw-r--r--   0 cwq        (501) staff       (20)      488 2023-04-02 07:46:39.000000 lama-cleaner-1.2.2/lama_cleaner/__init__.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.347308 lama-cleaner-1.2.2/lama_cleaner/app/
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.352174 lama-cleaner-1.2.2/lama_cleaner/app/build/
--rw-r--r--   0 cwq        (501) staff       (20)     6148 2023-05-19 13:47:41.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/.DS_Store
--rw-r--r--   0 cwq        (501) staff       (20)     4559 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/asset-manifest.json
--rw-r--r--   0 cwq        (501) staff       (20)    67646 2023-05-19 13:47:41.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/favicon.ico
--rw-r--r--   0 cwq        (501) staff       (20)      719 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/index.html
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.347561 lama-cleaner-1.2.2/lama_cleaner/app/build/static/
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.352424 lama-cleaner-1.2.2/lama_cleaner/app/build/static/css/
--rw-r--r--   0 cwq        (501) staff       (20)    39068 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/css/main.ce986cc8.css
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.354544 lama-cleaner-1.2.2/lama_cleaner/app/build/static/js/
--rw-r--r--   0 cwq        (501) staff       (20)   831766 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/js/main.1fda6320.js
--rw-r--r--   0 cwq        (501) staff       (20)     1971 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/js/main.1fda6320.js.LICENSE.txt
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.377521 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/
--rw-r--r--   0 cwq        (501) staff       (20)   102868 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Black.15ca31c0a2a68f76d2d1.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   138764 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Black.c6938660eec019fefd68.woff
--rw-r--r--   0 cwq        (501) staff       (20)   146824 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-BlackItalic.ca1e738e4f349f27514d.woff
--rw-r--r--   0 cwq        (501) staff       (20)   108752 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-BlackItalic.cb2a7335650c690077fe.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   143208 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Bold.93c1301bd9f486c573b3.woff
--rw-r--r--   0 cwq        (501) staff       (20)   106140 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   111808 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-BoldItalic.2d26c56a606662486796.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   151052 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-BoldItalic.b376885042f6c961a541.woff
--rw-r--r--   0 cwq        (501) staff       (20)   106108 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraBold.cbe0ae49c52c920fd563.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   142920 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraBold.d0fa3bb2b7c9063dc594.woff
--rw-r--r--   0 cwq        (501) staff       (20)   111708 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.535a6cf662596b3bd6a6.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   150628 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.6ab17abedc4d3f140953.woff
--rw-r--r--   0 cwq        (501) staff       (20)   104232 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraLight.72505e6a122c6acd5471.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   140724 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraLight.c4248615291a9e8f1fb7.woff
--rw-r--r--   0 cwq        (501) staff       (20)   149996 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.170dddfca278d3c2ad4a.woff
--rw-r--r--   0 cwq        (501) staff       (20)   111392 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.5c7d7d6deb1d2ec8d48c.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   144372 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Italic.890025e726861dba417f.woff
--rw-r--r--   0 cwq        (501) staff       (20)   106876 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Italic.cb10ffd7684cd9836a05.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   104332 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   140632 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Light.994e34451cc19ede31d3.woff
--rw-r--r--   0 cwq        (501) staff       (20)   150092 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-LightItalic.ef9f65d91d2b0ba9b2e4.woff
--rw-r--r--   0 cwq        (501) staff       (20)   111332 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-LightItalic.f86952265d7b0f02c921.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   105924 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   142552 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Medium.9053572c46aeb4b16caa.woff
--rw-r--r--   0 cwq        (501) staff       (20)   112184 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-MediumItalic.085cb93e613ba3d40d2b.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   150988 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-MediumItalic.3d0107dd43d0101274d3.woff
--rw-r--r--   0 cwq        (501) staff       (20)   133844 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Regular.8c206db99195777c6769.woff
--rw-r--r--   0 cwq        (501) staff       (20)    98868 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   105804 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   142932 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-SemiBold.cca62d21c8c555c392e5.woff
--rw-r--r--   0 cwq        (501) staff       (20)   151180 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.463bdbfb28abad0fa6df.woff
--rw-r--r--   0 cwq        (501) staff       (20)   112048 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.d9467ee321a8f38aefff.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   135920 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Thin.29b9c616a95a912abf73.woff
--rw-r--r--   0 cwq        (501) staff       (20)    99632 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Thin.fff2a096db014f6239d4.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   145480 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ThinItalic.bae95eb2f889c797e435.woff
--rw-r--r--   0 cwq        (501) staff       (20)   106496 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ThinItalic.bf213704dce6b437ede4.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   245036 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-italic.var.30807be7abc48ba8c73c.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   227180 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-roman.var.ba4caefcdf5b36b438db.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   324864 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter.var.c2fe3cb2b7c746f7966a.woff2
--rw-r--r--   0 cwq        (501) staff       (20)   431724 2023-05-19 13:47:58.000000 lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/coffee-machine-lineal.ee32631219cc3986f861.gif
--rw-r--r--   0 cwq        (501) staff       (20)     3244 2023-02-05 13:09:10.000000 lama-cleaner-1.2.2/lama_cleaner/benchmark.py
--rw-r--r--   0 cwq        (501) staff       (20)     5145 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/const.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.378678 lama-cleaner-1.2.2/lama_cleaner/file_manager/
--rw-r--r--   0 cwq        (501) staff       (20)       38 2023-02-05 13:09:10.000000 lama-cleaner-1.2.2/lama_cleaner/file_manager/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     8685 2023-04-02 07:46:39.000000 lama-cleaner-1.2.2/lama_cleaner/file_manager/file_manager.py
--rw-r--r--   0 cwq        (501) staff       (20)     1293 2023-02-05 13:09:10.000000 lama-cleaner-1.2.2/lama_cleaner/file_manager/storage_backends.py
--rw-r--r--   0 cwq        (501) staff       (20)     1758 2023-02-05 13:09:10.000000 lama-cleaner-1.2.2/lama_cleaner/file_manager/utils.py
--rw-r--r--   0 cwq        (501) staff       (20)     8651 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/helper.py
--rw-r--r--   0 cwq        (501) staff       (20)      232 2023-04-02 07:46:39.000000 lama-cleaner-1.2.2/lama_cleaner/installer.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.382172 lama-cleaner-1.2.2/lama_cleaner/model/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2023-02-05 13:09:10.000000 lama-cleaner-1.2.2/lama_cleaner/model/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     9606 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/model/base.py
--rw-r--r--   0 cwq        (501) staff       (20)    10883 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/model/controlnet.py
--rw-r--r--   0 cwq        (501) staff       (20)     6881 2023-02-05 13:09:10.000000 lama-cleaner-1.2.2/lama_cleaner/model/ddim_sampler.py
--rw-r--r--   0 cwq        (501) staff       (20)    57098 2023-02-27 13:02:16.000000 lama-cleaner-1.2.2/lama_cleaner/model/fcf.py
--rw-r--r--   0 cwq        (501) staff       (20)     3175 2023-03-01 13:56:56.000000 lama-cleaner-1.2.2/lama_cleaner/model/instruct_pix2pix.py
--rw-r--r--   0 cwq        (501) staff       (20)     1480 2023-02-27 13:02:16.000000 lama-cleaner-1.2.2/lama_cleaner/model/lama.py
--rw-r--r--   0 cwq        (501) staff       (20)    11275 2023-02-27 13:02:16.000000 lama-cleaner-1.2.2/lama_cleaner/model/ldm.py
--rw-r--r--   0 cwq        (501) staff       (20)     2884 2023-04-02 07:46:39.000000 lama-cleaner-1.2.2/lama_cleaner/model/manga.py
--rw-r--r--   0 cwq        (501) staff       (20)    62625 2023-04-02 07:46:39.000000 lama-cleaner-1.2.2/lama_cleaner/model/mat.py
--rw-r--r--   0 cwq        (501) staff       (20)      716 2023-02-19 13:09:51.000000 lama-cleaner-1.2.2/lama_cleaner/model/opencv2.py
--rw-r--r--   0 cwq        (501) staff       (20)     2934 2023-03-01 13:56:56.000000 lama-cleaner-1.2.2/lama_cleaner/model/paint_by_example.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.382556 lama-cleaner-1.2.2/lama_cleaner/model/pipeline/
--rw-r--r--   0 cwq        (501) staff       (20)      108 2023-05-01 05:55:02.000000 lama-cleaner-1.2.2/lama_cleaner/model/pipeline/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)    28156 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py
--rw-r--r--   0 cwq        (501) staff       (20)    11851 2023-02-05 13:09:10.000000 lama-cleaner-1.2.2/lama_cleaner/model/plms_sampler.py
--rw-r--r--   0 cwq        (501) staff       (20)     6644 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/model/sd.py
--rw-r--r--   0 cwq        (501) staff       (20)    33811 2023-04-02 07:46:39.000000 lama-cleaner-1.2.2/lama_cleaner/model/utils.py
--rw-r--r--   0 cwq        (501) staff       (20)    15637 2023-04-16 13:06:47.000000 lama-cleaner-1.2.2/lama_cleaner/model/zits.py
--rw-r--r--   0 cwq        (501) staff       (20)     4091 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/model_manager.py
--rw-r--r--   0 cwq        (501) staff       (20)     8695 2023-05-29 13:40:18.000000 lama-cleaner-1.2.2/lama_cleaner/parse_args.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.383933 lama-cleaner-1.2.2/lama_cleaner/plugins/
--rw-r--r--   0 cwq        (501) staff       (20)      263 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)    13473 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/anime_seg.py
--rw-r--r--   0 cwq        (501) staff       (20)      280 2023-04-02 07:46:39.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/base_plugin.py
--rw-r--r--   0 cwq        (501) staff       (20)     2400 2023-04-03 05:14:59.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/gfpgan_plugin.py
--rw-r--r--   0 cwq        (501) staff       (20)     2750 2023-04-02 07:46:39.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/gfpganer.py
--rw-r--r--   0 cwq        (501) staff       (20)     4156 2023-04-02 07:46:39.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/gif.py
--rw-r--r--   0 cwq        (501) staff       (20)     2555 2023-04-06 14:12:49.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/interactive_seg.py
--rw-r--r--   0 cwq        (501) staff       (20)     3573 2023-04-03 05:31:35.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/realesrgan.py
--rw-r--r--   0 cwq        (501) staff       (20)     1053 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/remove_bg.py
--rw-r--r--   0 cwq        (501) staff       (20)     1747 2023-04-03 05:15:02.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/restoreformer.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.384304 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/
--rw-r--r--   0 cwq        (501) staff       (20)      363 2023-04-06 14:12:49.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     2929 2023-04-06 14:12:49.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/build_sam.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.385261 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/
--rw-r--r--   0 cwq        (501) staff       (20)      385 2023-04-06 14:12:49.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     1479 2023-04-06 14:12:49.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/common.py
--rw-r--r--   0 cwq        (501) staff       (20)    14407 2023-04-06 14:12:49.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 cwq        (501) staff       (20)     6614 2023-04-06 14:12:49.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 cwq        (501) staff       (20)     8594 2023-04-06 14:12:49.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 cwq        (501) staff       (20)     7225 2023-04-06 14:12:49.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/sam.py
--rw-r--r--   0 cwq        (501) staff       (20)     8396 2023-04-06 14:12:49.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/transformer.py
--rw-r--r--   0 cwq        (501) staff       (20)    11845 2023-04-10 01:29:17.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/predictor.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.385629 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/utils/
--rw-r--r--   0 cwq        (501) staff       (20)      197 2023-04-06 14:12:49.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/utils/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     4054 2023-04-06 14:12:49.000000 lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/utils/transforms.py
--rw-r--r--   0 cwq        (501) staff       (20)     1374 2023-04-16 13:06:47.000000 lama-cleaner-1.2.2/lama_cleaner/runtime.py
--rw-r--r--   0 cwq        (501) staff       (20)     3399 2023-07-09 03:05:44.000000 lama-cleaner-1.2.2/lama_cleaner/schema.py
--rw-r--r--   0 cwq        (501) staff       (20)    18878 2023-06-17 14:05:39.000000 lama-cleaner-1.2.2/lama_cleaner/server.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.387321 lama-cleaner-1.2.2/lama_cleaner/tests/
--rw-r--r--   0 cwq        (501) staff       (20)        0 2023-02-05 13:09:10.000000 lama-cleaner-1.2.2/lama_cleaner/tests/__init__.py
--rw-r--r--   0 cwq        (501) staff       (20)     6219 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/tests/test_controlnet.py
--rw-r--r--   0 cwq        (501) staff       (20)     2322 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/tests/test_instruct_pix2pix.py
--rw-r--r--   0 cwq        (501) staff       (20)      596 2023-02-05 13:09:10.000000 lama-cleaner-1.2.2/lama_cleaner/tests/test_load_img.py
--rw-r--r--   0 cwq        (501) staff       (20)     5826 2023-04-02 07:46:39.000000 lama-cleaner-1.2.2/lama_cleaner/tests/test_model.py
--rw-r--r--   0 cwq        (501) staff       (20)     1505 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/tests/test_model_md5.py
--rw-r--r--   0 cwq        (501) staff       (20)     3985 2023-02-05 13:09:10.000000 lama-cleaner-1.2.2/lama_cleaner/tests/test_paint_by_example.py
--rw-r--r--   0 cwq        (501) staff       (20)     2965 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/tests/test_plugins.py
--rw-r--r--   0 cwq        (501) staff       (20)     1128 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/tests/test_save_exif.py
--rw-r--r--   0 cwq        (501) staff       (20)     7647 2023-04-02 07:46:39.000000 lama-cleaner-1.2.2/lama_cleaner/tests/test_sd_model.py
--rw-r--r--   0 cwq        (501) staff       (20)     8530 2023-05-19 13:47:19.000000 lama-cleaner-1.2.2/lama_cleaner/web_config.py
-drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-09 04:20:13.350765 lama-cleaner-1.2.2/lama_cleaner.egg-info/
--rw-r--r--   0 cwq        (501) staff       (20)     4273 2023-07-09 04:20:13.000000 lama-cleaner-1.2.2/lama_cleaner.egg-info/PKG-INFO
--rw-r--r--   0 cwq        (501) staff       (20)     6141 2023-07-09 04:20:13.000000 lama-cleaner-1.2.2/lama_cleaner.egg-info/SOURCES.txt
--rw-r--r--   0 cwq        (501) staff       (20)        1 2023-07-09 04:20:13.000000 lama-cleaner-1.2.2/lama_cleaner.egg-info/dependency_links.txt
--rw-r--r--   0 cwq        (501) staff       (20)       58 2023-07-09 04:20:13.000000 lama-cleaner-1.2.2/lama_cleaner.egg-info/entry_points.txt
--rw-r--r--   0 cwq        (501) staff       (20)      232 2023-07-09 04:20:13.000000 lama-cleaner-1.2.2/lama_cleaner.egg-info/requires.txt
--rw-r--r--   0 cwq        (501) staff       (20)       13 2023-07-09 04:20:13.000000 lama-cleaner-1.2.2/lama_cleaner.egg-info/top_level.txt
--rw-r--r--   0 cwq        (501) staff       (20)       38 2023-07-09 04:20:13.387760 lama-cleaner-1.2.2/setup.cfg
--rw-r--r--   0 cwq        (501) staff       (20)     1616 2023-07-09 04:19:43.000000 lama-cleaner-1.2.2/setup.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.723341 lama-cleaner-1.2.3/
+-rw-r--r--   0 cwq        (501) staff       (20)    11357 2023-02-05 13:09:10.000000 lama-cleaner-1.2.3/LICENSE
+-rw-r--r--   0 cwq        (501) staff       (20)     4273 2023-07-18 13:44:58.723217 lama-cleaner-1.2.3/PKG-INFO
+-rw-r--r--   0 cwq        (501) staff       (20)     3544 2023-06-17 14:05:39.000000 lama-cleaner-1.2.3/README.md
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.695566 lama-cleaner-1.2.3/lama_cleaner/
+-rw-r--r--   0 cwq        (501) staff       (20)      488 2023-04-02 07:46:39.000000 lama-cleaner-1.2.3/lama_cleaner/__init__.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.692858 lama-cleaner-1.2.3/lama_cleaner/app/
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.697317 lama-cleaner-1.2.3/lama_cleaner/app/build/
+-rw-r--r--   0 cwq        (501) staff       (20)     6148 2023-05-19 13:47:41.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/.DS_Store
+-rw-r--r--   0 cwq        (501) staff       (20)     4559 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/asset-manifest.json
+-rw-r--r--   0 cwq        (501) staff       (20)    67646 2023-05-19 13:47:41.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/favicon.ico
+-rw-r--r--   0 cwq        (501) staff       (20)      719 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/index.html
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.693105 lama-cleaner-1.2.3/lama_cleaner/app/build/static/
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.697448 lama-cleaner-1.2.3/lama_cleaner/app/build/static/css/
+-rw-r--r--   0 cwq        (501) staff       (20)    39068 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/css/main.ce986cc8.css
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.698253 lama-cleaner-1.2.3/lama_cleaner/app/build/static/js/
+-rw-r--r--   0 cwq        (501) staff       (20)   831766 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/js/main.1fda6320.js
+-rw-r--r--   0 cwq        (501) staff       (20)     1971 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/js/main.1fda6320.js.LICENSE.txt
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.715781 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/
+-rw-r--r--   0 cwq        (501) staff       (20)   102868 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Black.15ca31c0a2a68f76d2d1.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   138764 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Black.c6938660eec019fefd68.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   146824 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-BlackItalic.ca1e738e4f349f27514d.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   108752 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-BlackItalic.cb2a7335650c690077fe.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   143208 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Bold.93c1301bd9f486c573b3.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   106140 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   111808 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-BoldItalic.2d26c56a606662486796.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   151052 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-BoldItalic.b376885042f6c961a541.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   106108 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraBold.cbe0ae49c52c920fd563.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   142920 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraBold.d0fa3bb2b7c9063dc594.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   111708 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.535a6cf662596b3bd6a6.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   150628 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.6ab17abedc4d3f140953.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   104232 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraLight.72505e6a122c6acd5471.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   140724 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraLight.c4248615291a9e8f1fb7.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   149996 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.170dddfca278d3c2ad4a.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   111392 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.5c7d7d6deb1d2ec8d48c.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   144372 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Italic.890025e726861dba417f.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   106876 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Italic.cb10ffd7684cd9836a05.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   104332 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   140632 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Light.994e34451cc19ede31d3.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   150092 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-LightItalic.ef9f65d91d2b0ba9b2e4.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   111332 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-LightItalic.f86952265d7b0f02c921.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   105924 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   142552 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Medium.9053572c46aeb4b16caa.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   112184 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-MediumItalic.085cb93e613ba3d40d2b.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   150988 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-MediumItalic.3d0107dd43d0101274d3.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   133844 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Regular.8c206db99195777c6769.woff
+-rw-r--r--   0 cwq        (501) staff       (20)    98868 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   105804 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   142932 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-SemiBold.cca62d21c8c555c392e5.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   151180 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.463bdbfb28abad0fa6df.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   112048 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.d9467ee321a8f38aefff.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   135920 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Thin.29b9c616a95a912abf73.woff
+-rw-r--r--   0 cwq        (501) staff       (20)    99632 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Thin.fff2a096db014f6239d4.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   145480 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ThinItalic.bae95eb2f889c797e435.woff
+-rw-r--r--   0 cwq        (501) staff       (20)   106496 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ThinItalic.bf213704dce6b437ede4.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   245036 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-italic.var.30807be7abc48ba8c73c.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   227180 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-roman.var.ba4caefcdf5b36b438db.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   324864 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter.var.c2fe3cb2b7c746f7966a.woff2
+-rw-r--r--   0 cwq        (501) staff       (20)   431724 2023-05-19 13:47:58.000000 lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/coffee-machine-lineal.ee32631219cc3986f861.gif
+-rw-r--r--   0 cwq        (501) staff       (20)     3244 2023-02-05 13:09:10.000000 lama-cleaner-1.2.3/lama_cleaner/benchmark.py
+-rw-r--r--   0 cwq        (501) staff       (20)     5145 2023-07-18 13:33:26.000000 lama-cleaner-1.2.3/lama_cleaner/const.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.717028 lama-cleaner-1.2.3/lama_cleaner/file_manager/
+-rw-r--r--   0 cwq        (501) staff       (20)       38 2023-02-05 13:09:10.000000 lama-cleaner-1.2.3/lama_cleaner/file_manager/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8685 2023-04-02 07:46:39.000000 lama-cleaner-1.2.3/lama_cleaner/file_manager/file_manager.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1293 2023-02-05 13:09:10.000000 lama-cleaner-1.2.3/lama_cleaner/file_manager/storage_backends.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1758 2023-02-05 13:09:10.000000 lama-cleaner-1.2.3/lama_cleaner/file_manager/utils.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8651 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/helper.py
+-rw-r--r--   0 cwq        (501) staff       (20)      232 2023-04-02 07:46:39.000000 lama-cleaner-1.2.3/lama_cleaner/installer.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.718932 lama-cleaner-1.2.3/lama_cleaner/model/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2023-02-05 13:09:10.000000 lama-cleaner-1.2.3/lama_cleaner/model/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     9606 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/model/base.py
+-rw-r--r--   0 cwq        (501) staff       (20)    10883 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/model/controlnet.py
+-rw-r--r--   0 cwq        (501) staff       (20)     6881 2023-02-05 13:09:10.000000 lama-cleaner-1.2.3/lama_cleaner/model/ddim_sampler.py
+-rw-r--r--   0 cwq        (501) staff       (20)    57098 2023-02-27 13:02:16.000000 lama-cleaner-1.2.3/lama_cleaner/model/fcf.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3175 2023-03-01 13:56:56.000000 lama-cleaner-1.2.3/lama_cleaner/model/instruct_pix2pix.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1480 2023-02-27 13:02:16.000000 lama-cleaner-1.2.3/lama_cleaner/model/lama.py
+-rw-r--r--   0 cwq        (501) staff       (20)    11275 2023-02-27 13:02:16.000000 lama-cleaner-1.2.3/lama_cleaner/model/ldm.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2884 2023-04-02 07:46:39.000000 lama-cleaner-1.2.3/lama_cleaner/model/manga.py
+-rw-r--r--   0 cwq        (501) staff       (20)    62625 2023-04-02 07:46:39.000000 lama-cleaner-1.2.3/lama_cleaner/model/mat.py
+-rw-r--r--   0 cwq        (501) staff       (20)      716 2023-02-19 13:09:51.000000 lama-cleaner-1.2.3/lama_cleaner/model/opencv2.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2934 2023-03-01 13:56:56.000000 lama-cleaner-1.2.3/lama_cleaner/model/paint_by_example.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.719160 lama-cleaner-1.2.3/lama_cleaner/model/pipeline/
+-rw-r--r--   0 cwq        (501) staff       (20)      108 2023-05-01 05:55:02.000000 lama-cleaner-1.2.3/lama_cleaner/model/pipeline/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    28156 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py
+-rw-r--r--   0 cwq        (501) staff       (20)    11851 2023-02-05 13:09:10.000000 lama-cleaner-1.2.3/lama_cleaner/model/plms_sampler.py
+-rw-r--r--   0 cwq        (501) staff       (20)     6644 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/model/sd.py
+-rw-r--r--   0 cwq        (501) staff       (20)    33811 2023-04-02 07:46:39.000000 lama-cleaner-1.2.3/lama_cleaner/model/utils.py
+-rw-r--r--   0 cwq        (501) staff       (20)    15637 2023-04-16 13:06:47.000000 lama-cleaner-1.2.3/lama_cleaner/model/zits.py
+-rw-r--r--   0 cwq        (501) staff       (20)     4168 2023-07-18 13:34:37.000000 lama-cleaner-1.2.3/lama_cleaner/model_manager.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8695 2023-05-29 13:40:18.000000 lama-cleaner-1.2.3/lama_cleaner/parse_args.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.720352 lama-cleaner-1.2.3/lama_cleaner/plugins/
+-rw-r--r--   0 cwq        (501) staff       (20)      263 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)    13473 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/anime_seg.py
+-rw-r--r--   0 cwq        (501) staff       (20)      280 2023-04-02 07:46:39.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/base_plugin.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2400 2023-04-03 05:14:59.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/gfpgan_plugin.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2750 2023-04-02 07:46:39.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/gfpganer.py
+-rw-r--r--   0 cwq        (501) staff       (20)     4156 2023-04-02 07:46:39.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/gif.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2555 2023-04-06 14:12:49.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/interactive_seg.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3573 2023-04-03 05:31:35.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/realesrgan.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1053 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/remove_bg.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1747 2023-04-03 05:15:02.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/restoreformer.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.720704 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/
+-rw-r--r--   0 cwq        (501) staff       (20)      363 2023-04-06 14:12:49.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2929 2023-04-06 14:12:49.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/build_sam.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.721578 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/
+-rw-r--r--   0 cwq        (501) staff       (20)      385 2023-04-06 14:12:49.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1479 2023-04-06 14:12:49.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/common.py
+-rw-r--r--   0 cwq        (501) staff       (20)    14407 2023-04-06 14:12:49.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 cwq        (501) staff       (20)     6614 2023-04-06 14:12:49.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8594 2023-04-06 14:12:49.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 cwq        (501) staff       (20)     7225 2023-04-06 14:12:49.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/sam.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8396 2023-04-06 14:12:49.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/transformer.py
+-rw-r--r--   0 cwq        (501) staff       (20)    11845 2023-04-10 01:29:17.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/predictor.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.721856 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/utils/
+-rw-r--r--   0 cwq        (501) staff       (20)      197 2023-04-06 14:12:49.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/utils/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     4054 2023-04-06 14:12:49.000000 lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/utils/transforms.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1374 2023-04-16 13:06:47.000000 lama-cleaner-1.2.3/lama_cleaner/runtime.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3399 2023-07-09 03:05:44.000000 lama-cleaner-1.2.3/lama_cleaner/schema.py
+-rw-r--r--   0 cwq        (501) staff       (20)    18878 2023-06-17 14:05:39.000000 lama-cleaner-1.2.3/lama_cleaner/server.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.723029 lama-cleaner-1.2.3/lama_cleaner/tests/
+-rw-r--r--   0 cwq        (501) staff       (20)        0 2023-02-05 13:09:10.000000 lama-cleaner-1.2.3/lama_cleaner/tests/__init__.py
+-rw-r--r--   0 cwq        (501) staff       (20)     6219 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/tests/test_controlnet.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2322 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/tests/test_instruct_pix2pix.py
+-rw-r--r--   0 cwq        (501) staff       (20)      596 2023-02-05 13:09:10.000000 lama-cleaner-1.2.3/lama_cleaner/tests/test_load_img.py
+-rw-r--r--   0 cwq        (501) staff       (20)     5826 2023-04-02 07:46:39.000000 lama-cleaner-1.2.3/lama_cleaner/tests/test_model.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1505 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/tests/test_model_md5.py
+-rw-r--r--   0 cwq        (501) staff       (20)     3985 2023-02-05 13:09:10.000000 lama-cleaner-1.2.3/lama_cleaner/tests/test_paint_by_example.py
+-rw-r--r--   0 cwq        (501) staff       (20)     2965 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/tests/test_plugins.py
+-rw-r--r--   0 cwq        (501) staff       (20)     1128 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/tests/test_save_exif.py
+-rw-r--r--   0 cwq        (501) staff       (20)     7647 2023-04-02 07:46:39.000000 lama-cleaner-1.2.3/lama_cleaner/tests/test_sd_model.py
+-rw-r--r--   0 cwq        (501) staff       (20)     8530 2023-05-19 13:47:19.000000 lama-cleaner-1.2.3/lama_cleaner/web_config.py
+drwxr-xr-x   0 cwq        (501) staff       (20)        0 2023-07-18 13:44:58.696279 lama-cleaner-1.2.3/lama_cleaner.egg-info/
+-rw-r--r--   0 cwq        (501) staff       (20)     4273 2023-07-18 13:44:58.000000 lama-cleaner-1.2.3/lama_cleaner.egg-info/PKG-INFO
+-rw-r--r--   0 cwq        (501) staff       (20)     6141 2023-07-18 13:44:58.000000 lama-cleaner-1.2.3/lama_cleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 cwq        (501) staff       (20)        1 2023-07-18 13:44:58.000000 lama-cleaner-1.2.3/lama_cleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 cwq        (501) staff       (20)       58 2023-07-18 13:44:58.000000 lama-cleaner-1.2.3/lama_cleaner.egg-info/entry_points.txt
+-rw-r--r--   0 cwq        (501) staff       (20)      232 2023-07-18 13:44:58.000000 lama-cleaner-1.2.3/lama_cleaner.egg-info/requires.txt
+-rw-r--r--   0 cwq        (501) staff       (20)       13 2023-07-18 13:44:58.000000 lama-cleaner-1.2.3/lama_cleaner.egg-info/top_level.txt
+-rw-r--r--   0 cwq        (501) staff       (20)       38 2023-07-18 13:44:58.723383 lama-cleaner-1.2.3/setup.cfg
+-rw-r--r--   0 cwq        (501) staff       (20)     1616 2023-07-18 13:44:30.000000 lama-cleaner-1.2.3/setup.py
```

### Comparing `lama-cleaner-1.2.2/LICENSE` & `lama-cleaner-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/PKG-INFO` & `lama-cleaner-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama-cleaner
-Version: 1.2.2
+Version: 1.2.3
 Summary: Image inpainting tool powered by SOTA AI Model
 Home-page: https://github.com/Sanster/lama-cleaner
 Author: PanicByte
 Author-email: cwq1913@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lama-cleaner Version: 1.2.2 Summary: Image
+Metadata-Version: 2.1 Name: lama-cleaner Version: 1.2.3 Summary: Image
 inpainting tool powered by SOTA AI Model Home-page: https://github.com/Sanster/
 lama-cleaner Author: PanicByte Author-email: cwq1913@gmail.com Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
```

### Comparing `lama-cleaner-1.2.2/README.md` & `lama-cleaner-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/.DS_Store` & `lama-cleaner-1.2.3/lama_cleaner/app/build/.DS_Store`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/asset-manifest.json` & `lama-cleaner-1.2.3/lama_cleaner/app/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/favicon.ico` & `lama-cleaner-1.2.3/lama_cleaner/app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/index.html` & `lama-cleaner-1.2.3/lama_cleaner/app/build/index.html`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/css/main.ce986cc8.css` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/css/main.ce986cc8.css`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/js/main.1fda6320.js` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/js/main.1fda6320.js`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/js/main.1fda6320.js.LICENSE.txt` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/js/main.1fda6320.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Black.15ca31c0a2a68f76d2d1.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Black.15ca31c0a2a68f76d2d1.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Black.c6938660eec019fefd68.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Black.c6938660eec019fefd68.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-BlackItalic.ca1e738e4f349f27514d.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-BlackItalic.ca1e738e4f349f27514d.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-BlackItalic.cb2a7335650c690077fe.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-BlackItalic.cb2a7335650c690077fe.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Bold.93c1301bd9f486c573b3.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Bold.93c1301bd9f486c573b3.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Bold.ec64ea577b0349e055ad.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-BoldItalic.2d26c56a606662486796.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-BoldItalic.2d26c56a606662486796.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-BoldItalic.b376885042f6c961a541.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-BoldItalic.b376885042f6c961a541.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraBold.cbe0ae49c52c920fd563.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraBold.cbe0ae49c52c920fd563.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraBold.d0fa3bb2b7c9063dc594.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraBold.d0fa3bb2b7c9063dc594.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.535a6cf662596b3bd6a6.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.535a6cf662596b3bd6a6.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.6ab17abedc4d3f140953.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraBoldItalic.6ab17abedc4d3f140953.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraLight.72505e6a122c6acd5471.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraLight.72505e6a122c6acd5471.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraLight.c4248615291a9e8f1fb7.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraLight.c4248615291a9e8f1fb7.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.170dddfca278d3c2ad4a.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.170dddfca278d3c2ad4a.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.5c7d7d6deb1d2ec8d48c.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ExtraLightItalic.5c7d7d6deb1d2ec8d48c.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Italic.890025e726861dba417f.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Italic.890025e726861dba417f.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Italic.cb10ffd7684cd9836a05.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Italic.cb10ffd7684cd9836a05.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Light.2d5198822ab091ce4305.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Light.994e34451cc19ede31d3.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Light.994e34451cc19ede31d3.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-LightItalic.ef9f65d91d2b0ba9b2e4.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-LightItalic.ef9f65d91d2b0ba9b2e4.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-LightItalic.f86952265d7b0f02c921.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-LightItalic.f86952265d7b0f02c921.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Medium.293fd13dbca5a3e450ef.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Medium.9053572c46aeb4b16caa.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Medium.9053572c46aeb4b16caa.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-MediumItalic.085cb93e613ba3d40d2b.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-MediumItalic.085cb93e613ba3d40d2b.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-MediumItalic.3d0107dd43d0101274d3.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-MediumItalic.3d0107dd43d0101274d3.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Regular.8c206db99195777c6769.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Regular.8c206db99195777c6769.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Regular.c8ba52b05a9ef10f4758.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-SemiBold.b5f0f109bc88052d4000.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-SemiBold.cca62d21c8c555c392e5.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-SemiBold.cca62d21c8c555c392e5.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.463bdbfb28abad0fa6df.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.463bdbfb28abad0fa6df.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.d9467ee321a8f38aefff.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-SemiBoldItalic.d9467ee321a8f38aefff.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Thin.29b9c616a95a912abf73.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Thin.29b9c616a95a912abf73.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-Thin.fff2a096db014f6239d4.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-Thin.fff2a096db014f6239d4.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ThinItalic.bae95eb2f889c797e435.woff` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ThinItalic.bae95eb2f889c797e435.woff`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-ThinItalic.bf213704dce6b437ede4.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-ThinItalic.bf213704dce6b437ede4.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-italic.var.30807be7abc48ba8c73c.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-italic.var.30807be7abc48ba8c73c.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter-roman.var.ba4caefcdf5b36b438db.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter-roman.var.ba4caefcdf5b36b438db.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/Inter.var.c2fe3cb2b7c746f7966a.woff2` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/Inter.var.c2fe3cb2b7c746f7966a.woff2`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/app/build/static/media/coffee-machine-lineal.ee32631219cc3986f861.gif` & `lama-cleaner-1.2.3/lama_cleaner/app/build/static/media/coffee-machine-lineal.ee32631219cc3986f861.gif`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/benchmark.py` & `lama-cleaner-1.2.3/lama_cleaner/benchmark.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/const.py` & `lama-cleaner-1.2.3/lama_cleaner/const.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/file_manager/file_manager.py` & `lama-cleaner-1.2.3/lama_cleaner/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/file_manager/storage_backends.py` & `lama-cleaner-1.2.3/lama_cleaner/file_manager/storage_backends.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/file_manager/utils.py` & `lama-cleaner-1.2.3/lama_cleaner/file_manager/utils.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/helper.py` & `lama-cleaner-1.2.3/lama_cleaner/helper.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/base.py` & `lama-cleaner-1.2.3/lama_cleaner/model/base.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/controlnet.py` & `lama-cleaner-1.2.3/lama_cleaner/model/controlnet.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/ddim_sampler.py` & `lama-cleaner-1.2.3/lama_cleaner/model/ddim_sampler.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/fcf.py` & `lama-cleaner-1.2.3/lama_cleaner/model/fcf.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/instruct_pix2pix.py` & `lama-cleaner-1.2.3/lama_cleaner/model/instruct_pix2pix.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/lama.py` & `lama-cleaner-1.2.3/lama_cleaner/model/lama.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/ldm.py` & `lama-cleaner-1.2.3/lama_cleaner/model/ldm.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/manga.py` & `lama-cleaner-1.2.3/lama_cleaner/model/manga.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/mat.py` & `lama-cleaner-1.2.3/lama_cleaner/model/mat.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/opencv2.py` & `lama-cleaner-1.2.3/lama_cleaner/model/opencv2.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/paint_by_example.py` & `lama-cleaner-1.2.3/lama_cleaner/model/paint_by_example.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py` & `lama-cleaner-1.2.3/lama_cleaner/model/pipeline/pipeline_stable_diffusion_controlnet_inpaint.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/plms_sampler.py` & `lama-cleaner-1.2.3/lama_cleaner/model/plms_sampler.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/sd.py` & `lama-cleaner-1.2.3/lama_cleaner/model/sd.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/utils.py` & `lama-cleaner-1.2.3/lama_cleaner/model/utils.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model/zits.py` & `lama-cleaner-1.2.3/lama_cleaner/model/zits.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/model_manager.py` & `lama-cleaner-1.2.3/lama_cleaner/model_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,17 @@
             raise e
 
     def switch_controlnet_method(self, control_method: str):
         if not self.kwargs.get("sd_controlnet"):
             return
         if self.kwargs["sd_controlnet_method"] == control_method:
             return
+        if not hasattr(self.model, "is_local_sd_model"):
+            return
+
         if self.model.is_local_sd_model:
             # is_native_control_inpaint 表示加载了普通 SD 模型
             if (
                 self.model.is_native_control_inpaint
                 and control_method != "control_v11p_sd15_inpaint"
             ):
                 raise RuntimeError(
```

### Comparing `lama-cleaner-1.2.2/lama_cleaner/parse_args.py` & `lama-cleaner-1.2.3/lama_cleaner/parse_args.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/anime_seg.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/anime_seg.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/gfpgan_plugin.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/gfpgan_plugin.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/gfpganer.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/gfpganer.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/gif.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/gif.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/interactive_seg.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/interactive_seg.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/realesrgan.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/realesrgan.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/remove_bg.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/remove_bg.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/restoreformer.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/restoreformer.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/build_sam.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/common.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/image_encoder.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/mask_decoder.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/prompt_encoder.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/sam.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/modeling/transformer.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/predictor.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/plugins/segment_anything/utils/transforms.py` & `lama-cleaner-1.2.3/lama_cleaner/plugins/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/runtime.py` & `lama-cleaner-1.2.3/lama_cleaner/runtime.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/schema.py` & `lama-cleaner-1.2.3/lama_cleaner/schema.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/server.py` & `lama-cleaner-1.2.3/lama_cleaner/server.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/tests/test_controlnet.py` & `lama-cleaner-1.2.3/lama_cleaner/tests/test_controlnet.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/tests/test_instruct_pix2pix.py` & `lama-cleaner-1.2.3/lama_cleaner/tests/test_instruct_pix2pix.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/tests/test_load_img.py` & `lama-cleaner-1.2.3/lama_cleaner/tests/test_load_img.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/tests/test_model.py` & `lama-cleaner-1.2.3/lama_cleaner/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/tests/test_model_md5.py` & `lama-cleaner-1.2.3/lama_cleaner/tests/test_model_md5.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/tests/test_paint_by_example.py` & `lama-cleaner-1.2.3/lama_cleaner/tests/test_paint_by_example.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/tests/test_plugins.py` & `lama-cleaner-1.2.3/lama_cleaner/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/tests/test_save_exif.py` & `lama-cleaner-1.2.3/lama_cleaner/tests/test_save_exif.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/tests/test_sd_model.py` & `lama-cleaner-1.2.3/lama_cleaner/tests/test_sd_model.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner/web_config.py` & `lama-cleaner-1.2.3/lama_cleaner/web_config.py`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/lama_cleaner.egg-info/PKG-INFO` & `lama-cleaner-1.2.3/lama_cleaner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama-cleaner
-Version: 1.2.2
+Version: 1.2.3
 Summary: Image inpainting tool powered by SOTA AI Model
 Home-page: https://github.com/Sanster/lama-cleaner
 Author: PanicByte
 Author-email: cwq1913@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lama-cleaner Version: 1.2.2 Summary: Image
+Metadata-Version: 2.1 Name: lama-cleaner Version: 1.2.3 Summary: Image
 inpainting tool powered by SOTA AI Model Home-page: https://github.com/Sanster/
 lama-cleaner Author: PanicByte Author-email: cwq1913@gmail.com Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Scientific/
```

### Comparing `lama-cleaner-1.2.2/lama_cleaner.egg-info/SOURCES.txt` & `lama-cleaner-1.2.3/lama_cleaner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lama-cleaner-1.2.2/setup.py` & `lama-cleaner-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                 requires.append(line.strip())
     return requires
 
 
 # https://setuptools.readthedocs.io/en/latest/setuptools.html#including-data-files
 setuptools.setup(
     name="lama-cleaner",
-    version="1.2.2",
+    version="1.2.3",
     author="PanicByte",
     author_email="cwq1913@gmail.com",
     description="Image inpainting tool powered by SOTA AI Model",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Sanster/lama-cleaner",
     packages=setuptools.find_packages("./"),
```

