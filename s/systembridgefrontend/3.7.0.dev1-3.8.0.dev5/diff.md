# Comparing `tmp/systembridgefrontend-3.7.0.dev1.tar.gz` & `tmp/systembridgefrontend-3.8.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgefrontend-3.7.0.dev1.tar", last modified: Mon Jul  3 08:34:58 2023, max compression
+gzip compressed data, was "systembridgefrontend-3.8.0.dev5.tar", last modified: Tue Jul 18 09:49:41 2023, max compression
```

## Comparing `systembridgefrontend-3.7.0.dev1.tar` & `systembridgefrontend-3.8.0.dev5.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.341780 systembridgefrontend-3.7.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-03 08:34:58.341780 systembridgefrontend-3.7.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 08:34:58.345780 systembridgefrontend-3.7.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.325779 systembridgefrontend-3.7.0.dev1/systembridgefrontend/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-03 08:34:56.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.325779 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.321779 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.321779 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.325779 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/7cCNYQwxkasei7aJF3BXn/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.333779 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    60440 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/134-8b4cf5ad285047cd.js
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/142-b511304dc754f6ca.js
--rw-r--r--   0 runner    (1001) docker     (123)    51206 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/154-7942dd40332ec4bf.js
--rw-r--r--   0 runner    (1001) docker     (123)   116342 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/171.64880094f51dbbf7.js
--rw-r--r--   0 runner    (1001) docker     (123)    69766 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/418-f078369e2fd2524e.js
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/498-112306b4f8cd81ec.js
--rw-r--r--   0 runner    (1001) docker     (123)    50639 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/633-a2b446f38d34df6a.js
--rw-r--r--   0 runner    (1001) docker     (123)    69782 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/699-1a88a588882ce475.js
--rw-r--r--   0 runner    (1001) docker     (123)    22931 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/731-eb947eaba8f94f26.js
--rw-r--r--   0 runner    (1001) docker     (123)    58330 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js
--rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/767-b6df483a2f96f15d.js
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/826-e44464776abed9eb.js
--rw-r--r--   0 runner    (1001) docker     (123)    56873 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/913-948b3bc7b49750f4.js
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js
--rw-r--r--   0 runner    (1001) docker     (123)   141023 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/framework-305cb810cde7afac.js
--rw-r--r--   0 runner    (1001) docker     (123)    95829 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/main-d5c9aef8f3ea3bae.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.337780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/
--rw-r--r--   0 runner    (1001) docker     (123)    51895 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.337780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.337780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-ea5036b8dd1a507b.js
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-7e45aefe6a4d48af.js
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/data-a3eeebdc39c5f892.js
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/notification-0384bbf9e77dbfb4.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.337780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/player/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-8b29e9945ddce62c.js
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-b8b2ae3418f95cef.js
--rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/settings-0b5df1a27de4507f.js
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js
--rw-r--r--   0 runner    (1001) docker     (123)    91381 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-07-03 08:34:37.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/webpack-29bb9d3475e20ac7.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.337780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.341780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-03 08:34:38.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.d17f5f2b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.d6d4cf7b.woff
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.9600b4a6.woff
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.b339d926.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.341780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.341780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/bridges/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/bridges/openon.html
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/bridges/setup.html
--rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/data.html
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/notification.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.341780 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/player/
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/player/audio.html
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/player/video.html
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-03 08:34:39.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-03 08:34:36.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:34:58.325779 systembridgefrontend-3.7.0.dev1/systembridgefrontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-03 08:34:58.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-07-03 08:34:58.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:34:58.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 08:34:58.000000 systembridgefrontend-3.7.0.dev1/systembridgefrontend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.686462 systembridgefrontend-3.8.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-18 09:49:41.686462 systembridgefrontend-3.8.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 09:49:02.000000 systembridgefrontend-3.8.0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:49:41.686462 systembridgefrontend-3.8.0.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-18 09:49:02.000000 systembridgefrontend-3.8.0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.678462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-18 09:49:02.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-18 09:49:39.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.678462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-18 09:49:02.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.674462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.674462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.682462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    60819 2023-07-18 09:49:02.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/134-be8afb194db80d1f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-07-18 09:49:02.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/142-6fa2d4be01c7dab9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    51193 2023-07-18 09:49:02.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/154-454aae7a1f6cc481.js
+-rw-r--r--   0 runner    (1001) docker     (123)   116154 2023-07-18 09:49:02.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/171.cfc407cdf8574e41.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69763 2023-07-18 09:49:02.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/29107295-809b6f0b05884bf7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-07-18 09:49:02.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/361-70173883768cacf6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/498-c0ac8cca5a5197e4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    54369 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/514-17895623628db944.js
+-rw-r--r--   0 runner    (1001) docker     (123)    69853 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/699-a015e8646ccfaf97.js
+-rw-r--r--   0 runner    (1001) docker     (123)    56876 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/713-76d25fee0de05077.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8381 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/728-4d1eeb7a2f426351.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23306 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/731-b6cafe94e88ed8c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    58300 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/75fc9c18-c0cb841eaf75495d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/767-21712ed9071ee20e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/826-25c5c840b401fbf5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)   140978 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/framework-7a7e500878b44665.js
+-rw-r--r--   0 runner    (1001) docker     (123)    98361 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/main-2ecf43899f8683c2.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.682462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    51899 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/_app-4638cf4f01fc5510.js
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.682462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.682462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-57051d0ee30b9efa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-d4f904aedaf93672.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/data-59d72c465167efc4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/notification-416e0ab0e8597db3.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.682462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/player/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-3826169d9ca46804.js
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-9c7e9646d273d6aa.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/settings-c2e844bc6170d7a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91381 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-18 09:49:03.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/webpack-8c974454c1c3cd10.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.682462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.682462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/iX_HmcWE_KZJ1V0jDuyN4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.686462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.d17f5f2b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.d6d4cf7b.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.9600b4a6.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.b339d926.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.686462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.686462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/bridges/
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-18 09:49:05.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/bridges/openon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-18 09:49:05.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/bridges/setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20079 2023-07-18 09:49:05.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/data.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/notification.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.686462 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/player/
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-18 09:49:05.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/player/audio.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-07-18 09:49:05.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/player/video.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-18 09:49:04.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-18 09:49:02.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-18 09:49:02.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:41.678462 systembridgefrontend-3.8.0.dev5/systembridgefrontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-18 09:49:41.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-07-18 09:49:41.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:49:41.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-18 09:49:41.000000 systembridgefrontend-3.8.0.dev5/systembridgefrontend.egg-info/top_level.txt
```

### Comparing `systembridgefrontend-3.7.0.dev1/pyproject.toml` & `systembridgefrontend-3.8.0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/setup.py` & `systembridgefrontend-3.8.0.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/404.html` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/404.html`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>404: This page could not be found</title><meta name="next-head-count" content="3"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/pages/_error-54de1933a164a1ff.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_buildManifest.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><div style="font-family:system-ui,&quot;Segoe UI&quot;,Roboto,Helvetica,Arial,sans-serif,&quot;Apple Color Emoji&quot;,&quot;Segoe UI Emoji&quot;;height:100vh;text-align:center;display:flex;flex-direction:column;align-items:center;justify-content:center"><div style="line-height:48px"><style>body{color:#000;background:#fff;margin:0}.next-error-h1{border-right:1px solid rgba(0,0,0,.3)}@media (prefers-color-scheme:dark){body{color:#fff;background:#000}.next-error-h1{border-right:1px solid rgba(255,255,255,.3)}}</style><h1 class="next-error-h1" style="display:inline-block;margin:0 20px 0 0;padding-right:23px;font-size:24px;font-weight:500;vertical-align:top">404</h1><div style="display:inline-block"><h2 style="font-size:14px;font-weight:400;line-height:28px">This page could not be found<!-- -->.</h2></div></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"statusCode":404}},"page":"/_error","query":{},"buildId":"iX_HmcWE_KZJ1V0jDuyN4","nextExport":true,"isFallback":false,"gip":true,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_buildManifest.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
-self.__BUILD_MANIFEST = function(s, a, c, e, t, p, i, n, b, d, f, u) {
+self.__BUILD_MANIFEST = function(s, a, c, e, t, p, i, n, d, f, b, u) {
     return {
         __rewrites: {
             beforeFiles: [],
             afterFiles: [],
             fallback: []
         },
         "/": [s, a, "static/chunks/pages/index-f934b9a030f633a0.js"],
         "/_error": ["static/chunks/pages/_error-54de1933a164a1ff.js"],
-        "/app/bridges/openon": [s, a, c, e, p, i, n, "static/chunks/pages/app/bridges/openon-ea5036b8dd1a507b.js"],
-        "/app/bridges/setup": [s, a, c, e, p, i, b, "static/chunks/pages/app/bridges/setup-7e45aefe6a4d48af.js"],
-        "/app/data": [s, t, a, e, "static/chunks/731-eb947eaba8f94f26.js", "static/chunks/pages/app/data-a3eeebdc39c5f892.js"],
-        "/app/notification": [s, a, i, "static/chunks/pages/app/notification-0384bbf9e77dbfb4.js"],
-        "/app/player/audio": [s, t, d, a, c, f, u, "static/chunks/pages/app/player/audio-8b29e9945ddce62c.js"],
-        "/app/player/video": [s, t, d, a, c, f, u, "static/chunks/pages/app/player/video-b8b2ae3418f95cef.js"],
-        "/app/settings": [s, t, a, c, e, p, n, b, "static/chunks/826-e44464776abed9eb.js", "static/chunks/pages/app/settings-0b5df1a27de4507f.js"],
+        "/app/bridges/openon": [s, a, c, e, t, p, n, "static/chunks/pages/app/bridges/openon-57051d0ee30b9efa.js"],
+        "/app/bridges/setup": [s, a, c, e, t, p, d, "static/chunks/pages/app/bridges/setup-d4f904aedaf93672.js"],
+        "/app/data": [s, a, e, i, "static/chunks/731-b6cafe94e88ed8c7.js", "static/chunks/pages/app/data-59d72c465167efc4.js"],
+        "/app/notification": [s, a, p, "static/chunks/pages/app/notification-416e0ab0e8597db3.js"],
+        "/app/player/audio": [s, f, a, c, i, b, u, "static/chunks/pages/app/player/audio-3826169d9ca46804.js"],
+        "/app/player/video": [s, f, a, c, i, b, u, "static/chunks/pages/app/player/video-9c7e9646d273d6aa.js"],
+        "/app/settings": [s, "static/chunks/29107295-809b6f0b05884bf7.js", a, c, e, t, n, d, "static/chunks/826-25c5c840b401fbf5.js", "static/chunks/pages/app/settings-c2e844bc6170d7a5.js"],
         sortedPages: ["/", "/_app", "/_error", "/app/bridges/openon", "/app/bridges/setup", "/app/data", "/app/notification", "/app/player/audio", "/app/player/video", "/app/settings"]
     }
-}("static/chunks/b2e984c5-f44d94ec783f59d4.js", "static/chunks/134-8b4cf5ad285047cd.js", "static/chunks/418-f078369e2fd2524e.js", "static/chunks/498-112306b4f8cd81ec.js", "static/chunks/29107295-8f8fd7e7e27aa6a2.js", "static/chunks/699-1a88a588882ce475.js", "static/chunks/154-7942dd40332ec4bf.js", "static/chunks/913-948b3bc7b49750f4.js", "static/chunks/767-b6df483a2f96f15d.js", "static/chunks/75fc9c18-058f7f136d59a7a6.js", "static/chunks/633-a2b446f38d34df6a.js", "static/chunks/142-b511304dc754f6ca.js"), self.__BUILD_MANIFEST_CB && self.__BUILD_MANIFEST_CB();
+}("static/chunks/b2e984c5-f44d94ec783f59d4.js", "static/chunks/134-be8afb194db80d1f.js", "static/chunks/728-4d1eeb7a2f426351.js", "static/chunks/498-c0ac8cca5a5197e4.js", "static/chunks/699-a015e8646ccfaf97.js", "static/chunks/154-454aae7a1f6cc481.js", "static/chunks/361-70173883768cacf6.js", "static/chunks/713-76d25fee0de05077.js", "static/chunks/767-21712ed9071ee20e.js", "static/chunks/75fc9c18-c0cb841eaf75495d.js", "static/chunks/514-17895623628db944.js", "static/chunks/142-6fa2d4be01c7dab9.js"), self.__BUILD_MANIFEST_CB && self.__BUILD_MANIFEST_CB();
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/134-8b4cf5ad285047cd.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/134-be8afb194db80d1f.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -261,15 +261,15 @@
                 Z: function() {
                     return Z
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(7294),
-                a = r(6010),
+                a = r(3680),
                 l = r(4780),
                 s = r(948),
                 u = r(1657),
                 c = r(8216),
                 p = r(629),
                 d = r(1588),
                 f = r(4867);
@@ -401,15 +401,15 @@
                 Z: function() {
                     return b
                 }
             });
             var n = r(7462),
                 o = r(3366),
                 i = r(7294),
-                a = r(6010),
+                a = r(209),
                 l = r(9731),
                 s = r(6523),
                 u = r(9707),
                 c = r(6682),
                 p = r(5893);
             let d = ["className", "component"];
             var f = r(7078),
@@ -454,15 +454,15 @@
                 Z: function() {
                     return $
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(7294),
-                a = r(6010),
+                a = r(3680),
                 l = r(7925),
                 s = r(4780),
                 u = r(1796),
                 c = r(948),
                 p = r(1657),
                 d = r(2022),
                 f = r(8216),
@@ -736,15 +736,15 @@
                 Z: function() {
                     return F
                 }
             });
             var n = r(7462),
                 o = r(3366),
                 i = r(7294),
-                a = r(6010),
+                a = r(3680),
                 l = r(4780),
                 s = r(948),
                 u = r(1657),
                 c = r(1705),
                 p = r(2068),
                 d = r(9962).Z,
                 f = r(5068),
@@ -1336,15 +1336,15 @@
                 Z: function() {
                     return w
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(7294),
-                a = r(6010),
+                a = r(209),
                 l = r(4142),
                 s = r(4867),
                 u = r(4780),
                 c = r(9628),
                 p = r(3264),
                 d = r(6500),
                 f = r(5893);
@@ -1468,15 +1468,15 @@
                 ZP: function() {
                     return C
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(7294),
-                a = r(6010),
+                a = r(3680),
                 l = r(5408),
                 s = r(9707),
                 u = r(4780),
                 c = r(948),
                 p = r(1657),
                 d = r(2734);
             let f = i.createContext();
@@ -1788,15 +1788,15 @@
                 Z: function() {
                     return k
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(7294),
-                a = r(6010),
+                a = r(3680),
                 l = r(4780),
                 s = r(1796),
                 u = r(948),
                 c = r(1657),
                 p = r(2022),
                 d = r(8216),
                 f = r(1588),
@@ -1927,15 +1927,15 @@
                 Z: function() {
                     return x
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(7294),
-                a = r(6010),
+                a = r(3680),
                 l = r(4780),
                 s = r(1796),
                 u = r(948),
                 c = e => ((e < 1 ? 5.11916 * e ** 2 : 4.5 * Math.log(e + 1) + 2) / 100).toFixed(2),
                 p = r(1657),
                 d = r(1588),
                 f = r(4867);
@@ -2021,15 +2021,15 @@
                 Z: function() {
                     return b
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(7294),
-                a = r(6010),
+                a = r(3680),
                 l = r(4780),
                 s = r(1657),
                 u = r(948),
                 c = r(1588),
                 p = r(4867);
 
             function d(e) {
@@ -2109,15 +2109,15 @@
                 Z: function() {
                     return w
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(7294),
-                a = r(6010),
+                a = r(3680),
                 l = r(9707),
                 s = r(4780),
                 u = r(948),
                 c = r(1657),
                 p = r(8216),
                 d = r(1588),
                 f = r(4867);
@@ -2224,14 +2224,31 @@
                         ref: t,
                         ownerState: R,
                         className: (0, a.Z)($.root, p)
                     }, S))
                 });
             var w = k
         },
+        3680: function(e, t, r) {
+            "use strict";
+            t.Z = function() {
+                for (var e, t, r = 0, n = ""; r < arguments.length;)(e = arguments[r++]) && (t = function e(t) {
+                    var r, n, o = "";
+                    if ("string" == typeof t || "number" == typeof t) o += t;
+                    else if ("object" == typeof t) {
+                        if (Array.isArray(t))
+                            for (r = 0; r < t.length; r++) t[r] && (n = e(t[r])) && (o && (o += " "), o += n);
+                        else
+                            for (r in t) t[r] && (o && (o += " "), o += r)
+                    }
+                    return o
+                }(e)) && (n && (n += " "), n += t);
+                return n
+            }
+        },
         948: function(e, t, r) {
             "use strict";
             r.d(t, {
                 Dz: function() {
                     return l
                 },
                 FO: function() {
@@ -2616,14 +2633,31 @@
         },
         3264: function(e, t, r) {
             "use strict";
             var n = r(182);
             let o = (0, n.ZP)();
             t.Z = o
         },
+        209: function(e, t, r) {
+            "use strict";
+            t.Z = function() {
+                for (var e, t, r = 0, n = ""; r < arguments.length;)(e = arguments[r++]) && (t = function e(t) {
+                    var r, n, o = "";
+                    if ("string" == typeof t || "number" == typeof t) o += t;
+                    else if ("object" == typeof t) {
+                        if (Array.isArray(t))
+                            for (r = 0; r < t.length; r++) t[r] && (n = e(t[r])) && (o && (o += " "), o += n);
+                        else
+                            for (r in t) t[r] && (o && (o += " "), o += r)
+                    }
+                    return o
+                }(e)) && (n && (n += " "), n += t);
+                return n
+            }
+        },
         7078: function(e, t) {
             "use strict";
             let r;
             let n = e => e,
                 o = (r = n, {
                     configure(e) {
                         r = e
@@ -2823,31 +2857,14 @@
                             a = !1
                         }, 100), t.current = !1, !0)
                     },
                     ref: e
                 }
             }
         },
-        6010: function(e, t, r) {
-            "use strict";
-            t.Z = function() {
-                for (var e, t, r = 0, n = ""; r < arguments.length;)(e = arguments[r++]) && (t = function e(t) {
-                    var r, n, o = "";
-                    if ("string" == typeof t || "number" == typeof t) o += t;
-                    else if ("object" == typeof t) {
-                        if (Array.isArray(t))
-                            for (r = 0; r < t.length; r++) t[r] && (n = e(t[r])) && (o && (o += " "), o += n);
-                        else
-                            for (r in t) t[r] && (o && (o += " "), o += r)
-                    }
-                    return o
-                }(e)) && (n && (n += " "), n += t);
-                return n
-            }
-        },
         1163: function(e, t, r) {
             e.exports = r(6885)
         },
         2703: function(e, t, r) {
             "use strict";
             var n = r(414);
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/142-b511304dc754f6ca.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/142-6fa2d4be01c7dab9.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -197,45 +197,45 @@
                 }
                 isConnected() {
                     var e;
                     return (null === (e = this.websocket) || void 0 === e ? void 0 : e.readyState) === WebSocket.OPEN
                 }
                 getData(e) {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && (console.log("Get data:", e), this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "GET_DATA",
                         modules: e
                     })))
                 }
                 getSettings() {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && (console.log("Get settings"), this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "GET_SETTINGS"
                     })))
                 }
                 registerDataListener(e) {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && (console.log("Register data listener:", e), this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "REGISTER_DATA_LISTENER",
                         modules: e
                     })))
                 }
                 sendPlayerStatus(e) {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "MEDIA_STATUS",
                         status: e
                     }))
                 }
                 updateSetting(e, t) {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && (console.log("Update setting:", {
                         key: e,
                         value: t
                     }), this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "UPDATE_SETTING",
                         setting: e,
                         value: t
                     })))
                 }
                 constructor(e, t, n) {
                     this.port = e || 9170, this.apiKey = t, (async () => {
@@ -244,116 +244,119 @@
                 }
             }
         },
         630: function(e, t, n) {
             let s;
             n.d(t, {
                 Z: function() {
-                    return E
+                    return I
                 }
             });
             var o = n(5893),
                 i = n(7294),
                 a = n(6885),
-                r = n(6486),
-                l = n(8096),
-                c = n(8995),
-                u = n(6018),
-                d = n(2734),
-                p = n(6886),
-                m = n(7357),
-                h = n(2022),
-                y = n(6628),
-                x = n(5861),
-                g = n(3946),
-                v = n(3754),
-                b = n(8849),
-                k = n(5317),
-                f = n(381),
-                w = n.n(f),
-                j = n(6310),
-                S = function() {
-                    let [e, t] = (0, l.nn)(), [n, s] = (0, i.useState)(!1), [a, r] = (0, l.XI)(), c = (0, i.useRef)(null), {
-                        duration: u,
-                        playing: f,
-                        muted: S,
-                        loaded: P,
-                        position: E,
+                r = n(361),
+                l = n.n(r),
+                c = n(8446),
+                u = n.n(c),
+                d = n(8096),
+                p = n(8995),
+                m = n(6018),
+                h = n(2734),
+                y = n(6886),
+                x = n(7357),
+                g = n(2022),
+                v = n(6628),
+                b = n(5861),
+                k = n(3946),
+                f = n(5929),
+                w = n(8849),
+                j = n(5317),
+                S = n(381),
+                P = n.n(S),
+                E = n(6310),
+                C = function() {
+                    let [e, t] = (0, d.nn)(), [n, s] = (0, i.useState)(!1), [a, r] = (0, d.XI)(), l = (0, i.useRef)(null), {
+                        duration: c,
+                        playing: u,
+                        muted: p,
+                        loaded: m,
+                        position: S,
                         volume: C
                     } = (0, i.useMemo)(() => e, [e]), Z = (0, i.useMemo)(() => "".concat((100 * C).toFixed(0), "%"), [C]), I = (0, i.useMemo)(() => {
-                        let e = w().duration(E, "seconds");
+                        let e = P().duration(S, "seconds");
                         return "".concat(e.minutes().toString().padStart(2, "0"), ":").concat(e.seconds().toString().padStart(2, "0"))
-                    }, [E]), D = (0, i.useMemo)(() => {
-                        let e = w().duration(u, "seconds");
+                    }, [S]), _ = (0, i.useMemo)(() => {
+                        let e = P().duration(c, "seconds");
                         return "".concat(e.minutes().toString().padStart(2, "0"), ":").concat(e.seconds().toString().padStart(2, "0"))
-                    }, [u]), {
+                    }, [c]), {
                         artist: M,
                         album: N,
-                        cover: _,
-                        source: A,
+                        cover: A,
+                        source: D,
                         title: O
                     } = (0, i.useMemo)(() => e.source, [e]), T = (0, i.useCallback)(n => {
                         t({
                             ...e,
                             loaded: n
                         })
                     }, [e, t]), L = (0, i.useCallback)(n => {
                         t({
                             ...e,
                             playing: n
                         })
                     }, [e, t]), U = (0, i.useCallback)(() => {
-                        L(!f)
-                    }, [f, L]), K = (0, i.useCallback)(n => {
+                        L(!u)
+                    }, [u, L]), K = (0, i.useCallback)(n => {
                         t({
                             ...e,
                             muted: n
                         })
                     }, [e, t]), R = (0, i.useCallback)(() => {
-                        K(!S)
-                    }, [S, K]), W = (0, i.useCallback)((n, s) => {
+                        K(!p)
+                    }, [p, K]), W = (0, i.useCallback)((n, s) => {
                         let o = "down" === s ? C - n : "up" === s ? C + n : n;
                         o > 1 && (o = 1), o < 0 && (o = 0), t({
                             ...e,
                             volume: o
-                        }), S && K(!1)
-                    }, [S, C, e, t, K]), q = (0, i.useCallback)(n => {
+                        }), p && K(!1)
+                    }, [p, C, e, t, K]), q = (0, i.useCallback)(n => {
                         t({
                             ...e,
                             duration: n
                         })
                     }, [e, t]), z = (0, i.useCallback)(n => {
-                        u && n > u && (n = u), n < 0 && (n = 0), t({
+                        c && n > c && (n = c), n < 0 && (n = 0), t({
                             ...e,
                             position: n
                         })
-                    }, [e, u, t]), F = (0, i.useCallback)(e => {
+                    }, [e, c, t]), F = (0, i.useCallback)(e => {
                         var t;
-                        null === (t = c.current) || void 0 === t || t.seekTo(e, "seconds"), s(!1), f || L(!0)
-                    }, [f, L]);
+                        null === (t = l.current) || void 0 === t || t.seekTo(e, "seconds"), s(!1), u || L(!0)
+                    }, [u, L]);
 
                     function G() {
                         L(!1), s(!0)
                     }
 
                     function B() {
-                        E && F(E)
+                        S && F(S)
                     }(0, i.useEffect)(() => {
-                        P || T(!0)
-                    }, [P, T, L]);
-                    let J = (0, d.Z)();
+                        m || T(!0)
+                    }, [m, T, L]);
+                    let J = (0, h.Z)();
                     return (0, o.jsxs)(o.Fragment, {
-                        children: [(0, o.jsx)(j.Z, {
-                            ref: c,
+                        children: [(0, o.jsx)(E.Z, {
+                            ref: l,
                             height: "0px",
                             width: "0px",
-                            muted: S,
-                            playing: f,
+                            muted: p,
+                            playing: u,
                             stopOnUnmount: !0,
-                            url: A,
+                            url: D,
                             volume: C,
                             onDuration: e => {
                                 q(e)
                             },
                             onPause: () => {
                                 L(!1)
                             },
@@ -365,203 +368,203 @@
                             },
                             onProgress: e => {
                                 let {
                                     playedSeconds: t
                                 } = e;
                                 n || z(t)
                             }
-                        }), (0, o.jsxs)(p.ZP, {
+                        }), (0, o.jsxs)(y.ZP, {
                             container: !0,
                             direction: "row",
                             alignItems: "center",
                             justifyItems: "center",
                             wrap: "nowrap",
                             sx: {
                                 height: 140,
                                 width: 540,
                                 overflow: "hidden"
                             },
-                            children: [(0, o.jsx)(p.ZP, {
+                            children: [(0, o.jsx)(y.ZP, {
                                 item: !0,
                                 sx: {
                                     width: 140,
                                     margin: J.spacing(0, 1, 0, 0)
                                 },
-                                children: (0, o.jsx)(m.Z, {
+                                children: (0, o.jsx)(x.Z, {
                                     ref: a,
-                                    children: (0, o.jsxs)(h.Z, {
-                                        "aria-label": f ? "Pause" : "Play",
+                                    children: (0, o.jsxs)(g.Z, {
+                                        "aria-label": u ? "Pause" : "Play",
                                         onClick: U,
                                         children: [(0, o.jsx)("img", {
                                             alt: "".concat(M, " - ").concat(N),
-                                            src: _ || "https://raw.githubusercontent.com/timmo001/system-bridge/master/resources/system-bridge-dimmed.svg",
+                                            src: A || "https://raw.githubusercontent.com/timmo001/system-bridge/master/resources/system-bridge-dimmed.svg",
                                             width: 140
-                                        }), (0, o.jsx)(y.Z, {
+                                        }), (0, o.jsx)(v.Z, {
                                             in: !!r,
                                             timeout: {
                                                 enter: 200,
                                                 exit: 400
                                             },
-                                            children: (0, o.jsx)(m.Z, {
+                                            children: (0, o.jsx)(x.Z, {
                                                 sx: {
                                                     position: "absolute",
                                                     display: "flex",
                                                     height: "100%",
                                                     width: "100%",
                                                     zIndex: 100
                                                 },
-                                                children: (0, o.jsx)(b.Icon, {
-                                                    id: f ? "pause" : "play",
-                                                    path: f ? k.Wa1 : k._86,
+                                                children: (0, o.jsx)(w.Icon, {
+                                                    id: u ? "pause" : "play",
+                                                    path: u ? j.Wa1 : j._86,
                                                     size: 6,
                                                     style: {
                                                         position: "relative",
                                                         margin: "auto"
                                                     }
                                                 })
                                             })
                                         })]
                                     })
                                 })
-                            }), (0, o.jsx)(p.ZP, {
+                            }), (0, o.jsx)(y.ZP, {
                                 item: !0,
                                 xs: !0,
-                                children: (0, o.jsxs)(p.ZP, {
+                                children: (0, o.jsxs)(y.ZP, {
                                     container: !0,
                                     direction: "column",
                                     alignItems: "flex-start",
                                     justifyItems: "space-around",
-                                    children: [(0, o.jsx)(p.ZP, {
+                                    children: [(0, o.jsx)(y.ZP, {
                                         item: !0,
-                                        children: (0, o.jsxs)(x.Z, {
+                                        children: (0, o.jsxs)(b.Z, {
                                             color: "textPrimary",
                                             component: "span",
                                             variant: "subtitle1",
                                             noWrap: !0,
                                             children: [M, " - ", O]
                                         })
-                                    }), (0, o.jsx)(p.ZP, {
+                                    }), (0, o.jsx)(y.ZP, {
                                         item: !0,
-                                        children: (0, o.jsx)(x.Z, {
+                                        children: (0, o.jsx)(b.Z, {
                                             color: "textSecondary",
                                             component: "span",
                                             variant: "subtitle2",
                                             noWrap: !0,
                                             children: N
                                         })
-                                    }), (0, o.jsxs)(p.ZP, {
+                                    }), (0, o.jsxs)(y.ZP, {
                                         item: !0,
                                         container: !0,
                                         alignContent: "center",
-                                        children: [(0, o.jsx)(p.ZP, {
+                                        children: [(0, o.jsx)(y.ZP, {
                                             item: !0,
                                             xs: 4
-                                        }), (0, o.jsx)(p.ZP, {
+                                        }), (0, o.jsx)(y.ZP, {
                                             sx: {
                                                 margin: J.spacing(0, 1, 0, 0)
                                             },
                                             item: !0,
-                                            children: (0, o.jsx)(g.Z, {
+                                            children: (0, o.jsx)(k.Z, {
                                                 size: "small",
                                                 onClick: R,
-                                                children: S ? (0, o.jsx)(b.Icon, {
+                                                children: p ? (0, o.jsx)(w.Icon, {
                                                     id: "mute",
-                                                    path: k.PLS,
+                                                    path: j.PLS,
                                                     size: 1.25
-                                                }) : (0, o.jsx)(b.Icon, {
+                                                }) : (0, o.jsx)(w.Icon, {
                                                     id: "unmute",
-                                                    path: k.dw,
+                                                    path: j.dw,
                                                     size: 1.25
                                                 })
                                             })
-                                        }), (0, o.jsx)(p.ZP, {
+                                        }), (0, o.jsx)(y.ZP, {
                                             sx: {
                                                 margin: J.spacing(.6, 2, 0, 0)
                                             },
                                             item: !0,
                                             xs: !0,
-                                            children: (0, o.jsx)(v.ZP, {
+                                            children: (0, o.jsx)(f.ZP, {
                                                 min: 0,
                                                 max: 1,
                                                 step: .01,
                                                 value: C,
                                                 onChange: (e, t) => {
                                                     "number" == typeof t && W(t)
                                                 }
                                             })
-                                        }), (0, o.jsx)(p.ZP, {
+                                        }), (0, o.jsx)(y.ZP, {
                                             sx: {
                                                 margin: J.spacing(.9, C >= 1 ? 1 : 2, 0, 0)
                                             },
                                             item: !0,
-                                            children: (0, o.jsx)(x.Z, {
+                                            children: (0, o.jsx)(b.Z, {
                                                 component: "span",
                                                 variant: "body2",
                                                 children: Z
                                             })
                                         })]
-                                    }), (0, o.jsxs)(p.ZP, {
+                                    }), (0, o.jsxs)(y.ZP, {
                                         container: !0,
-                                        children: [(0, o.jsx)(p.ZP, {
+                                        children: [(0, o.jsx)(y.ZP, {
                                             sx: {
                                                 margin: J.spacing(.25, 2, 0, 0)
                                             },
                                             item: !0,
-                                            children: (0, o.jsx)(x.Z, {
+                                            children: (0, o.jsx)(b.Z, {
                                                 component: "span",
                                                 variant: "body2",
                                                 children: I
                                             })
-                                        }), (0, o.jsx)(p.ZP, {
+                                        }), (0, o.jsx)(y.ZP, {
                                             sx: {
                                                 margin: J.spacing(0, 2, 0, 0)
                                             },
                                             item: !0,
                                             xs: !0,
-                                            children: (0, o.jsx)(v.ZP, {
+                                            children: (0, o.jsx)(f.ZP, {
                                                 min: 0,
-                                                max: u,
+                                                max: c,
                                                 step: .1,
-                                                value: E,
+                                                value: S,
                                                 valueLabelDisplay: "off",
                                                 onMouseDown: G,
                                                 onKeyDown: G,
                                                 onChange: function(e, t) {
                                                     z(t)
                                                 },
                                                 onMouseUp: B,
                                                 onKeyUp: B
                                             })
-                                        }), (0, o.jsx)(p.ZP, {
+                                        }), (0, o.jsx)(y.ZP, {
                                             sx: {
                                                 margin: J.spacing(.25, 1, 0, 0)
                                             },
                                             item: !0,
-                                            children: (0, o.jsx)(x.Z, {
+                                            children: (0, o.jsx)(b.Z, {
                                                 component: "span",
                                                 variant: "body2",
-                                                children: D
+                                                children: _
                                             })
                                         })]
                                     })]
                                 })
                             })]
                         })]
                     })
                 },
-                P = function() {
-                    let [e, t] = (0, l.nn)(), {
+                Z = function() {
+                    let [e, t] = (0, d.nn)(), {
                         autoplay: n,
                         duration: s,
                         playing: a,
                         muted: r,
-                        loaded: c,
-                        volume: u
+                        loaded: l,
+                        volume: c
                     } = (0, i.useMemo)(() => e, [e]), {
-                        source: d
+                        source: u
                     } = (0, i.useMemo)(() => e.source, [e]), p = (0, i.useCallback)(n => {
                         t({
                             ...e,
                             loaded: n
                         })
                     }, [e, t]), m = (0, i.useCallback)(n => {
                         console.log("Set playing:", n), t({
@@ -571,43 +574,43 @@
                     }, [e, t]), h = (0, i.useCallback)(n => {
                         t({
                             ...e,
                             muted: n
                         })
                     }, [e, t]);
                     (0, i.useCallback)((n, s) => {
-                        let o = "down" === s ? u - n : "up" === s ? u + n : n;
+                        let o = "down" === s ? c - n : "up" === s ? c + n : n;
                         o > 1 && (o = 1), o < 0 && (o = 0), t({
                             ...e,
                             volume: o
                         }), r && h(!1)
-                    }, [r, u, e, t, h]);
+                    }, [r, c, e, t, h]);
                     let y = (0, i.useCallback)(n => t({
                             ...e,
                             duration: n
                         }), [e, t]),
                         x = (0, i.useCallback)(n => {
                             s && n > s && (n = s), n < 0 && (n = 0), t({
                                 ...e,
                                 position: n
                             })
                         }, [e, s, t]);
                     return (0, i.useEffect)(() => {
-                        c || p(!0)
-                    }, [c, p]), (0, o.jsx)(o.Fragment, {
-                        children: (0, o.jsx)(j.Z, {
+                        l || p(!0)
+                    }, [l, p]), (0, o.jsx)(o.Fragment, {
+                        children: (0, o.jsx)(E.Z, {
                             autoPlay: n,
                             controls: !0,
                             height: "270px",
                             width: "480px",
                             playsinline: !0,
                             muted: r,
                             playing: a,
-                            url: d,
-                            volume: u,
+                            url: u,
+                            volume: c,
                             style: {
                                 position: "absolute",
                                 top: "0",
                                 left: "0",
                                 overflow: "hidden"
                             },
                             onReady: () => {
@@ -622,126 +625,126 @@
                                     playedSeconds: t
                                 } = e;
                                 return x(t)
                             }
                         })
                     })
                 },
-                E = function(e) {
+                I = function(e) {
                     let {
                         playerType: t
-                    } = e, [n, d] = (0, i.useState)(!1), [p, m] = (0, l.nn)(), h = (0, c.D)(p), y = (0, a.useRouter)(), x = y.query, g = (0, i.useCallback)(e => {
+                    } = e, [n, r] = (0, i.useState)(!1), [c, h] = (0, d.nn)(), y = (0, p.D)(c), x = (0, a.useRouter)(), g = x.query, v = (0, i.useCallback)(e => {
                         switch (console.log("Event:", e), e.type) {
                             case "MEDIA_PAUSE":
-                                m({
-                                    ...p,
+                                h({
+                                    ...c,
                                     playing: !1
                                 });
                                 break;
                             case "MEDIA_PLAY":
-                                m({
-                                    ...p,
+                                h({
+                                    ...c,
                                     playing: !0
                                 });
                                 break;
                             case "MEDIA_VOLUME_DOWN":
-                                e.volume && m({
-                                    ...p,
-                                    volume: p.volume - e.volume
+                                e.volume && h({
+                                    ...c,
+                                    volume: c.volume - e.volume
                                 });
                                 break;
                             case "MEDIA_VOLUME_UP":
-                                e.volume && m({
-                                    ...p,
-                                    volume: p.volume + e.volume
+                                e.volume && h({
+                                    ...c,
+                                    volume: c.volume + e.volume
                                 });
                                 break;
                             case "MEDIA_VOLUME_SET":
-                                e.volume && m({
-                                    ...p,
+                                e.volume && h({
+                                    ...c,
                                     volume: e.volume
                                 });
                                 break;
                             case "MEDIA_VOLUME_SET":
-                                e.position && m({
-                                    ...p,
+                                e.position && h({
+                                    ...c,
                                     position: e.position
                                 })
                         }
-                    }, [p, m]), v = (0, i.useCallback)((e, t) => {
-                        console.log("Setup WebSocketConnection"), (s = new u.C(e, t, async () => {
+                    }, [c, h]), b = (0, i.useCallback)((e, t) => {
+                        console.log("Setup WebSocketConnection"), (s = new m.C(e, t, async () => {
                             console.log("Connected to WebSocket")
-                        })).onEvent = g
-                    }, [g]);
+                        })).onEvent = v
+                    }, [v]);
                     (0, i.useEffect)(() => {
-                        !n && x && x.apiKey && (d(!0), v(Number(x.apiPort) || 9170, String(x.apiKey)))
-                    }, [n, v, x]), (0, i.useEffect)(() => {
-                        if (!p && y.isReady) {
+                        !n && g && g.apiKey && (r(!0), b(Number(g.apiPort) || 9170, String(g.apiKey)))
+                    }, [n, b, g]), (0, i.useEffect)(() => {
+                        if (!c && x.isReady) {
                             var e, n;
-                            let s = Number(x.volume);
+                            let s = Number(g.volume);
                             switch (t) {
                                 default:
                                     break;
                                 case "audio":
-                                    m({
-                                        autoplay: (null === (e = x.autoplay) || void 0 === e ? void 0 : e.toLowerCase()) === "true",
+                                    h({
+                                        autoplay: (null === (e = g.autoplay) || void 0 === e ? void 0 : e.toLowerCase()) === "true",
                                         muted: !1,
                                         playing: !1,
                                         loaded: !1,
                                         position: 0,
                                         duration: 1,
                                         source: {
                                             type: "audio",
-                                            source: x.url,
-                                            album: x.album || "Unknown Album",
-                                            artist: x.artist || "Unknown Aritst",
-                                            cover: x.cover,
-                                            title: x.title || "Unknown Title",
+                                            source: g.url,
+                                            album: g.album || "Unknown Album",
+                                            artist: g.artist || "Unknown Aritst",
+                                            cover: g.cover,
+                                            title: g.title || "Unknown Title",
                                             volumeInitial: (s > 0 ? s : 40) / 100
                                         },
                                         volume: (s > 0 ? s : 40) / 100
                                     });
                                     break;
                                 case "video":
-                                    m({
-                                        autoplay: (null === (n = x.autoplay) || void 0 === n ? void 0 : n.toLowerCase()) === "true",
+                                    h({
+                                        autoplay: (null === (n = g.autoplay) || void 0 === n ? void 0 : n.toLowerCase()) === "true",
                                         muted: !1,
                                         playing: !1,
                                         loaded: !1,
                                         position: 0,
                                         duration: 1,
                                         source: {
                                             type: "video",
-                                            source: String(x.url),
+                                            source: String(g.url),
                                             volumeInitial: (s > 0 ? s : 40) / 100
                                         },
                                         volume: (s > 0 ? s : 40) / 100
                                     })
                             }
                         }
-                    }, [p, m, t, y, x]), (0, i.useEffect)(() => {
-                        if (p) {
+                    }, [c, h, t, x, g]), (0, i.useEffect)(() => {
+                        if (c) {
                             let e;
-                            h && "audio" === (e = (0, r.cloneDeep)(h)).source.type && delete e.source.cover;
-                            let t = (0, r.cloneDeep)(p);
-                            if ("audio" === t.source.type && delete t.source.cover, !(0, r.isEqual)(t, e)) {
+                            y && "audio" === (e = l()(y)).source.type && delete e.source.cover;
+                            let t = l()(c);
+                            if ("audio" === t.source.type && delete t.source.cover, !u()(t, e)) {
                                 if (console.log("Player update\n\npreviousStatus:", e, "\nnewStatus:", t), !t.loaded || !s) return;
                                 if (!s.isConnected()) {
-                                    d(!1), console.warn("WebSocket not connected");
+                                    r(!1), console.warn("WebSocket not connected");
                                     return
                                 }
                                 s.sendPlayerStatus(t)
                             }
                         }
-                    }, [p, h]);
-                    let b = (0, i.useMemo)(() => {
-                        if (p) return p.source.type
-                    }, [p]);
+                    }, [c, y]);
+                    let k = (0, i.useMemo)(() => {
+                        if (c) return c.source.type
+                    }, [c]);
                     return (0, o.jsx)(o.Fragment, {
-                        children: "audio" === b ? (0, o.jsx)(S, {}) : "video" === b ? (0, o.jsx)(P, {}) : ""
+                        children: "audio" === k ? (0, o.jsx)(C, {}) : "video" === k ? (0, o.jsx)(Z, {}) : ""
                     })
                 }
         },
         8096: function(e, t, n) {
             n.d(t, {
                 I0: function() {
                     return r
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/154-7942dd40332ec4bf.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/154-454aae7a1f6cc481.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1147,15 +1147,14 @@
                 },
                 te = "undefined" != typeof URLSearchParams ? URLSearchParams : G,
                 tr = "undefined" != typeof FormData ? FormData : null,
                 tn = "undefined" != typeof Blob ? Blob : null;
             let to = ("undefined" == typeof navigator || "ReactNative" !== (n = navigator.product) && "NativeScript" !== n && "NS" !== n) && "undefined" != typeof window && "undefined" != typeof document,
                 ti = "undefined" != typeof WorkerGlobalScope && self instanceof WorkerGlobalScope && "function" == typeof self.importScripts;
             var ts = {
-                    isBrowser: !0,
                     classes: {
                         URLSearchParams: te,
                         FormData: tr,
                         Blob: tn
                     },
                     isStandardBrowserEnv: to,
                     isStandardBrowserWebWorkerEnv: ti,
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/171.64880094f51dbbf7.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/171.cfc407cdf8574e41.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -53,17 +53,17 @@
                     version: "2.6.12"
                 };
                 "number" == typeof __e && (__e = n)
             }, function(e, t, n) {
                 var a = n(26)("wks"),
                     r = n(17),
                     o = n(3).Symbol,
-                    i = "function" == typeof o;
+                    s = "function" == typeof o;
                 (e.exports = function(e) {
-                    return a[e] || (a[e] = i && o[e] || (i ? o : r)("Symbol." + e))
+                    return a[e] || (a[e] = s && o[e] || (s ? o : r)("Symbol." + e))
                 }).store = a
             }, function(e, t) {
                 var n = e.exports = "undefined" != typeof window && window.Math == Math ? window : "undefined" != typeof self && self.Math == Math ? self : Function("return this")();
                 "number" == typeof __g && (__g = n)
             }, function(e, t, n) {
                 e.exports = !n(8)(function() {
                     return 7 != Object.defineProperty({}, "a", {
@@ -85,18 +85,18 @@
                 } : function(e, t, n) {
                     return e[t] = n, e
                 }
             }, function(e, t, n) {
                 var a = n(10),
                     r = n(35),
                     o = n(23),
-                    i = Object.defineProperty;
+                    s = Object.defineProperty;
                 t.f = n(4) ? Object.defineProperty : function(e, t, n) {
                     if (a(e), t = o(t, !0), a(n), r) try {
-                        return i(e, t, n)
+                        return s(e, t, n)
                     } catch (e) {}
                     if ("get" in n || "set" in n) throw TypeError("Accessors not supported!");
                     return "value" in n && (e[t] = n.value), e
                 }
             }, function(e, t) {
                 e.exports = function(e) {
                     try {
@@ -131,27 +131,27 @@
                 }
             }, function(e, t) {
                 e.exports = !0
             }, function(e, t, n) {
                 var a = n(3),
                     r = n(1),
                     o = n(53),
-                    i = n(6),
-                    s = n(5),
+                    s = n(6),
+                    i = n(5),
                     c = function(e, t, n) {
-                        var l, u, p, d = e & c.F,
-                            f = e & c.G,
+                        var l, u, p, f = e & c.F,
+                            d = e & c.G,
                             b = e & c.S,
                             h = e & c.P,
                             v = e & c.B,
                             m = e & c.W,
-                            y = f ? r : r[t] || (r[t] = {}),
+                            y = d ? r : r[t] || (r[t] = {}),
                             g = y.prototype,
-                            E = f ? a : b ? a[t] : (a[t] || {}).prototype;
-                        for (l in f && (n = t), n)(u = !d && E && void 0 !== E[l]) && s(y, l) || (p = u ? E[l] : n[l], y[l] = f && "function" != typeof E[l] ? n[l] : v && u ? o(p, a) : m && E[l] == p ? function(e) {
+                            E = d ? a : b ? a[t] : (a[t] || {}).prototype;
+                        for (l in d && (n = t), n)(u = !f && E && void 0 !== E[l]) && i(y, l) || (p = u ? E[l] : n[l], y[l] = d && "function" != typeof E[l] ? n[l] : v && u ? o(p, a) : m && E[l] == p ? function(e) {
                             var t = function(t, n, a) {
                                 if (this instanceof e) {
                                     switch (arguments.length) {
                                         case 0:
                                             return new e;
                                         case 1:
                                             return new e(t);
@@ -159,15 +159,15 @@
                                             return new e(t, n)
                                     }
                                     return new e(t, n, a)
                                 }
                                 return e.apply(this, arguments)
                             };
                             return t.prototype = e.prototype, t
-                        }(p) : h && "function" == typeof p ? o(Function.call, p) : p, h && ((y.virtual || (y.virtual = {}))[l] = p, e & c.R && g && !g[l] && i(g, l, p)))
+                        }(p) : h && "function" == typeof p ? o(Function.call, p) : p, h && ((y.virtual || (y.virtual = {}))[l] = p, e & c.R && g && !g[l] && s(g, l, p)))
                     };
                 c.F = 1, c.G = 2, c.S = 4, c.P = 8, c.B = 16, c.W = 32, c.U = 64, c.R = 128, e.exports = c
             }, function(e, t) {
                 e.exports = function(e, t) {
                     return {
                         enumerable: !(1 & e),
                         configurable: !(2 & e),
@@ -255,80 +255,80 @@
                     e && !r(e = n ? e : e.prototype, o) && a(e, o, {
                         configurable: !0,
                         value: t
                     })
                 }
             }, function(e, t, n) {
                 n(62);
-                for (var a = n(3), r = n(6), o = n(12), i = n(2)("toStringTag"), s = "CSSRuleList,CSSStyleDeclaration,CSSValueList,ClientRectList,DOMRectList,DOMStringList,DOMTokenList,DataTransferItemList,FileList,HTMLAllCollection,HTMLCollection,HTMLFormElement,HTMLSelectElement,MediaList,MimeTypeArray,NamedNodeMap,NodeList,PaintRequestList,Plugin,PluginArray,SVGLengthList,SVGNumberList,SVGPathSegList,SVGPointList,SVGStringList,SVGTransformList,SourceBufferList,StyleSheetList,TextTrackCueList,TextTrackList,TouchList".split(","), c = 0; c < s.length; c++) {
-                    var l = s[c],
+                for (var a = n(3), r = n(6), o = n(12), s = n(2)("toStringTag"), i = "CSSRuleList,CSSStyleDeclaration,CSSValueList,ClientRectList,DOMRectList,DOMStringList,DOMTokenList,DataTransferItemList,FileList,HTMLAllCollection,HTMLCollection,HTMLFormElement,HTMLSelectElement,MediaList,MimeTypeArray,NamedNodeMap,NodeList,PaintRequestList,Plugin,PluginArray,SVGLengthList,SVGNumberList,SVGPathSegList,SVGPointList,SVGStringList,SVGTransformList,SourceBufferList,StyleSheetList,TextTrackCueList,TextTrackList,TouchList".split(","), c = 0; c < i.length; c++) {
+                    var l = i[c],
                         u = a[l],
                         p = u && u.prototype;
-                    p && !p[i] && r(p, i, l), o[l] = o.Array
+                    p && !p[s] && r(p, s, l), o[l] = o.Array
                 }
             }, function(e, t, n) {
                 t.f = n(2)
             }, function(e, t, n) {
                 var a = n(3),
                     r = n(1),
                     o = n(14),
-                    i = n(30),
-                    s = n(7).f;
+                    s = n(30),
+                    i = n(7).f;
                 e.exports = function(e) {
                     var t = r.Symbol || (r.Symbol = o ? {} : a.Symbol || {});
-                    "_" == e.charAt(0) || e in t || s(t, e, {
-                        value: i.f(e)
+                    "_" == e.charAt(0) || e in t || i(t, e, {
+                        value: s.f(e)
                     })
                 }
             }, function(e, t) {
                 t.f = Object.getOwnPropertySymbols
             }, function(e, t) {
                 e.exports = function(e, t, n) {
                     return Math.min(Math.max(e, t), n)
                 }
             }, function(e, t, n) {
                 "use strict";
                 var a = n(14),
                     r = n(15),
                     o = n(37),
-                    i = n(6),
-                    s = n(12),
+                    s = n(6),
+                    i = n(12),
                     c = n(55),
                     l = n(28),
                     u = n(61),
                     p = n(2)("iterator"),
-                    d = !([].keys && "next" in [].keys()),
-                    f = function() {
+                    f = !([].keys && "next" in [].keys()),
+                    d = function() {
                         return this
                     };
                 e.exports = function(e, t, n, b, h, v, m) {
                     c(n, t, b);
                     var y, g, E, j = function(e) {
-                            return !d && e in O ? O[e] : function() {
+                            return !f && e in O ? O[e] : function() {
                                 return new n(this, e)
                             }
                         },
                         x = t + " Iterator",
                         _ = "values" == h,
                         k = !1,
                         O = e.prototype,
                         C = O[p] || O["@@iterator"] || h && O[h],
                         S = C || j(h),
                         w = h ? _ ? j("entries") : S : void 0,
                         A = "Array" == t && O.entries || C;
-                    if (A && (E = u(A.call(new e))) !== Object.prototype && E.next && (l(E, x, !0), a || "function" == typeof E[p] || i(E, p, f)), _ && C && "values" !== C.name && (k = !0, S = function() {
+                    if (A && (E = u(A.call(new e))) !== Object.prototype && E.next && (l(E, x, !0), a || "function" == typeof E[p] || s(E, p, d)), _ && C && "values" !== C.name && (k = !0, S = function() {
                             return C.call(this)
-                        }), (!a || m) && (d || k || !O[p]) && i(O, p, S), s[t] = S, s[x] = f, h) {
+                        }), (!a || m) && (f || k || !O[p]) && s(O, p, S), i[t] = S, i[x] = d, h) {
                         if (y = {
                                 values: _ ? S : j("values"),
                                 keys: v ? S : j("keys"),
                                 entries: w
                             }, m)
                             for (g in y) g in O || o(O, g, y[g]);
-                        else r(r.P + r.F * (d || k), t, y)
+                        else r(r.P + r.F * (f || k), t, y)
                     }
                     return y
                 }
             }, function(e, t, n) {
                 e.exports = !n(4) && !n(8)(function() {
                     return 7 != Object.defineProperty(n(36)("div"), "a", {
                         get: function() {
@@ -345,37 +345,37 @@
                 }
             }, function(e, t, n) {
                 e.exports = n(6)
             }, function(e, t, n) {
                 var a = n(10),
                     r = n(56),
                     o = n(27),
-                    i = n(25)("IE_PROTO"),
-                    s = function() {},
+                    s = n(25)("IE_PROTO"),
+                    i = function() {},
                     c = function() {
                         var e, t = n(36)("iframe"),
                             a = o.length;
                         for (t.style.display = "none", n(60).appendChild(t), t.src = "javascript:", (e = t.contentWindow.document).open(), e.write("<script>document.F=Object</script>"), e.close(), c = e.F; a--;) delete c.prototype[o[a]];
                         return c()
                     };
                 e.exports = Object.create || function(e, t) {
                     var n;
-                    return null !== e ? (s.prototype = a(e), n = new s, s.prototype = null, n[i] = e) : n = c(), void 0 === t ? n : r(n, t)
+                    return null !== e ? (i.prototype = a(e), n = new i, i.prototype = null, n[s] = e) : n = c(), void 0 === t ? n : r(n, t)
                 }
             }, function(e, t, n) {
                 var a = n(5),
                     r = n(9),
                     o = n(57)(!1),
-                    i = n(25)("IE_PROTO");
+                    s = n(25)("IE_PROTO");
                 e.exports = function(e, t) {
-                    var n, s = r(e),
+                    var n, i = r(e),
                         c = 0,
                         l = [];
-                    for (n in s) n != i && a(s, n) && l.push(n);
-                    for (; t.length > c;) a(s, n = t[c++]) && (~o(l, n) || l.push(n));
+                    for (n in i) n != s && a(i, n) && l.push(n);
+                    for (; t.length > c;) a(i, n = t[c++]) && (~o(l, n) || l.push(n));
                     return l
                 }
             }, function(e, t, n) {
                 var a = n(24);
                 e.exports = Object("z").propertyIsEnumerable(0) ? Object : function(e) {
                     return "String" == a(e) ? e.split("") : Object(e)
                 }
@@ -388,20 +388,20 @@
             }, function(e, t, n) {
                 var a = n(24),
                     r = n(2)("toStringTag"),
                     o = "Arguments" == a(function() {
                         return arguments
                     }());
                 e.exports = function(e) {
-                    var t, n, i;
+                    var t, n, s;
                     return void 0 === e ? "Undefined" : null === e ? "Null" : "string" == typeof(n = function(e, t) {
                         try {
                             return e[t]
                         } catch (e) {}
-                    }(t = Object(e), r)) ? n : o ? a(t) : "Object" == (i = a(t)) && "function" == typeof t.callee ? "Arguments" : i
+                    }(t = Object(e), r)) ? n : o ? a(t) : "Object" == (s = a(t)) && "function" == typeof t.callee ? "Arguments" : s
                 }
             }, function(e, t) {
                 var n;
                 n = function() {
                     return this
                 }();
                 try {
@@ -416,53 +416,53 @@
                     return e.match(n)
                 }
             }, function(e, t, n) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.getBase16Theme = t.createStyling = t.invertTheme = void 0;
-                var a = f(n(49)),
-                    r = f(n(76)),
-                    o = f(n(81)),
-                    i = f(n(89)),
-                    s = f(n(93)),
+                var a = d(n(49)),
+                    r = d(n(76)),
+                    o = d(n(81)),
+                    s = d(n(89)),
+                    i = d(n(93)),
                     c = function(e) {
                         if (e && e.__esModule) return e;
                         var t = {};
                         if (null != e)
                             for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && (t[n] = e[n]);
                         return t.default = e, t
                     }(n(94)),
-                    l = f(n(132)),
-                    u = f(n(133)),
-                    p = f(n(138)),
-                    d = n(139);
+                    l = d(n(132)),
+                    u = d(n(133)),
+                    p = d(n(138)),
+                    f = n(139);
 
-                function f(e) {
+                function d(e) {
                     return e && e.__esModule ? e : {
                         default: e
                     }
                 }
                 var b = c.default,
-                    h = (0, i.default)(b),
-                    v = (0, p.default)(u.default, d.rgb2yuv, function(e) {
+                    h = (0, s.default)(b),
+                    v = (0, p.default)(u.default, f.rgb2yuv, function(e) {
                         var t = (0, o.default)(e, 3),
                             n = t[0];
                         return [n < .25 ? 1 : n < .5 ? .9 - n : 1.1 - n, t[1], t[2]]
-                    }, d.yuv2rgb, l.default),
+                    }, f.yuv2rgb, l.default),
                     m = function(e) {
                         return function(t) {
                             return {
                                 className: [t.className, e.className].filter(Boolean).join(" "),
                                 style: (0, r.default)({}, t.style || {}, e.style || {})
                             }
                         }
                     },
                     y = function(e, t) {
-                        var n = (0, i.default)(t);
+                        var n = (0, s.default)(t);
                         for (var o in e) - 1 === n.indexOf(o) && n.push(o);
                         return n.reduce(function(n, o) {
                             return n[o] = function(e, t) {
                                 if (void 0 === e) return t;
                                 if (void 0 === t) return e;
                                 var n = void 0 === e ? "undefined" : (0, a.default)(e),
                                     o = void 0 === t ? "undefined" : (0, a.default)(t);
@@ -524,122 +524,122 @@
                                                 }
                                         }
                                 }
                             }(e[o], t[o]), n
                         }, {})
                     },
                     g = function(e, t) {
-                        for (var n = arguments.length, o = Array(n > 2 ? n - 2 : 0), s = 2; s < n; s++) o[s - 2] = arguments[s];
+                        for (var n = arguments.length, o = Array(n > 2 ? n - 2 : 0), i = 2; i < n; i++) o[i - 2] = arguments[i];
                         if (null === t) return e;
                         Array.isArray(t) || (t = [t]);
                         var c = t.map(function(t) {
                             return e[t]
                         }).filter(Boolean).reduce(function(e, t) {
                             return "string" == typeof t ? e.className = [e.className, t].filter(Boolean).join(" ") : "object" === (void 0 === t ? "undefined" : (0, a.default)(t)) ? e.style = (0, r.default)({}, e.style, t) : "function" == typeof t && (e = (0, r.default)({}, e, t.apply(void 0, [e].concat(o)))), e
                         }, {
                             className: "",
                             style: {}
                         });
-                        return c.className || delete c.className, 0 === (0, i.default)(c.style).length && delete c.style, c
+                        return c.className || delete c.className, 0 === (0, s.default)(c.style).length && delete c.style, c
                     },
                     E = t.invertTheme = function(e) {
-                        return (0, i.default)(e).reduce(function(t, n) {
+                        return (0, s.default)(e).reduce(function(t, n) {
                             return t[n] = /^base/.test(n) ? v(e[n]) : "scheme" === n ? e[n] + ":inverted" : e[n], t
                         }, {})
                     },
-                    j = (t.createStyling = (0, s.default)(function(e) {
+                    j = (t.createStyling = (0, i.default)(function(e) {
                         for (var t = arguments.length, n = Array(t > 3 ? t - 3 : 0), a = 3; a < t; a++) n[a - 3] = arguments[a];
                         var o = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {},
                             c = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {},
                             l = o.defaultBase16,
                             u = void 0 === l ? b : l,
                             p = o.base16Themes,
-                            d = j(c, void 0 === p ? null : p);
-                        d && (c = (0, r.default)({}, d, c));
-                        var f = h.reduce(function(e, t) {
+                            f = j(c, void 0 === p ? null : p);
+                        f && (c = (0, r.default)({}, f, c));
+                        var d = h.reduce(function(e, t) {
                                 return e[t] = c[t] || u[t], e
                             }, {}),
-                            v = y((0, i.default)(c).reduce(function(e, t) {
+                            v = y((0, s.default)(c).reduce(function(e, t) {
                                 return -1 === h.indexOf(t) && (e[t] = c[t]), e
-                            }, {}), e(f));
-                        return (0, s.default)(g, 2).apply(void 0, [v].concat(n))
+                            }, {}), e(d));
+                        return (0, i.default)(g, 2).apply(void 0, [v].concat(n))
                     }, 3), t.getBase16Theme = function(e, t) {
                         if (e && e.extend && (e = e.extend), "string" == typeof e) {
                             var n = e.split(":"),
                                 a = (0, o.default)(n, 2),
                                 r = a[0],
-                                i = a[1];
-                            e = (t || {})[r] || c[r], "inverted" === i && (e = E(e))
+                                s = a[1];
+                            e = (t || {})[r] || c[r], "inverted" === s && (e = E(e))
                         }
                         return e && e.hasOwnProperty("base00") ? e : void 0
                     })
             }, function(e, t, n) {
                 "use strict";
                 var a, r = "object" == typeof Reflect ? Reflect : null,
                     o = r && "function" == typeof r.apply ? r.apply : function(e, t, n) {
                         return Function.prototype.apply.call(e, t, n)
                     };
                 a = r && "function" == typeof r.ownKeys ? r.ownKeys : Object.getOwnPropertySymbols ? function(e) {
                     return Object.getOwnPropertyNames(e).concat(Object.getOwnPropertySymbols(e))
                 } : function(e) {
                     return Object.getOwnPropertyNames(e)
                 };
-                var i = Number.isNaN || function(e) {
+                var s = Number.isNaN || function(e) {
                     return e != e
                 };
 
-                function s() {
-                    s.init.call(this)
+                function i() {
+                    i.init.call(this)
                 }
-                e.exports = s, e.exports.once = function(e, t) {
+                e.exports = i, e.exports.once = function(e, t) {
                     return new Promise(function(n, a) {
                         var r;
 
                         function o() {
                             void 0 !== r && e.removeListener("error", r), n([].slice.call(arguments))
                         }
                         "error" !== t && (r = function(n) {
                             e.removeListener(t, o), a(n)
                         }, e.once("error", r)), e.once(t, o)
                     })
-                }, s.EventEmitter = s, s.prototype._events = void 0, s.prototype._eventsCount = 0, s.prototype._maxListeners = void 0;
+                }, i.EventEmitter = i, i.prototype._events = void 0, i.prototype._eventsCount = 0, i.prototype._maxListeners = void 0;
                 var c = 10;
 
                 function l(e) {
                     if ("function" != typeof e) throw TypeError('The "listener" argument must be of type Function. Received type ' + typeof e)
                 }
 
                 function u(e) {
-                    return void 0 === e._maxListeners ? s.defaultMaxListeners : e._maxListeners
+                    return void 0 === e._maxListeners ? i.defaultMaxListeners : e._maxListeners
                 }
 
                 function p(e, t, n, a) {
-                    var r, o, i;
-                    if (l(n), void 0 === (o = e._events) ? (o = e._events = Object.create(null), e._eventsCount = 0) : (void 0 !== o.newListener && (e.emit("newListener", t, n.listener ? n.listener : n), o = e._events), i = o[t]), void 0 === i) i = o[t] = n, ++e._eventsCount;
-                    else if ("function" == typeof i ? i = o[t] = a ? [n, i] : [i, n] : a ? i.unshift(n) : i.push(n), (r = u(e)) > 0 && i.length > r && !i.warned) {
-                        i.warned = !0;
-                        var s = Error("Possible EventEmitter memory leak detected. " + i.length + " " + String(t) + " listeners added. Use emitter.setMaxListeners() to increase limit");
-                        s.name = "MaxListenersExceededWarning", s.emitter = e, s.type = t, s.count = i.length, console && console.warn && console.warn(s)
+                    var r, o, s;
+                    if (l(n), void 0 === (o = e._events) ? (o = e._events = Object.create(null), e._eventsCount = 0) : (void 0 !== o.newListener && (e.emit("newListener", t, n.listener ? n.listener : n), o = e._events), s = o[t]), void 0 === s) s = o[t] = n, ++e._eventsCount;
+                    else if ("function" == typeof s ? s = o[t] = a ? [n, s] : [s, n] : a ? s.unshift(n) : s.push(n), (r = u(e)) > 0 && s.length > r && !s.warned) {
+                        s.warned = !0;
+                        var i = Error("Possible EventEmitter memory leak detected. " + s.length + " " + String(t) + " listeners added. Use emitter.setMaxListeners() to increase limit");
+                        i.name = "MaxListenersExceededWarning", i.emitter = e, i.type = t, i.count = s.length, console && console.warn && console.warn(i)
                     }
                     return e
                 }
 
-                function d() {
+                function f() {
                     if (!this.fired) return this.target.removeListener(this.type, this.wrapFn), this.fired = !0, 0 == arguments.length ? this.listener.call(this.target) : this.listener.apply(this.target, arguments)
                 }
 
-                function f(e, t, n) {
+                function d(e, t, n) {
                     var a = {
                             fired: !1,
                             wrapFn: void 0,
                             target: e,
                             type: t,
                             listener: n
                         },
-                        r = d.bind(a);
+                        r = f.bind(a);
                     return r.listener = n, a.wrapFn = r, r
                 }
 
                 function b(e, t, n) {
                     var a = e._events;
                     if (void 0 === a) return [];
                     var r = a[t];
@@ -659,112 +659,112 @@
                     return 0
                 }
 
                 function v(e, t) {
                     for (var n = Array(t), a = 0; a < t; ++a) n[a] = e[a];
                     return n
                 }
-                Object.defineProperty(s, "defaultMaxListeners", {
+                Object.defineProperty(i, "defaultMaxListeners", {
                     enumerable: !0,
                     get: function() {
                         return c
                     },
                     set: function(e) {
-                        if ("number" != typeof e || e < 0 || i(e)) throw RangeError('The value of "defaultMaxListeners" is out of range. It must be a non-negative number. Received ' + e + ".");
+                        if ("number" != typeof e || e < 0 || s(e)) throw RangeError('The value of "defaultMaxListeners" is out of range. It must be a non-negative number. Received ' + e + ".");
                         c = e
                     }
-                }), s.init = function() {
+                }), i.init = function() {
                     void 0 !== this._events && this._events !== Object.getPrototypeOf(this)._events || (this._events = Object.create(null), this._eventsCount = 0), this._maxListeners = this._maxListeners || void 0
-                }, s.prototype.setMaxListeners = function(e) {
-                    if ("number" != typeof e || e < 0 || i(e)) throw RangeError('The value of "n" is out of range. It must be a non-negative number. Received ' + e + ".");
+                }, i.prototype.setMaxListeners = function(e) {
+                    if ("number" != typeof e || e < 0 || s(e)) throw RangeError('The value of "n" is out of range. It must be a non-negative number. Received ' + e + ".");
                     return this._maxListeners = e, this
-                }, s.prototype.getMaxListeners = function() {
+                }, i.prototype.getMaxListeners = function() {
                     return u(this)
-                }, s.prototype.emit = function(e) {
+                }, i.prototype.emit = function(e) {
                     for (var t = [], n = 1; n < arguments.length; n++) t.push(arguments[n]);
                     var a = "error" === e,
                         r = this._events;
                     if (void 0 !== r) a = a && void 0 === r.error;
                     else if (!a) return !1;
                     if (a) {
-                        if (t.length > 0 && (i = t[0]), i instanceof Error) throw i;
-                        var i, s = Error("Unhandled error." + (i ? " (" + i.message + ")" : ""));
-                        throw s.context = i, s
+                        if (t.length > 0 && (s = t[0]), s instanceof Error) throw s;
+                        var s, i = Error("Unhandled error." + (s ? " (" + s.message + ")" : ""));
+                        throw i.context = s, i
                     }
                     var c = r[e];
                     if (void 0 === c) return !1;
                     if ("function" == typeof c) o(c, this, t);
                     else {
                         var l = c.length,
                             u = v(c, l);
                         for (n = 0; n < l; ++n) o(u[n], this, t)
                     }
                     return !0
-                }, s.prototype.addListener = function(e, t) {
+                }, i.prototype.addListener = function(e, t) {
                     return p(this, e, t, !1)
-                }, s.prototype.on = s.prototype.addListener, s.prototype.prependListener = function(e, t) {
+                }, i.prototype.on = i.prototype.addListener, i.prototype.prependListener = function(e, t) {
                     return p(this, e, t, !0)
-                }, s.prototype.once = function(e, t) {
-                    return l(t), this.on(e, f(this, e, t)), this
-                }, s.prototype.prependOnceListener = function(e, t) {
-                    return l(t), this.prependListener(e, f(this, e, t)), this
-                }, s.prototype.removeListener = function(e, t) {
-                    var n, a, r, o, i;
+                }, i.prototype.once = function(e, t) {
+                    return l(t), this.on(e, d(this, e, t)), this
+                }, i.prototype.prependOnceListener = function(e, t) {
+                    return l(t), this.prependListener(e, d(this, e, t)), this
+                }, i.prototype.removeListener = function(e, t) {
+                    var n, a, r, o, s;
                     if (l(t), void 0 === (a = this._events) || void 0 === (n = a[e])) return this;
                     if (n === t || n.listener === t) 0 == --this._eventsCount ? this._events = Object.create(null) : (delete a[e], a.removeListener && this.emit("removeListener", e, n.listener || t));
                     else if ("function" != typeof n) {
                         for (r = -1, o = n.length - 1; o >= 0; o--)
                             if (n[o] === t || n[o].listener === t) {
-                                i = n[o].listener, r = o;
+                                s = n[o].listener, r = o;
                                 break
                             } if (r < 0) return this;
                         0 === r ? n.shift() : function(e, t) {
                             for (; t + 1 < e.length; t++) e[t] = e[t + 1];
                             e.pop()
-                        }(n, r), 1 === n.length && (a[e] = n[0]), void 0 !== a.removeListener && this.emit("removeListener", e, i || t)
+                        }(n, r), 1 === n.length && (a[e] = n[0]), void 0 !== a.removeListener && this.emit("removeListener", e, s || t)
                     }
                     return this
-                }, s.prototype.off = s.prototype.removeListener, s.prototype.removeAllListeners = function(e) {
+                }, i.prototype.off = i.prototype.removeListener, i.prototype.removeAllListeners = function(e) {
                     var t, n, a;
                     if (void 0 === (n = this._events)) return this;
                     if (void 0 === n.removeListener) return 0 == arguments.length ? (this._events = Object.create(null), this._eventsCount = 0) : void 0 !== n[e] && (0 == --this._eventsCount ? this._events = Object.create(null) : delete n[e]), this;
                     if (0 == arguments.length) {
                         var r, o = Object.keys(n);
                         for (a = 0; a < o.length; ++a) "removeListener" !== (r = o[a]) && this.removeAllListeners(r);
                         return this.removeAllListeners("removeListener"), this._events = Object.create(null), this._eventsCount = 0, this
                     }
                     if ("function" == typeof(t = n[e])) this.removeListener(e, t);
                     else if (void 0 !== t)
                         for (a = t.length - 1; a >= 0; a--) this.removeListener(e, t[a]);
                     return this
-                }, s.prototype.listeners = function(e) {
+                }, i.prototype.listeners = function(e) {
                     return b(this, e, !0)
-                }, s.prototype.rawListeners = function(e) {
+                }, i.prototype.rawListeners = function(e) {
                     return b(this, e, !1)
-                }, s.listenerCount = function(e, t) {
+                }, i.listenerCount = function(e, t) {
                     return "function" == typeof e.listenerCount ? e.listenerCount(t) : h.call(e, t)
-                }, s.prototype.listenerCount = h, s.prototype.eventNames = function() {
+                }, i.prototype.listenerCount = h, i.prototype.eventNames = function() {
                     return this._eventsCount > 0 ? a(this._events) : []
                 }
             }, function(e, t, n) {
                 e.exports.Dispatcher = n(140)
             }, function(e, t, n) {
                 e.exports = n(142)
             }, function(e, t, n) {
                 "use strict";
                 t.__esModule = !0;
-                var a = i(n(50)),
-                    r = i(n(65)),
+                var a = s(n(50)),
+                    r = s(n(65)),
                     o = "function" == typeof r.default && "symbol" == typeof a.default ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof r.default && e.constructor === r.default && e !== r.default.prototype ? "symbol" : typeof e
                     };
 
-                function i(e) {
+                function s(e) {
                     return e && e.__esModule ? e : {
                         default: e
                     }
                 }
                 t.default = "function" == typeof r.default && "symbol" === o(a.default) ? function(e) {
                     return void 0 === e ? "undefined" : o(e)
                 } : function(e) {
@@ -778,18 +778,18 @@
             }, function(e, t, n) {
                 n(20), n(29), e.exports = n(30).f("iterator")
             }, function(e, t, n) {
                 var a = n(21),
                     r = n(22);
                 e.exports = function(e) {
                     return function(t, n) {
-                        var o, i, s = String(r(t)),
+                        var o, s, i = String(r(t)),
                             c = a(n),
-                            l = s.length;
-                        return c < 0 || c >= l ? e ? "" : void 0 : (o = s.charCodeAt(c)) < 55296 || o > 56319 || c + 1 === l || (i = s.charCodeAt(c + 1)) < 56320 || i > 57343 ? e ? s.charAt(c) : o : e ? s.slice(c, c + 2) : i - 56320 + (o - 55296 << 10) + 65536
+                            l = i.length;
+                        return c < 0 || c >= l ? e ? "" : void 0 : (o = i.charCodeAt(c)) < 55296 || o > 56319 || c + 1 === l || (s = i.charCodeAt(c + 1)) < 56320 || s > 57343 ? e ? i.charAt(c) : o : e ? i.slice(c, c + 2) : s - 56320 + (o - 55296 << 10) + 65536
                     }
                 }
             }, function(e, t, n) {
                 var a = n(54);
                 e.exports = function(e, t, n) {
                     if (a(e), void 0 === t) return e;
                     switch (n) {
@@ -816,43 +816,43 @@
                     return e
                 }
             }, function(e, t, n) {
                 "use strict";
                 var a = n(38),
                     r = n(16),
                     o = n(28),
-                    i = {};
-                n(6)(i, n(2)("iterator"), function() {
+                    s = {};
+                n(6)(s, n(2)("iterator"), function() {
                     return this
                 }), e.exports = function(e, t, n) {
-                    e.prototype = a(i, {
+                    e.prototype = a(s, {
                         next: r(1, n)
                     }), o(e, t + " Iterator")
                 }
             }, function(e, t, n) {
                 var a = n(7),
                     r = n(10),
                     o = n(13);
                 e.exports = n(4) ? Object.defineProperties : function(e, t) {
                     r(e);
-                    for (var n, i = o(t), s = i.length, c = 0; s > c;) a.f(e, n = i[c++], t[n]);
+                    for (var n, s = o(t), i = s.length, c = 0; i > c;) a.f(e, n = s[c++], t[n]);
                     return e
                 }
             }, function(e, t, n) {
                 var a = n(9),
                     r = n(58),
                     o = n(59);
                 e.exports = function(e) {
-                    return function(t, n, i) {
-                        var s, c = a(t),
+                    return function(t, n, s) {
+                        var i, c = a(t),
                             l = r(c.length),
-                            u = o(i, l);
+                            u = o(s, l);
                         if (e && n != n) {
                             for (; l > u;)
-                                if ((s = c[u++]) != s) return !0
+                                if ((i = c[u++]) != i) return !0
                         } else
                             for (; l > u; u++)
                                 if ((e || u in c) && c[u] === n) return e || u || 0;
                         return !e && -1
                     }
                 }
             }, function(e, t, n) {
@@ -871,26 +871,26 @@
             }, function(e, t, n) {
                 var a = n(3).document;
                 e.exports = a && a.documentElement
             }, function(e, t, n) {
                 var a = n(5),
                     r = n(18),
                     o = n(25)("IE_PROTO"),
-                    i = Object.prototype;
+                    s = Object.prototype;
                 e.exports = Object.getPrototypeOf || function(e) {
-                    return a(e = r(e), o) ? e[o] : "function" == typeof e.constructor && e instanceof e.constructor ? e.constructor.prototype : e instanceof Object ? i : null
+                    return a(e = r(e), o) ? e[o] : "function" == typeof e.constructor && e instanceof e.constructor ? e.constructor.prototype : e instanceof Object ? s : null
                 }
             }, function(e, t, n) {
                 "use strict";
                 var a = n(63),
                     r = n(64),
                     o = n(12),
-                    i = n(9);
+                    s = n(9);
                 e.exports = n(34)(Array, "Array", function(e, t) {
-                    this._t = i(e), this._i = 0, this._k = t
+                    this._t = s(e), this._i = 0, this._k = t
                 }, function() {
                     var e = this._t,
                         t = this._k,
                         n = this._i++;
                     return !e || n >= e.length ? (this._t = void 0, r(1)) : r(0, "keys" == t ? n : "values" == t ? e[n] : [n, e[n]])
                 }, "values"), o.Arguments = o.Array, a("keys"), a("values"), a("entries")
             }, function(e, t) {
@@ -910,22 +910,22 @@
             }, function(e, t, n) {
                 n(67), n(73), n(74), n(75), e.exports = n(1).Symbol
             }, function(e, t, n) {
                 "use strict";
                 var a = n(3),
                     r = n(5),
                     o = n(4),
-                    i = n(15),
-                    s = n(37),
+                    s = n(15),
+                    i = n(37),
                     c = n(68).KEY,
                     l = n(8),
                     u = n(26),
                     p = n(28),
-                    d = n(17),
-                    f = n(2),
+                    f = n(17),
+                    d = n(2),
                     b = n(30),
                     h = n(31),
                     v = n(69),
                     m = n(70),
                     y = n(10),
                     g = n(11),
                     E = n(18),
@@ -940,16 +940,16 @@
                     A = n(13),
                     M = C.f,
                     P = w.f,
                     F = O.f,
                     D = a.Symbol,
                     I = a.JSON,
                     R = I && I.stringify,
-                    L = f("_hidden"),
-                    B = f("toPrimitive"),
+                    L = d("_hidden"),
+                    B = d("toPrimitive"),
                     N = {}.propertyIsEnumerable,
                     z = u("symbol-registry"),
                     T = u("symbols"),
                     q = u("op-symbols"),
                     V = Object.prototype,
                     K = "function" == typeof D && !!S.f,
                     W = a.QObject,
@@ -996,69 +996,69 @@
                         }
                     },
                     X = function(e) {
                         for (var t, n = F(j(e)), a = [], o = 0; n.length > o;) r(T, t = n[o++]) || t == L || t == c || a.push(t);
                         return a
                     },
                     ee = function(e) {
-                        for (var t, n = e === V, a = F(n ? q : j(e)), o = [], i = 0; a.length > i;) r(T, t = a[i++]) && (!n || r(V, t)) && o.push(T[t]);
+                        for (var t, n = e === V, a = F(n ? q : j(e)), o = [], s = 0; a.length > s;) r(T, t = a[s++]) && (!n || r(V, t)) && o.push(T[t]);
                         return o
                     };
-                K || (s((D = function() {
+                K || (i((D = function() {
                     if (this instanceof D) throw TypeError("Symbol is not a constructor!");
-                    var e = d(arguments.length > 0 ? arguments[0] : void 0),
+                    var e = f(arguments.length > 0 ? arguments[0] : void 0),
                         t = function(n) {
                             this === V && t.call(q, n), r(this, L) && r(this[L], e) && (this[L][e] = !1), U(this, e, _(1, n))
                         };
                     return o && H && U(V, e, {
                         configurable: !0,
                         set: t
                     }), G(e)
                 }).prototype, "toString", function() {
                     return this._k
-                }), C.f = Z, w.f = $, n(41).f = O.f = X, n(19).f = Q, S.f = ee, o && !n(14) && s(V, "propertyIsEnumerable", Q, !0), b.f = function(e) {
-                    return G(f(e))
-                }), i(i.G + i.W + !K * i.F, {
+                }), C.f = Z, w.f = $, n(41).f = O.f = X, n(19).f = Q, S.f = ee, o && !n(14) && i(V, "propertyIsEnumerable", Q, !0), b.f = function(e) {
+                    return G(d(e))
+                }), s(s.G + s.W + !K * s.F, {
                     Symbol: D
                 });
-                for (var et = "hasInstance,isConcatSpreadable,iterator,match,replace,search,species,split,toPrimitive,toStringTag,unscopables".split(","), en = 0; et.length > en;) f(et[en++]);
-                for (var ea = A(f.store), er = 0; ea.length > er;) h(ea[er++]);
-                i(i.S + !K * i.F, "Symbol", {
+                for (var et = "hasInstance,isConcatSpreadable,iterator,match,replace,search,species,split,toPrimitive,toStringTag,unscopables".split(","), en = 0; et.length > en;) d(et[en++]);
+                for (var ea = A(d.store), er = 0; ea.length > er;) h(ea[er++]);
+                s(s.S + !K * s.F, "Symbol", {
                     for: function(e) {
                         return r(z, e += "") ? z[e] : z[e] = D(e)
                     },
                     keyFor: function(e) {
                         if (!Y(e)) throw TypeError(e + " is not a symbol!");
                         for (var t in z)
                             if (z[t] === e) return t
                     },
                     useSetter: function() {
                         H = !0
                     },
                     useSimple: function() {
                         H = !1
                     }
-                }), i(i.S + !K * i.F, "Object", {
+                }), s(s.S + !K * s.F, "Object", {
                     create: function(e, t) {
                         return void 0 === t ? k(e) : J(k(e), t)
                     },
                     defineProperty: $,
                     defineProperties: J,
                     getOwnPropertyDescriptor: Z,
                     getOwnPropertyNames: X,
                     getOwnPropertySymbols: ee
                 });
                 var eo = l(function() {
                     S.f(1)
                 });
-                i(i.S + i.F * eo, "Object", {
+                s(s.S + s.F * eo, "Object", {
                     getOwnPropertySymbols: function(e) {
                         return S.f(E(e))
                     }
-                }), I && i(i.S + i.F * (!K || l(function() {
+                }), I && s(s.S + s.F * (!K || l(function() {
                     var e = D();
                     return "[null]" != R([e]) || "{}" != R({
                         a: e
                     }) || "{}" != R(Object(e))
                 })), "JSON", {
                     stringify: function(e) {
                         for (var t, n, a = [e], r = 1; arguments.length > r;) a.push(arguments[r++]);
@@ -1067,26 +1067,26 @@
                         }), a[1] = t, R.apply(I, a)
                     }
                 }), D.prototype[B] || n(6)(D.prototype, B, D.prototype.valueOf), p(D, "Symbol"), p(Math, "Math", !0), p(a.JSON, "JSON", !0)
             }, function(e, t, n) {
                 var a = n(17)("meta"),
                     r = n(11),
                     o = n(5),
-                    i = n(7).f,
-                    s = 0,
+                    s = n(7).f,
+                    i = 0,
                     c = Object.isExtensible || function() {
                         return !0
                     },
                     l = !n(8)(function() {
                         return c(Object.preventExtensions({}))
                     }),
                     u = function(e) {
-                        i(e, a, {
+                        s(e, a, {
                             value: {
-                                i: "O" + ++s,
+                                i: "O" + ++i,
                                 w: {}
                             }
                         })
                     },
                     p = e.exports = {
                         KEY: a,
                         NEED: !1,
@@ -1115,49 +1115,49 @@
                 var a = n(13),
                     r = n(32),
                     o = n(19);
                 e.exports = function(e) {
                     var t = a(e),
                         n = r.f;
                     if (n)
-                        for (var i, s = n(e), c = o.f, l = 0; s.length > l;) c.call(e, i = s[l++]) && t.push(i);
+                        for (var s, i = n(e), c = o.f, l = 0; i.length > l;) c.call(e, s = i[l++]) && t.push(s);
                     return t
                 }
             }, function(e, t, n) {
                 var a = n(24);
                 e.exports = Array.isArray || function(e) {
                     return "Array" == a(e)
                 }
             }, function(e, t, n) {
                 var a = n(9),
                     r = n(41).f,
                     o = {}.toString,
-                    i = "object" == typeof window && window && Object.getOwnPropertyNames ? Object.getOwnPropertyNames(window) : [];
+                    s = "object" == typeof window && window && Object.getOwnPropertyNames ? Object.getOwnPropertyNames(window) : [];
                 e.exports.f = function(e) {
-                    return i && "[object Window]" == o.call(e) ? function(e) {
+                    return s && "[object Window]" == o.call(e) ? function(e) {
                         try {
                             return r(e)
                         } catch (e) {
-                            return i.slice()
+                            return s.slice()
                         }
                     }(e) : r(a(e))
                 }
             }, function(e, t, n) {
                 var a = n(19),
                     r = n(16),
                     o = n(9),
-                    i = n(23),
-                    s = n(5),
+                    s = n(23),
+                    i = n(5),
                     c = n(35),
                     l = Object.getOwnPropertyDescriptor;
                 t.f = n(4) ? l : function(e, t) {
-                    if (e = o(e), t = i(t, !0), c) try {
+                    if (e = o(e), t = s(t, !0), c) try {
                         return l(e, t)
                     } catch (e) {}
-                    if (s(e, t)) return r(!a.f.call(e, t), e[t])
+                    if (i(e, t)) return r(!a.f.call(e, t), e[t])
                 }
             }, function(e, t) {}, function(e, t, n) {
                 n(31)("asyncIterator")
             }, function(e, t, n) {
                 n(31)("observable")
             }, function(e, t, n) {
                 "use strict";
@@ -1186,29 +1186,29 @@
                     assign: n(80)
                 })
             }, function(e, t, n) {
                 "use strict";
                 var a = n(4),
                     r = n(13),
                     o = n(32),
-                    i = n(19),
-                    s = n(18),
+                    s = n(19),
+                    i = n(18),
                     c = n(40),
                     l = Object.assign;
                 e.exports = !l || n(8)(function() {
                     var e = {},
                         t = {},
                         n = Symbol(),
                         a = "abcdefghijklmnopqrst";
                     return e[n] = 7, a.split("").forEach(function(e) {
                         t[e] = e
                     }), 7 != l({}, e)[n] || Object.keys(l({}, t)).join("") != a
                 }) ? function(e, t) {
-                    for (var n = s(e), l = arguments.length, u = 1, p = o.f, d = i.f; l > u;)
-                        for (var f, b = c(arguments[u++]), h = p ? r(b).concat(p(b)) : r(b), v = h.length, m = 0; v > m;) f = h[m++], a && !d.call(b, f) || (n[f] = b[f]);
+                    for (var n = i(e), l = arguments.length, u = 1, p = o.f, f = s.f; l > u;)
+                        for (var d, b = c(arguments[u++]), h = p ? r(b).concat(p(b)) : r(b), v = h.length, m = 0; v > m;) d = h[m++], a && !f.call(b, d) || (n[d] = b[d]);
                     return n
                 } : l
             }, function(e, t, n) {
                 "use strict";
                 t.__esModule = !0;
                 var a = o(n(82)),
                     r = o(n(85));
@@ -1220,24 +1220,24 @@
                 }
                 t.default = function(e, t) {
                     if (Array.isArray(e)) return e;
                     if ((0, a.default)(Object(e))) return function(e, t) {
                         var n = [],
                             a = !0,
                             o = !1,
-                            i = void 0;
+                            s = void 0;
                         try {
-                            for (var s, c = (0, r.default)(e); !(a = (s = c.next()).done) && (n.push(s.value), !t || n.length !== t); a = !0);
+                            for (var i, c = (0, r.default)(e); !(a = (i = c.next()).done) && (n.push(i.value), !t || n.length !== t); a = !0);
                         } catch (e) {
-                            o = !0, i = e
+                            o = !0, s = e
                         } finally {
                             try {
                                 !a && c.return && c.return()
                             } finally {
-                                if (o) throw i
+                                if (o) throw s
                             }
                         }
                         return n
                     }(e, t);
                     throw TypeError("Invalid attempt to destructure non-iterable instance")
                 }
             }, function(e, t, n) {
@@ -1294,18 +1294,18 @@
                 })
             }, function(e, t, n) {
                 var a = n(15),
                     r = n(1),
                     o = n(8);
                 e.exports = function(e, t) {
                     var n = (r.Object || {})[e] || Object[e],
-                        i = {};
-                    i[e] = t(n), a(a.S + a.F * o(function() {
+                        s = {};
+                    s[e] = t(n), a(a.S + a.F * o(function() {
                         n(1)
-                    }), "Object", i)
+                    }), "Object", s)
                 }
             }, function(e, t, n) {
                 (function(t) {
                     var n = [
                             ["ary", 128],
                             ["bind", 1],
                             ["bindKey", 2],
@@ -1315,24 +1315,24 @@
                             ["partial", 32],
                             ["partialRight", 64],
                             ["rearg", 256]
                         ],
                         a = /^\s+|\s+$/g,
                         r = /\{(?:\n\/\* \[wrapped with .+\] \*\/)?\n?/,
                         o = /\{\n\/\* \[wrapped with (.+)\] \*/,
-                        i = /,? & /,
-                        s = /^[-+]0x[0-9a-f]+$/i,
+                        s = /,? & /,
+                        i = /^[-+]0x[0-9a-f]+$/i,
                         c = /^0b[01]+$/i,
                         l = /^\[object .+?Constructor\]$/,
                         u = /^0o[0-7]+$/i,
                         p = /^(?:0|[1-9]\d*)$/,
-                        d = parseInt,
-                        f = "object" == typeof t && t && t.Object === Object && t,
+                        f = parseInt,
+                        d = "object" == typeof t && t && t.Object === Object && t,
                         b = "object" == typeof self && self && self.Object === Object && self,
-                        h = f || b || Function("return this")();
+                        h = d || b || Function("return this")();
 
                     function v(e, t, n) {
                         switch (n.length) {
                             case 0:
                                 return e.call(t);
                             case 1:
                                 return e.call(t, n[0]);
@@ -1346,16 +1346,16 @@
 
                     function m(e) {
                         return e != e
                     }
 
                     function y(e, t) {
                         for (var n = -1, a = e.length, r = 0, o = []; ++n < a;) {
-                            var i = e[n];
-                            i !== t && "__lodash_placeholder__" !== i || (e[n] = "__lodash_placeholder__", o[r++] = n)
+                            var s = e[n];
+                            s !== t && "__lodash_placeholder__" !== s || (e[n] = "__lodash_placeholder__", o[r++] = n)
                         }
                         return o
                     }
                     var g, E, j, x = Function.prototype,
                         _ = Object.prototype,
                         k = h["__core-js_shared__"],
                         O = (g = /[^.]+$/.exec(k && k.keys && k.keys.IE_PROTO || "")) ? "Symbol(src)_1." + g : "",
@@ -1391,63 +1391,63 @@
                             }
                             var a = q(t = e.prototype) ? M(t) : {},
                                 r = e.apply(a, n);
                             return q(r) ? r : a
                         }
                     }
 
-                    function R(e, t, n, a, r, o, i, s, c, l) {
+                    function R(e, t, n, a, r, o, s, i, c, l) {
                         var u = 128 & t,
-                            d = 1 & t,
-                            f = 2 & t,
+                            f = 1 & t,
+                            d = 2 & t,
                             b = 24 & t,
                             v = 512 & t,
-                            m = f ? void 0 : I(e);
+                            m = d ? void 0 : I(e);
                         return function g() {
                             for (var E = arguments.length, j = Array(E), x = E; x--;) j[x] = arguments[x];
                             if (b) var _ = B(g),
                                 k = function(e, t) {
                                     for (var n = e.length, a = 0; n--;) e[n] === t && a++;
                                     return a
                                 }(j, _);
                             if (a && (j = function(e, t, n, a) {
-                                    for (var r = -1, o = e.length, i = n.length, s = -1, c = t.length, l = P(o - i, 0), u = Array(c + l), p = !a; ++s < c;) u[s] = t[s];
-                                    for (; ++r < i;)(p || r < o) && (u[n[r]] = e[r]);
-                                    for (; l--;) u[s++] = e[r++];
+                                    for (var r = -1, o = e.length, s = n.length, i = -1, c = t.length, l = P(o - s, 0), u = Array(c + l), p = !a; ++i < c;) u[i] = t[i];
+                                    for (; ++r < s;)(p || r < o) && (u[n[r]] = e[r]);
+                                    for (; l--;) u[i++] = e[r++];
                                     return u
                                 }(j, a, r, b)), o && (j = function(e, t, n, a) {
-                                    for (var r = -1, o = e.length, i = -1, s = n.length, c = -1, l = t.length, u = P(o - s, 0), p = Array(u + l), d = !a; ++r < u;) p[r] = e[r];
-                                    for (var f = r; ++c < l;) p[f + c] = t[c];
-                                    for (; ++i < s;)(d || r < o) && (p[f + n[i]] = e[r++]);
+                                    for (var r = -1, o = e.length, s = -1, i = n.length, c = -1, l = t.length, u = P(o - i, 0), p = Array(u + l), f = !a; ++r < u;) p[r] = e[r];
+                                    for (var d = r; ++c < l;) p[d + c] = t[c];
+                                    for (; ++s < i;)(f || r < o) && (p[d + n[s]] = e[r++]);
                                     return p
-                                }(j, o, i, b)), E -= k, b && E < l) {
+                                }(j, o, s, b)), E -= k, b && E < l) {
                                 var O = y(j, _);
-                                return L(e, t, R, g.placeholder, n, j, O, s, c, l - E)
+                                return L(e, t, R, g.placeholder, n, j, O, i, c, l - E)
                             }
-                            var C = d ? n : this,
-                                S = f ? C[e] : e;
-                            return E = j.length, s ? j = function(e, t) {
+                            var C = f ? n : this,
+                                S = d ? C[e] : e;
+                            return E = j.length, i ? j = function(e, t) {
                                 for (var n = e.length, a = F(t.length, n), r = function(e, t) {
                                         var n = -1,
                                             a = e.length;
                                         for (t || (t = Array(a)); ++n < a;) t[n] = e[n];
                                         return t
                                     }(e); a--;) {
-                                    var o, i = t[a];
-                                    e[a] = (o = null == (o = n) ? 9007199254740991 : o) && ("number" == typeof i || p.test(i)) && i > -1 && i % 1 == 0 && i < o ? r[i] : void 0
+                                    var o, s = t[a];
+                                    e[a] = (o = null == (o = n) ? 9007199254740991 : o) && ("number" == typeof s || p.test(s)) && s > -1 && s % 1 == 0 && s < o ? r[s] : void 0
                                 }
                                 return e
-                            }(j, s) : v && E > 1 && j.reverse(), u && c < E && (j.length = c), this && this !== h && this instanceof g && (S = m || I(S)), S.apply(C, j)
+                            }(j, i) : v && E > 1 && j.reverse(), u && c < E && (j.length = c), this && this !== h && this instanceof g && (S = m || I(S)), S.apply(C, j)
                         }
                     }
 
-                    function L(e, t, n, a, r, o, i, s, c, l) {
+                    function L(e, t, n, a, r, o, s, i, c, l) {
                         var u = 8 & t;
                         t |= u ? 32 : 64, 4 & (t &= ~(u ? 64 : 32)) || (t &= -4);
-                        var p = n(e, t, r, u ? o : void 0, u ? i : void 0, u ? void 0 : o, u ? void 0 : i, s, c, l);
+                        var p = n(e, t, r, u ? o : void 0, u ? s : void 0, u ? void 0 : o, u ? void 0 : s, i, c, l);
                         return p.placeholder = a, z(p, e, t)
                     }
 
                     function B(e) {
                         return e.placeholder
                     }
 
@@ -1468,61 +1468,61 @@
                                     return e + ""
                                 } catch (e) {}
                             }
                             return ""
                         }(a)) ? a : void 0
                     }
                     var z = D ? function(e, t, a) {
-                        var s, c, l, u, p, d, f = t + "";
+                        var i, c, l, u, p, f, d = t + "";
                         return D(e, "toString", {
                             configurable: !0,
                             enumerable: !1,
-                            value: (p = (u = (s = (c = f.match(o)) ? c[1].split(i) : [], function(e, t) {
+                            value: (p = (u = (i = (c = d.match(o)) ? c[1].split(s) : [], function(e, t) {
                                 for (var n = -1, a = e ? e.length : 0; ++n < a && !1 !== t(e[n], n, e););
                             }(n, function(e) {
                                 var t = "_." + e[0];
-                                !(a & e[1]) || (s ? s.length : 0) && function(e, t, n) {
+                                !(a & e[1]) || (i ? i.length : 0) && function(e, t, n) {
                                     if (t != t) return function(e, t, n, a) {
                                         for (var r = e.length, o = n + (a ? 1 : -1); a ? o-- : ++o < r;)
                                             if (t(e[o], o, e)) return o;
                                         return -1
                                     }(e, m, n);
                                     for (var a = n - 1, r = e.length; ++a < r;)
                                         if (e[a] === t) return a;
                                     return -1
-                                }(s, t, 0) > -1 || s.push(t)
-                            }), l = s.sort()).length) - 1, l[p] = (u > 1 ? "& " : "") + l[p], l = l.join(u > 2 ? ", " : " "), d = f.replace(r, "{\n/* [wrapped with " + l + "] */\n"), function() {
-                                return d
+                                }(i, t, 0) > -1 || i.push(t)
+                            }), l = i.sort()).length) - 1, l[p] = (u > 1 ? "& " : "") + l[p], l = l.join(u > 2 ? ", " : " "), f = d.replace(r, "{\n/* [wrapped with " + l + "] */\n"), function() {
+                                return f
                             })
                         })
                     } : function(e) {
                         return e
                     };
 
                     function T(e, t, n) {
-                        var a = function(e, t, n, a, r, o, i, s) {
+                        var a = function(e, t, n, a, r, o, s, i) {
                             var c = 2 & t;
                             if (!c && "function" != typeof e) throw TypeError("Expected a function");
                             var l = a ? a.length : 0;
-                            if (l || (t &= -97, a = r = void 0), i = void 0 === i ? i : P(V(i), 0), s = void 0 === s ? s : V(s), l -= r ? r.length : 0, 64 & t) {
+                            if (l || (t &= -97, a = r = void 0), s = void 0 === s ? s : P(V(s), 0), i = void 0 === i ? i : V(i), l -= r ? r.length : 0, 64 & t) {
                                 var u = a,
                                     p = r;
                                 a = r = void 0
                             }
-                            var d = [e, t, n, a, r, u, p, o, i, s];
-                            if (e = d[0], t = d[1], n = d[2], a = d[3], r = d[4], (s = d[9] = null == d[9] ? c ? 0 : e.length : P(d[9] - l, 0)) || !(24 & t) || (t &= -25), t && 1 != t) F = 8 == t || 16 == t ? (f = e, b = t, m = s, g = I(f), function e() {
+                            var f = [e, t, n, a, r, u, p, o, s, i];
+                            if (e = f[0], t = f[1], n = f[2], a = f[3], r = f[4], (i = f[9] = null == f[9] ? c ? 0 : e.length : P(f[9] - l, 0)) || !(24 & t) || (t &= -25), t && 1 != t) F = 8 == t || 16 == t ? (d = e, b = t, m = i, g = I(d), function e() {
                                 for (var t = arguments.length, n = Array(t), a = t, r = B(e); a--;) n[a] = arguments[a];
                                 var o = t < 3 && n[0] !== r && n[t - 1] !== r ? [] : y(n, r);
-                                return (t -= o.length) < m ? L(f, b, R, e.placeholder, void 0, n, o, void 0, void 0, m - t) : v(this && this !== h && this instanceof e ? g : f, this, n)
-                            }) : 32 != t && 33 != t || r.length ? R.apply(void 0, d) : (E = e, j = t, x = n, _ = a, k = 1 & j, O = I(E), function e() {
-                                for (var t = -1, n = arguments.length, a = -1, r = _.length, o = Array(r + n), i = this && this !== h && this instanceof e ? O : E; ++a < r;) o[a] = _[a];
+                                return (t -= o.length) < m ? L(d, b, R, e.placeholder, void 0, n, o, void 0, void 0, m - t) : v(this && this !== h && this instanceof e ? g : d, this, n)
+                            }) : 32 != t && 33 != t || r.length ? R.apply(void 0, f) : (E = e, j = t, x = n, _ = a, k = 1 & j, O = I(E), function e() {
+                                for (var t = -1, n = arguments.length, a = -1, r = _.length, o = Array(r + n), s = this && this !== h && this instanceof e ? O : E; ++a < r;) o[a] = _[a];
                                 for (; n--;) o[a++] = arguments[++t];
-                                return v(i, k ? x : this, o)
+                                return v(s, k ? x : this, o)
                             });
-                            else var f, b, m, g, E, j, x, _, k, O, C, S, w, A, M, F = (C = e, S = t, w = n, A = 1 & S, M = I(C), function e() {
+                            else var d, b, m, g, E, j, x, _, k, O, C, S, w, A, M, F = (C = e, S = t, w = n, A = 1 & S, M = I(C), function e() {
                                 return (this && this !== h && this instanceof e ? M : C).apply(A ? w : this, arguments)
                             });
                             return z(F, e, t)
                         }(e, 8, void 0, void 0, void 0, void 0, void 0, t = n ? void 0 : t);
                         return a.placeholder = T.placeholder, a
                     }
 
@@ -1538,15 +1538,15 @@
                                 if (q(e)) {
                                     var t, n = "function" == typeof e.valueOf ? e.valueOf() : e;
                                     e = q(n) ? n + "" : n
                                 }
                                 if ("string" != typeof e) return 0 === e ? e : +e;
                                 e = e.replace(a, "");
                                 var r = c.test(e);
-                                return r || u.test(e) ? d(e.slice(2), r ? 2 : 8) : s.test(e) ? NaN : +e
+                                return r || u.test(e) ? f(e.slice(2), r ? 2 : 8) : i.test(e) ? NaN : +e
                             }(t)) === 1 / 0 || t === -1 / 0 ? 17976931348623157e292 * (t < 0 ? -1 : 1) : t == t ? t : 0 : 0 === t ? t : 0,
                             r = n % 1;
                         return n == n ? r ? n - r : n : 0
                     }
                     T.placeholder = {}, e.exports = T
                 }).call(this, n(43))
             }, function(e, t, n) {
@@ -1556,30 +1556,30 @@
                     return e && e.__esModule ? e.default : e
                 }
                 t.__esModule = !0;
                 var r = n(95);
                 t.threezerotwofour = a(r);
                 var o = n(96);
                 t.apathy = a(o);
-                var i = n(97);
-                t.ashes = a(i);
-                var s = n(98);
-                t.atelierDune = a(s);
+                var s = n(97);
+                t.ashes = a(s);
+                var i = n(98);
+                t.atelierDune = a(i);
                 var c = n(99);
                 t.atelierForest = a(c);
                 var l = n(100);
                 t.atelierHeath = a(l);
                 var u = n(101);
                 t.atelierLakeside = a(u);
                 var p = n(102);
                 t.atelierSeaside = a(p);
-                var d = n(103);
-                t.bespin = a(d);
-                var f = n(104);
-                t.brewer = a(f);
+                var f = n(103);
+                t.bespin = a(f);
+                var d = n(104);
+                t.brewer = a(d);
                 var b = n(105);
                 t.bright = a(b);
                 var h = n(106);
                 t.chalk = a(h);
                 var v = n(107);
                 t.codeschool = a(v);
                 var m = n(108);
@@ -2455,28 +2455,28 @@
                     var t = 4 === e.length ? r(255 * e[3]) : "";
                     return "#" + r(e[0]) + r(e[1]) + r(e[2]) + t
                 }
             }, function(e, t, n) {
                 var a = n(134),
                     r = n(135),
                     o = n(136),
-                    i = n(137),
-                    s = {
+                    s = n(137),
+                    i = {
                         "#": r,
                         hsl: function(e) {
                             var t = a(e),
-                                n = i(t);
+                                n = s(t);
                             return 4 === t.length && n.push(t[3]), n
                         },
                         rgb: o
                     };
 
                 function c(e) {
-                    for (var t in s)
-                        if (0 === e.indexOf(t)) return s[t](e)
+                    for (var t in i)
+                        if (0 === e.indexOf(t)) return i[t](e)
                 }
                 c.rgb = o, c.hsl = a, c.hex = r, e.exports = c
             }, function(e, t, n) {
                 var a = n(44),
                     r = n(33);
 
                 function o(e, t) {
@@ -2517,55 +2517,55 @@
                     return t < 3 ? -1 != e.indexOf("%") ? Math.round(255 * r(parseInt(e, 10), 0, 100) / 100) : r(parseInt(e, 10), 0, 255) : r(parseFloat(e), 0, 1)
                 }
                 e.exports = function(e) {
                     return a(e).map(o)
                 }
             }, function(e, t) {
                 e.exports = function(e) {
-                    var t, n, a, r, o, i = e[0] / 360,
-                        s = e[1] / 100,
+                    var t, n, a, r, o, s = e[0] / 360,
+                        i = e[1] / 100,
                         c = e[2] / 100;
-                    if (0 == s) return [o = 255 * c, o, o];
-                    t = 2 * c - (n = c < .5 ? c * (1 + s) : c + s - c * s), r = [0, 0, 0];
-                    for (var l = 0; l < 3; l++)(a = i + -(1 / 3 * (l - 1))) < 0 && a++, a > 1 && a--, o = 6 * a < 1 ? t + 6 * (n - t) * a : 2 * a < 1 ? n : 3 * a < 2 ? t + (n - t) * (2 / 3 - a) * 6 : t, r[l] = 255 * o;
+                    if (0 == i) return [o = 255 * c, o, o];
+                    t = 2 * c - (n = c < .5 ? c * (1 + i) : c + i - c * i), r = [0, 0, 0];
+                    for (var l = 0; l < 3; l++)(a = s + -(1 / 3 * (l - 1))) < 0 && a++, a > 1 && a--, o = 6 * a < 1 ? t + 6 * (n - t) * a : 2 * a < 1 ? n : 3 * a < 2 ? t + (n - t) * (2 / 3 - a) * 6 : t, r[l] = 255 * o;
                     return r
                 }
             }, function(e, t, n) {
                 (function(t) {
                     var n = "object" == typeof t && t && t.Object === Object && t,
                         a = "object" == typeof self && self && self.Object === Object && self,
                         r = n || a || Function("return this")(),
                         o = Object.prototype,
-                        i = o.hasOwnProperty,
-                        s = o.toString,
+                        s = o.hasOwnProperty,
+                        i = o.toString,
                         c = r.Symbol,
                         l = o.propertyIsEnumerable,
                         u = c ? c.isConcatSpreadable : void 0,
                         p = Math.max;
 
-                    function d(e) {
+                    function f(e) {
                         var t, n, a, r, o, c;
-                        return v(e) || !!e && "object" == typeof e && null != (t = e) && "number" == typeof(n = t.length) && n > -1 && n % 1 == 0 && n <= 9007199254740991 && (o = typeof(r = a = t), "[object Function]" != (c = r && ("object" == o || "function" == o) ? s.call(a) : "") && "[object GeneratorFunction]" != c) && i.call(e, "callee") && (!l.call(e, "callee") || "[object Arguments]" == s.call(e)) || !!(u && e && e[u])
+                        return v(e) || !!e && "object" == typeof e && null != (t = e) && "number" == typeof(n = t.length) && n > -1 && n % 1 == 0 && n <= 9007199254740991 && (o = typeof(r = a = t), "[object Function]" != (c = r && ("object" == o || "function" == o) ? i.call(a) : "") && "[object GeneratorFunction]" != c) && s.call(e, "callee") && (!l.call(e, "callee") || "[object Arguments]" == i.call(e)) || !!(u && e && e[u])
                     }
-                    var f, b, h, v = Array.isArray,
+                    var d, b, h, v = Array.isArray,
                         m = (b = function(e) {
                             var t = (e = function e(t, n, a, r, o) {
-                                    var i = -1,
-                                        s = t.length;
-                                    for (a || (a = d), o || (o = []); ++i < s;) {
-                                        var c = t[i];
+                                    var s = -1,
+                                        i = t.length;
+                                    for (a || (a = f), o || (o = []); ++s < i;) {
+                                        var c = t[s];
                                         n > 0 && a(c) ? n > 1 ? e(c, n - 1, a, r, o) : function(e, t) {
                                             for (var n = -1, a = t.length, r = e.length; ++n < a;) e[r + n] = t[n];
                                             return e
                                         }(o, c) : r || (o[o.length] = c)
                                     }
                                     return o
                                 }(e, 1)).length,
                                 n = t;
-                            for (f && e.reverse(); n--;)
+                            for (d && e.reverse(); n--;)
                                 if ("function" != typeof e[n]) throw TypeError("Expected a function");
                             return function() {
                                 for (var n = 0, a = t ? e[n].apply(this, arguments) : arguments[0]; ++n < t;) a = e[n].call(this, a);
                                 return a
                             }
                         }, h = p(void 0 === h ? b.length - 1 : h, 0), function() {
                             for (var e = arguments, t = -1, n = p(e.length - h, 0), a = Array(n); ++t < n;) a[t] = e[h + t];
@@ -2591,16 +2591,16 @@
             }, function(e, t, n) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.yuv2rgb = function(e) {
                     var t, n, a, r = e[0],
                         o = e[1],
-                        i = e[2];
-                    return t = 1 * r + 0 * o + 1.13983 * i, n = 1 * r + -.39465 * o + -.5806 * i, a = 1 * r + 2.02311 * o + 0 * i, [255 * (t = Math.min(Math.max(0, t), 1)), 255 * (n = Math.min(Math.max(0, n), 1)), 255 * (a = Math.min(Math.max(0, a), 1))]
+                        s = e[2];
+                    return t = 1 * r + 0 * o + 1.13983 * s, n = 1 * r + -.39465 * o + -.5806 * s, a = 1 * r + 2.02311 * o + 0 * s, [255 * (t = Math.min(Math.max(0, t), 1)), 255 * (n = Math.min(Math.max(0, n), 1)), 255 * (a = Math.min(Math.max(0, a), 1))]
                 }, t.rgb2yuv = function(e) {
                     var t = e[0] / 255,
                         n = e[1] / 255,
                         a = e[2] / 255;
                     return [.299 * t + .587 * n + .114 * a, -.14713 * t + -.28886 * n + .436 * a, .615 * t + -.51499 * n + -.10001 * a]
                 }
             }, function(e, t, n) {
@@ -2650,21 +2650,21 @@
                         }, e
                     }();
                 e.exports = o
             }, function(e, t, n) {
                 "use strict";
                 var a = function(e) {};
                 e.exports = function(e, t) {
-                    for (var n, r = arguments.length, o = Array(r > 2 ? r - 2 : 0), i = 2; i < r; i++) o[i - 2] = arguments[i];
+                    for (var n, r = arguments.length, o = Array(r > 2 ? r - 2 : 0), s = 2; s < r; s++) o[s - 2] = arguments[s];
                     if (a(t), !e) {
                         if (void 0 === t) n = Error("Minified exception occurred; use the non-minified dev environment for the full error message and additional helpful warnings.");
                         else {
-                            var s = 0;
+                            var i = 0;
                             (n = Error(t.replace(/%s/g, function() {
-                                return String(o[s++])
+                                return String(o[i++])
                             }))).name = "Invariant Violation"
                         }
                         throw n.framesToPop = 1, n
                     }
                 }
             }, function(e, t, n) {
                 "use strict";
@@ -2698,23 +2698,23 @@
                     return e
                 }
 
                 function o(e, t) {
                     if (!(e instanceof t)) throw TypeError("Cannot call a class as a function")
                 }
 
-                function i(e, t) {
+                function s(e, t) {
                     for (var n = 0; n < t.length; n++) {
                         var a = t[n];
                         a.enumerable = a.enumerable || !1, a.configurable = !0, "value" in a && (a.writable = !0), Object.defineProperty(e, a.key, a)
                     }
                 }
 
-                function s(e, t, n) {
-                    return t && i(e.prototype, t), n && i(e, n), e
+                function i(e, t, n) {
+                    return t && s(e.prototype, t), n && s(e, n), e
                 }
 
                 function c(e, t) {
                     return (c = Object.setPrototypeOf || function(e, t) {
                         return e.__proto__ = t, e
                     })(e, t)
                 }
@@ -2740,20 +2740,20 @@
                     return (p = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                     })(e)
                 }
 
-                function d(e) {
+                function f(e) {
                     if (void 0 === e) throw ReferenceError("this hasn't been initialised - super() hasn't been called");
                     return e
                 }
 
-                function f(e) {
+                function d(e) {
                     var t = function() {
                         if ("undefined" == typeof Reflect || !Reflect.construct || Reflect.construct.sham) return !1;
                         if ("function" == typeof Proxy) return !0;
                         try {
                             return Date.prototype.toString.call(Reflect.construct(Date, [], function() {})), !0
                         } catch (e) {
                             return !1
@@ -2761,15 +2761,15 @@
                     }();
                     return function() {
                         var n, a, r = u(e);
                         if (t) {
                             var o = u(this).constructor;
                             a = Reflect.construct(r, arguments, o)
                         } else a = r.apply(this, arguments);
-                        return (n = a) && ("object" === p(n) || "function" == typeof n) ? n : d(this)
+                        return (n = a) && ("object" === p(n) || "function" == typeof n) ? n : f(this)
                     }
                 }
                 n.r(t);
                 var b = n(0),
                     h = n.n(b);
 
                 function v() {
@@ -2872,51 +2872,43 @@
                         base0B: "rgba(1, 1, 1, 0.8)",
                         base0C: "rgba(1, 1, 1, 0.8)",
                         base0D: "rgba(1, 1, 1, 0.8)",
                         base0E: "rgba(1, 1, 1, 0.8)",
                         base0F: "rgba(1, 1, 1, 0.8)"
                     },
                     k = {
-                        white: "#fff",
-                        black: "#000",
-                        transparent: "rgba(1, 1, 1, 0)",
                         globalFontFamily: "monospace",
                         globalCursor: "default",
-                        indentBlockWidth: "5px",
                         braceFontWeight: "bold",
                         braceCursor: "pointer",
                         ellipsisFontSize: "18px",
                         ellipsisLineHeight: "10px",
                         ellipsisCursor: "pointer",
                         keyMargin: "0px 5px",
                         keyLetterSpacing: "0.5px",
                         keyFontStyle: "none",
-                        keyBorderRadius: "3px",
-                        keyColonWeight: "bold",
                         keyVerticalAlign: "top",
                         keyOpacity: "0.85",
                         keyOpacityHover: "1",
                         keyValPaddingTop: "3px",
                         keyValPaddingBottom: "3px",
                         keyValPaddingRight: "5px",
                         keyValBorderLeft: "1px solid",
                         keyValBorderHover: "2px solid",
-                        keyValPaddingHover: "3px 5px 3px 4px",
                         pushedContentMarginLeft: "6px",
                         variableValuePaddingRight: "6px",
                         nullFontSize: "11px",
                         nullFontWeight: "bold",
                         nullPadding: "1px 2px",
                         nullBorderRadius: "3px",
                         nanFontSize: "11px",
                         nanFontWeight: "bold",
                         nanPadding: "1px 2px",
                         nanBorderRadius: "3px",
                         undefinedFontSize: "11px",
-                        undefinedFontWeight: "bold",
                         undefinedPadding: "1px 2px",
                         undefinedBorderRadius: "3px",
                         dataTypeFontSize: "11px",
                         dataTypeMarginRight: "4px",
                         datatypeOpacity: "0.8",
                         objectSizeBorderRadius: "3px",
                         objectSizeFontStyle: "italic",
@@ -3329,57 +3321,57 @@
                     var a;
                     return e || console.error("theme has not been set"), (a = x, !1 !== e && "none" !== e || (a = _), Object(O.createStyling)(C, {
                         defaultBase16: a
                     })(e))(t, n)
                 }
                 var w = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = (e.rjvId, e.type_name),
                                     n = e.displayDataTypes,
                                     a = e.theme;
                                 return n ? h.a.createElement("span", Object.assign({
                                     className: "data-type-label"
                                 }, S(a, "data-type-label")), t) : null
                             }
                         }]), n
                     }(h.a.PureComponent),
                     A = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props;
                                 return h.a.createElement("div", S(e.theme, "boolean"), h.a.createElement(w, Object.assign({
                                     type_name: "bool"
                                 }, e)), e.value ? "true" : "false")
                             }
                         }]), n
                     }(h.a.PureComponent),
                     M = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props;
                                 return h.a.createElement("div", S(e.theme, "date"), h.a.createElement(w, Object.assign({
                                     type_name: "date"
                                 }, e)), h.a.createElement("span", Object.assign({
                                     className: "date-value"
@@ -3392,20 +3384,20 @@
                                     minute: "2-digit"
                                 })))
                             }
                         }]), n
                     }(h.a.PureComponent),
                     P = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props;
                                 return h.a.createElement("div", S(e.theme, "float"), h.a.createElement(w, Object.assign({
                                     type_name: "float"
                                 }, e)), this.props.value)
                             }
@@ -3435,21 +3427,21 @@
                         throw TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                     }()
                 }
                 var R = n(46),
                     L = new(n(47)).Dispatcher,
                     B = new(function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             var e;
                             o(this, n);
-                            for (var a = arguments.length, i = Array(a), s = 0; s < a; s++) i[s] = arguments[s];
-                            return (e = t.call.apply(t, [this].concat(i))).objects = {}, e.set = function(t, n, a, r) {
+                            for (var a = arguments.length, s = Array(a), i = 0; i < a; i++) s[i] = arguments[i];
+                            return (e = t.call.apply(t, [this].concat(s))).objects = {}, e.set = function(t, n, a, r) {
                                 void 0 === e.objects[t] && (e.objects[t] = {}), void 0 === e.objects[t][n] && (e.objects[t][n] = {}), e.objects[t][n][a] = r
                             }, e.get = function(t, n, a, r) {
                                 return void 0 === e.objects[t] || void 0 === e.objects[t][n] || null == e.objects[t][n][a] ? r : e.objects[t][n][a]
                             }, e.handleAction = function(t) {
                                 var n = t.rjvId,
                                     a = t.data;
                                 switch (t.name) {
@@ -3474,17 +3466,17 @@
                                     case "ADD_VARIABLE_KEY_REQUEST":
                                         e.set(n, "action", "new-key-request", a), e.emit("add-key-request-" + n)
                                 }
                             }, e.updateSrc = function(t, n) {
                                 var a = n.name,
                                     r = n.namespace,
                                     o = n.new_value,
-                                    i = (n.existing_value, n.variable_removed);
+                                    s = (n.existing_value, n.variable_removed);
                                 r.shift();
-                                var s, c = e.get(t, "global", "src"),
+                                var i, c = e.get(t, "global", "src"),
                                     l = e.deepCopy(c, I(r)),
                                     u = l,
                                     p = function(e, t) {
                                         if ("undefined" == typeof Symbol || null == e[Symbol.iterator]) {
                                             if (Array.isArray(e) || (r = D(e))) {
                                                 r && (e = r);
                                                 var n = 0,
@@ -3503,78 +3495,78 @@
                                                         throw e
                                                     },
                                                     f: a
                                                 }
                                             }
                                             throw TypeError("Invalid attempt to iterate non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                                         }
-                                        var r, o, i = !0,
-                                            s = !1;
+                                        var r, o, s = !0,
+                                            i = !1;
                                         return {
                                             s: function() {
                                                 r = e[Symbol.iterator]()
                                             },
                                             n: function() {
                                                 var e = r.next();
-                                                return i = e.done, e
+                                                return s = e.done, e
                                             },
                                             e: function(e) {
-                                                s = !0, o = e
+                                                i = !0, o = e
                                             },
                                             f: function() {
                                                 try {
-                                                    i || null == r.return || r.return()
+                                                    s || null == r.return || r.return()
                                                 } finally {
-                                                    if (s) throw o
+                                                    if (i) throw o
                                                 }
                                             }
                                         }
                                     }(r);
                                 try {
-                                    for (p.s(); !(s = p.n()).done;) u = u[s.value]
+                                    for (p.s(); !(i = p.n()).done;) u = u[i.value]
                                 } catch (e) {
                                     p.e(e)
                                 } finally {
                                     p.f()
                                 }
-                                return i ? "array" == j(u) ? u.splice(a, 1) : delete u[a] : null !== a ? u[a] = o : l = o, e.set(t, "global", "src", l), l
+                                return s ? "array" == j(u) ? u.splice(a, 1) : delete u[a] : null !== a ? u[a] = o : l = o, e.set(t, "global", "src", l), l
                             }, e.deepCopy = function(t, n) {
                                 var a, o = j(t),
-                                    i = n.shift();
-                                return "array" == o ? a = I(t) : "object" == o && (a = r({}, t)), void 0 !== i && (a[i] = e.deepCopy(t[i], n)), a
+                                    s = n.shift();
+                                return "array" == o ? a = I(t) : "object" == o && (a = r({}, t)), void 0 !== s && (a[s] = e.deepCopy(t[s], n)), a
                             }, e
                         }
                         return n
                     }(R.EventEmitter));
                 L.register(B.handleAction.bind(B));
                 var N = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n(e) {
                             var a;
                             return o(this, n), (a = t.call(this, e)).toggleCollapsed = function() {
                                 a.setState({
                                     collapsed: !a.state.collapsed
                                 }, function() {
                                     B.set(a.props.rjvId, a.props.namespace, "collapsed", a.state.collapsed)
                                 })
                             }, a.getFunctionDisplay = function(e) {
-                                var t = d(a).props;
+                                var t = f(a).props;
                                 return e ? h.a.createElement("span", null, a.props.value.toString().slice(9, -1).replace(/\{[\s\S]+/, ""), h.a.createElement("span", {
                                     className: "function-collapsed",
                                     style: {
                                         fontWeight: "bold"
                                     }
                                 }, h.a.createElement("span", null, "{"), h.a.createElement("span", S(t.theme, "ellipsis"), "..."), h.a.createElement("span", null, "}"))) : a.props.value.toString().slice(9, -1)
                             }, a.state = {
                                 collapsed: B.get(e.rjvId, e.namespace, "collapsed", !0)
                             }, a
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = this.state.collapsed;
                                 return h.a.createElement("div", S(e.theme, "function"), h.a.createElement(w, Object.assign({
                                     type_name: "function"
                                 }, e)), h.a.createElement("span", Object.assign({}, S(e.theme, "function-value"), {
@@ -3582,91 +3574,91 @@
                                     onClick: this.toggleCollapsed
                                 }), this.getFunctionDisplay(t)))
                             }
                         }]), n
                     }(h.a.PureComponent),
                     z = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 return h.a.createElement("div", S(this.props.theme, "nan"), "NaN")
                             }
                         }]), n
                     }(h.a.PureComponent),
                     T = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 return h.a.createElement("div", S(this.props.theme, "null"), "NULL")
                             }
                         }]), n
                     }(h.a.PureComponent),
                     q = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props;
                                 return h.a.createElement("div", S(e.theme, "integer"), h.a.createElement(w, Object.assign({
                                     type_name: "int"
                                 }, e)), this.props.value)
                             }
                         }]), n
                     }(h.a.PureComponent),
                     V = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props;
                                 return h.a.createElement("div", S(e.theme, "regexp"), h.a.createElement(w, Object.assign({
                                     type_name: "regexp"
                                 }, e)), this.props.value.toString())
                             }
                         }]), n
                     }(h.a.PureComponent),
                     K = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n(e) {
                             var a;
                             return o(this, n), (a = t.call(this, e)).toggleCollapsed = function() {
                                 a.setState({
                                     collapsed: !a.state.collapsed
                                 }, function() {
                                     B.set(a.props.rjvId, a.props.namespace, "collapsed", a.state.collapsed)
                                 })
                             }, a.state = {
                                 collapsed: B.get(e.rjvId, e.namespace, "collapsed", !0)
                             }, a
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 this.state.collapsed;
                                 var e = this.props,
                                     t = e.collapseStringsAfterLength,
                                     n = e.theme,
                                     a = e.value,
@@ -3683,20 +3675,20 @@
                                     onClick: this.toggleCollapsed
                                 }), '"', a, '"'))
                             }
                         }]), n
                     }(h.a.PureComponent),
                     W = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 return h.a.createElement("div", S(this.props.theme, "undefined"), "undefined")
                             }
                         }]), n
                     }(h.a.PureComponent);
 
@@ -3745,32 +3737,32 @@
                     X = function() {},
                     ee = ["borderBottomWidth", "borderLeftWidth", "borderRightWidth", "borderTopWidth", "boxSizing", "fontFamily", "fontSize", "fontStyle", "fontWeight", "letterSpacing", "lineHeight", "paddingBottom", "paddingLeft", "paddingRight", "paddingTop", "tabSize", "textIndent", "textRendering", "textTransform", "width"],
                     et = !!document.documentElement.currentStyle,
                     en = Object(b.forwardRef)(function(e, t) {
                         var n, a = e.cacheMeasurements,
                             r = e.maxRows,
                             o = e.minRows,
-                            i = e.onChange,
-                            s = void 0 === i ? X : i,
+                            s = e.onChange,
+                            i = void 0 === s ? X : s,
                             c = e.onHeightChange,
                             l = void 0 === c ? X : c,
                             u = function(e, t) {
                                 if (null == e) return {};
                                 var n, a, r = {},
                                     o = Object.keys(e);
                                 for (a = 0; a < o.length; a++) t.indexOf(n = o[a]) >= 0 || (r[n] = e[n]);
                                 return r
                             }(e, ["cacheMeasurements", "maxRows", "minRows", "onChange", "onHeightChange"]),
                             p = void 0 !== u.value,
-                            d = Object(b.useRef)(null),
-                            f = $(d, t),
+                            f = Object(b.useRef)(null),
+                            d = $(f, t),
                             h = Object(b.useRef)(0),
                             v = Object(b.useRef)(),
                             m = function() {
-                                var e = d.current,
+                                var e = f.current,
                                     t = a && v.current ? v.current : function(e) {
                                         var t = window.getComputedStyle(e);
                                         if (null === t) return null;
                                         var n = ee.reduce(function(e, n) {
                                                 return e[n] = t[n], e
                                             }, {}),
                                             a = n.boxSizing;
@@ -3778,17 +3770,17 @@
                                             sizingStyle: n,
                                             paddingSize: parseFloat(n.paddingBottom) + parseFloat(n.paddingTop),
                                             borderSize: parseFloat(n.borderBottomWidth) + parseFloat(n.borderTopWidth)
                                         })
                                     }(e);
                                 if (t) {
                                     v.current = t;
-                                    var n, i, s, c, u, p, f, b, m, y, g, E, j = (n = e.value || e.placeholder || "x", void 0 === (i = o) && (i = 1), void 0 === (s = r) && (s = 1 / 0), Z || ((Z = document.createElement("textarea")).setAttribute("tab-index", "-1"), Z.setAttribute("aria-hidden", "true"), Q(Z)), null === Z.parentNode && document.body.appendChild(Z), c = t.paddingSize, u = t.borderSize, f = (p = t.sizingStyle).boxSizing, Object.keys(p).forEach(function(e) {
+                                    var n, s, i, c, u, p, d, b, m, y, g, E, j = (n = e.value || e.placeholder || "x", void 0 === (s = o) && (s = 1), void 0 === (i = r) && (i = 1 / 0), Z || ((Z = document.createElement("textarea")).setAttribute("tab-index", "-1"), Z.setAttribute("aria-hidden", "true"), Q(Z)), null === Z.parentNode && document.body.appendChild(Z), c = t.paddingSize, u = t.borderSize, d = (p = t.sizingStyle).boxSizing, Object.keys(p).forEach(function(e) {
                                             Z.style[e] = p[e]
-                                        }), Q(Z), Z.value = n, b = Z.scrollHeight, m = "border-box" === t.sizingStyle.boxSizing ? b + t.borderSize : b - t.paddingSize, Z.value = "x", g = (y = Z.scrollHeight - c) * i, "border-box" === f && (g = g + c + u), m = Math.max(g, m), E = y * s, "border-box" === f && (E = E + c + u), [m = Math.min(E, m), y]),
+                                        }), Q(Z), Z.value = n, b = Z.scrollHeight, m = "border-box" === t.sizingStyle.boxSizing ? b + t.borderSize : b - t.paddingSize, Z.value = "x", g = (y = Z.scrollHeight - c) * s, "border-box" === d && (g = g + c + u), m = Math.max(g, m), E = y * i, "border-box" === d && (E = E + c + u), [m = Math.min(E, m), y]),
                                         x = j[0],
                                         _ = j[1];
                                     h.current !== x && (h.current = x, e.style.setProperty("height", x + "px", "important"), l(x, {
                                         rowHeight: _
                                     }))
                                 }
                             };
@@ -3798,17 +3790,17 @@
                             };
                             return window.addEventListener("resize", e),
                                 function() {
                                     window.removeEventListener("resize", e)
                                 }
                         }, []), Object(b.createElement)("textarea", H({}, u, {
                             onChange: function(e) {
-                                p || m(), s(e)
+                                p || m(), i(e)
                             },
-                            ref: f
+                            ref: d
                         }))
                     });
 
                 function ea(e) {
                     e = e.trim();
                     try {
                         if ("[" === (e = JSON.stringify(JSON.parse(e)))[0]) return er("array", JSON.parse(e));
@@ -3839,20 +3831,20 @@
                     return {
                         type: e,
                         value: t
                     }
                 }
                 var eo = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     n = E(e, ["style"]);
                                 return h.a.createElement("span", n, h.a.createElement("svg", Object.assign({}, em(t), {
                                     viewBox: "0 0 24 24",
@@ -3860,22 +3852,22 @@
                                     preserveAspectRatio: "xMidYMid meet"
                                 }), h.a.createElement("path", {
                                     d: "M12,20C7.59,20 4,16.41 4,12C4,7.59 7.59,4 12,4C16.41,4 20,7.59 20,12C20,16.41 16.41,20 12,20M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M7,13H17V11H7"
                                 })))
                             }
                         }]), n
                     }(h.a.PureComponent),
-                    ei = function(e) {
+                    es = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     n = E(e, ["style"]);
                                 return h.a.createElement("span", n, h.a.createElement("svg", Object.assign({}, em(t), {
                                     viewBox: "0 0 24 24",
@@ -3883,22 +3875,22 @@
                                     preserveAspectRatio: "xMidYMid meet"
                                 }), h.a.createElement("path", {
                                     d: "M12,20C7.59,20 4,16.41 4,12C4,7.59 7.59,4 12,4C16.41,4 20,7.59 20,12C20,16.41 16.41,20 12,20M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2M13,7H11V11H7V13H11V17H13V13H17V11H13V7Z"
                                 })))
                             }
                         }]), n
                     }(h.a.PureComponent),
-                    es = function(e) {
+                    ei = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     n = E(e, ["style"]),
                                     a = em(t).style;
                                 return h.a.createElement("span", n, h.a.createElement("svg", {
@@ -3911,20 +3903,20 @@
                                     d: "M1344 800v64q0 14-9 23t-23 9h-832q-14 0-23-9t-9-23v-64q0-14 9-23t23-9h832q14 0 23 9t9 23zm128 448v-832q0-66-47-113t-113-47h-832q-66 0-113 47t-47 113v832q0 66 47 113t113 47h832q66 0 113-47t47-113zm128-832v832q0 119-84.5 203.5t-203.5 84.5h-832q-119 0-203.5-84.5t-84.5-203.5v-832q0-119 84.5-203.5t203.5-84.5h832q119 0 203.5 84.5t84.5 203.5z"
                                 })))
                             }
                         }]), n
                     }(h.a.PureComponent),
                     ec = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     n = E(e, ["style"]),
                                     a = em(t).style;
                                 return h.a.createElement("span", n, h.a.createElement("svg", {
@@ -3937,20 +3929,20 @@
                                     d: "M1344 800v64q0 14-9 23t-23 9h-352v352q0 14-9 23t-23 9h-64q-14 0-23-9t-9-23v-352h-352q-14 0-23-9t-9-23v-64q0-14 9-23t23-9h352v-352q0-14 9-23t23-9h64q14 0 23 9t9 23v352h352q14 0 23 9t9 23zm128 448v-832q0-66-47-113t-113-47h-832q-66 0-113 47t-47 113v832q0 66 47 113t113 47h832q66 0 113-47t47-113zm128-832v832q0 119-84.5 203.5t-203.5 84.5h-832q-119 0-203.5-84.5t-84.5-203.5v-832q0-119 84.5-203.5t203.5-84.5h832q119 0 203.5 84.5t84.5 203.5z"
                                 })))
                             }
                         }]), n
                     }(h.a.PureComponent),
                     el = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     n = E(e, ["style"]);
                                 return h.a.createElement("span", n, h.a.createElement("svg", {
                                     style: r(r({}, em(t).style), {}, {
@@ -3963,20 +3955,20 @@
                                     d: "M0 14l6-6-6-6z"
                                 })))
                             }
                         }]), n
                     }(h.a.PureComponent),
                     eu = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     n = E(e, ["style"]);
                                 return h.a.createElement("span", n, h.a.createElement("svg", {
                                     style: r(r({}, em(t).style), {}, {
@@ -3989,20 +3981,20 @@
                                     d: "M0 5l6 6 6-6z"
                                 })))
                             }
                         }]), n
                     }(h.a.PureComponent),
                     ep = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     n = E(e, ["style"]);
                                 return h.a.createElement("span", n, h.a.createElement("svg", Object.assign({}, em(t), {
                                     viewBox: "0 0 40 40",
@@ -4010,22 +4002,22 @@
                                     preserveAspectRatio: "xMidYMid meet"
                                 }), h.a.createElement("g", null, h.a.createElement("path", {
                                     d: "m30 35h-25v-22.5h25v7.5h2.5v-12.5c0-1.4-1.1-2.5-2.5-2.5h-7.5c0-2.8-2.2-5-5-5s-5 2.2-5 5h-7.5c-1.4 0-2.5 1.1-2.5 2.5v27.5c0 1.4 1.1 2.5 2.5 2.5h25c1.4 0 2.5-1.1 2.5-2.5v-5h-2.5v5z m-20-27.5h2.5s2.5-1.1 2.5-2.5 1.1-2.5 2.5-2.5 2.5 1.1 2.5 2.5 1.3 2.5 2.5 2.5h2.5s2.5 1.1 2.5 2.5h-20c0-1.5 1.1-2.5 2.5-2.5z m-2.5 20h5v-2.5h-5v2.5z m17.5-5v-5l-10 7.5 10 7.5v-5h12.5v-5h-12.5z m-17.5 10h7.5v-2.5h-7.5v2.5z m12.5-17.5h-12.5v2.5h12.5v-2.5z m-7.5 5h-5v2.5h5v-2.5z"
                                 }))))
                             }
                         }]), n
                     }(h.a.PureComponent),
-                    ed = function(e) {
+                    ef = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     n = E(e, ["style"]);
                                 return h.a.createElement("span", n, h.a.createElement("svg", Object.assign({}, em(t), {
                                     viewBox: "0 0 40 40",
@@ -4033,22 +4025,22 @@
                                     preserveAspectRatio: "xMidYMid meet"
                                 }), h.a.createElement("g", null, h.a.createElement("path", {
                                     d: "m28.6 25q0-0.5-0.4-1l-4-4 4-4q0.4-0.5 0.4-1 0-0.6-0.4-1.1l-2-2q-0.4-0.4-1-0.4-0.6 0-1 0.4l-4.1 4.1-4-4.1q-0.4-0.4-1-0.4-0.6 0-1 0.4l-2 2q-0.5 0.5-0.5 1.1 0 0.5 0.5 1l4 4-4 4q-0.5 0.5-0.5 1 0 0.7 0.5 1.1l2 2q0.4 0.4 1 0.4 0.6 0 1-0.4l4-4.1 4.1 4.1q0.4 0.4 1 0.4 0.6 0 1-0.4l2-2q0.4-0.4 0.4-1z m8.7-5q0 4.7-2.3 8.6t-6.3 6.2-8.6 2.3-8.6-2.3-6.2-6.2-2.3-8.6 2.3-8.6 6.2-6.2 8.6-2.3 8.6 2.3 6.3 6.2 2.3 8.6z"
                                 }))))
                             }
                         }]), n
                     }(h.a.PureComponent),
-                    ef = function(e) {
+                    ed = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     n = E(e, ["style"]);
                                 return h.a.createElement("span", n, h.a.createElement("svg", Object.assign({}, em(t), {
                                     viewBox: "0 0 40 40",
@@ -4058,20 +4050,20 @@
                                     d: "m30.1 21.4v-2.8q0-0.6-0.4-1t-1-0.5h-5.7v-5.7q0-0.6-0.4-1t-1-0.4h-2.9q-0.6 0-1 0.4t-0.4 1v5.7h-5.7q-0.6 0-1 0.5t-0.5 1v2.8q0 0.6 0.5 1t1 0.5h5.7v5.7q0 0.5 0.4 1t1 0.4h2.9q0.6 0 1-0.4t0.4-1v-5.7h5.7q0.6 0 1-0.5t0.4-1z m7.2-1.4q0 4.7-2.3 8.6t-6.3 6.2-8.6 2.3-8.6-2.3-6.2-6.2-2.3-8.6 2.3-8.6 6.2-6.2 8.6-2.3 8.6 2.3 6.3 6.2 2.3 8.6z"
                                 }))))
                             }
                         }]), n
                     }(h.a.PureComponent),
                     eb = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     n = E(e, ["style"]);
                                 return h.a.createElement("span", n, h.a.createElement("svg", Object.assign({}, em(t), {
                                     viewBox: "0 0 40 40",
@@ -4081,20 +4073,20 @@
                                     d: "m31.6 21.6h-10v10h-3.2v-10h-10v-3.2h10v-10h3.2v10h10v3.2z"
                                 }))))
                             }
                         }]), n
                     }(h.a.PureComponent),
                     eh = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     n = E(e, ["style"]);
                                 return h.a.createElement("span", n, h.a.createElement("svg", Object.assign({}, em(t), {
                                     viewBox: "0 0 40 40",
@@ -4104,20 +4096,20 @@
                                     d: "m19.8 26.4l2.6-2.6-3.4-3.4-2.6 2.6v1.3h2.2v2.1h1.2z m9.8-16q-0.3-0.4-0.7 0l-7.8 7.8q-0.4 0.4 0 0.7t0.7 0l7.8-7.8q0.4-0.4 0-0.7z m1.8 13.2v4.3q0 2.6-1.9 4.5t-4.5 1.9h-18.6q-2.6 0-4.5-1.9t-1.9-4.5v-18.6q0-2.7 1.9-4.6t4.5-1.8h18.6q1.4 0 2.6 0.5 0.3 0.2 0.4 0.5 0.1 0.4-0.2 0.7l-1.1 1.1q-0.3 0.3-0.7 0.1-0.5-0.1-1-0.1h-18.6q-1.4 0-2.5 1.1t-1 2.5v18.6q0 1.4 1 2.5t2.5 1h18.6q1.5 0 2.5-1t1.1-2.5v-2.9q0-0.2 0.2-0.4l1.4-1.5q0.3-0.3 0.8-0.1t0.4 0.6z m-2.1-16.5l6.4 6.5-15 15h-6.4v-6.5z m9.9 3l-2.1 2-6.4-6.4 2.1-2q0.6-0.7 1.5-0.7t1.5 0.7l3.4 3.4q0.6 0.6 0.6 1.5t-0.6 1.5z"
                                 }))))
                             }
                         }]), n
                     }(h.a.PureComponent),
                     ev = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.style,
                                     n = E(e, ["style"]);
                                 return h.a.createElement("span", n, h.a.createElement("svg", Object.assign({}, em(t), {
                                     viewBox: "0 0 40 40",
@@ -4139,15 +4131,15 @@
                             height: "1em",
                             width: "1em"
                         })
                     }
                 }
                 var ey = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n(e) {
                             var a;
                             return o(this, n), (a = t.call(this, e)).copiedTimer = null, a.handleCopy = function() {
                                 var e = document.createElement("textarea"),
                                     t = a.props,
                                     n = t.clickCallback,
@@ -4181,47 +4173,47 @@
                                     default:
                                         return e
                                 }
                             }, a.state = {
                                 copied: !1
                             }, a
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "componentWillUnmount",
                             value: function() {
                                 this.copiedTimer && (clearTimeout(this.copiedTimer), this.copiedTimer = null)
                             }
                         }, {
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = (e.src, e.theme),
                                     n = e.hidden,
                                     a = e.rowHovered,
                                     o = S(t, "copy-to-clipboard").style,
-                                    i = "inline";
-                                return n && (i = "none"), h.a.createElement("span", {
+                                    s = "inline";
+                                return n && (s = "none"), h.a.createElement("span", {
                                     className: "copy-to-clipboard-container",
                                     title: "Copy to clipboard",
                                     style: {
                                         verticalAlign: "top",
                                         display: a ? "inline-block" : "none"
                                     }
                                 }, h.a.createElement("span", {
                                     style: r(r({}, o), {}, {
-                                        display: i
+                                        display: s
                                     }),
                                     onClick: this.handleCopy
                                 }, this.getClippyIcon()))
                             }
                         }]), n
                     }(h.a.PureComponent),
                     eg = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n(e) {
                             var a;
                             return o(this, n), (a = t.call(this, e)).getEditIcon = function() {
                                 var e = a.props,
                                     t = e.variable,
                                     n = e.theme;
@@ -4284,15 +4276,15 @@
                                     o = e.rjvId;
                                 return h.a.createElement("div", {
                                     className: "click-to-remove",
                                     style: {
                                         verticalAlign: "top",
                                         display: a.state.hovered ? "inline-block" : "none"
                                     }
-                                }, h.a.createElement(ed, Object.assign({
+                                }, h.a.createElement(ef, Object.assign({
                                     className: "click-to-remove-icon"
                                 }, S(r, "removeVarIcon"), {
                                     onClick: function() {
                                         L.dispatch({
                                             name: "VARIABLE_REMOVED",
                                             rjvId: o,
                                             data: {
@@ -4302,15 +4294,15 @@
                                                 variable_removed: !0
                                             }
                                         })
                                     }
                                 })))
                             }, a.getValue = function(e, t) {
                                 var n = !t && e.type,
-                                    r = d(a).props;
+                                    r = f(a).props;
                                 switch (n) {
                                     case !1:
                                         return a.getEditInput();
                                     case "string":
                                         return h.a.createElement(K, Object.assign({
                                             value: e.value
                                         }, r));
@@ -4381,15 +4373,15 @@
                                             case "Enter":
                                                 (e.ctrlKey || e.metaKey) && a.submitEdit(!0)
                                         }
                                         e.stopPropagation()
                                     },
                                     placeholder: "update this value",
                                     minRows: 2
-                                }, S(e, "edit-input"))), h.a.createElement("div", S(e, "edit-icon-container"), h.a.createElement(ed, Object.assign({
+                                }, S(e, "edit-input"))), h.a.createElement("div", S(e, "edit-icon-container"), h.a.createElement(ef, Object.assign({
                                     className: "edit-cancel"
                                 }, S(e, "cancel-icon"), {
                                     onClick: function() {
                                         a.setState({
                                             editMode: !1,
                                             editValue: ""
                                         })
@@ -4402,18 +4394,18 @@
                                     }
                                 })), h.a.createElement("div", null, a.showDetected())))
                             }, a.submitEdit = function(e) {
                                 var t = a.props,
                                     n = t.variable,
                                     r = t.namespace,
                                     o = t.rjvId,
-                                    i = a.state,
-                                    s = i.editValue,
-                                    c = i.parsedInput,
-                                    l = s;
+                                    s = a.state,
+                                    i = s.editValue,
+                                    c = s.parsedInput,
+                                    l = i;
                                 e && c.type && (l = c.value), a.setState({
                                     editMode: !1
                                 }), L.dispatch({
                                     name: "VARIABLE_UPDATED",
                                     rjvId: o,
                                     data: {
                                         name: n.name,
@@ -4438,42 +4430,42 @@
                                         a.submitEdit(!0)
                                     }
                                 })))
                             }, a.getDetectedInput = function() {
                                 var e = a.state.parsedInput,
                                     t = e.type,
                                     n = e.value,
-                                    o = d(a).props,
-                                    i = o.theme;
+                                    o = f(a).props,
+                                    s = o.theme;
                                 if (!1 !== t) switch (t.toLowerCase()) {
                                     case "object":
                                         return h.a.createElement("span", null, h.a.createElement("span", {
-                                            style: r(r({}, S(i, "brace").style), {}, {
+                                            style: r(r({}, S(s, "brace").style), {}, {
                                                 cursor: "default"
                                             })
                                         }, "{"), h.a.createElement("span", {
-                                            style: r(r({}, S(i, "ellipsis").style), {}, {
+                                            style: r(r({}, S(s, "ellipsis").style), {}, {
                                                 cursor: "default"
                                             })
                                         }, "..."), h.a.createElement("span", {
-                                            style: r(r({}, S(i, "brace").style), {}, {
+                                            style: r(r({}, S(s, "brace").style), {}, {
                                                 cursor: "default"
                                             })
                                         }, "}"));
                                     case "array":
                                         return h.a.createElement("span", null, h.a.createElement("span", {
-                                            style: r(r({}, S(i, "brace").style), {}, {
+                                            style: r(r({}, S(s, "brace").style), {}, {
                                                 cursor: "default"
                                             })
                                         }, "["), h.a.createElement("span", {
-                                            style: r(r({}, S(i, "ellipsis").style), {}, {
+                                            style: r(r({}, S(s, "ellipsis").style), {}, {
                                                 cursor: "default"
                                             })
                                         }, "..."), h.a.createElement("span", {
-                                            style: r(r({}, S(i, "brace").style), {}, {
+                                            style: r(r({}, S(s, "brace").style), {}, {
                                                 cursor: "default"
                                             })
                                         }, "]"));
                                     case "string":
                                         return h.a.createElement(K, Object.assign({
                                             value: n
                                         }, o));
@@ -4511,202 +4503,202 @@
                                 renameKey: !1,
                                 parsedInput: {
                                     type: !1,
                                     value: null
                                 }
                             }, a
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this,
                                     t = this.props,
                                     n = t.variable,
                                     a = t.singleIndent,
                                     o = t.type,
-                                    i = t.theme,
-                                    s = t.namespace,
+                                    s = t.theme,
+                                    i = t.namespace,
                                     c = t.indentWidth,
                                     l = t.enableClipboard,
                                     u = t.onEdit,
                                     p = t.onDelete,
-                                    d = t.onSelect,
-                                    f = t.displayArrayKey,
+                                    f = t.onSelect,
+                                    d = t.displayArrayKey,
                                     b = t.quotesOnKeys,
                                     v = this.state.editMode;
-                                return h.a.createElement("div", Object.assign({}, S(i, "objectKeyVal", {
+                                return h.a.createElement("div", Object.assign({}, S(s, "objectKeyVal", {
                                     paddingLeft: c * a
                                 }), {
                                     onMouseEnter: function() {
                                         return e.setState(r(r({}, e.state), {}, {
                                             hovered: !0
                                         }))
                                     },
                                     onMouseLeave: function() {
                                         return e.setState(r(r({}, e.state), {}, {
                                             hovered: !1
                                         }))
                                     },
                                     className: "variable-row",
                                     key: n.name
-                                }), "array" == o ? f ? h.a.createElement("span", Object.assign({}, S(i, "array-key"), {
-                                    key: n.name + "_" + s
-                                }), n.name, h.a.createElement("div", S(i, "colon"), ":")) : null : h.a.createElement("span", null, h.a.createElement("span", Object.assign({}, S(i, "object-name"), {
+                                }), "array" == o ? d ? h.a.createElement("span", Object.assign({}, S(s, "array-key"), {
+                                    key: n.name + "_" + i
+                                }), n.name, h.a.createElement("div", S(s, "colon"), ":")) : null : h.a.createElement("span", null, h.a.createElement("span", Object.assign({}, S(s, "object-name"), {
                                     className: "object-key",
-                                    key: n.name + "_" + s
+                                    key: n.name + "_" + i
                                 }), !!b && h.a.createElement("span", {
                                     style: {
                                         verticalAlign: "top"
                                     }
                                 }, '"'), h.a.createElement("span", {
                                     style: {
                                         display: "inline-block"
                                     }
                                 }, n.name), !!b && h.a.createElement("span", {
                                     style: {
                                         verticalAlign: "top"
                                     }
-                                }, '"')), h.a.createElement("span", S(i, "colon"), ":")), h.a.createElement("div", Object.assign({
+                                }, '"')), h.a.createElement("span", S(s, "colon"), ":")), h.a.createElement("div", Object.assign({
                                     className: "variable-value",
-                                    onClick: !1 === d && !1 === u ? null : function(t) {
-                                        var a = I(s);
-                                        (t.ctrlKey || t.metaKey) && !1 !== u ? e.prepopInput(n) : !1 !== d && (a.shift(), d(r(r({}, n), {}, {
+                                    onClick: !1 === f && !1 === u ? null : function(t) {
+                                        var a = I(i);
+                                        (t.ctrlKey || t.metaKey) && !1 !== u ? e.prepopInput(n) : !1 !== f && (a.shift(), f(r(r({}, n), {}, {
                                             namespace: a
                                         })))
                                     }
-                                }, S(i, "variableValue", {
-                                    cursor: !1 === d ? "default" : "pointer"
+                                }, S(s, "variableValue", {
+                                    cursor: !1 === f ? "default" : "pointer"
                                 })), this.getValue(n, v)), l ? h.a.createElement(ey, {
                                     rowHovered: this.state.hovered,
                                     hidden: v,
                                     src: n.value,
                                     clickCallback: l,
-                                    theme: i,
-                                    namespace: [].concat(I(s), [n.name])
+                                    theme: s,
+                                    namespace: [].concat(I(i), [n.name])
                                 }) : null, !1 !== u && 0 == v ? this.getEditIcon() : null, !1 !== p && 0 == v ? this.getRemoveIcon() : null)
                             }
                         }]), n
                     }(h.a.PureComponent),
                     eE = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             var e;
                             o(this, n);
-                            for (var a = arguments.length, i = Array(a), s = 0; s < a; s++) i[s] = arguments[s];
-                            return (e = t.call.apply(t, [this].concat(i))).getObjectSize = function() {
+                            for (var a = arguments.length, s = Array(a), i = 0; i < a; i++) s[i] = arguments[i];
+                            return (e = t.call.apply(t, [this].concat(s))).getObjectSize = function() {
                                 var t = e.props,
                                     n = t.size,
                                     a = t.theme;
                                 if (t.displayObjectSize) return h.a.createElement("span", Object.assign({
                                     className: "object-size"
                                 }, S(a, "object-size")), n, " item", 1 === n ? "" : "s")
                             }, e.getAddAttribute = function(t) {
                                 var n = e.props,
                                     a = n.theme,
                                     o = n.namespace,
-                                    i = n.name,
-                                    s = n.src,
+                                    s = n.name,
+                                    i = n.src,
                                     c = n.rjvId,
                                     l = n.depth;
                                 return h.a.createElement("span", {
                                     className: "click-to-add",
                                     style: {
                                         verticalAlign: "top",
                                         display: t ? "inline-block" : "none"
                                     }
-                                }, h.a.createElement(ef, Object.assign({
+                                }, h.a.createElement(ed, Object.assign({
                                     className: "click-to-add-icon"
                                 }, S(a, "addVarIcon"), {
                                     onClick: function() {
                                         var e = {
-                                            name: l > 0 ? i : null,
+                                            name: l > 0 ? s : null,
                                             namespace: o.splice(0, o.length - 1),
-                                            existing_value: s,
+                                            existing_value: i,
                                             variable_removed: !1,
                                             key_name: null
                                         };
-                                        "object" === j(s) ? L.dispatch({
+                                        "object" === j(i) ? L.dispatch({
                                             name: "ADD_VARIABLE_KEY_REQUEST",
                                             rjvId: c,
                                             data: e
                                         }) : L.dispatch({
                                             name: "VARIABLE_ADDED",
                                             rjvId: c,
                                             data: r(r({}, e), {}, {
-                                                new_value: [].concat(I(s), [null])
+                                                new_value: [].concat(I(i), [null])
                                             })
                                         })
                                     }
                                 })))
                             }, e.getRemoveObject = function(t) {
                                 var n = e.props,
                                     a = n.theme,
                                     r = (n.hover, n.namespace),
                                     o = n.name,
-                                    i = n.src,
-                                    s = n.rjvId;
+                                    s = n.src,
+                                    i = n.rjvId;
                                 if (1 !== r.length) return h.a.createElement("span", {
                                     className: "click-to-remove",
                                     style: {
                                         display: t ? "inline-block" : "none"
                                     }
-                                }, h.a.createElement(ed, Object.assign({
+                                }, h.a.createElement(ef, Object.assign({
                                     className: "click-to-remove-icon"
                                 }, S(a, "removeVarIcon"), {
                                     onClick: function() {
                                         L.dispatch({
                                             name: "VARIABLE_REMOVED",
-                                            rjvId: s,
+                                            rjvId: i,
                                             data: {
                                                 name: o,
                                                 namespace: r.splice(0, r.length - 1),
-                                                existing_value: i,
+                                                existing_value: s,
                                                 variable_removed: !0
                                             }
                                         })
                                     }
                                 })))
                             }, e.render = function() {
                                 var t = e.props,
                                     n = t.theme,
                                     a = t.onDelete,
                                     r = t.onAdd,
                                     o = t.enableClipboard,
-                                    i = t.src,
-                                    s = t.namespace,
+                                    s = t.src,
+                                    i = t.namespace,
                                     c = t.rowHovered;
                                 return h.a.createElement("div", Object.assign({}, S(n, "object-meta-data"), {
                                     className: "object-meta-data",
                                     onClick: function(e) {
                                         e.stopPropagation()
                                     }
                                 }), e.getObjectSize(), o ? h.a.createElement(ey, {
                                     rowHovered: c,
                                     clickCallback: o,
-                                    src: i,
+                                    src: s,
                                     theme: n,
-                                    namespace: s
+                                    namespace: i
                                 }) : null, !1 !== r ? e.getAddAttribute(c) : null, !1 !== a ? e.getRemoveObject(c) : null)
                             }, e
                         }
                         return n
                     }(h.a.PureComponent);
 
                 function ej(e) {
                     var t = e.parent_type,
                         n = e.namespace,
                         a = e.quotesOnKeys,
                         r = e.theme,
                         o = e.jsvRoot,
-                        i = e.name,
-                        s = e.displayArrayKey,
+                        s = e.name,
+                        i = e.displayArrayKey,
                         c = e.name ? e.name : "";
-                    return o && (!1 === i || null === i) ? h.a.createElement("span", null) : "array" == t ? s ? h.a.createElement("span", Object.assign({}, S(r, "array-key"), {
+                    return o && (!1 === s || null === s) ? h.a.createElement("span", null) : "array" == t ? i ? h.a.createElement("span", Object.assign({}, S(r, "array-key"), {
                         key: n
                     }), h.a.createElement("span", {
                         className: "array-key"
                     }, c), h.a.createElement("span", S(r, "colon"), ":")) : h.a.createElement("span", null) : h.a.createElement("span", Object.assign({}, S(r, "object-name"), {
                         key: n
                     }), h.a.createElement("span", {
                         className: "object-key"
@@ -4725,15 +4717,15 @@
                     var t = e.theme;
                     switch (e.iconStyle) {
                         case "triangle":
                             return h.a.createElement(eu, Object.assign({}, S(t, "expanded-icon"), {
                                 className: "expanded-icon"
                             }));
                         case "square":
-                            return h.a.createElement(es, Object.assign({}, S(t, "expanded-icon"), {
+                            return h.a.createElement(ei, Object.assign({}, S(t, "expanded-icon"), {
                                 className: "expanded-icon"
                             }));
                         default:
                             return h.a.createElement(eo, Object.assign({}, S(t, "expanded-icon"), {
                                 className: "expanded-icon"
                             }))
                     }
@@ -4747,36 +4739,36 @@
                                 className: "collapsed-icon"
                             }));
                         case "square":
                             return h.a.createElement(ec, Object.assign({}, S(t, "collapsed-icon"), {
                                 className: "collapsed-icon"
                             }));
                         default:
-                            return h.a.createElement(ei, Object.assign({}, S(t, "collapsed-icon"), {
+                            return h.a.createElement(es, Object.assign({}, S(t, "collapsed-icon"), {
                                 className: "collapsed-icon"
                             }))
                     }
                 }
                 var ek = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n(e) {
                             var a;
                             return o(this, n), (a = t.call(this, e)).toggleCollapsed = function(e) {
                                 var t = [];
                                 for (var n in a.state.expanded) t.push(a.state.expanded[n]);
                                 t[e] = !t[e], a.setState({
                                     expanded: t
                                 })
                             }, a.state = {
                                 expanded: []
                             }, a
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "getExpandedIcon",
                             value: function(e) {
                                 var t = this.props,
                                     n = t.theme,
                                     a = t.iconStyle;
                                 return this.state.expanded[e] ? h.a.createElement(ex, {
                                     theme: n,
@@ -4791,69 +4783,69 @@
                             value: function() {
                                 var e = this,
                                     t = this.props,
                                     n = t.src,
                                     a = t.groupArraysAfterLength,
                                     r = (t.depth, t.name),
                                     o = t.theme,
-                                    i = t.jsvRoot,
-                                    s = t.namespace,
+                                    s = t.jsvRoot,
+                                    i = t.namespace,
                                     c = (t.parent_type, E(t, ["src", "groupArraysAfterLength", "depth", "name", "theme", "jsvRoot", "namespace", "parent_type"])),
                                     l = 0,
                                     u = 5 * this.props.indentWidth;
-                                i || (l = 5 * this.props.indentWidth);
+                                s || (l = 5 * this.props.indentWidth);
                                 var p = Math.ceil(n.length / a);
                                 return h.a.createElement("div", Object.assign({
                                     className: "object-key-val"
-                                }, S(o, i ? "jsv-root" : "objectKeyVal", {
+                                }, S(o, s ? "jsv-root" : "objectKeyVal", {
                                     paddingLeft: l
                                 })), h.a.createElement(ej, this.props), h.a.createElement("span", null, h.a.createElement(eE, Object.assign({
                                     size: n.length
-                                }, this.props))), I(Array(p)).map(function(t, i) {
+                                }, this.props))), I(Array(p)).map(function(t, s) {
                                     return h.a.createElement("div", Object.assign({
-                                        key: i,
+                                        key: s,
                                         className: "object-key-val array-group"
                                     }, S(o, "objectKeyVal", {
                                         marginLeft: 6,
                                         paddingLeft: u
                                     })), h.a.createElement("span", S(o, "brace-row"), h.a.createElement("div", Object.assign({
                                         className: "icon-container"
                                     }, S(o, "icon-container"), {
                                         onClick: function(t) {
-                                            e.toggleCollapsed(i)
+                                            e.toggleCollapsed(s)
                                         }
-                                    }), e.getExpandedIcon(i)), e.state.expanded[i] ? h.a.createElement(eS, Object.assign({
-                                        key: r + i,
+                                    }), e.getExpandedIcon(s)), e.state.expanded[s] ? h.a.createElement(eS, Object.assign({
+                                        key: r + s,
                                         depth: 0,
                                         name: !1,
                                         collapsed: !1,
                                         groupArraysAfterLength: a,
-                                        index_offset: i * a,
-                                        src: n.slice(i * a, i * a + a),
-                                        namespace: s,
+                                        index_offset: s * a,
+                                        src: n.slice(s * a, s * a + a),
+                                        namespace: i,
                                         type: "array",
                                         parent_type: "array_group",
                                         theme: o
                                     }, c)) : h.a.createElement("span", Object.assign({}, S(o, "brace"), {
                                         onClick: function(t) {
-                                            e.toggleCollapsed(i)
+                                            e.toggleCollapsed(s)
                                         },
                                         className: "array-group-brace"
                                     }), "[", h.a.createElement("div", Object.assign({}, S(o, "array-group-meta-data"), {
                                         className: "array-group-meta-data"
                                     }), h.a.createElement("span", Object.assign({
                                         className: "object-size"
-                                    }, S(o, "object-size")), i * a, " - ", i * a + a > n.length ? n.length : i * a + a)), "]")))
+                                    }, S(o, "object-size")), s * a, " - ", s * a + a > n.length ? n.length : s * a + a)), "]")))
                                 }))
                             }
                         }]), n
                     }(h.a.PureComponent),
                     eO = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n(e) {
                             o(this, n), (a = t.call(this, e)).toggleCollapsed = function() {
                                 a.setState({
                                     expanded: !a.state.expanded
                                 }, function() {
                                     B.set(a.props.rjvId, a.props.namespace, "expanded", a.state.expanded)
@@ -4877,34 +4869,34 @@
                                 return h.a.createElement(eE, Object.assign({
                                     rowHovered: o,
                                     size: r
                                 }, a.props))
                             }, a.renderObjectContents = function(e, t) {
                                 var n, r = a.props,
                                     o = r.depth,
-                                    i = r.parent_type,
-                                    s = r.index_offset,
+                                    s = r.parent_type,
+                                    i = r.index_offset,
                                     c = r.groupArraysAfterLength,
                                     l = r.namespace,
                                     u = a.state.object_type,
                                     p = [],
-                                    d = Object.keys(e || {});
-                                return a.props.sortKeys && "array" !== u && (d = d.sort()), d.forEach(function(r) {
-                                    if (n = new eC(r, e[r]), "array_group" === i && s && (n.name = parseInt(n.name) + s), e.hasOwnProperty(r)) {
+                                    f = Object.keys(e || {});
+                                return a.props.sortKeys && "array" !== u && (f = f.sort()), f.forEach(function(r) {
+                                    if (n = new eC(r, e[r]), "array_group" === s && i && (n.name = parseInt(n.name) + i), e.hasOwnProperty(r)) {
                                         if ("object" === n.type) p.push(h.a.createElement(eS, Object.assign({
                                             key: n.name,
                                             depth: o + 1,
                                             name: n.name,
                                             src: n.value,
                                             namespace: l.concat(n.name),
                                             parent_type: u
                                         }, t)));
                                         else if ("array" === n.type) {
-                                            var d = eS;
-                                            c && n.value.length > c && (d = ek), p.push(h.a.createElement(d, Object.assign({
+                                            var f = eS;
+                                            c && n.value.length > c && (f = ek), p.push(h.a.createElement(f, Object.assign({
                                                 key: n.name,
                                                 depth: o + 1,
                                                 name: n.name,
                                                 src: n.value,
                                                 namespace: l.concat(n.name),
                                                 type: "array",
                                                 parent_type: u
@@ -4915,78 +4907,78 @@
                                             singleIndent: 5,
                                             namespace: l,
                                             type: a.props.type
                                         }, t)))
                                     }
                                 }), p
                             };
-                            var a, i = n.getState(e);
-                            return a.state = r(r({}, i), {}, {
+                            var a, s = n.getState(e);
+                            return a.state = r(r({}, s), {}, {
                                 prevProps: {}
                             }), a
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "getBraceStart",
                             value: function(e, t) {
                                 var n = this,
                                     a = this.props,
                                     r = a.src,
                                     o = a.theme,
-                                    i = a.iconStyle;
+                                    s = a.iconStyle;
                                 if ("array_group" === a.parent_type) return h.a.createElement("span", null, h.a.createElement("span", S(o, "brace"), "array" === e ? "[" : "{"), t ? this.getObjectMetaData(r) : null);
-                                var s = t ? ex : e_;
+                                var i = t ? ex : e_;
                                 return h.a.createElement("span", null, h.a.createElement("span", Object.assign({
                                     onClick: function(e) {
                                         n.toggleCollapsed()
                                     }
                                 }, S(o, "brace-row")), h.a.createElement("div", Object.assign({
                                     className: "icon-container"
-                                }, S(o, "icon-container")), h.a.createElement(s, {
+                                }, S(o, "icon-container")), h.a.createElement(i, {
                                     theme: o,
-                                    iconStyle: i
+                                    iconStyle: s
                                 })), h.a.createElement(ej, this.props), h.a.createElement("span", S(o, "brace"), "array" === e ? "[" : "{")), t ? this.getObjectMetaData(r) : null)
                             }
                         }, {
                             key: "render",
                             value: function() {
                                 var e = this,
                                     t = this.props,
                                     n = t.depth,
                                     a = t.src,
                                     o = (t.namespace, t.name, t.type, t.parent_type),
-                                    i = t.theme,
-                                    s = t.jsvRoot,
+                                    s = t.theme,
+                                    i = t.jsvRoot,
                                     c = t.iconStyle,
                                     l = E(t, ["depth", "src", "namespace", "name", "type", "parent_type", "theme", "jsvRoot", "iconStyle"]),
                                     u = this.state,
                                     p = u.object_type,
-                                    d = u.expanded,
-                                    f = {};
-                                return s || "array_group" === o ? "array_group" === o && (f.borderLeft = 0, f.display = "inline") : f.paddingLeft = 5 * this.props.indentWidth, h.a.createElement("div", Object.assign({
+                                    f = u.expanded,
+                                    d = {};
+                                return i || "array_group" === o ? "array_group" === o && (d.borderLeft = 0, d.display = "inline") : d.paddingLeft = 5 * this.props.indentWidth, h.a.createElement("div", Object.assign({
                                     className: "object-key-val",
                                     onMouseEnter: function() {
                                         return e.setState(r(r({}, e.state), {}, {
                                             hovered: !0
                                         }))
                                     },
                                     onMouseLeave: function() {
                                         return e.setState(r(r({}, e.state), {}, {
                                             hovered: !1
                                         }))
                                     }
-                                }, S(i, s ? "jsv-root" : "objectKeyVal", f)), this.getBraceStart(p, d), d ? this.getObjectContent(n, a, r({
-                                    theme: i,
+                                }, S(s, i ? "jsv-root" : "objectKeyVal", d)), this.getBraceStart(p, f), f ? this.getObjectContent(n, a, r({
+                                    theme: s,
                                     iconStyle: c
                                 }, l)) : this.getEllipsis(), h.a.createElement("span", {
                                     className: "brace-row"
                                 }, h.a.createElement("span", {
-                                    style: r(r({}, S(i, "brace").style), {}, {
-                                        paddingLeft: d ? "3px" : "0px"
+                                    style: r(r({}, S(s, "brace").style), {}, {
+                                        paddingLeft: f ? "3px" : "0px"
                                     })
-                                }, "array" === p ? "]" : "}"), d ? null : this.getObjectMetaData(a)))
+                                }, "array" === p ? "]" : "}"), f ? null : this.getObjectMetaData(a)))
                             }
                         }], [{
                             key: "getDerivedStateFromProps",
                             value: function(e, t) {
                                 var a = t.prevProps;
                                 return e.src !== a.src || e.collapsed !== a.collapsed || e.name !== a.name || e.namespace !== a.namespace || e.rjvId !== a.rjvId ? r(r({}, n.getState(e)), {}, {
                                     prevProps: e
@@ -5013,22 +5005,22 @@
                 var eC = function e(t, n) {
                     o(this, e), this.name = t, this.value = n, this.type = j(n)
                 };
                 g(eO);
                 var eS = eO,
                     ew = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             var e;
                             o(this, n);
-                            for (var a = arguments.length, r = Array(a), i = 0; i < a; i++) r[i] = arguments[i];
+                            for (var a = arguments.length, r = Array(a), s = 0; s < a; s++) r[s] = arguments[s];
                             return (e = t.call.apply(t, [this].concat(r))).render = function() {
-                                var t = d(e).props,
+                                var t = f(e).props,
                                     n = [t.name],
                                     a = eS;
                                 return Array.isArray(t.src) && t.groupArraysAfterLength && t.src.length > t.groupArraysAfterLength && (a = ek), h.a.createElement("div", {
                                     className: "pretty-json-container object-container"
                                 }, h.a.createElement("div", {
                                     className: "object-content"
                                 }, h.a.createElement(a, Object.assign({
@@ -5038,39 +5030,39 @@
                                 }, t))))
                             }, e
                         }
                         return n
                     }(h.a.PureComponent),
                     eA = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n(e) {
                             var a;
                             return o(this, n), (a = t.call(this, e)).closeModal = function() {
                                 L.dispatch({
                                     rjvId: a.props.rjvId,
                                     name: "RESET"
                                 })
                             }, a.submit = function() {
                                 a.props.submit(a.state.input)
                             }, a.state = {
                                 input: e.input ? e.input : ""
                             }, a
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this,
                                     t = this.props,
                                     n = t.theme,
                                     a = t.rjvId,
                                     r = t.isValid,
                                     o = this.state.input,
-                                    i = r(o);
+                                    s = r(o);
                                 return h.a.createElement("div", Object.assign({
                                     className: "key-modal-request"
                                 }, S(n, "key-modal-request"), {
                                     onClick: this.closeModal
                                 }), h.a.createElement("div", Object.assign({}, S(n, "key-modal"), {
                                     onClick: function(e) {
                                         e.stopPropagation()
@@ -5089,17 +5081,17 @@
                                     placeholder: "...",
                                     onChange: function(t) {
                                         e.setState({
                                             input: t.target.value
                                         })
                                     },
                                     onKeyPress: function(t) {
-                                        i && "Enter" === t.key ? e.submit() : "Escape" === t.key && e.closeModal()
+                                        s && "Enter" === t.key ? e.submit() : "Escape" === t.key && e.closeModal()
                                     }
-                                })), i ? h.a.createElement(ev, Object.assign({}, S(n, "key-modal-submit"), {
+                                })), s ? h.a.createElement(ev, Object.assign({}, S(n, "key-modal-submit"), {
                                     className: "key-modal-submit",
                                     onClick: function(t) {
                                         return e.submit()
                                     }
                                 })) : null), h.a.createElement("span", S(n, "key-modal-cancel"), h.a.createElement(eb, Object.assign({}, S(n, "key-modal-cancel-icon"), {
                                     className: "key-modal-cancel",
                                     onClick: function() {
@@ -5110,35 +5102,35 @@
                                     }
                                 })))))
                             }
                         }]), n
                     }(h.a.PureComponent),
                     eM = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             var e;
                             o(this, n);
-                            for (var a = arguments.length, i = Array(a), s = 0; s < a; s++) i[s] = arguments[s];
-                            return (e = t.call.apply(t, [this].concat(i))).isValid = function(t) {
+                            for (var a = arguments.length, s = Array(a), i = 0; i < a; i++) s[i] = arguments[i];
+                            return (e = t.call.apply(t, [this].concat(s))).isValid = function(t) {
                                 var n = e.props.rjvId,
                                     a = B.get(n, "action", "new-key-request");
                                 return "" != t && -1 === Object.keys(a.existing_value).indexOf(t)
                             }, e.submit = function(t) {
                                 var n = e.props.rjvId,
                                     a = B.get(n, "action", "new-key-request");
                                 a.new_value = r({}, a.existing_value), a.new_value[t] = e.props.defaultValue, L.dispatch({
                                     name: "VARIABLE_ADDED",
                                     rjvId: n,
                                     data: a
                                 })
                             }, e
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.active,
                                     n = e.theme,
                                     a = e.rjvId;
                                 return t ? h.a.createElement(eA, {
@@ -5148,20 +5140,20 @@
                                     submit: this.submit
                                 }) : null
                             }
                         }]), n
                     }(h.a.PureComponent),
                     eP = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n() {
                             return o(this, n), t.apply(this, arguments)
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "render",
                             value: function() {
                                 var e = this.props,
                                     t = e.message,
                                     n = e.active,
                                     a = e.theme,
                                     r = e.rjvId;
@@ -5176,55 +5168,55 @@
                                     }
                                 }), h.a.createElement("span", S(a, "validation-failure-label"), t), h.a.createElement(eb, S(a, "validation-failure-clear"))) : null
                             }
                         }]), n
                     }(h.a.PureComponent),
                     eF = function(e) {
                         l(n, e);
-                        var t = f(n);
+                        var t = d(n);
 
                         function n(e) {
                             var a;
                             return o(this, n), (a = t.call(this, e)).rjvId = Date.now().toString(), a.getListeners = function() {
                                 return {
                                     reset: a.resetState,
                                     "variable-update": a.updateSrc,
                                     "add-key-request": a.addKeyRequest
                                 }
                             }, a.updateSrc = function() {
                                 var e, t = B.get(a.rjvId, "action", "variable-update"),
                                     n = t.name,
                                     r = t.namespace,
                                     o = t.new_value,
-                                    i = t.existing_value,
-                                    s = (t.variable_removed, t.updated_src),
+                                    s = t.existing_value,
+                                    i = (t.variable_removed, t.updated_src),
                                     c = t.type,
                                     l = a.props,
                                     u = l.onEdit,
                                     p = l.onDelete,
-                                    d = l.onAdd,
-                                    f = {
+                                    f = l.onAdd,
+                                    d = {
                                         existing_src: a.state.src,
                                         new_value: o,
-                                        updated_src: s,
+                                        updated_src: i,
                                         name: n,
                                         namespace: r,
-                                        existing_value: i
+                                        existing_value: s
                                     };
                                 switch (c) {
                                     case "variable-added":
-                                        e = d(f);
+                                        e = f(d);
                                         break;
                                     case "variable-edited":
-                                        e = u(f);
+                                        e = u(d);
                                         break;
                                     case "variable-removed":
-                                        e = p(f)
-                                }!1 !== e ? (B.set(a.rjvId, "global", "src", s), a.setState({
-                                    src: s
+                                        e = p(d)
+                                }!1 !== e ? (B.set(a.rjvId, "global", "src", i), a.setState({
+                                    src: i
                                 })) : a.setState({
                                     validationFailure: !0
                                 })
                             }, a.addKeyRequest = function() {
                                 a.setState({
                                     addKeyRequest: !0
                                 })
@@ -5242,15 +5234,15 @@
                                 theme: n.defaultProps.theme,
                                 validationMessage: n.defaultProps.validationMessage,
                                 prevSrc: n.defaultProps.src,
                                 prevName: n.defaultProps.name,
                                 prevTheme: n.defaultProps.theme
                             }, a
                         }
-                        return s(n, [{
+                        return i(n, [{
                             key: "componentDidMount",
                             value: function() {
                                 B.set(this.rjvId, "global", "src", this.state.src);
                                 var e = this.getListeners();
                                 for (var t in e) B.on(t + "-" + this.rjvId, e[t]);
                                 this.setState({
                                     addKeyRequest: !1,
@@ -5276,32 +5268,32 @@
                             key: "render",
                             value: function() {
                                 var e = this.state,
                                     t = e.validationFailure,
                                     n = e.validationMessage,
                                     a = e.addKeyRequest,
                                     o = e.theme,
-                                    i = e.src,
-                                    s = e.name,
+                                    s = e.src,
+                                    i = e.name,
                                     c = this.props,
                                     l = c.style,
                                     u = c.defaultValue;
                                 return h.a.createElement("div", {
                                     className: "react-json-view",
                                     style: r(r({}, S(o, "app-container").style), l)
                                 }, h.a.createElement(eP, {
                                     message: n,
                                     active: t,
                                     theme: o,
                                     rjvId: this.rjvId
                                 }), h.a.createElement(ew, Object.assign({}, this.props, {
-                                    src: i,
-                                    name: s,
+                                    src: s,
+                                    name: i,
                                     theme: o,
-                                    type: j(i),
+                                    type: j(s),
                                     rjvId: this.rjvId
                                 })), h.a.createElement(eM, {
                                     active: a,
                                     theme: o,
                                     rjvId: this.rjvId,
                                     defaultValue: u
                                 }))
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/29107295-809b6f0b05884bf7.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1672,17 +1672,16 @@
                                 return t
                             }
                         }
 
                         function eQ(n) {
                             return function(t) {
                                 var r = tF(t = oi(t)) ? tV(t) : u,
-                                    e = r ? r[0] : t.charAt(0),
-                                    i = r ? e$(r, 1).join("") : t.slice(1);
-                                return e[n]() + i
+                                    e = r ? e$(r, 1).join("") : t.slice(1);
+                                return (r ? r[0] : t.charAt(0))[n]() + e
                             }
                         }
 
                         function eX(n) {
                             return function(t) {
                                 return ty(o$(oz(t).replace(nq, "")), n, "")
                             }
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/418-f078369e2fd2524e.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/728-4d1eeb7a2f426351.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,206 +1,220 @@
 "use strict";
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
-    [418], {
+    [728], {
+        8442: function(t, n, e) {
+            e.d(n, {
+                Z: function() {
+                    return i
+                }
+            });
+
+            function i(t) {
+                return "string" == typeof t
+            }
+        },
+        1276: function(t, n, e) {
+            e.d(n, {
+                Z: function() {
+                    return i
+                }
+            });
+
+            function i(t, n, e) {
+                return "function" == typeof t ? t(n, e) : t
+            }
+        },
+        9235: function(t, n, e) {
+            e.d(n, {
+                Z: function() {
+                    return p
+                }
+            });
+            var i = e(7462),
+                o = e(3366),
+                r = e(3703),
+                s = e(8442),
+                a = function() {
+                    for (var t, n, e = 0, i = ""; e < arguments.length;)(t = arguments[e++]) && (n = function t(n) {
+                        var e, i, o = "";
+                        if ("string" == typeof n || "number" == typeof n) o += n;
+                        else if ("object" == typeof n) {
+                            if (Array.isArray(n))
+                                for (e = 0; e < n.length; e++) n[e] && (i = t(n[e])) && (o && (o += " "), o += i);
+                            else
+                                for (e in n) n[e] && (o && (o += " "), o += e)
+                        }
+                        return o
+                    }(t)) && (i && (i += " "), i += n);
+                    return i
+                };
+
+            function u(t) {
+                if (void 0 === t) return {};
+                let n = {};
+                return Object.keys(t).filter(n => !(n.match(/^on[A-Z]/) && "function" == typeof t[n])).forEach(e => {
+                    n[e] = t[e]
+                }), n
+            }
+            var l = e(1276);
+            let c = ["elementType", "externalSlotProps", "ownerState", "skipResolvingSlotProps"];
+
+            function p(t) {
+                var n, e;
+                let {
+                    elementType: p,
+                    externalSlotProps: f,
+                    ownerState: d,
+                    skipResolvingSlotProps: h = !1
+                } = t, E = (0, o.Z)(t, c), x = h ? {} : (0, l.Z)(f, d), {
+                    props: m,
+                    internalRef: v
+                } = function(t) {
+                    let {
+                        getSlotProps: n,
+                        additionalProps: e,
+                        externalSlotProps: o,
+                        externalForwardedProps: r,
+                        className: s
+                    } = t;
+                    if (!n) {
+                        let t = a(null == r ? void 0 : r.className, null == o ? void 0 : o.className, s, null == e ? void 0 : e.className),
+                            n = (0, i.Z)({}, null == e ? void 0 : e.style, null == r ? void 0 : r.style, null == o ? void 0 : o.style),
+                            u = (0, i.Z)({}, e, r, o);
+                        return t.length > 0 && (u.className = t), Object.keys(n).length > 0 && (u.style = n), {
+                            props: u,
+                            internalRef: void 0
+                        }
+                    }
+                    let l = function(t, n = []) {
+                            if (void 0 === t) return {};
+                            let e = {};
+                            return Object.keys(t).filter(e => e.match(/^on[A-Z]/) && "function" == typeof t[e] && !n.includes(e)).forEach(n => {
+                                e[n] = t[n]
+                            }), e
+                        }((0, i.Z)({}, r, o)),
+                        c = u(o),
+                        p = u(r),
+                        f = n(l),
+                        d = a(null == f ? void 0 : f.className, null == e ? void 0 : e.className, s, null == r ? void 0 : r.className, null == o ? void 0 : o.className),
+                        h = (0, i.Z)({}, null == f ? void 0 : f.style, null == e ? void 0 : e.style, null == r ? void 0 : r.style, null == o ? void 0 : o.style),
+                        E = (0, i.Z)({}, f, e, p, c);
+                    return d.length > 0 && (E.className = d), Object.keys(h).length > 0 && (E.style = h), {
+                        props: E,
+                        internalRef: f.ref
+                    }
+                }((0, i.Z)({}, E, {
+                    externalSlotProps: x
+                })), y = (0, r.Z)(v, null == x ? void 0 : x.ref, null == (n = t.additionalProps) ? void 0 : n.ref), b = (e = (0, i.Z)({}, m, {
+                    ref: y
+                }), void 0 === p || (0, s.Z)(p) ? e : (0, i.Z)({}, e, {
+                    ownerState: (0, i.Z)({}, e.ownerState, d)
+                }));
+                return b
+            }
+        },
         6628: function(t, n, e) {
             var i = e(7462),
                 o = e(3366),
                 r = e(7294),
                 s = e(8662),
                 a = e(2734),
                 u = e(577),
                 l = e(1705),
                 c = e(5893);
-            let d = ["addEndListener", "appear", "children", "easing", "in", "onEnter", "onEntered", "onEntering", "onExit", "onExited", "onExiting", "style", "timeout", "TransitionComponent"],
-                p = {
+            let p = ["addEndListener", "appear", "children", "easing", "in", "onEnter", "onEntered", "onEntering", "onExit", "onExited", "onExiting", "style", "timeout", "TransitionComponent"],
+                f = {
                     entering: {
                         opacity: 1
                     },
                     entered: {
                         opacity: 1
                     }
                 },
-                f = r.forwardRef(function(t, n) {
+                d = r.forwardRef(function(t, n) {
                     let e = (0, a.Z)(),
-                        f = {
+                        d = {
                             enter: e.transitions.duration.enteringScreen,
                             exit: e.transitions.duration.leavingScreen
                         },
                         {
                             addEndListener: h,
                             appear: E = !0,
                             children: x,
                             easing: m,
                             in: v,
                             onEnter: y,
-                            onEntered: Z,
-                            onEntering: b,
-                            onExit: g,
+                            onEntered: b,
+                            onEntering: g,
+                            onExit: Z,
                             onExited: S,
                             onExiting: k,
                             style: C,
-                            timeout: N = f,
+                            timeout: N = d,
                             TransitionComponent: T = s.ZP
                         } = t,
-                        O = (0, o.Z)(t, d),
+                        O = (0, o.Z)(t, p),
                         R = r.useRef(null),
                         D = (0, l.Z)(R, x.ref, n),
                         w = t => n => {
                             if (t) {
                                 let e = R.current;
                                 void 0 === n ? t(e) : t(e, n)
                             }
                         },
-                        M = w(b),
-                        P = w((t, n) => {
+                        P = w(g),
+                        M = w((t, n) => {
                             (0, u.n)(t);
                             let i = (0, u.C)({
                                 style: C,
                                 timeout: N,
                                 easing: m
                             }, {
                                 mode: "enter"
                             });
                             t.style.webkitTransition = e.transitions.create("opacity", i), t.style.transition = e.transitions.create("opacity", i), y && y(t, n)
                         }),
-                        L = w(Z),
-                        j = w(k),
-                        I = w(t => {
+                        j = w(b),
+                        L = w(k),
+                        A = w(t => {
                             let n = (0, u.C)({
                                 style: C,
                                 timeout: N,
                                 easing: m
                             }, {
                                 mode: "exit"
                             });
-                            t.style.webkitTransition = e.transitions.create("opacity", n), t.style.transition = e.transitions.create("opacity", n), g && g(t)
+                            t.style.webkitTransition = e.transitions.create("opacity", n), t.style.transition = e.transitions.create("opacity", n), Z && Z(t)
                         }),
-                        U = w(S);
+                        I = w(S);
                     return (0, c.jsx)(T, (0, i.Z)({
                         appear: E,
                         in: v,
                         nodeRef: R,
-                        onEnter: P,
-                        onEntered: L,
-                        onEntering: M,
-                        onExit: I,
-                        onExited: U,
-                        onExiting: j,
+                        onEnter: M,
+                        onEntered: j,
+                        onEntering: P,
+                        onExit: A,
+                        onExited: I,
+                        onExiting: L,
                         addEndListener: t => {
                             h && h(R.current, t)
                         },
                         timeout: N
                     }, O, {
                         children: (t, n) => r.cloneElement(x, (0, i.Z)({
                             style: (0, i.Z)({
                                 opacity: 0,
                                 visibility: "exited" !== t || v ? void 0 : "hidden"
-                            }, p[t], C, x.props.style),
+                            }, f[t], C, x.props.style),
                             ref: D
                         }, n))
                     }))
                 });
-            n.Z = f
-        },
-        3247: function(t, n, e) {
-            e.d(n, {
-                Z: function() {
-                    return i
-                }
-            });
-
-            function i(t) {
-                return "string" == typeof t
-            }
-        },
-        7488: function(t, n, e) {
-            e.d(n, {
-                Z: function() {
-                    return i
-                }
-            });
-
-            function i(t, n) {
-                return "function" == typeof t ? t(n) : t
-            }
-        },
-        3249: function(t, n, e) {
-            e.d(n, {
-                Z: function() {
-                    return d
-                }
-            });
-            var i = e(7462),
-                o = e(3366),
-                r = e(3703),
-                s = e(3247),
-                a = e(6010);
-
-            function u(t) {
-                if (void 0 === t) return {};
-                let n = {};
-                return Object.keys(t).filter(n => !(n.match(/^on[A-Z]/) && "function" == typeof t[n])).forEach(e => {
-                    n[e] = t[e]
-                }), n
-            }
-            var l = e(7488);
-            let c = ["elementType", "externalSlotProps", "ownerState"];
-
-            function d(t) {
-                var n, e;
-                let {
-                    elementType: d,
-                    externalSlotProps: p,
-                    ownerState: f
-                } = t, h = (0, o.Z)(t, c), E = (0, l.Z)(p, f), {
-                    props: x,
-                    internalRef: m
-                } = function(t) {
-                    let {
-                        getSlotProps: n,
-                        additionalProps: e,
-                        externalSlotProps: o,
-                        externalForwardedProps: r,
-                        className: s
-                    } = t;
-                    if (!n) {
-                        let t = (0, a.Z)(null == r ? void 0 : r.className, null == o ? void 0 : o.className, s, null == e ? void 0 : e.className),
-                            n = (0, i.Z)({}, null == e ? void 0 : e.style, null == r ? void 0 : r.style, null == o ? void 0 : o.style),
-                            u = (0, i.Z)({}, e, r, o);
-                        return t.length > 0 && (u.className = t), Object.keys(n).length > 0 && (u.style = n), {
-                            props: u,
-                            internalRef: void 0
-                        }
-                    }
-                    let l = function(t, n = []) {
-                            if (void 0 === t) return {};
-                            let e = {};
-                            return Object.keys(t).filter(e => e.match(/^on[A-Z]/) && "function" == typeof t[e] && !n.includes(e)).forEach(n => {
-                                e[n] = t[n]
-                            }), e
-                        }((0, i.Z)({}, r, o)),
-                        c = u(o),
-                        d = u(r),
-                        p = n(l),
-                        f = (0, a.Z)(null == p ? void 0 : p.className, null == e ? void 0 : e.className, s, null == r ? void 0 : r.className, null == o ? void 0 : o.className),
-                        h = (0, i.Z)({}, null == p ? void 0 : p.style, null == e ? void 0 : e.style, null == r ? void 0 : r.style, null == o ? void 0 : o.style),
-                        E = (0, i.Z)({}, p, e, d, c);
-                    return f.length > 0 && (E.className = f), Object.keys(h).length > 0 && (E.style = h), {
-                        props: E,
-                        internalRef: p.ref
-                    }
-                }((0, i.Z)({}, h, {
-                    externalSlotProps: E
-                })), v = (0, r.Z)(m, null == E ? void 0 : E.ref, null == (n = t.additionalProps) ? void 0 : n.ref), y = (e = (0, i.Z)({}, x, {
-                    ref: v
-                }), void 0 === d || (0, s.Z)(d) ? e : (0, i.Z)({}, e, {
-                    ownerState: (0, i.Z)({}, e.ownerState, f)
-                }));
-                return y
-            }
+            n.Z = d
         },
         577: function(t, n, e) {
             e.d(n, {
                 C: function() {
                     return o
                 },
                 n: function() {
@@ -268,51 +282,51 @@
                 s = e(3935),
                 a = {
                     disabled: !1
                 },
                 u = e(220),
                 l = "unmounted",
                 c = "exited",
-                d = "entering",
-                p = "entered",
-                f = "exiting",
+                p = "entering",
+                f = "entered",
+                d = "exiting",
                 h = function(t) {
                     function n(n, e) {
                         i = t.call(this, n, e) || this;
                         var i, o, r = e && !e.isMounting ? n.enter : n.appear;
-                        return i.appearStatus = null, n.in ? r ? (o = c, i.appearStatus = d) : o = p : o = n.unmountOnExit || n.mountOnEnter ? l : c, i.state = {
+                        return i.appearStatus = null, n.in ? r ? (o = c, i.appearStatus = p) : o = f : o = n.unmountOnExit || n.mountOnEnter ? l : c, i.state = {
                             status: o
                         }, i.nextCallback = null, i
                     }(0, o.Z)(n, t), n.getDerivedStateFromProps = function(t, n) {
                         return t.in && n.status === l ? {
                             status: c
                         } : null
                     };
                     var e = n.prototype;
                     return e.componentDidMount = function() {
                         this.updateStatus(!0, this.appearStatus)
                     }, e.componentDidUpdate = function(t) {
                         var n = null;
                         if (t !== this.props) {
                             var e = this.state.status;
-                            this.props.in ? e !== d && e !== p && (n = d) : (e === d || e === p) && (n = f)
+                            this.props.in ? e !== p && e !== f && (n = p) : (e === p || e === f) && (n = d)
                         }
                         this.updateStatus(!1, n)
                     }, e.componentWillUnmount = function() {
                         this.cancelNextCallback()
                     }, e.getTimeouts = function() {
                         var t, n, e, i = this.props.timeout;
                         return t = n = e = i, null != i && "number" != typeof i && (t = i.exit, n = i.enter, e = void 0 !== i.appear ? i.appear : n), {
                             exit: t,
                             enter: n,
                             appear: e
                         }
                     }, e.updateStatus = function(t, n) {
                         if (void 0 === t && (t = !1), null !== n) {
-                            if (this.cancelNextCallback(), n === d) {
+                            if (this.cancelNextCallback(), n === p) {
                                 if (this.props.unmountOnExit || this.props.mountOnEnter) {
                                     var e = this.props.nodeRef ? this.props.nodeRef.current : s.findDOMNode(this);
                                     e && e.scrollTop
                                 }
                                 this.performEnter(t)
                             } else this.performExit()
                         } else this.props.unmountOnExit && this.state.status === c && this.setState({
@@ -325,26 +339,26 @@
                             o = this.props.nodeRef ? [i] : [s.findDOMNode(this), i],
                             r = o[0],
                             u = o[1],
                             l = this.getTimeouts(),
                             c = i ? l.appear : l.enter;
                         if (!t && !e || a.disabled) {
                             this.safeSetState({
-                                status: p
+                                status: f
                             }, function() {
                                 n.props.onEntered(r)
                             });
                             return
                         }
                         this.props.onEnter(r, u), this.safeSetState({
-                            status: d
+                            status: p
                         }, function() {
                             n.props.onEntering(r, u), n.onTransitionEnd(c, function() {
                                 n.safeSetState({
-                                    status: p
+                                    status: f
                                 }, function() {
                                     n.props.onEntered(r, u)
                                 })
                             })
                         })
                     }, e.performExit = function() {
                         var t = this,
@@ -356,15 +370,15 @@
                                 status: c
                             }, function() {
                                 t.props.onExited(i)
                             });
                             return
                         }
                         this.props.onExit(i), this.safeSetState({
-                            status: f
+                            status: d
                         }, function() {
                             t.props.onExiting(i), t.onTransitionEnd(e.exit, function() {
                                 t.safeSetState({
                                     status: c
                                 }, function() {
                                     t.props.onExited(i)
                                 })
@@ -419,12 +433,12 @@
                 exit: !0,
                 onEnter: E,
                 onEntering: E,
                 onEntered: E,
                 onExit: E,
                 onExiting: E,
                 onExited: E
-            }, h.UNMOUNTED = l, h.EXITED = c, h.ENTERING = d, h.ENTERED = p, h.EXITING = f;
+            }, h.UNMOUNTED = l, h.EXITED = c, h.ENTERING = p, h.ENTERED = f, h.EXITING = d;
             var x = h
         }
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/498-112306b4f8cd81ec.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/498-c0ac8cca5a5197e4.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
                 Z: function() {
                     return R
                 }
             });
             var t = o(3366),
                 i = o(7462),
                 n = o(7294),
-                a = o(6010),
+                a = o(3680),
                 l = o(4780),
                 s = o(917),
                 c = o(8216),
                 u = o(1657),
                 d = o(948),
                 f = o(1588),
                 m = o(4867);
@@ -183,15 +183,15 @@
                 Z: function() {
                     return y
                 }
             });
             var t = o(7462),
                 i = o(7294),
                 n = o(3366),
-                a = o(6010),
+                a = o(3680),
                 l = o(4780),
                 s = o(8216),
                 c = o(1657),
                 u = o(948),
                 d = o(1588),
                 f = o(4867);
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/633-a2b446f38d34df6a.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/514-17895623628db944.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
-    [633], {
-        3754: function(e, t, r) {
+    [514], {
+        5929: function(e, t, r) {
             "use strict";
             let n;
             r.d(t, {
                 ZP: function() {
                     return G
                 }
             });
-            var a = r(3366),
-                o = r(7462),
-                l = r(7294),
-                i = r(6010),
+            var o = r(3366),
+                a = r(7462),
+                i = r(7294),
+                l = r(3680),
                 u = r(4780),
-                s = r(3249),
-                c = r(3247),
-                d = r(2690),
-                f = r(9032),
+                s = r(9235),
+                c = r(8442),
+                f = r(2690),
+                d = r(9032),
                 p = r(9962),
                 y = r(3703),
                 h = r(3546),
-                m = r(9948),
-                v = {
+                v = r(9948),
+                m = {
                     border: 0,
                     clip: "rect(0 0 0 0)",
                     height: "1px",
                     margin: -1,
                     overflow: "hidden",
                     padding: 0,
                     position: "absolute",
@@ -42,17 +42,17 @@
             }
 
             function P(e, t) {
                 var r;
                 let {
                     index: n
                 } = null != (r = e.reduce((e, r, n) => {
-                    let a = Math.abs(t - r);
-                    return null === e || a < e.distance || a === e.distance ? {
-                        distance: a,
+                    let o = Math.abs(t - r);
+                    return null === e || o < e.distance || o === e.distance ? {
+                        distance: o,
                         index: n
                     } : e
                 }, null)) ? r : {};
                 return n
             }
 
             function w(e, t) {
@@ -77,30 +77,30 @@
                 newValue: t,
                 index: r
             }) {
                 let n = e.slice();
                 return n[r] = t, n.sort(b)
             }
 
-            function S({
+            function O({
                 sliderRef: e,
                 activeIndex: t,
                 setActive: r
             }) {
-                var n, a, o;
-                let l = (0, d.Z)(e.current);
-                null != (n = e.current) && n.contains(l.activeElement) && Number(null == l ? void 0 : null == (a = l.activeElement) ? void 0 : a.getAttribute("data-index")) === t || null == (o = e.current) || o.querySelector(`[type="range"][data-index="${t}"]`).focus(), r && r(t)
+                var n, o, a;
+                let i = (0, f.Z)(e.current);
+                null != (n = e.current) && n.contains(i.activeElement) && Number(null == i ? void 0 : null == (o = i.activeElement) ? void 0 : o.getAttribute("data-index")) === t || null == (a = e.current) || a.querySelector(`[type="range"][data-index="${t}"]`).focus(), r && r(t)
             }
 
-            function O(e, t) {
+            function S(e, t) {
                 return "number" == typeof e && "number" == typeof t ? e === t : "object" == typeof e && "object" == typeof t && function(e, t, r = (e, t) => e === t) {
                     return e.length === t.length && e.every((e, n) => r(e, t[n]))
                 }(e, t)
             }
-            let x = {
+            let _ = {
                     horizontal: {
                         offset: e => ({
                             left: `${e}%`
                         }),
                         leap: e => ({
                             width: `${e}%`
                         })
@@ -118,38 +118,38 @@
                             bottom: `${e}%`
                         }),
                         leap: e => ({
                             height: `${e}%`
                         })
                     }
                 },
-                _ = e => e;
+                x = e => e;
 
             function A() {
                 return void 0 === n && (n = "undefined" == typeof CSS || "function" != typeof CSS.supports || CSS.supports("touch-action", "none")), n
             }
             var T = r(1796),
-                C = r(1657),
+                j = r(1657),
                 E = r(948),
                 L = r(2734),
-                R = e => !e || !(0, c.Z)(e),
-                j = r(8216),
+                C = e => !e || !(0, c.Z)(e),
+                R = r(8216),
                 M = r(1588),
                 I = r(4867);
 
             function Z(e) {
                 return (0, I.Z)("MuiSlider", e)
             }
             let z = (0, M.Z)("MuiSlider", ["root", "active", "colorPrimary", "colorSecondary", "disabled", "dragging", "focusVisible", "mark", "markActive", "marked", "markLabel", "markLabelActive", "rail", "sizeSmall", "thumb", "thumbColorPrimary", "thumbColorSecondary", "track", "trackInverted", "trackFalse", "thumbSizeSmall", "valueLabel", "valueLabelOpen", "valueLabelCircle", "valueLabelLabel", "vertical"]);
             var D = r(5893);
             let N = e => {
                     let {
                         open: t
                     } = e, r = {
-                        offset: (0, i.Z)(t && z.valueLabelOpen),
+                        offset: (0, l.Z)(t && z.valueLabelOpen),
                         circle: z.valueLabelCircle,
                         label: z.valueLabelLabel
                     };
                     return r
                 },
                 U = ["aria-label", "aria-valuetext", "aria-labelledby", "component", "components", "componentsProps", "color", "classes", "className", "disableSwap", "disabled", "getAriaLabel", "getAriaValueText", "marks", "max", "min", "name", "onChange", "onChangeCommitted", "orientation", "size", "step", "scale", "slotProps", "slots", "tabIndex", "track", "value", "valueLabelDisplay", "valueLabelFormat"];
 
@@ -159,40 +159,40 @@
             let H = (0, E.ZP)("span", {
                     name: "MuiSlider",
                     slot: "Root",
                     overridesResolver: (e, t) => {
                         let {
                             ownerState: r
                         } = e;
-                        return [t.root, t[`color${(0,j.Z)(r.color)}`], "medium" !== r.size && t[`size${(0,j.Z)(r.size)}`], r.marked && t.marked, "vertical" === r.orientation && t.vertical, "inverted" === r.track && t.trackInverted, !1 === r.track && t.trackFalse]
+                        return [t.root, t[`color${(0,R.Z)(r.color)}`], "medium" !== r.size && t[`size${(0,R.Z)(r.size)}`], r.marked && t.marked, "vertical" === r.orientation && t.vertical, "inverted" === r.track && t.trackInverted, !1 === r.track && t.trackFalse]
                     }
                 })(({
                     theme: e,
                     ownerState: t
-                }) => (0, o.Z)({
+                }) => (0, a.Z)({
                     borderRadius: 12,
                     boxSizing: "content-box",
                     display: "inline-block",
                     position: "relative",
                     cursor: "pointer",
                     touchAction: "none",
                     color: (e.vars || e).palette[t.color].main,
                     WebkitTapHighlightColor: "transparent"
-                }, "horizontal" === t.orientation && (0, o.Z)({
+                }, "horizontal" === t.orientation && (0, a.Z)({
                     height: 4,
                     width: "100%",
                     padding: "13px 0",
                     "@media (pointer: coarse)": {
                         padding: "20px 0"
                     }
                 }, "small" === t.size && {
                     height: 2
                 }, t.marked && {
                     marginBottom: 20
-                }), "vertical" === t.orientation && (0, o.Z)({
+                }), "vertical" === t.orientation && (0, a.Z)({
                     height: "100%",
                     width: 4,
                     padding: "0 13px",
                     "@media (pointer: coarse)": {
                         padding: "0 20px"
                     }
                 }, "small" === t.size && {
@@ -216,15 +216,15 @@
                 })),
                 V = (0, E.ZP)("span", {
                     name: "MuiSlider",
                     slot: "Rail",
                     overridesResolver: (e, t) => t.rail
                 })(({
                     ownerState: e
-                }) => (0, o.Z)({
+                }) => (0, a.Z)({
                     display: "block",
                     position: "absolute",
                     borderRadius: "inherit",
                     backgroundColor: "currentColor",
                     opacity: .38
                 }, "horizontal" === e.orientation && {
                     width: "100%",
@@ -244,15 +244,15 @@
                     slot: "Track",
                     overridesResolver: (e, t) => t.track
                 })(({
                     theme: e,
                     ownerState: t
                 }) => {
                     let r = "light" === e.palette.mode ? (0, T.$n)(e.palette[t.color].main, .62) : (0, T._j)(e.palette[t.color].main, .5);
-                    return (0, o.Z)({
+                    return (0, a.Z)({
                         display: "block",
                         position: "absolute",
                         borderRadius: "inherit",
                         border: "1px solid currentColor",
                         backgroundColor: "currentColor",
                         transition: e.transitions.create(["left", "width", "bottom", "height"], {
                             duration: e.transitions.duration.shortest
@@ -277,20 +277,20 @@
                 B = (0, E.ZP)("span", {
                     name: "MuiSlider",
                     slot: "Thumb",
                     overridesResolver: (e, t) => {
                         let {
                             ownerState: r
                         } = e;
-                        return [t.thumb, t[`thumbColor${(0,j.Z)(r.color)}`], "medium" !== r.size && t[`thumbSize${(0,j.Z)(r.size)}`]]
+                        return [t.thumb, t[`thumbColor${(0,R.Z)(r.color)}`], "medium" !== r.size && t[`thumbSize${(0,R.Z)(r.size)}`]]
                     }
                 })(({
                     theme: e,
                     ownerState: t
-                }) => (0, o.Z)({
+                }) => (0, a.Z)({
                     position: "absolute",
                     width: 20,
                     height: 20,
                     boxSizing: "border-box",
                     borderRadius: "50%",
                     outline: 0,
                     backgroundColor: "currentColor",
@@ -306,15 +306,15 @@
                 }, "horizontal" === t.orientation && {
                     top: "50%",
                     transform: "translate(-50%, -50%)"
                 }, "vertical" === t.orientation && {
                     left: "50%",
                     transform: "translate(-50%, 50%)"
                 }, {
-                    "&:before": (0, o.Z)({
+                    "&:before": (0, a.Z)({
                         position: "absolute",
                         content: '""',
                         borderRadius: "inherit",
                         width: "100%",
                         height: "100%",
                         boxShadow: (e.vars || e).shadows[2]
                     }, "small" === t.size && {
@@ -346,38 +346,38 @@
                     }
                 })),
                 W = (0, E.ZP)(function(e) {
                     let {
                         children: t,
                         className: r,
                         value: n
-                    } = e, a = N(e);
-                    return t ? l.cloneElement(t, {
-                        className: (0, i.Z)(t.props.className)
-                    }, (0, D.jsxs)(l.Fragment, {
+                    } = e, o = N(e);
+                    return t ? i.cloneElement(t, {
+                        className: (0, l.Z)(t.props.className)
+                    }, (0, D.jsxs)(i.Fragment, {
                         children: [t.props.children, (0, D.jsx)("span", {
-                            className: (0, i.Z)(a.offset, r),
+                            className: (0, l.Z)(o.offset, r),
                             "aria-hidden": !0,
                             children: (0, D.jsx)("span", {
-                                className: a.circle,
+                                className: o.circle,
                                 children: (0, D.jsx)("span", {
-                                    className: a.label,
+                                    className: o.label,
                                     children: n
                                 })
                             })
                         })]
                     })) : null
                 }, {
                     name: "MuiSlider",
                     slot: "ValueLabel",
                     overridesResolver: (e, t) => t.valueLabel
                 })(({
                     theme: e,
                     ownerState: t
-                }) => (0, o.Z)({
+                }) => (0, a.Z)({
                     [`&.${z.valueLabelOpen}`]: {
                         transform: `${"vertical"===t.orientation?"translateY(-50%)":"translateY(-100%)"} scale(1)`
                     },
                     zIndex: 1,
                     whiteSpace: "nowrap"
                 }, e.typography.body2, {
                     fontWeight: 500,
@@ -434,15 +434,15 @@
                         } = e;
                         return [t.mark, r && t.markActive]
                     }
                 })(({
                     theme: e,
                     ownerState: t,
                     markActive: r
-                }) => (0, o.Z)({
+                }) => (0, a.Z)({
                     position: "absolute",
                     width: 2,
                     height: 2,
                     borderRadius: 1,
                     backgroundColor: "currentColor"
                 }, "horizontal" === t.orientation && {
                     top: "50%",
@@ -459,15 +459,15 @@
                     slot: "MarkLabel",
                     shouldForwardProp: e => (0, E.Dz)(e) && "markLabelActive" !== e,
                     overridesResolver: (e, t) => t.markLabel
                 })(({
                     theme: e,
                     ownerState: t,
                     markLabelActive: r
-                }) => (0, o.Z)({}, e.typography.body2, {
+                }) => (0, a.Z)({}, e.typography.body2, {
                     color: (e.vars || e).palette.text.secondary,
                     position: "absolute",
                     whiteSpace: "nowrap"
                 }, "horizontal" === t.orientation && {
                     top: 30,
                     transform: "translateX(-50%)",
                     "@media (pointer: coarse)": {
@@ -483,87 +483,87 @@
                     color: (e.vars || e).palette.text.primary
                 })),
                 K = e => {
                     let {
                         disabled: t,
                         dragging: r,
                         marked: n,
-                        orientation: a,
-                        track: o,
-                        classes: l,
-                        color: i,
+                        orientation: o,
+                        track: a,
+                        classes: i,
+                        color: l,
                         size: s
                     } = e, c = {
-                        root: ["root", t && "disabled", r && "dragging", n && "marked", "vertical" === a && "vertical", "inverted" === o && "trackInverted", !1 === o && "trackFalse", i && `color${(0,j.Z)(i)}`, s && `size${(0,j.Z)(s)}`],
+                        root: ["root", t && "disabled", r && "dragging", n && "marked", "vertical" === o && "vertical", "inverted" === a && "trackInverted", !1 === a && "trackFalse", l && `color${(0,R.Z)(l)}`, s && `size${(0,R.Z)(s)}`],
                         rail: ["rail"],
                         track: ["track"],
                         mark: ["mark"],
                         markActive: ["markActive"],
                         markLabel: ["markLabel"],
                         markLabelActive: ["markLabelActive"],
                         valueLabel: ["valueLabel"],
-                        thumb: ["thumb", t && "disabled", s && `thumbSize${(0,j.Z)(s)}`, i && `thumbColor${(0,j.Z)(i)}`],
+                        thumb: ["thumb", t && "disabled", s && `thumbSize${(0,R.Z)(s)}`, l && `thumbColor${(0,R.Z)(l)}`],
                         active: ["active"],
                         disabled: ["disabled"],
                         focusVisible: ["focusVisible"]
                     };
-                    return (0, u.Z)(c, Z, l)
+                    return (0, u.Z)(c, Z, i)
                 },
                 q = ({
                     children: e
                 }) => e,
-                J = l.forwardRef(function(e, t) {
-                    var r, n, u, T, E, j, M, I, Z, z, N, J, G, Q, ee, et, er, en, ea, eo, el, ei, eu, es;
-                    let ec = (0, C.Z)({
+                J = i.forwardRef(function(e, t) {
+                    var r, n, u, T, E, R, M, I, Z, z, N, J, G, Q, ee, et, er, en, eo, ea, ei, el, eu, es;
+                    let ec = (0, j.Z)({
                             props: e,
                             name: "MuiSlider"
                         }),
-                        ed = (0, L.Z)(),
-                        ef = "rtl" === ed.direction,
+                        ef = (0, L.Z)(),
+                        ed = "rtl" === ef.direction,
                         {
                             "aria-label": ep,
                             "aria-valuetext": ey,
                             "aria-labelledby": eh,
-                            component: em = "span",
-                            components: ev = {},
+                            component: ev = "span",
+                            components: em = {},
                             componentsProps: eb = {},
                             color: eg = "primary",
                             classes: eP,
                             className: ew,
                             disableSwap: ek = !1,
-                            disabled: eS = !1,
-                            getAriaLabel: eO,
-                            getAriaValueText: ex,
-                            marks: e_ = !1,
+                            disabled: eO = !1,
+                            getAriaLabel: eS,
+                            getAriaValueText: e_,
+                            marks: ex = !1,
                             max: eA = 100,
                             min: eT = 0,
-                            orientation: eC = "horizontal",
+                            orientation: ej = "horizontal",
                             size: eE = "medium",
                             step: eL = 1,
-                            scale: eR = $,
-                            slotProps: ej,
+                            scale: eC = $,
+                            slotProps: eR,
                             slots: eM,
                             track: eI = "normal",
                             valueLabelDisplay: eZ = "off",
                             valueLabelFormat: ez = $
                         } = ec,
-                        eD = (0, a.Z)(ec, U),
-                        eN = (0, o.Z)({}, ec, {
-                            isRtl: ef,
+                        eD = (0, o.Z)(ec, U),
+                        eN = (0, a.Z)({}, ec, {
+                            isRtl: ed,
                             max: eA,
                             min: eT,
                             classes: eP,
-                            disabled: eS,
+                            disabled: eO,
                             disableSwap: ek,
-                            orientation: eC,
-                            marks: e_,
+                            orientation: ej,
+                            marks: ex,
                             color: eg,
                             size: eE,
                             step: eL,
-                            scale: eR,
+                            scale: eC,
                             track: eI,
                             valueLabelDisplay: eZ,
                             valueLabelFormat: ez
                         }),
                         {
                             axisProps: eU,
                             getRootProps: e$,
@@ -574,123 +574,124 @@
                             axis: eW,
                             focusedThumbIndex: eX,
                             range: eY,
                             dragging: eK,
                             marks: eq,
                             values: eJ,
                             trackOffset: eG,
-                            trackLeap: eQ
+                            trackLeap: eQ,
+                            getThumbStyle: e0
                         } = function(e) {
                             let {
                                 "aria-labelledby": t,
                                 defaultValue: r,
                                 disabled: n = !1,
-                                disableSwap: a = !1,
-                                isRtl: i = !1,
+                                disableSwap: o = !1,
+                                isRtl: l = !1,
                                 marks: u = !1,
                                 max: s = 100,
                                 min: c = 0,
                                 name: T,
-                                onChange: C,
+                                onChange: j,
                                 onChangeCommitted: E,
                                 orientation: L = "horizontal",
-                                rootRef: R,
-                                scale: j = _,
+                                rootRef: C,
+                                scale: R = x,
                                 step: M = 1,
                                 tabIndex: I,
                                 value: Z
-                            } = e, z = l.useRef(), [D, N] = l.useState(-1), [U, $] = l.useState(-1), [H, V] = l.useState(!1), F = l.useRef(0), [B, W] = (0, f.Z)({
+                            } = e, z = i.useRef(), [D, N] = i.useState(-1), [U, $] = i.useState(-1), [H, V] = i.useState(!1), F = i.useRef(0), [B, W] = (0, d.Z)({
                                 controlled: Z,
                                 default: null != r ? r : c,
                                 name: "Slider"
-                            }), X = C && ((e, t, r) => {
+                            }), X = j && ((e, t, r) => {
                                 let n = e.nativeEvent || e,
-                                    a = new n.constructor(n.type, n);
-                                Object.defineProperty(a, "target", {
+                                    o = new n.constructor(n.type, n);
+                                Object.defineProperty(o, "target", {
                                     writable: !0,
                                     value: {
                                         value: t,
                                         name: T
                                     }
-                                }), C(a, t, r)
+                                }), j(o, t, r)
                             }), Y = Array.isArray(B), K = Y ? B.slice().sort(b) : [B];
                             K = K.map(e => g(e, c, s));
                             let q = !0 === u && null !== M ? [...Array(Math.floor((s - c) / M) + 1)].map((e, t) => ({
                                     value: c + M * t
                                 })) : u || [],
                                 J = q.map(e => e.value),
                                 {
                                     isFocusVisibleRef: G,
                                     onBlur: Q,
                                     onFocus: ee,
                                     ref: et
                                 } = (0, p.Z)(),
-                                [er, en] = l.useState(-1),
-                                ea = l.useRef(),
-                                eo = (0, y.Z)(et, ea),
-                                el = (0, y.Z)(R, eo),
-                                ei = e => t => {
+                                [er, en] = i.useState(-1),
+                                eo = i.useRef(),
+                                ea = (0, y.Z)(et, eo),
+                                ei = (0, y.Z)(C, ea),
+                                el = e => t => {
                                     var r;
                                     let n = Number(t.currentTarget.getAttribute("data-index"));
                                     ee(t), !0 === G.current && en(n), $(n), null == e || null == (r = e.onFocus) || r.call(e, t)
                                 },
                                 eu = e => t => {
                                     var r;
                                     Q(t), !1 === G.current && en(-1), $(-1), null == e || null == (r = e.onBlur) || r.call(e, t)
                                 };
                             (0, h.Z)(() => {
-                                if (n && ea.current.contains(document.activeElement)) {
+                                if (n && eo.current.contains(document.activeElement)) {
                                     var e;
                                     null == (e = document.activeElement) || e.blur()
                                 }
                             }, [n]), n && -1 !== D && N(-1), n && -1 !== er && en(-1);
                             let es = e => t => {
                                     var r;
                                     null == (r = e.onChange) || r.call(e, t);
                                     let n = Number(t.currentTarget.getAttribute("data-index")),
-                                        o = K[n],
-                                        l = J.indexOf(o),
-                                        i = t.target.valueAsNumber;
+                                        a = K[n],
+                                        i = J.indexOf(a),
+                                        l = t.target.valueAsNumber;
                                     if (q && null == M) {
                                         let e = J[J.length - 1];
-                                        i = i > e ? e : i < J[0] ? J[0] : i < o ? J[l - 1] : J[l + 1]
+                                        l = l > e ? e : l < J[0] ? J[0] : l < a ? J[i - 1] : J[i + 1]
                                     }
-                                    if (i = g(i, c, s), Y) {
-                                        a && (i = g(i, K[n - 1] || -1 / 0, K[n + 1] || 1 / 0));
-                                        let e = i;
-                                        i = k({
+                                    if (l = g(l, c, s), Y) {
+                                        o && (l = g(l, K[n - 1] || -1 / 0, K[n + 1] || 1 / 0));
+                                        let e = l;
+                                        l = k({
                                             values: K,
-                                            newValue: i,
+                                            newValue: l,
                                             index: n
                                         });
                                         let t = n;
-                                        a || (t = i.indexOf(e)), S({
-                                            sliderRef: ea,
+                                        o || (t = l.indexOf(e)), O({
+                                            sliderRef: eo,
                                             activeIndex: t
                                         })
                                     }
-                                    W(i), en(n), X && !O(i, B) && X(t, i, n), E && E(t, i)
+                                    W(l), en(n), X && !S(l, B) && X(t, l, n), E && E(t, l)
                                 },
-                                ec = l.useRef(),
-                                ed = L;
-                            i && "horizontal" === L && (ed += "-reverse");
-                            let ef = ({
+                                ec = i.useRef(),
+                                ef = L;
+                            l && "horizontal" === L && (ef += "-reverse");
+                            let ed = ({
                                     finger: e,
                                     move: t = !1
                                 }) => {
                                     let r, n;
                                     let {
-                                        current: o
-                                    } = ea, {
-                                        width: l,
-                                        height: i,
+                                        current: a
+                                    } = eo, {
+                                        width: i,
+                                        height: l,
                                         bottom: u,
-                                        left: d
-                                    } = o.getBoundingClientRect();
-                                    if (r = 0 === ed.indexOf("vertical") ? (u - e.y) / i : (e.x - d) / l, -1 !== ed.indexOf("-reverse") && (r = 1 - r), n = (s - c) * r + c, M) n = function(e, t, r) {
+                                        left: f
+                                    } = a.getBoundingClientRect();
+                                    if (r = 0 === ef.indexOf("vertical") ? (u - e.y) / l : (e.x - f) / i, -1 !== ef.indexOf("-reverse") && (r = 1 - r), n = (s - c) * r + c, M) n = function(e, t, r) {
                                         let n = Math.round((e - r) / t) * t + r;
                                         return Number(n.toFixed(function(e) {
                                             if (1 > Math.abs(e)) {
                                                 let t = e.toExponential().split("e-"),
                                                     r = t[0].split(".")[1];
                                                 return (r ? r.length : 0) + parseInt(t[1], 10)
                                             }
@@ -699,122 +700,122 @@
                                         }(t)))
                                     }(n, M, c);
                                     else {
                                         let e = P(J, n);
                                         n = J[e]
                                     }
                                     n = g(n, c, s);
-                                    let f = 0;
+                                    let d = 0;
                                     if (Y) {
-                                        f = t ? ec.current : P(K, n), a && (n = g(n, K[f - 1] || -1 / 0, K[f + 1] || 1 / 0));
+                                        d = t ? ec.current : P(K, n), o && (n = g(n, K[d - 1] || -1 / 0, K[d + 1] || 1 / 0));
                                         let e = n;
                                         n = k({
                                             values: K,
                                             newValue: n,
-                                            index: f
-                                        }), a && t || (f = n.indexOf(e), ec.current = f)
+                                            index: d
+                                        }), o && t || (d = n.indexOf(e), ec.current = d)
                                     }
                                     return {
                                         newValue: n,
-                                        activeIndex: f
+                                        activeIndex: d
                                     }
                                 },
-                                ep = (0, m.Z)(e => {
+                                ep = (0, v.Z)(e => {
                                     let t = w(e, z);
                                     if (!t) return;
                                     if (F.current += 1, "mousemove" === e.type && 0 === e.buttons) {
                                         ey(e);
                                         return
                                     }
                                     let {
                                         newValue: r,
                                         activeIndex: n
-                                    } = ef({
+                                    } = ed({
                                         finger: t,
                                         move: !0
                                     });
-                                    S({
-                                        sliderRef: ea,
+                                    O({
+                                        sliderRef: eo,
                                         activeIndex: n,
                                         setActive: N
-                                    }), W(r), !H && F.current > 2 && V(!0), X && !O(r, B) && X(e, r, n)
+                                    }), W(r), !H && F.current > 2 && V(!0), X && !S(r, B) && X(e, r, n)
                                 }),
-                                ey = (0, m.Z)(e => {
+                                ey = (0, v.Z)(e => {
                                     let t = w(e, z);
                                     if (V(!1), !t) return;
                                     let {
                                         newValue: r
-                                    } = ef({
+                                    } = ed({
                                         finger: t,
                                         move: !0
                                     });
-                                    N(-1), "touchend" === e.type && $(-1), E && E(e, r), z.current = void 0, em()
+                                    N(-1), "touchend" === e.type && $(-1), E && E(e, r), z.current = void 0, ev()
                                 }),
-                                eh = (0, m.Z)(e => {
+                                eh = (0, v.Z)(e => {
                                     if (n) return;
                                     A() || e.preventDefault();
                                     let t = e.changedTouches[0];
                                     null != t && (z.current = t.identifier);
                                     let r = w(e, z);
                                     if (!1 !== r) {
                                         let {
                                             newValue: t,
                                             activeIndex: n
-                                        } = ef({
+                                        } = ed({
                                             finger: r
                                         });
-                                        S({
-                                            sliderRef: ea,
+                                        O({
+                                            sliderRef: eo,
                                             activeIndex: n,
                                             setActive: N
-                                        }), W(t), X && !O(t, B) && X(e, t, n)
+                                        }), W(t), X && !S(t, B) && X(e, t, n)
                                     }
                                     F.current = 0;
-                                    let a = (0, d.Z)(ea.current);
-                                    a.addEventListener("touchmove", ep), a.addEventListener("touchend", ey)
+                                    let o = (0, f.Z)(eo.current);
+                                    o.addEventListener("touchmove", ep), o.addEventListener("touchend", ey)
                                 }),
-                                em = l.useCallback(() => {
-                                    let e = (0, d.Z)(ea.current);
+                                ev = i.useCallback(() => {
+                                    let e = (0, f.Z)(eo.current);
                                     e.removeEventListener("mousemove", ep), e.removeEventListener("mouseup", ey), e.removeEventListener("touchmove", ep), e.removeEventListener("touchend", ey)
                                 }, [ey, ep]);
-                            l.useEffect(() => {
+                            i.useEffect(() => {
                                 let {
                                     current: e
-                                } = ea;
+                                } = eo;
                                 return e.addEventListener("touchstart", eh, {
                                     passive: A()
                                 }), () => {
                                     e.removeEventListener("touchstart", eh, {
                                         passive: A()
-                                    }), em()
+                                    }), ev()
                                 }
-                            }, [em, eh]), l.useEffect(() => {
-                                n && em()
-                            }, [n, em]);
-                            let ev = e => t => {
+                            }, [ev, eh]), i.useEffect(() => {
+                                n && ev()
+                            }, [n, ev]);
+                            let em = e => t => {
                                     var r;
                                     if (null == (r = e.onMouseDown) || r.call(e, t), n || t.defaultPrevented || 0 !== t.button) return;
                                     t.preventDefault();
-                                    let a = w(t, z);
-                                    if (!1 !== a) {
+                                    let o = w(t, z);
+                                    if (!1 !== o) {
                                         let {
                                             newValue: e,
                                             activeIndex: r
-                                        } = ef({
-                                            finger: a
+                                        } = ed({
+                                            finger: o
                                         });
-                                        S({
-                                            sliderRef: ea,
+                                        O({
+                                            sliderRef: eo,
                                             activeIndex: r,
                                             setActive: N
-                                        }), W(e), X && !O(e, B) && X(t, e, r)
+                                        }), W(e), X && !S(e, B) && X(t, e, r)
                                     }
                                     F.current = 0;
-                                    let o = (0, d.Z)(ea.current);
-                                    o.addEventListener("mousemove", ep), o.addEventListener("mouseup", ey)
+                                    let a = (0, f.Z)(eo.current);
+                                    a.addEventListener("mousemove", ep), a.addEventListener("mouseup", ey)
                                 },
                                 eb = ((Y ? K[0] : c) - c) * 100 / (s - c),
                                 eg = (K[K.length - 1] - c) * 100 / (s - c) - eb,
                                 eP = e => t => {
                                     var r;
                                     null == (r = e.onMouseOver) || r.call(e, t);
                                     let n = Number(t.currentTarget.getAttribute("data-index"));
@@ -822,199 +823,200 @@
                                 },
                                 ew = e => t => {
                                     var r;
                                     null == (r = e.onMouseLeave) || r.call(e, t), $(-1)
                                 };
                             return {
                                 active: D,
-                                axis: ed,
-                                axisProps: x,
+                                axis: ef,
+                                axisProps: _,
                                 dragging: H,
                                 focusedThumbIndex: er,
                                 getHiddenInputProps: (r = {}) => {
-                                    var a;
-                                    let l = {
+                                    var o;
+                                    let i = {
                                             onChange: es(r || {}),
-                                            onFocus: ei(r || {}),
+                                            onFocus: el(r || {}),
                                             onBlur: eu(r || {})
                                         },
-                                        u = (0, o.Z)({}, r, l);
-                                    return (0, o.Z)({
+                                        u = (0, a.Z)({}, r, i);
+                                    return (0, a.Z)({
                                         tabIndex: I,
                                         "aria-labelledby": t,
                                         "aria-orientation": L,
-                                        "aria-valuemax": j(s),
-                                        "aria-valuemin": j(c),
+                                        "aria-valuemax": R(s),
+                                        "aria-valuemin": R(c),
                                         name: T,
                                         type: "range",
                                         min: e.min,
                                         max: e.max,
-                                        step: null === e.step && e.marks ? "any" : null != (a = e.step) ? a : void 0,
+                                        step: null === e.step && e.marks ? "any" : null != (o = e.step) ? o : void 0,
                                         disabled: n
                                     }, u, {
-                                        style: (0, o.Z)({}, v, {
-                                            direction: i ? "rtl" : "ltr",
+                                        style: (0, a.Z)({}, m, {
+                                            direction: l ? "rtl" : "ltr",
                                             width: "100%",
                                             height: "100%"
                                         })
                                     })
                                 },
                                 getRootProps: (e = {}) => {
                                     let t = {
-                                            onMouseDown: ev(e || {})
+                                            onMouseDown: em(e || {})
                                         },
-                                        r = (0, o.Z)({}, e, t);
-                                    return (0, o.Z)({
-                                        ref: el
+                                        r = (0, a.Z)({}, e, t);
+                                    return (0, a.Z)({
+                                        ref: ei
                                     }, r)
                                 },
                                 getThumbProps: (e = {}) => {
                                     let t = {
                                         onMouseOver: eP(e || {}),
                                         onMouseLeave: ew(e || {})
                                     };
-                                    return (0, o.Z)({}, e, t)
+                                    return (0, a.Z)({}, e, t)
                                 },
                                 marks: q,
                                 open: U,
                                 range: Y,
-                                rootRef: el,
+                                rootRef: ei,
                                 trackLeap: eg,
                                 trackOffset: eb,
-                                values: K
+                                values: K,
+                                getThumbStyle: e => ({
+                                    pointerEvents: -1 !== D && D !== e ? "none" : void 0
+                                })
                             }
-                        }((0, o.Z)({}, eN, {
+                        }((0, a.Z)({}, eN, {
                             rootRef: t
                         }));
                     eN.marked = eq.length > 0 && eq.some(e => e.label), eN.dragging = eK, eN.focusedThumbIndex = eX;
-                    let e0 = K(eN),
-                        e1 = null != (r = null != (n = null == eM ? void 0 : eM.root) ? n : ev.Root) ? r : H,
-                        e5 = null != (u = null != (T = null == eM ? void 0 : eM.rail) ? T : ev.Rail) ? u : V,
-                        e9 = null != (E = null != (j = null == eM ? void 0 : eM.track) ? j : ev.Track) ? E : F,
-                        e2 = null != (M = null != (I = null == eM ? void 0 : eM.thumb) ? I : ev.Thumb) ? M : B,
-                        e6 = null != (Z = null != (z = null == eM ? void 0 : eM.valueLabel) ? z : ev.ValueLabel) ? Z : W,
-                        e4 = null != (N = null != (J = null == eM ? void 0 : eM.mark) ? J : ev.Mark) ? N : X,
-                        e3 = null != (G = null != (Q = null == eM ? void 0 : eM.markLabel) ? Q : ev.MarkLabel) ? G : Y,
-                        e8 = null != (ee = null != (et = null == eM ? void 0 : eM.input) ? et : ev.Input) ? ee : "input",
-                        e7 = null != (er = null == ej ? void 0 : ej.root) ? er : eb.root,
-                        te = null != (en = null == ej ? void 0 : ej.rail) ? en : eb.rail,
-                        tt = null != (ea = null == ej ? void 0 : ej.track) ? ea : eb.track,
-                        tr = null != (eo = null == ej ? void 0 : ej.thumb) ? eo : eb.thumb,
-                        tn = null != (el = null == ej ? void 0 : ej.valueLabel) ? el : eb.valueLabel,
-                        ta = null != (ei = null == ej ? void 0 : ej.mark) ? ei : eb.mark,
-                        to = null != (eu = null == ej ? void 0 : ej.markLabel) ? eu : eb.markLabel,
-                        tl = null != (es = null == ej ? void 0 : ej.input) ? es : eb.input,
-                        ti = (0, s.Z)({
-                            elementType: e1,
+                    let e1 = K(eN),
+                        e9 = null != (r = null != (n = null == eM ? void 0 : eM.root) ? n : em.Root) ? r : H,
+                        e5 = null != (u = null != (T = null == eM ? void 0 : eM.rail) ? T : em.Rail) ? u : V,
+                        e4 = null != (E = null != (R = null == eM ? void 0 : eM.track) ? R : em.Track) ? E : F,
+                        e2 = null != (M = null != (I = null == eM ? void 0 : eM.thumb) ? I : em.Thumb) ? M : B,
+                        e6 = null != (Z = null != (z = null == eM ? void 0 : eM.valueLabel) ? z : em.ValueLabel) ? Z : W,
+                        e8 = null != (N = null != (J = null == eM ? void 0 : eM.mark) ? J : em.Mark) ? N : X,
+                        e3 = null != (G = null != (Q = null == eM ? void 0 : eM.markLabel) ? Q : em.MarkLabel) ? G : Y,
+                        e7 = null != (ee = null != (et = null == eM ? void 0 : eM.input) ? et : em.Input) ? ee : "input",
+                        te = null != (er = null == eR ? void 0 : eR.root) ? er : eb.root,
+                        tt = null != (en = null == eR ? void 0 : eR.rail) ? en : eb.rail,
+                        tr = null != (eo = null == eR ? void 0 : eR.track) ? eo : eb.track,
+                        tn = null != (ea = null == eR ? void 0 : eR.thumb) ? ea : eb.thumb,
+                        to = null != (ei = null == eR ? void 0 : eR.valueLabel) ? ei : eb.valueLabel,
+                        ta = null != (el = null == eR ? void 0 : eR.mark) ? el : eb.mark,
+                        ti = null != (eu = null == eR ? void 0 : eR.markLabel) ? eu : eb.markLabel,
+                        tl = null != (es = null == eR ? void 0 : eR.input) ? es : eb.input,
+                        tu = (0, s.Z)({
+                            elementType: e9,
                             getSlotProps: e$,
-                            externalSlotProps: e7,
+                            externalSlotProps: te,
                             externalForwardedProps: eD,
-                            additionalProps: (0, o.Z)({}, R(e1) && {
-                                as: em
+                            additionalProps: (0, a.Z)({}, C(e9) && {
+                                as: ev
                             }),
-                            ownerState: (0, o.Z)({}, eN, null == e7 ? void 0 : e7.ownerState),
-                            className: [e0.root, ew]
+                            ownerState: (0, a.Z)({}, eN, null == te ? void 0 : te.ownerState),
+                            className: [e1.root, ew]
                         }),
-                        tu = (0, s.Z)({
+                        ts = (0, s.Z)({
                             elementType: e5,
-                            externalSlotProps: te,
+                            externalSlotProps: tt,
                             ownerState: eN,
-                            className: e0.rail
+                            className: e1.rail
                         }),
-                        ts = (0, s.Z)({
-                            elementType: e9,
-                            externalSlotProps: tt,
+                        tc = (0, s.Z)({
+                            elementType: e4,
+                            externalSlotProps: tr,
                             additionalProps: {
-                                style: (0, o.Z)({}, eU[eW].offset(eG), eU[eW].leap(eQ))
+                                style: (0, a.Z)({}, eU[eW].offset(eG), eU[eW].leap(eQ))
                             },
-                            ownerState: (0, o.Z)({}, eN, null == tt ? void 0 : tt.ownerState),
-                            className: e0.track
+                            ownerState: (0, a.Z)({}, eN, null == tr ? void 0 : tr.ownerState),
+                            className: e1.track
                         }),
-                        tc = (0, s.Z)({
+                        tf = (0, s.Z)({
                             elementType: e2,
                             getSlotProps: eV,
-                            externalSlotProps: tr,
-                            ownerState: (0, o.Z)({}, eN, null == tr ? void 0 : tr.ownerState),
-                            className: e0.thumb
+                            externalSlotProps: tn,
+                            ownerState: (0, a.Z)({}, eN, null == tn ? void 0 : tn.ownerState),
+                            className: e1.thumb
                         }),
                         td = (0, s.Z)({
                             elementType: e6,
-                            externalSlotProps: tn,
-                            ownerState: (0, o.Z)({}, eN, null == tn ? void 0 : tn.ownerState),
-                            className: e0.valueLabel
+                            externalSlotProps: to,
+                            ownerState: (0, a.Z)({}, eN, null == to ? void 0 : to.ownerState),
+                            className: e1.valueLabel
                         }),
-                        tf = (0, s.Z)({
-                            elementType: e4,
+                        tp = (0, s.Z)({
+                            elementType: e8,
                             externalSlotProps: ta,
                             ownerState: eN,
-                            className: e0.mark
+                            className: e1.mark
                         }),
-                        tp = (0, s.Z)({
+                        ty = (0, s.Z)({
                             elementType: e3,
-                            externalSlotProps: to,
+                            externalSlotProps: ti,
                             ownerState: eN,
-                            className: e0.markLabel
+                            className: e1.markLabel
                         }),
-                        ty = (0, s.Z)({
-                            elementType: e8,
+                        th = (0, s.Z)({
+                            elementType: e7,
                             getSlotProps: eH,
                             externalSlotProps: tl,
                             ownerState: eN
                         });
-                    return (0, D.jsxs)(e1, (0, o.Z)({}, ti, {
-                        children: [(0, D.jsx)(e5, (0, o.Z)({}, tu)), (0, D.jsx)(e9, (0, o.Z)({}, ts)), eq.filter(e => e.value >= eT && e.value <= eA).map((e, t) => {
+                    return (0, D.jsxs)(e9, (0, a.Z)({}, tu, {
+                        children: [(0, D.jsx)(e5, (0, a.Z)({}, ts)), (0, D.jsx)(e4, (0, a.Z)({}, tc)), eq.filter(e => e.value >= eT && e.value <= eA).map((e, t) => {
                             let r;
                             let n = (e.value - eT) * 100 / (eA - eT),
-                                a = eU[eW].offset(n);
-                            return r = !1 === eI ? -1 !== eJ.indexOf(e.value) : "normal" === eI && (eY ? e.value >= eJ[0] && e.value <= eJ[eJ.length - 1] : e.value <= eJ[0]) || "inverted" === eI && (eY ? e.value <= eJ[0] || e.value >= eJ[eJ.length - 1] : e.value >= eJ[0]), (0, D.jsxs)(l.Fragment, {
-                                children: [(0, D.jsx)(e4, (0, o.Z)({
+                                o = eU[eW].offset(n);
+                            return r = !1 === eI ? -1 !== eJ.indexOf(e.value) : "normal" === eI && (eY ? e.value >= eJ[0] && e.value <= eJ[eJ.length - 1] : e.value <= eJ[0]) || "inverted" === eI && (eY ? e.value <= eJ[0] || e.value >= eJ[eJ.length - 1] : e.value >= eJ[0]), (0, D.jsxs)(i.Fragment, {
+                                children: [(0, D.jsx)(e8, (0, a.Z)({
                                     "data-index": t
-                                }, tf, !(0, c.Z)(e4) && {
+                                }, tp, !(0, c.Z)(e8) && {
                                     markActive: r
                                 }, {
-                                    style: (0, o.Z)({}, a, tf.style),
-                                    className: (0, i.Z)(tf.className, r && e0.markActive)
-                                })), null != e.label ? (0, D.jsx)(e3, (0, o.Z)({
+                                    style: (0, a.Z)({}, o, tp.style),
+                                    className: (0, l.Z)(tp.className, r && e1.markActive)
+                                })), null != e.label ? (0, D.jsx)(e3, (0, a.Z)({
                                     "aria-hidden": !0,
                                     "data-index": t
-                                }, tp, !(0, c.Z)(e3) && {
+                                }, ty, !(0, c.Z)(e3) && {
                                     markLabelActive: r
                                 }, {
-                                    style: (0, o.Z)({}, a, tp.style),
-                                    className: (0, i.Z)(e0.markLabel, tp.className, r && e0.markLabelActive),
+                                    style: (0, a.Z)({}, o, ty.style),
+                                    className: (0, l.Z)(e1.markLabel, ty.className, r && e1.markLabelActive),
                                     children: e.label
                                 })) : null]
                             }, t)
                         }), eJ.map((e, t) => {
                             let r = (e - eT) * 100 / (eA - eT),
                                 n = eU[eW].offset(r),
-                                a = "off" === eZ ? q : e6;
-                            return (0, D.jsx)(a, (0, o.Z)({}, !(0, c.Z)(a) && {
+                                o = "off" === eZ ? q : e6;
+                            return (0, D.jsx)(o, (0, a.Z)({}, !(0, c.Z)(o) && {
                                 valueLabelFormat: ez,
                                 valueLabelDisplay: eZ,
-                                value: "function" == typeof ez ? ez(eR(e), t) : ez,
+                                value: "function" == typeof ez ? ez(eC(e), t) : ez,
                                 index: t,
                                 open: eF === t || eB === t || "on" === eZ,
-                                disabled: eS
+                                disabled: eO
                             }, td, {
-                                children: (0, D.jsx)(e2, (0, o.Z)({
+                                children: (0, D.jsx)(e2, (0, a.Z)({
                                     "data-index": t
-                                }, tc, {
-                                    className: (0, i.Z)(e0.thumb, tc.className, eB === t && e0.active, eX === t && e0.focusVisible),
-                                    style: (0, o.Z)({}, n, {
-                                        pointerEvents: ek && eB !== t ? "none" : void 0
-                                    }, tc.style),
-                                    children: (0, D.jsx)(e8, (0, o.Z)({
+                                }, tf, {
+                                    className: (0, l.Z)(e1.thumb, tf.className, eB === t && e1.active, eX === t && e1.focusVisible),
+                                    style: (0, a.Z)({}, n, e0(t), tf.style),
+                                    children: (0, D.jsx)(e7, (0, a.Z)({
                                         "data-index": t,
-                                        "aria-label": eO ? eO(t) : ep,
-                                        "aria-valuenow": eR(e),
+                                        "aria-label": eS ? eS(t) : ep,
+                                        "aria-valuenow": eC(e),
                                         "aria-labelledby": eh,
-                                        "aria-valuetext": ex ? ex(eR(e), t) : ey,
+                                        "aria-valuetext": e_ ? e_(eC(e), t) : ey,
                                         value: eJ[t]
-                                    }, ty))
+                                    }, th))
                                 }))
                             }), t)
                         })]
                     }))
                 });
             var G = J
         },
@@ -1023,56 +1025,56 @@
             var t = function(e) {
                     var t;
                     return !!e && "object" == typeof e && "[object RegExp]" !== (t = Object.prototype.toString.call(e)) && "[object Date]" !== t && e.$$typeof !== r
                 },
                 r = "function" == typeof Symbol && Symbol.for ? Symbol.for("react.element") : 60103;
 
             function n(e, t) {
-                return !1 !== t.clone && t.isMergeableObject(e) ? i(Array.isArray(e) ? [] : {}, e, t) : e
+                return !1 !== t.clone && t.isMergeableObject(e) ? l(Array.isArray(e) ? [] : {}, e, t) : e
             }
 
-            function a(e, t, r) {
+            function o(e, t, r) {
                 return e.concat(t).map(function(e) {
                     return n(e, r)
                 })
             }
 
-            function o(e) {
+            function a(e) {
                 return Object.keys(e).concat(Object.getOwnPropertySymbols ? Object.getOwnPropertySymbols(e).filter(function(t) {
                     return e.propertyIsEnumerable(t)
                 }) : [])
             }
 
-            function l(e, t) {
+            function i(e, t) {
                 try {
                     return t in e
                 } catch (e) {
                     return !1
                 }
             }
 
-            function i(e, r, u) {
-                (u = u || {}).arrayMerge = u.arrayMerge || a, u.isMergeableObject = u.isMergeableObject || t, u.cloneUnlessOtherwiseSpecified = n;
-                var s, c, d = Array.isArray(r);
-                return d !== Array.isArray(e) ? n(r, u) : d ? u.arrayMerge(e, r, u) : (c = {}, (s = u).isMergeableObject(e) && o(e).forEach(function(t) {
+            function l(e, r, u) {
+                (u = u || {}).arrayMerge = u.arrayMerge || o, u.isMergeableObject = u.isMergeableObject || t, u.cloneUnlessOtherwiseSpecified = n;
+                var s, c, f = Array.isArray(r);
+                return f !== Array.isArray(e) ? n(r, u) : f ? u.arrayMerge(e, r, u) : (c = {}, (s = u).isMergeableObject(e) && a(e).forEach(function(t) {
                     c[t] = n(e[t], s)
-                }), o(r).forEach(function(t) {
-                    (!l(e, t) || Object.hasOwnProperty.call(e, t) && Object.propertyIsEnumerable.call(e, t)) && (l(e, t) && s.isMergeableObject(r[t]) ? c[t] = (function(e, t) {
-                        if (!t.customMerge) return i;
+                }), a(r).forEach(function(t) {
+                    (!i(e, t) || Object.hasOwnProperty.call(e, t) && Object.propertyIsEnumerable.call(e, t)) && (i(e, t) && s.isMergeableObject(r[t]) ? c[t] = (function(e, t) {
+                        if (!t.customMerge) return l;
                         var r = t.customMerge(e);
-                        return "function" == typeof r ? r : i
+                        return "function" == typeof r ? r : l
                     })(t, s)(e[t], r[t], s) : c[t] = n(r[t], s))
                 }), c)
             }
-            i.all = function(e, t) {
+            l.all = function(e, t) {
                 if (!Array.isArray(e)) throw Error("first argument should be an array");
                 return e.reduce(function(e, r) {
-                    return i(e, r, t)
+                    return l(e, r, t)
                 }, {})
-            }, e.exports = i
+            }, e.exports = l
         },
         9090: function(e) {
             function t(e, t) {
                 e.onload = function() {
                     this.onerror = this.onload = null, t(null, e)
                 }, e.onerror = function() {
                     this.onerror = this.onload = null, t(Error("Failed to load " + this.src), e)
@@ -1080,96 +1082,316 @@
             }
 
             function r(e, t) {
                 e.onreadystatechange = function() {
                     ("complete" == this.readyState || "loaded" == this.readyState) && (this.onreadystatechange = null, t(null, e))
                 }
             }
-            e.exports = function(e, n, a) {
-                var o = document.head || document.getElementsByTagName("head")[0],
-                    l = document.createElement("script");
-                "function" == typeof n && (a = n, n = {}), n = n || {}, a = a || function() {}, l.type = n.type || "text/javascript", l.charset = n.charset || "utf8", l.async = !("async" in n) || !!n.async, l.src = e, n.attrs && function(e, t) {
+            e.exports = function(e, n, o) {
+                var a = document.head || document.getElementsByTagName("head")[0],
+                    i = document.createElement("script");
+                "function" == typeof n && (o = n, n = {}), n = n || {}, o = o || function() {}, i.type = n.type || "text/javascript", i.charset = n.charset || "utf8", i.async = !("async" in n) || !!n.async, i.src = e, n.attrs && function(e, t) {
                     for (var r in t) e.setAttribute(r, t[r])
-                }(l, n.attrs), n.text && (l.text = "" + n.text), ("onload" in l ? t : r)(l, a), l.onload || t(l, a), o.appendChild(l)
+                }(i, n.attrs), n.text && (i.text = "" + n.text), ("onload" in i ? t : r)(i, o), i.onload || t(i, o), a.appendChild(i)
+            }
+        },
+        8668: function(e, t, r) {
+            var n = r(3369),
+                o = r(619),
+                a = r(2385);
+
+            function i(e) {
+                var t = -1,
+                    r = null == e ? 0 : e.length;
+                for (this.__data__ = new n; ++t < r;) this.add(e[t])
+            }
+            i.prototype.add = i.prototype.push = o, i.prototype.has = a, e.exports = i
+        },
+        2908: function(e) {
+            e.exports = function(e, t) {
+                for (var r = -1, n = null == e ? 0 : e.length; ++r < n;)
+                    if (t(e[r], r, e)) return !0;
+                return !1
+            }
+        },
+        939: function(e, t, r) {
+            var n = r(2492),
+                o = r(7005);
+            e.exports = function e(t, r, a, i, l) {
+                return t === r || (null != t && null != r && (o(t) || o(r)) ? n(t, r, a, i, e, l) : t != t && r != r)
+            }
+        },
+        2492: function(e, t, r) {
+            var n = r(6384),
+                o = r(7114),
+                a = r(8351),
+                i = r(6096),
+                l = r(4160),
+                u = r(1469),
+                s = r(4144),
+                c = r(6719),
+                f = "[object Arguments]",
+                d = "[object Array]",
+                p = "[object Object]",
+                y = Object.prototype.hasOwnProperty;
+            e.exports = function(e, t, r, h, v, m) {
+                var b = u(e),
+                    g = u(t),
+                    P = b ? d : l(e),
+                    w = g ? d : l(t);
+                P = P == f ? p : P, w = w == f ? p : w;
+                var k = P == p,
+                    O = w == p,
+                    S = P == w;
+                if (S && s(e)) {
+                    if (!s(t)) return !1;
+                    b = !0, k = !1
+                }
+                if (S && !k) return m || (m = new n), b || c(e) ? o(e, t, r, h, v, m) : a(e, t, P, r, h, v, m);
+                if (!(1 & r)) {
+                    var _ = k && y.call(e, "__wrapped__"),
+                        x = O && y.call(t, "__wrapped__");
+                    if (_ || x) {
+                        var A = _ ? e.value() : e,
+                            T = x ? t.value() : t;
+                        return m || (m = new n), v(A, T, r, h, m)
+                    }
+                }
+                return !!S && (m || (m = new n), i(e, t, r, h, v, m))
+            }
+        },
+        4757: function(e) {
+            e.exports = function(e, t) {
+                return e.has(t)
+            }
+        },
+        7114: function(e, t, r) {
+            var n = r(8668),
+                o = r(2908),
+                a = r(4757);
+            e.exports = function(e, t, r, i, l, u) {
+                var s = 1 & r,
+                    c = e.length,
+                    f = t.length;
+                if (c != f && !(s && f > c)) return !1;
+                var d = u.get(e),
+                    p = u.get(t);
+                if (d && p) return d == t && p == e;
+                var y = -1,
+                    h = !0,
+                    v = 2 & r ? new n : void 0;
+                for (u.set(e, t), u.set(t, e); ++y < c;) {
+                    var m = e[y],
+                        b = t[y];
+                    if (i) var g = s ? i(b, m, y, t, e, u) : i(m, b, y, e, t, u);
+                    if (void 0 !== g) {
+                        if (g) continue;
+                        h = !1;
+                        break
+                    }
+                    if (v) {
+                        if (!o(t, function(e, t) {
+                                if (!a(v, t) && (m === e || l(m, e, r, i, u))) return v.push(t)
+                            })) {
+                            h = !1;
+                            break
+                        }
+                    } else if (!(m === b || l(m, b, r, i, u))) {
+                        h = !1;
+                        break
+                    }
+                }
+                return u.delete(e), u.delete(t), h
+            }
+        },
+        8351: function(e, t, r) {
+            var n = r(2705),
+                o = r(1149),
+                a = r(7813),
+                i = r(7114),
+                l = r(8776),
+                u = r(1814),
+                s = n ? n.prototype : void 0,
+                c = s ? s.valueOf : void 0;
+            e.exports = function(e, t, r, n, s, f, d) {
+                switch (r) {
+                    case "[object DataView]":
+                        if (e.byteLength != t.byteLength || e.byteOffset != t.byteOffset) break;
+                        e = e.buffer, t = t.buffer;
+                    case "[object ArrayBuffer]":
+                        if (e.byteLength != t.byteLength || !f(new o(e), new o(t))) break;
+                        return !0;
+                    case "[object Boolean]":
+                    case "[object Date]":
+                    case "[object Number]":
+                        return a(+e, +t);
+                    case "[object Error]":
+                        return e.name == t.name && e.message == t.message;
+                    case "[object RegExp]":
+                    case "[object String]":
+                        return e == t + "";
+                    case "[object Map]":
+                        var p = l;
+                    case "[object Set]":
+                        var y = 1 & n;
+                        if (p || (p = u), e.size != t.size && !y) break;
+                        var h = d.get(e);
+                        if (h) return h == t;
+                        n |= 2, d.set(e, t);
+                        var v = i(p(e), p(t), n, s, f, d);
+                        return d.delete(e), v;
+                    case "[object Symbol]":
+                        if (c) return c.call(e) == c.call(t)
+                }
+                return !1
+            }
+        },
+        6096: function(e, t, r) {
+            var n = r(8234),
+                o = Object.prototype.hasOwnProperty;
+            e.exports = function(e, t, r, a, i, l) {
+                var u = 1 & r,
+                    s = n(e),
+                    c = s.length;
+                if (c != n(t).length && !u) return !1;
+                for (var f = c; f--;) {
+                    var d = s[f];
+                    if (!(u ? d in t : o.call(t, d))) return !1
+                }
+                var p = l.get(e),
+                    y = l.get(t);
+                if (p && y) return p == t && y == e;
+                var h = !0;
+                l.set(e, t), l.set(t, e);
+                for (var v = u; ++f < c;) {
+                    var m = e[d = s[f]],
+                        b = t[d];
+                    if (a) var g = u ? a(b, m, d, t, e, l) : a(m, b, d, e, t, l);
+                    if (!(void 0 === g ? m === b || i(m, b, r, a, l) : g)) {
+                        h = !1;
+                        break
+                    }
+                    v || (v = "constructor" == d)
+                }
+                if (h && !v) {
+                    var P = e.constructor,
+                        w = t.constructor;
+                    P != w && "constructor" in e && "constructor" in t && !("function" == typeof P && P instanceof P && "function" == typeof w && w instanceof w) && (h = !1)
+                }
+                return l.delete(e), l.delete(t), h
+            }
+        },
+        8776: function(e) {
+            e.exports = function(e) {
+                var t = -1,
+                    r = Array(e.size);
+                return e.forEach(function(e, n) {
+                    r[++t] = [n, e]
+                }), r
+            }
+        },
+        619: function(e) {
+            e.exports = function(e) {
+                return this.__data__.set(e, "__lodash_hash_undefined__"), this
+            }
+        },
+        2385: function(e) {
+            e.exports = function(e) {
+                return this.__data__.has(e)
+            }
+        },
+        1814: function(e) {
+            e.exports = function(e) {
+                var t = -1,
+                    r = Array(e.size);
+                return e.forEach(function(e) {
+                    r[++t] = e
+                }), r
+            }
+        },
+        8446: function(e, t, r) {
+            var n = r(939);
+            e.exports = function(e, t) {
+                return n(e, t)
             }
         },
         845: function(e, t, r) {
             "use strict";
             r.r(t);
             var n = Number.isNaN || function(e) {
                 return "number" == typeof e && e != e
             };
 
-            function a(e, t) {
+            function o(e, t) {
                 if (e.length !== t.length) return !1;
-                for (var r, a, o = 0; o < e.length; o++)
-                    if (!((r = e[o]) === (a = t[o]) || n(r) && n(a))) return !1;
+                for (var r, o, a = 0; a < e.length; a++)
+                    if (!((r = e[a]) === (o = t[a]) || n(r) && n(o))) return !1;
                 return !0
             }
             t.default = function(e, t) {
-                void 0 === t && (t = a);
-                var r, n, o = [],
-                    l = !1;
+                void 0 === t && (t = o);
+                var r, n, a = [],
+                    i = !1;
                 return function() {
-                    for (var a = [], i = 0; i < arguments.length; i++) a[i] = arguments[i];
-                    return l && r === this && t(a, o) || (n = e.apply(this, a), l = !0, r = this, o = a), n
+                    for (var o = [], l = 0; l < arguments.length; l++) o[l] = arguments[l];
+                    return i && r === this && t(o, a) || (n = e.apply(this, o), i = !0, r = this, a = o), n
                 }
             }
         },
         9590: function(e) {
             var t = "undefined" != typeof Element,
                 r = "function" == typeof Map,
                 n = "function" == typeof Set,
-                a = "function" == typeof ArrayBuffer && !!ArrayBuffer.isView;
-            e.exports = function(e, o) {
+                o = "function" == typeof ArrayBuffer && !!ArrayBuffer.isView;
+            e.exports = function(e, a) {
                 try {
-                    return function e(o, l) {
-                        if (o === l) return !0;
-                        if (o && l && "object" == typeof o && "object" == typeof l) {
-                            var i, u, s, c;
-                            if (o.constructor !== l.constructor) return !1;
-                            if (Array.isArray(o)) {
-                                if ((i = o.length) != l.length) return !1;
-                                for (u = i; 0 != u--;)
-                                    if (!e(o[u], l[u])) return !1;
+                    return function e(a, i) {
+                        if (a === i) return !0;
+                        if (a && i && "object" == typeof a && "object" == typeof i) {
+                            var l, u, s, c;
+                            if (a.constructor !== i.constructor) return !1;
+                            if (Array.isArray(a)) {
+                                if ((l = a.length) != i.length) return !1;
+                                for (u = l; 0 != u--;)
+                                    if (!e(a[u], i[u])) return !1;
                                 return !0
                             }
-                            if (r && o instanceof Map && l instanceof Map) {
-                                if (o.size !== l.size) return !1;
-                                for (c = o.entries(); !(u = c.next()).done;)
-                                    if (!l.has(u.value[0])) return !1;
-                                for (c = o.entries(); !(u = c.next()).done;)
-                                    if (!e(u.value[1], l.get(u.value[0]))) return !1;
+                            if (r && a instanceof Map && i instanceof Map) {
+                                if (a.size !== i.size) return !1;
+                                for (c = a.entries(); !(u = c.next()).done;)
+                                    if (!i.has(u.value[0])) return !1;
+                                for (c = a.entries(); !(u = c.next()).done;)
+                                    if (!e(u.value[1], i.get(u.value[0]))) return !1;
                                 return !0
                             }
-                            if (n && o instanceof Set && l instanceof Set) {
-                                if (o.size !== l.size) return !1;
-                                for (c = o.entries(); !(u = c.next()).done;)
-                                    if (!l.has(u.value[0])) return !1;
+                            if (n && a instanceof Set && i instanceof Set) {
+                                if (a.size !== i.size) return !1;
+                                for (c = a.entries(); !(u = c.next()).done;)
+                                    if (!i.has(u.value[0])) return !1;
                                 return !0
                             }
-                            if (a && ArrayBuffer.isView(o) && ArrayBuffer.isView(l)) {
-                                if ((i = o.length) != l.length) return !1;
-                                for (u = i; 0 != u--;)
-                                    if (o[u] !== l[u]) return !1;
+                            if (o && ArrayBuffer.isView(a) && ArrayBuffer.isView(i)) {
+                                if ((l = a.length) != i.length) return !1;
+                                for (u = l; 0 != u--;)
+                                    if (a[u] !== i[u]) return !1;
                                 return !0
                             }
-                            if (o.constructor === RegExp) return o.source === l.source && o.flags === l.flags;
-                            if (o.valueOf !== Object.prototype.valueOf) return o.valueOf() === l.valueOf();
-                            if (o.toString !== Object.prototype.toString) return o.toString() === l.toString();
-                            if ((i = (s = Object.keys(o)).length) !== Object.keys(l).length) return !1;
-                            for (u = i; 0 != u--;)
-                                if (!Object.prototype.hasOwnProperty.call(l, s[u])) return !1;
-                            if (t && o instanceof Element) return !1;
-                            for (u = i; 0 != u--;)
-                                if (("_owner" !== s[u] && "__v" !== s[u] && "__o" !== s[u] || !o.$$typeof) && !e(o[s[u]], l[s[u]])) return !1;
+                            if (a.constructor === RegExp) return a.source === i.source && a.flags === i.flags;
+                            if (a.valueOf !== Object.prototype.valueOf) return a.valueOf() === i.valueOf();
+                            if (a.toString !== Object.prototype.toString) return a.toString() === i.toString();
+                            if ((l = (s = Object.keys(a)).length) !== Object.keys(i).length) return !1;
+                            for (u = l; 0 != u--;)
+                                if (!Object.prototype.hasOwnProperty.call(i, s[u])) return !1;
+                            if (t && a instanceof Element) return !1;
+                            for (u = l; 0 != u--;)
+                                if (("_owner" !== s[u] && "__v" !== s[u] && "__o" !== s[u] || !a.$$typeof) && !e(a[s[u]], i[s[u]])) return !1;
                             return !0
                         }
-                        return o != o && l != l
-                    }(e, o)
+                        return a != a && i != i
+                    }(e, a)
                 } catch (e) {
                     if ((e.message || "").match(/stack|recursion/i)) return console.warn("react-fast-compare cannot handle circular refs"), !1;
                     throw e
                 }
             }
         },
         9605: function(e, t, r) {
@@ -1181,33 +1403,33 @@
                 } : function(e) {
                     return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                 })(e)
             }
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.default = void 0;
-            var a, o = function(e) {
+            var o, a = function(e) {
                     if (e && e.__esModule) return e;
                     if (null === e || "object" !== n(e) && "function" != typeof e) return {
                         default: e
                     };
                     var t = s();
                     if (t && t.has(e)) return t.get(e);
                     var r = {},
-                        a = Object.defineProperty && Object.getOwnPropertyDescriptor;
-                    for (var o in e)
-                        if (Object.prototype.hasOwnProperty.call(e, o)) {
-                            var l = a ? Object.getOwnPropertyDescriptor(e, o) : null;
-                            l && (l.get || l.set) ? Object.defineProperty(r, o, l) : r[o] = e[o]
+                        o = Object.defineProperty && Object.getOwnPropertyDescriptor;
+                    for (var a in e)
+                        if (Object.prototype.hasOwnProperty.call(e, a)) {
+                            var i = o ? Object.getOwnPropertyDescriptor(e, a) : null;
+                            i && (i.get || i.set) ? Object.defineProperty(r, a, i) : r[a] = e[a]
                         } return r.default = e, t && t.set(e, r), r
                 }(r(7294)),
-                l = (a = r(9590)) && a.__esModule ? a : {
-                    default: a
+                i = (o = r(9590)) && o.__esModule ? o : {
+                    default: o
                 },
-                i = r(9448),
+                l = r(9448),
                 u = r(6281);
 
             function s() {
                 if ("function" != typeof WeakMap) return null;
                 var e = new WeakMap;
                 return s = function() {
                     return e
@@ -1220,23 +1442,23 @@
                         var r = arguments[t];
                         for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
                     }
                     return e
                 }).apply(this, arguments)
             }
 
-            function d(e, t) {
+            function f(e, t) {
                 for (var r = 0; r < t.length; r++) {
                     var n = t[r];
                     n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
                 }
             }
 
-            function f(e, t) {
-                return (f = Object.setPrototypeOf || function(e, t) {
+            function d(e, t) {
+                return (d = Object.setPrototypeOf || function(e, t) {
                     return e.__proto__ = t, e
                 })(e, t)
             }
 
             function p(e) {
                 if (void 0 === e) throw ReferenceError("this hasn't been initialised - super() hasn't been called");
                 return e
@@ -1252,95 +1474,95 @@
                 return t in e ? Object.defineProperty(e, t, {
                     value: r,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[t] = r, e
             }
-            var m = function(e) {
+            var v = function(e) {
                 ! function(e, t) {
                     if ("function" != typeof t && null !== t) throw TypeError("Super expression must either be null or a function");
                     e.prototype = Object.create(t && t.prototype, {
                         constructor: {
                             value: e,
                             writable: !0,
                             configurable: !0
                         }
-                    }), t && f(e, t)
+                    }), t && d(e, t)
                 }(s, e);
-                var t, r, a, i = (t = function() {
+                var t, r, o, l = (t = function() {
                     if ("undefined" == typeof Reflect || !Reflect.construct || Reflect.construct.sham) return !1;
                     if ("function" == typeof Proxy) return !0;
                     try {
                         return Date.prototype.toString.call(Reflect.construct(Date, [], function() {})), !0
                     } catch (e) {
                         return !1
                     }
                 }(), function() {
-                    var e, r, a = y(s);
+                    var e, r, o = y(s);
                     if (t) {
-                        var o = y(this).constructor;
-                        r = Reflect.construct(a, arguments, o)
-                    } else r = a.apply(this, arguments);
+                        var a = y(this).constructor;
+                        r = Reflect.construct(o, arguments, a)
+                    } else r = o.apply(this, arguments);
                     return (e = r) && ("object" === n(e) || "function" == typeof e) ? e : p(this)
                 });
 
                 function s() {
                     var e;
                     ! function(e, t) {
                         if (!(e instanceof t)) throw TypeError("Cannot call a class as a function")
                     }(this, s);
                     for (var t = arguments.length, r = Array(t), n = 0; n < t; n++) r[n] = arguments[n];
-                    return h(p(e = i.call.apply(i, [this].concat(r))), "mounted", !1), h(p(e), "isReady", !1), h(p(e), "isPlaying", !1), h(p(e), "isLoading", !0), h(p(e), "loadOnReady", null), h(p(e), "startOnPlay", !0), h(p(e), "seekOnPlay", null), h(p(e), "onDurationCalled", !1), h(p(e), "handlePlayerMount", function(t) {
+                    return h(p(e = l.call.apply(l, [this].concat(r))), "mounted", !1), h(p(e), "isReady", !1), h(p(e), "isPlaying", !1), h(p(e), "isLoading", !0), h(p(e), "loadOnReady", null), h(p(e), "startOnPlay", !0), h(p(e), "seekOnPlay", null), h(p(e), "onDurationCalled", !1), h(p(e), "handlePlayerMount", function(t) {
                         if (e.player) {
                             e.progress();
                             return
                         }
                         e.player = t, e.player.load(e.props.url), e.progress()
                     }), h(p(e), "getInternalPlayer", function(t) {
                         return e.player ? e.player[t] : null
                     }), h(p(e), "progress", function() {
                         if (e.props.url && e.player && e.isReady) {
                             var t = e.getCurrentTime() || 0,
                                 r = e.getSecondsLoaded(),
                                 n = e.getDuration();
                             if (n) {
-                                var a = {
+                                var o = {
                                     playedSeconds: t,
                                     played: t / n
                                 };
-                                null !== r && (a.loadedSeconds = r, a.loaded = r / n), (a.playedSeconds !== e.prevPlayed || a.loadedSeconds !== e.prevLoaded) && e.props.onProgress(a), e.prevPlayed = a.playedSeconds, e.prevLoaded = a.loadedSeconds
+                                null !== r && (o.loadedSeconds = r, o.loaded = r / n), (o.playedSeconds !== e.prevPlayed || o.loadedSeconds !== e.prevLoaded) && e.props.onProgress(o), e.prevPlayed = o.playedSeconds, e.prevLoaded = o.loadedSeconds
                             }
                         }
                         e.progressTimeout = setTimeout(e.progress, e.props.progressFrequency || e.props.progressInterval)
                     }), h(p(e), "handleReady", function() {
                         if (e.mounted) {
                             e.isReady = !0, e.isLoading = !1;
                             var t = e.props,
                                 r = t.onReady,
                                 n = t.playing,
-                                a = t.volume,
-                                o = t.muted;
-                            r(), o || null === a || e.player.setVolume(a), e.loadOnReady ? (e.player.load(e.loadOnReady, !0), e.loadOnReady = null) : n && e.player.play(), e.handleDurationCheck()
+                                o = t.volume,
+                                a = t.muted;
+                            r(), a || null === o || e.player.setVolume(o), e.loadOnReady ? (e.player.load(e.loadOnReady, !0), e.loadOnReady = null) : n && e.player.play(), e.handleDurationCheck()
                         }
                     }), h(p(e), "handlePlay", function() {
                         e.isPlaying = !0, e.isLoading = !1;
                         var t = e.props,
                             r = t.onStart,
                             n = t.onPlay,
-                            a = t.playbackRate;
-                        e.startOnPlay && (e.player.setPlaybackRate && 1 !== a && e.player.setPlaybackRate(a), r(), e.startOnPlay = !1), n(), e.seekOnPlay && (e.seekTo(e.seekOnPlay), e.seekOnPlay = null), e.handleDurationCheck()
+                            o = t.playbackRate;
+                        e.startOnPlay && (e.player.setPlaybackRate && 1 !== o && e.player.setPlaybackRate(o), r(), e.startOnPlay = !1), n(), e.seekOnPlay && (e.seekTo(e.seekOnPlay), e.seekOnPlay = null), e.handleDurationCheck()
                     }), h(p(e), "handlePause", function(t) {
                         e.isPlaying = !1, e.isLoading || e.props.onPause(t)
                     }), h(p(e), "handleEnded", function() {
                         var t = e.props,
                             r = t.activePlayer,
                             n = t.loop,
-                            a = t.onEnded;
-                        r.loopOnEnded && n && e.seekTo(0), n || (e.isPlaying = !1, a())
+                            o = t.onEnded;
+                        r.loopOnEnded && n && e.seekTo(0), n || (e.isPlaying = !1, o())
                     }), h(p(e), "handleError", function() {
                         var t;
                         e.isLoading = !1, (t = e.props).onError.apply(t, arguments)
                     }), h(p(e), "handleDurationCheck", function() {
                         clearTimeout(e.durationCheckTimeout);
                         var t = e.getDuration();
                         t ? e.onDurationCalled || (e.props.onDuration(t), e.onDurationCalled = !0) : e.durationCheckTimeout = setTimeout(e.handleDurationCheck, 100)
@@ -1361,32 +1583,32 @@
                 }, {
                     key: "componentDidUpdate",
                     value: function(e) {
                         var t = this;
                         if (this.player) {
                             var r = this.props,
                                 n = r.url,
-                                a = r.playing,
-                                o = r.volume,
-                                i = r.muted,
+                                o = r.playing,
+                                a = r.volume,
+                                l = r.muted,
                                 s = r.playbackRate,
                                 c = r.pip,
-                                d = r.loop,
-                                f = r.activePlayer,
+                                f = r.loop,
+                                d = r.activePlayer,
                                 p = r.disableDeferredLoading;
-                            if (!(0, l.default)(e.url, n)) {
-                                if (this.isLoading && !f.forceLoad && !p && !(0, u.isMediaStream)(n)) {
+                            if (!(0, i.default)(e.url, n)) {
+                                if (this.isLoading && !d.forceLoad && !p && !(0, u.isMediaStream)(n)) {
                                     console.warn("ReactPlayer: the attempt to load ".concat(n, " is being deferred until the player has loaded")), this.loadOnReady = n;
                                     return
                                 }
                                 this.isLoading = !0, this.startOnPlay = !0, this.onDurationCalled = !1, this.player.load(n, this.isReady)
                             }
-                            e.playing || !a || this.isPlaying || this.player.play(), e.playing && !a && this.isPlaying && this.player.pause(), !e.pip && c && this.player.enablePIP && this.player.enablePIP(), e.pip && !c && this.player.disablePIP && this.player.disablePIP(), e.volume !== o && null !== o && this.player.setVolume(o), e.muted !== i && (i ? this.player.mute() : (this.player.unmute(), null !== o && setTimeout(function() {
-                                return t.player.setVolume(o)
-                            }))), e.playbackRate !== s && this.player.setPlaybackRate && this.player.setPlaybackRate(s), e.loop !== d && this.player.setLoop && this.player.setLoop(d)
+                            e.playing || !o || this.isPlaying || this.player.play(), e.playing && !o && this.isPlaying && this.player.pause(), !e.pip && c && this.player.enablePIP && this.player.enablePIP(), e.pip && !c && this.player.disablePIP && this.player.disablePIP(), e.volume !== a && null !== a && this.player.setVolume(a), e.muted !== l && (l ? this.player.mute() : (this.player.unmute(), null !== a && setTimeout(function() {
+                                return t.player.setVolume(a)
+                            }))), e.playbackRate !== s && this.player.setPlaybackRate && this.player.setPlaybackRate(s), e.loop !== f && this.player.setLoop && this.player.setLoop(f)
                         }
                     }
                 }, {
                     key: "getDuration",
                     value: function() {
                         return this.isReady ? this.player.getDuration() : null
                     }
@@ -1421,73 +1643,73 @@
                         }
                         this.player.seekTo(e)
                     }
                 }, {
                     key: "render",
                     value: function() {
                         var e = this.props.activePlayer;
-                        return e ? o.default.createElement(e, c({}, this.props, {
+                        return e ? a.default.createElement(e, c({}, this.props, {
                             onMount: this.handlePlayerMount,
                             onReady: this.handleReady,
                             onPlay: this.handlePlay,
                             onPause: this.handlePause,
                             onEnded: this.handleEnded,
                             onLoaded: this.handleLoaded,
                             onError: this.handleError
                         })) : null
                     }
-                }], d(s.prototype, r), a && d(s, a), s
-            }(o.Component);
-            t.default = m, h(m, "displayName", "Player"), h(m, "propTypes", i.propTypes), h(m, "defaultProps", i.defaultProps)
+                }], f(s.prototype, r), o && f(s, o), s
+            }(a.Component);
+            t.default = v, h(v, "displayName", "Player"), h(v, "propTypes", l.propTypes), h(v, "defaultProps", l.defaultProps)
         },
-        1276: function(e, t, r) {
+        8800: function(e, t, r) {
             "use strict";
 
             function n(e) {
                 return (n = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                     return typeof e
                 } : function(e) {
                     return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                 })(e)
             }
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.createReactPlayer = void 0;
-            var a = function(e) {
+            var o = function(e) {
                     if (e && e.__esModule) return e;
                     if (null === e || "object" !== n(e) && "function" != typeof e) return {
                         default: e
                     };
-                    var t = f();
+                    var t = d();
                     if (t && t.has(e)) return t.get(e);
                     var r = {},
-                        a = Object.defineProperty && Object.getOwnPropertyDescriptor;
-                    for (var o in e)
-                        if (Object.prototype.hasOwnProperty.call(e, o)) {
-                            var l = a ? Object.getOwnPropertyDescriptor(e, o) : null;
-                            l && (l.get || l.set) ? Object.defineProperty(r, o, l) : r[o] = e[o]
+                        o = Object.defineProperty && Object.getOwnPropertyDescriptor;
+                    for (var a in e)
+                        if (Object.prototype.hasOwnProperty.call(e, a)) {
+                            var i = o ? Object.getOwnPropertyDescriptor(e, a) : null;
+                            i && (i.get || i.set) ? Object.defineProperty(r, a, i) : r[a] = e[a]
                         } return r.default = e, t && t.set(e, r), r
                 }(r(7294)),
-                o = d(r(9996)),
-                l = d(r(845)),
-                i = d(r(9590)),
+                a = f(r(9996)),
+                i = f(r(845)),
+                l = f(r(9590)),
                 u = r(9448),
                 s = r(6281),
-                c = d(r(9605));
+                c = f(r(9605));
 
-            function d(e) {
+            function f(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
             }
 
-            function f() {
+            function d() {
                 if ("function" != typeof WeakMap) return null;
                 var e = new WeakMap;
-                return f = function() {
+                return d = function() {
                     return e
                 }, e
             }
 
             function p(e, t) {
                 var r = Object.keys(e);
                 if (Object.getOwnPropertySymbols) {
@@ -1517,32 +1739,32 @@
                         var r = arguments[t];
                         for (var n in r) Object.prototype.hasOwnProperty.call(r, n) && (e[n] = r[n])
                     }
                     return e
                 }).apply(this, arguments)
             }
 
-            function m(e) {
+            function v(e) {
                 return function(e) {
-                    if (Array.isArray(e)) return v(e)
+                    if (Array.isArray(e)) return m(e)
                 }(e) || function(e) {
                     if ("undefined" != typeof Symbol && Symbol.iterator in Object(e)) return Array.from(e)
                 }(e) || function(e, t) {
                     if (e) {
-                        if ("string" == typeof e) return v(e, t);
+                        if ("string" == typeof e) return m(e, t);
                         var r = Object.prototype.toString.call(e).slice(8, -1);
                         if ("Object" === r && e.constructor && (r = e.constructor.name), "Map" === r || "Set" === r) return Array.from(e);
-                        if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return v(e, t)
+                        if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return m(e, t)
                     }
                 }(e) || function() {
                     throw TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                 }()
             }
 
-            function v(e, t) {
+            function m(e, t) {
                 (null == t || t > e.length) && (t = e.length);
                 for (var r = 0, n = Array(t); r < t; r++) n[r] = e[r];
                 return n
             }
 
             function b(e, t) {
                 for (var r = 0; r < t.length; r++) {
@@ -1572,61 +1794,61 @@
                 return t in e ? Object.defineProperty(e, t, {
                     value: r,
                     enumerable: !0,
                     configurable: !0,
                     writable: !0
                 }) : e[t] = r, e
             }
-            var S = (0, a.lazy)(function() {
+            var O = (0, o.lazy)(function() {
                     return r.e(664).then(r.bind(r, 7284))
                 }),
-                O = "undefined" != typeof window && window.document,
-                x = void 0 !== r.g && r.g.window && r.g.window.document,
-                _ = Object.keys(u.propTypes),
-                A = O || x ? a.Suspense : function() {
+                S = "undefined" != typeof window && window.document,
+                _ = void 0 !== r.g && r.g.window && r.g.window.document,
+                x = Object.keys(u.propTypes),
+                A = S || _ ? o.Suspense : function() {
                     return null
                 },
                 T = [];
             t.createReactPlayer = function(e, t) {
-                var r, d;
-                return d = r = function(r) {
+                var r, f;
+                return f = r = function(r) {
                     (function(e, t) {
                         if ("function" != typeof t && null !== t) throw TypeError("Super expression must either be null or a function");
                         e.prototype = Object.create(t && t.prototype, {
                             constructor: {
                                 value: e,
                                 writable: !0,
                                 configurable: !0
                             }
                         }), t && g(e, t)
-                    })(O, r);
-                    var d, f, p, v = (d = function() {
+                    })(S, r);
+                    var f, d, p, m = (f = function() {
                         if ("undefined" == typeof Reflect || !Reflect.construct || Reflect.construct.sham) return !1;
                         if ("function" == typeof Proxy) return !0;
                         try {
                             return Date.prototype.toString.call(Reflect.construct(Date, [], function() {})), !0
                         } catch (e) {
                             return !1
                         }
                     }(), function() {
-                        var e, t, r = w(O);
-                        if (d) {
-                            var a = w(this).constructor;
-                            t = Reflect.construct(r, arguments, a)
+                        var e, t, r = w(S);
+                        if (f) {
+                            var o = w(this).constructor;
+                            t = Reflect.construct(r, arguments, o)
                         } else t = r.apply(this, arguments);
                         return (e = t) && ("object" === n(e) || "function" == typeof e) ? e : P(this)
                     });
 
-                    function O() {
+                    function S() {
                         var r;
                         (function(e, t) {
                             if (!(e instanceof t)) throw TypeError("Cannot call a class as a function")
-                        })(this, O);
-                        for (var n = arguments.length, i = Array(n), d = 0; d < n; d++) i[d] = arguments[d];
-                        return k(P(r = v.call.apply(v, [this].concat(i))), "state", {
+                        })(this, S);
+                        for (var n = arguments.length, l = Array(n), f = 0; f < n; f++) l[f] = arguments[f];
+                        return k(P(r = m.call.apply(m, [this].concat(l))), "state", {
                             showPreview: !!r.props.light
                         }), k(P(r), "references", {
                             wrapper: function(e) {
                                 r.wrapper = e
                             },
                             player: function(e) {
                                 r.player = e
@@ -1649,43 +1871,43 @@
                             var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "player";
                             return r.player ? r.player.getInternalPlayer(e) : null
                         }), k(P(r), "seekTo", function(e, t) {
                             if (!r.player) return null;
                             r.player.seekTo(e, t)
                         }), k(P(r), "handleReady", function() {
                             r.props.onReady(P(r))
-                        }), k(P(r), "getActivePlayer", (0, l.default)(function(r) {
-                            for (var n = 0, a = [].concat(T, m(e)); n < a.length; n++) {
-                                var o = a[n];
-                                if (o.canPlay(r)) return o
+                        }), k(P(r), "getActivePlayer", (0, i.default)(function(r) {
+                            for (var n = 0, o = [].concat(T, v(e)); n < o.length; n++) {
+                                var a = o[n];
+                                if (a.canPlay(r)) return a
                             }
                             return t || null
-                        })), k(P(r), "getConfig", (0, l.default)(function(e, t) {
+                        })), k(P(r), "getConfig", (0, i.default)(function(e, t) {
                             var n = r.props.config;
-                            return o.default.all([u.defaultProps.config, u.defaultProps.config[t] || {}, n, n[t] || {}])
-                        })), k(P(r), "getAttributes", (0, l.default)(function(e) {
-                            return (0, s.omit)(r.props, _)
+                            return a.default.all([u.defaultProps.config, u.defaultProps.config[t] || {}, n, n[t] || {}])
+                        })), k(P(r), "getAttributes", (0, i.default)(function(e) {
+                            return (0, s.omit)(r.props, x)
                         })), k(P(r), "renderActivePlayer", function(e) {
                             if (!e) return null;
                             var t = r.getActivePlayer(e);
                             if (!t) return null;
                             var n = r.getConfig(e, t.key);
-                            return a.default.createElement(c.default, h({}, r.props, {
+                            return o.default.createElement(c.default, h({}, r.props, {
                                 key: t.key,
                                 ref: r.references.player,
                                 config: n,
                                 activePlayer: t.lazyPlayer || t,
                                 onReady: r.handleReady
                             }))
                         }), r
                     }
-                    return f = [{
+                    return d = [{
                         key: "shouldComponentUpdate",
                         value: function(e, t) {
-                            return !(0, i.default)(this.props, e) || !(0, i.default)(this.state, t)
+                            return !(0, l.default)(this.props, e) || !(0, l.default)(this.state, t)
                         }
                     }, {
                         key: "componentDidUpdate",
                         value: function(e) {
                             var t = this.props.light;
                             !e.light && t && this.setState({
                                 showPreview: !0
@@ -1696,173 +1918,173 @@
                     }, {
                         key: "renderPreview",
                         value: function(e) {
                             if (!e) return null;
                             var t = this.props,
                                 r = t.light,
                                 n = t.playIcon,
-                                o = t.previewTabIndex,
-                                l = t.oEmbedUrl;
-                            return a.default.createElement(S, {
+                                a = t.previewTabIndex,
+                                i = t.oEmbedUrl;
+                            return o.default.createElement(O, {
                                 url: e,
                                 light: r,
                                 playIcon: n,
-                                previewTabIndex: o,
-                                oEmbedUrl: l,
+                                previewTabIndex: a,
+                                oEmbedUrl: i,
                                 onClick: this.handleClickPreview
                             })
                         }
                     }, {
                         key: "render",
                         value: function() {
                             var e = this.props,
                                 t = e.url,
                                 r = e.style,
                                 n = e.width,
-                                o = e.height,
-                                l = e.fallback,
-                                i = e.wrapper,
+                                a = e.height,
+                                i = e.fallback,
+                                l = e.wrapper,
                                 u = this.state.showPreview,
                                 s = this.getAttributes(t),
-                                c = "string" == typeof i ? this.references.wrapper : void 0;
-                            return a.default.createElement(i, h({
+                                c = "string" == typeof l ? this.references.wrapper : void 0;
+                            return o.default.createElement(l, h({
                                 ref: c,
                                 style: y(y({}, r), {}, {
                                     width: n,
-                                    height: o
+                                    height: a
                                 })
-                            }, s), a.default.createElement(A, {
-                                fallback: l
+                            }, s), o.default.createElement(A, {
+                                fallback: i
                             }, u ? this.renderPreview(t) : this.renderActivePlayer(t)))
                         }
-                    }], b(O.prototype, f), p && b(O, p), O
-                }(a.Component), k(r, "displayName", "ReactPlayer"), k(r, "propTypes", u.propTypes), k(r, "defaultProps", u.defaultProps), k(r, "addCustomPlayer", function(e) {
+                    }], b(S.prototype, d), p && b(S, p), S
+                }(o.Component), k(r, "displayName", "ReactPlayer"), k(r, "propTypes", u.propTypes), k(r, "defaultProps", u.defaultProps), k(r, "addCustomPlayer", function(e) {
                     T.push(e)
                 }), k(r, "removeCustomPlayers", function() {
                     T.length = 0
                 }), k(r, "canPlay", function(t) {
-                    for (var r = 0, n = [].concat(T, m(e)); r < n.length; r++)
+                    for (var r = 0, n = [].concat(T, v(e)); r < n.length; r++)
                         if (n[r].canPlay(t)) return !0;
                     return !1
                 }), k(r, "canEnablePIP", function(t) {
-                    for (var r = 0, n = [].concat(T, m(e)); r < n.length; r++) {
-                        var a = n[r];
-                        if (a.canEnablePIP && a.canEnablePIP(t)) return !0
+                    for (var r = 0, n = [].concat(T, v(e)); r < n.length; r++) {
+                        var o = n[r];
+                        if (o.canEnablePIP && o.canEnablePIP(t)) return !0
                     }
                     return !1
-                }), d
+                }), f
             }
         },
         6310: function(e, t, r) {
             "use strict";
             t.Z = void 0;
-            var n, a = (n = r(9760)) && n.__esModule ? n : {
+            var n, o = (n = r(9760)) && n.__esModule ? n : {
                     default: n
                 },
-                o = r(1276),
-                l = a.default[a.default.length - 1],
-                i = (0, o.createReactPlayer)(a.default, l);
-            t.Z = i
+                a = r(8800),
+                i = o.default[o.default.length - 1],
+                l = (0, a.createReactPlayer)(o.default, i);
+            t.Z = l
         },
         9790: function(e, t, r) {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.canPlay = t.FLV_EXTENSIONS = t.DASH_EXTENSIONS = t.HLS_EXTENSIONS = t.VIDEO_EXTENSIONS = t.AUDIO_EXTENSIONS = t.MATCH_URL_KALTURA = t.MATCH_URL_VIDYARD = t.MATCH_URL_MIXCLOUD = t.MATCH_URL_DAILYMOTION = t.MATCH_URL_TWITCH_CHANNEL = t.MATCH_URL_TWITCH_VIDEO = t.MATCH_URL_WISTIA = t.MATCH_URL_STREAMABLE = t.MATCH_URL_FACEBOOK_WATCH = t.MATCH_URL_FACEBOOK = t.MATCH_URL_VIMEO = t.MATCH_URL_SOUNDCLOUD = t.MATCH_URL_YOUTUBE = void 0;
             var n = r(6281);
 
-            function a(e, t) {
+            function o(e, t) {
                 (null == t || t > e.length) && (t = e.length);
                 for (var r = 0, n = Array(t); r < t; r++) n[r] = e[r];
                 return n
             }
-            var o = /(?:youtu\.be\/|youtube(?:-nocookie)?\.com\/(?:embed\/|v\/|watch\/|watch\?v=|watch\?.+&v=|shorts\/|live\/))((\w|-){11})|youtube\.com\/playlist\?list=|youtube\.com\/user\//;
-            t.MATCH_URL_YOUTUBE = o;
-            var l = /(?:soundcloud\.com|snd\.sc)\/[^.]+$/;
-            t.MATCH_URL_SOUNDCLOUD = l;
-            var i = /vimeo\.com\/(?!progressive_redirect).+/;
-            t.MATCH_URL_VIMEO = i;
+            var a = /(?:youtu\.be\/|youtube(?:-nocookie)?\.com\/(?:embed\/|v\/|watch\/|watch\?v=|watch\?.+&v=|shorts\/|live\/))((\w|-){11})|youtube\.com\/playlist\?list=|youtube\.com\/user\//;
+            t.MATCH_URL_YOUTUBE = a;
+            var i = /(?:soundcloud\.com|snd\.sc)\/[^.]+$/;
+            t.MATCH_URL_SOUNDCLOUD = i;
+            var l = /vimeo\.com\/(?!progressive_redirect).+/;
+            t.MATCH_URL_VIMEO = l;
             var u = /^https?:\/\/(www\.)?facebook\.com.*\/(video(s)?|watch|story)(\.php?|\/).+$/;
             t.MATCH_URL_FACEBOOK = u;
             var s = /^https?:\/\/fb\.watch\/.+$/;
             t.MATCH_URL_FACEBOOK_WATCH = s;
             var c = /streamable\.com\/([a-z0-9]+)$/;
             t.MATCH_URL_STREAMABLE = c;
-            var d = /(?:wistia\.(?:com|net)|wi\.st)\/(?:medias|embed)\/(?:iframe\/)?(.*)$/;
-            t.MATCH_URL_WISTIA = d;
-            var f = /(?:www\.|go\.)?twitch\.tv\/videos\/(\d+)($|\?)/;
-            t.MATCH_URL_TWITCH_VIDEO = f;
+            var f = /(?:wistia\.(?:com|net)|wi\.st)\/(?:medias|embed)\/(?:iframe\/)?(.*)$/;
+            t.MATCH_URL_WISTIA = f;
+            var d = /(?:www\.|go\.)?twitch\.tv\/videos\/(\d+)($|\?)/;
+            t.MATCH_URL_TWITCH_VIDEO = d;
             var p = /(?:www\.|go\.)?twitch\.tv\/([a-zA-Z0-9_]+)($|\?)/;
             t.MATCH_URL_TWITCH_CHANNEL = p;
             var y = /^(?:(?:https?):)?(?:\/\/)?(?:www\.)?(?:(?:dailymotion\.com(?:\/embed)?\/video)|dai\.ly)\/([a-zA-Z0-9]+)(?:_[\w_-]+)?(?:[\w.#_-]+)?/;
             t.MATCH_URL_DAILYMOTION = y;
             var h = /mixcloud\.com\/([^/]+\/[^/]+)/;
             t.MATCH_URL_MIXCLOUD = h;
-            var m = /vidyard.com\/(?:watch\/)?([a-zA-Z0-9-_]+)/;
-            t.MATCH_URL_VIDYARD = m;
-            var v = /^https?:\/\/[a-zA-Z]+\.kaltura.(com|org)\/p\/([0-9]+)\/sp\/([0-9]+)00\/embedIframeJs\/uiconf_id\/([0-9]+)\/partner_id\/([0-9]+)(.*)entry_id.([a-zA-Z0-9-_].*)$/;
-            t.MATCH_URL_KALTURA = v;
+            var v = /vidyard.com\/(?:watch\/)?([a-zA-Z0-9-_]+)/;
+            t.MATCH_URL_VIDYARD = v;
+            var m = /^https?:\/\/[a-zA-Z]+\.kaltura.(com|org)\/p\/([0-9]+)\/sp\/([0-9]+)00\/embedIframeJs\/uiconf_id\/([0-9]+)\/partner_id\/([0-9]+)(.*)entry_id.([a-zA-Z0-9-_].*)$/;
+            t.MATCH_URL_KALTURA = m;
             var b = /\.(m4a|m4b|mp4a|mpga|mp2|mp2a|mp3|m2a|m3a|wav|weba|aac|oga|spx)($|\?)/i;
             t.AUDIO_EXTENSIONS = b;
             var g = /\.(mp4|og[gv]|webm|mov|m4v)(#t=[,\d+]+)?($|\?)/i;
             t.VIDEO_EXTENSIONS = g;
             var P = /\.(m3u8)($|\?)/i;
             t.HLS_EXTENSIONS = P;
             var w = /\.(mpd)($|\?)/i;
             t.DASH_EXTENSIONS = w;
             var k = /\.(flv)($|\?)/i;
             t.FLV_EXTENSIONS = k, t.canPlay = {
                 youtube: function(e) {
                     return e instanceof Array ? e.every(function(e) {
-                        return o.test(e)
-                    }) : o.test(e)
+                        return a.test(e)
+                    }) : a.test(e)
                 },
                 soundcloud: function(e) {
-                    return l.test(e) && !b.test(e)
+                    return i.test(e) && !b.test(e)
                 },
                 vimeo: function(e) {
-                    return i.test(e) && !g.test(e) && !P.test(e)
+                    return l.test(e) && !g.test(e) && !P.test(e)
                 },
                 facebook: function(e) {
                     return u.test(e) || s.test(e)
                 },
                 streamable: function(e) {
                     return c.test(e)
                 },
                 wistia: function(e) {
-                    return d.test(e)
+                    return f.test(e)
                 },
                 twitch: function(e) {
-                    return f.test(e) || p.test(e)
+                    return d.test(e) || p.test(e)
                 },
                 dailymotion: function(e) {
                     return y.test(e)
                 },
                 mixcloud: function(e) {
                     return h.test(e)
                 },
                 vidyard: function(e) {
-                    return m.test(e)
+                    return v.test(e)
                 },
                 kaltura: function(e) {
-                    return v.test(e)
+                    return m.test(e)
                 },
                 file: function e(t) {
                     if (t instanceof Array) {
-                        var r, o = function(e, t) {
+                        var r, a = function(e, t) {
                             if ("undefined" == typeof Symbol || null == e[Symbol.iterator]) {
-                                if (Array.isArray(e) || (o = function(e, t) {
+                                if (Array.isArray(e) || (a = function(e, t) {
                                         if (e) {
-                                            if ("string" == typeof e) return a(e, t);
+                                            if ("string" == typeof e) return o(e, t);
                                             var r = Object.prototype.toString.call(e).slice(8, -1);
                                             if ("Object" === r && e.constructor && (r = e.constructor.name), "Map" === r || "Set" === r) return Array.from(e);
-                                            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return a(e, t)
+                                            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return o(e, t)
                                         }
                                     }(e))) {
-                                    o && (e = o);
+                                    a && (e = a);
                                     var r = 0,
                                         n = function() {};
                                     return {
                                         s: n,
                                         n: function() {
                                             return r >= e.length ? {
                                                 done: !0
@@ -1875,257 +2097,257 @@
                                             throw e
                                         },
                                         f: n
                                     }
                                 }
                                 throw TypeError("Invalid attempt to iterate non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                             }
-                            var o, l, i = !0,
+                            var a, i, l = !0,
                                 u = !1;
                             return {
                                 s: function() {
-                                    o = e[Symbol.iterator]()
+                                    a = e[Symbol.iterator]()
                                 },
                                 n: function() {
-                                    var e = o.next();
-                                    return i = e.done, e
+                                    var e = a.next();
+                                    return l = e.done, e
                                 },
                                 e: function(e) {
-                                    u = !0, l = e
+                                    u = !0, i = e
                                 },
                                 f: function() {
                                     try {
-                                        i || null == o.return || o.return()
+                                        l || null == a.return || a.return()
                                     } finally {
-                                        if (u) throw l
+                                        if (u) throw i
                                     }
                                 }
                             }
                         }(t);
                         try {
-                            for (o.s(); !(r = o.n()).done;) {
-                                var l = r.value;
-                                if ("string" == typeof l && e(l) || e(l.src)) return !0
+                            for (a.s(); !(r = a.n()).done;) {
+                                var i = r.value;
+                                if ("string" == typeof i && e(i) || e(i.src)) return !0
                             }
                         } catch (e) {
-                            o.e(e)
+                            a.e(e)
                         } finally {
-                            o.f()
+                            a.f()
                         }
                         return !1
                     }
                     return !!((0, n.isMediaStream)(t) || (0, n.isBlobUrl)(t)) || b.test(t) || g.test(t) || P.test(t) || w.test(t) || k.test(t)
                 }
             }
         },
         9760: function(e, t, r) {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.default = void 0;
             var n = r(7294),
-                a = r(6281),
-                o = r(9790),
-                l = [{
+                o = r(6281),
+                a = r(9790),
+                i = [{
                     key: "youtube",
                     name: "YouTube",
-                    canPlay: o.canPlay.youtube,
+                    canPlay: a.canPlay.youtube,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(439).then(r.bind(r, 5034))
                     })
                 }, {
                     key: "soundcloud",
                     name: "SoundCloud",
-                    canPlay: o.canPlay.soundcloud,
+                    canPlay: a.canPlay.soundcloud,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(125).then(r.bind(r, 6655))
                     })
                 }, {
                     key: "vimeo",
                     name: "Vimeo",
-                    canPlay: o.canPlay.vimeo,
+                    canPlay: a.canPlay.vimeo,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(743).then(r.bind(r, 6746))
                     })
                 }, {
                     key: "facebook",
                     name: "Facebook",
-                    canPlay: o.canPlay.facebook,
+                    canPlay: a.canPlay.facebook,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(121).then(r.bind(r, 6429))
                     })
                 }, {
                     key: "streamable",
                     name: "Streamable",
-                    canPlay: o.canPlay.streamable,
+                    canPlay: a.canPlay.streamable,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(546).then(r.bind(r, 6479))
                     })
                 }, {
                     key: "wistia",
                     name: "Wistia",
-                    canPlay: o.canPlay.wistia,
+                    canPlay: a.canPlay.wistia,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(55).then(r.bind(r, 3134))
                     })
                 }, {
                     key: "twitch",
                     name: "Twitch",
-                    canPlay: o.canPlay.twitch,
+                    canPlay: a.canPlay.twitch,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(216).then(r.bind(r, 9743))
                     })
                 }, {
                     key: "dailymotion",
                     name: "DailyMotion",
-                    canPlay: o.canPlay.dailymotion,
+                    canPlay: a.canPlay.dailymotion,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(596).then(r.bind(r, 5134))
                     })
                 }, {
                     key: "mixcloud",
                     name: "Mixcloud",
-                    canPlay: o.canPlay.mixcloud,
+                    canPlay: a.canPlay.mixcloud,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(667).then(r.bind(r, 9734))
                     })
                 }, {
                     key: "vidyard",
                     name: "Vidyard",
-                    canPlay: o.canPlay.vidyard,
+                    canPlay: a.canPlay.vidyard,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(965).then(r.bind(r, 7287))
                     })
                 }, {
                     key: "kaltura",
                     name: "Kaltura",
-                    canPlay: o.canPlay.kaltura,
+                    canPlay: a.canPlay.kaltura,
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(261).then(r.bind(r, 9289))
                     })
                 }, {
                     key: "file",
                     name: "FilePlayer",
-                    canPlay: o.canPlay.file,
+                    canPlay: a.canPlay.file,
                     canEnablePIP: function(e) {
-                        return o.canPlay.file(e) && (document.pictureInPictureEnabled || (0, a.supportsWebKitPresentationMode)()) && !o.AUDIO_EXTENSIONS.test(e)
+                        return a.canPlay.file(e) && (document.pictureInPictureEnabled || (0, o.supportsWebKitPresentationMode)()) && !a.AUDIO_EXTENSIONS.test(e)
                     },
                     lazyPlayer: (0, n.lazy)(function() {
                         return r.e(11).then(r.bind(r, 3364))
                     })
                 }];
-            t.default = l
+            t.default = i
         },
         9448: function(e, t, r) {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.defaultProps = t.propTypes = void 0;
-            var n, a = (n = r(5697)) && n.__esModule ? n : {
+            var n, o = (n = r(5697)) && n.__esModule ? n : {
                     default: n
                 },
-                o = a.default.string,
-                l = a.default.bool,
-                i = a.default.number,
-                u = a.default.array,
-                s = a.default.oneOfType,
-                c = a.default.shape,
-                d = a.default.object,
-                f = a.default.func,
-                p = a.default.node,
+                a = o.default.string,
+                i = o.default.bool,
+                l = o.default.number,
+                u = o.default.array,
+                s = o.default.oneOfType,
+                c = o.default.shape,
+                f = o.default.object,
+                d = o.default.func,
+                p = o.default.node,
                 y = {
-                    url: s([o, u, d]),
-                    playing: l,
-                    loop: l,
-                    controls: l,
-                    volume: i,
-                    muted: l,
-                    playbackRate: i,
-                    width: s([o, i]),
-                    height: s([o, i]),
-                    style: d,
-                    progressInterval: i,
-                    playsinline: l,
-                    pip: l,
-                    stopOnUnmount: l,
-                    light: s([l, o, d]),
+                    url: s([a, u, f]),
+                    playing: i,
+                    loop: i,
+                    controls: i,
+                    volume: l,
+                    muted: i,
+                    playbackRate: l,
+                    width: s([a, l]),
+                    height: s([a, l]),
+                    style: f,
+                    progressInterval: l,
+                    playsinline: i,
+                    pip: i,
+                    stopOnUnmount: i,
+                    light: s([i, a, f]),
                     playIcon: p,
-                    previewTabIndex: i,
+                    previewTabIndex: l,
                     fallback: p,
-                    oEmbedUrl: o,
-                    wrapper: s([o, f, c({
-                        render: f.isRequired
+                    oEmbedUrl: a,
+                    wrapper: s([a, d, c({
+                        render: d.isRequired
                     })]),
                     config: c({
                         soundcloud: c({
-                            options: d
+                            options: f
                         }),
                         youtube: c({
-                            playerVars: d,
-                            embedOptions: d,
-                            onUnstarted: f
+                            playerVars: f,
+                            embedOptions: f,
+                            onUnstarted: d
                         }),
                         facebook: c({
-                            appId: o,
-                            version: o,
-                            playerId: o,
-                            attributes: d
+                            appId: a,
+                            version: a,
+                            playerId: a,
+                            attributes: f
                         }),
                         dailymotion: c({
-                            params: d
+                            params: f
                         }),
                         vimeo: c({
-                            playerOptions: d,
-                            title: o
+                            playerOptions: f,
+                            title: a
                         }),
                         file: c({
-                            attributes: d,
+                            attributes: f,
                             tracks: u,
-                            forceVideo: l,
-                            forceAudio: l,
-                            forceHLS: l,
-                            forceSafariHLS: l,
-                            forceDASH: l,
-                            forceFLV: l,
-                            hlsOptions: d,
-                            hlsVersion: o,
-                            dashVersion: o,
-                            flvVersion: o
+                            forceVideo: i,
+                            forceAudio: i,
+                            forceHLS: i,
+                            forceSafariHLS: i,
+                            forceDASH: i,
+                            forceFLV: i,
+                            hlsOptions: f,
+                            hlsVersion: a,
+                            dashVersion: a,
+                            flvVersion: a
                         }),
                         wistia: c({
-                            options: d,
-                            playerId: o,
+                            options: f,
+                            playerId: a,
                             customControls: u
                         }),
                         mixcloud: c({
-                            options: d
+                            options: f
                         }),
                         twitch: c({
-                            options: d,
-                            playerId: o
+                            options: f,
+                            playerId: a
                         }),
                         vidyard: c({
-                            options: d
+                            options: f
                         })
                     }),
-                    onReady: f,
-                    onStart: f,
-                    onPlay: f,
-                    onPause: f,
-                    onBuffer: f,
-                    onBufferEnd: f,
-                    onEnded: f,
-                    onError: f,
-                    onDuration: f,
-                    onSeek: f,
-                    onPlaybackRateChange: f,
-                    onProgress: f,
-                    onClickPreview: f,
-                    onEnablePIP: f,
-                    onDisablePIP: f
+                    onReady: d,
+                    onStart: d,
+                    onPlay: d,
+                    onPause: d,
+                    onBuffer: d,
+                    onBufferEnd: d,
+                    onEnded: d,
+                    onError: d,
+                    onDuration: d,
+                    onSeek: d,
+                    onPlaybackRateChange: d,
+                    onProgress: d,
+                    onClickPreview: d,
+                    onEnablePIP: d,
+                    onDisablePIP: d
                 };
             t.propTypes = y;
             var h = function() {};
             t.defaultProps = {
                 playing: !1,
                 loop: !1,
                 controls: !1,
@@ -2237,152 +2459,152 @@
             }
         },
         6281: function(e, t, r) {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.parseStartTime = function(e) {
-                return d(e, i)
+                return f(e, l)
             }, t.parseEndTime = function(e) {
-                return d(e, u)
+                return f(e, u)
             }, t.randomString = function() {
                 return Math.random().toString(36).substr(2, 5)
             }, t.queryString = function(e) {
                 return Object.keys(e).map(function(t) {
                     return "".concat(t, "=").concat(e[t])
                 }).join("&")
             }, t.getSDK = function(e, t) {
                 var r = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : null,
-                    a = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : function() {
+                    o = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : function() {
                         return !0
                     },
-                    o = arguments.length > 4 && void 0 !== arguments[4] ? arguments[4] : n.default,
-                    l = f(t);
-                return l && a(l) ? Promise.resolve(l) : new Promise(function(n, a) {
+                    a = arguments.length > 4 && void 0 !== arguments[4] ? arguments[4] : n.default,
+                    i = d(t);
+                return i && o(i) ? Promise.resolve(i) : new Promise(function(n, o) {
                     if (p[e]) {
                         p[e].push({
                             resolve: n,
-                            reject: a
+                            reject: o
                         });
                         return
                     }
                     p[e] = [{
                         resolve: n,
-                        reject: a
+                        reject: o
                     }];
-                    var l = function(t) {
+                    var i = function(t) {
                         p[e].forEach(function(e) {
                             return e.resolve(t)
                         })
                     };
                     if (r) {
-                        var i = window[r];
+                        var l = window[r];
                         window[r] = function() {
-                            i && i(), l(f(t))
+                            l && l(), i(d(t))
                         }
                     }
-                    o(e, function(n) {
+                    a(e, function(n) {
                         n ? (p[e].forEach(function(e) {
                             return e.reject(n)
-                        }), p[e] = null) : r || l(f(t))
+                        }), p[e] = null) : r || i(d(t))
                     })
                 })
             }, t.getConfig = function(e, t) {
-                return (0, a.default)(t.config, e.config)
+                return (0, o.default)(t.config, e.config)
             }, t.omit = function(e) {
-                for (var t, r = arguments.length, n = Array(r > 1 ? r - 1 : 0), a = 1; a < r; a++) n[a - 1] = arguments[a];
-                for (var o = (t = []).concat.apply(t, n), l = {}, i = Object.keys(e), u = 0; u < i.length; u++) {
-                    var s = i[u]; - 1 === o.indexOf(s) && (l[s] = e[s])
+                for (var t, r = arguments.length, n = Array(r > 1 ? r - 1 : 0), o = 1; o < r; o++) n[o - 1] = arguments[o];
+                for (var a = (t = []).concat.apply(t, n), i = {}, l = Object.keys(e), u = 0; u < l.length; u++) {
+                    var s = l[u]; - 1 === a.indexOf(s) && (i[s] = e[s])
                 }
-                return l
+                return i
             }, t.callPlayer = function(e) {
                 var t;
                 if (!this.player || !this.player[e]) {
                     var r = "ReactPlayer: ".concat(this.constructor.displayName, " player could not call %c").concat(e, "%c – ");
                     return this.player ? this.player[e] || (r += "The method was not available") : r += "The player was not available", console.warn(r, "font-weight: bold", ""), null
                 }
-                for (var n = arguments.length, a = Array(n > 1 ? n - 1 : 0), o = 1; o < n; o++) a[o - 1] = arguments[o];
-                return (t = this.player)[e].apply(t, a)
+                for (var n = arguments.length, o = Array(n > 1 ? n - 1 : 0), a = 1; a < n; a++) o[a - 1] = arguments[a];
+                return (t = this.player)[e].apply(t, o)
             }, t.isMediaStream = function(e) {
                 return "undefined" != typeof window && void 0 !== window.MediaStream && e instanceof window.MediaStream
             }, t.isBlobUrl = function(e) {
                 return /^blob:/.test(e)
             }, t.supportsWebKitPresentationMode = function() {
                 var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : document.createElement("video"),
                     t = !1 === /iPhone|iPod/.test(navigator.userAgent);
                 return e.webkitSupportsPresentationMode && "function" == typeof e.webkitSetPresentationMode && t
             };
-            var n = o(r(9090)),
-                a = o(r(9996));
+            var n = a(r(9090)),
+                o = a(r(9996));
 
-            function o(e) {
+            function a(e) {
                 return e && e.__esModule ? e : {
                     default: e
                 }
             }
 
-            function l(e, t) {
+            function i(e, t) {
                 (null == t || t > e.length) && (t = e.length);
                 for (var r = 0, n = Array(t); r < t; r++) n[r] = e[r];
                 return n
             }
-            var i = /[?&#](?:start|t)=([0-9hms]+)/,
+            var l = /[?&#](?:start|t)=([0-9hms]+)/,
                 u = /[?&#]end=([0-9hms]+)/,
                 s = /(\d+)(h|m|s)/g,
                 c = /^\d+$/;
 
-            function d(e, t) {
+            function f(e, t) {
                 if (!(e instanceof Array)) {
                     var r = e.match(t);
                     if (r) {
                         var n = r[1];
                         if (n.match(s)) return function(e) {
                             for (var t = 0, r = s.exec(e); null !== r;) {
-                                var n, a = function(e) {
+                                var n, o = function(e) {
                                         if (Array.isArray(e)) return e
                                     }(n = r) || function(e, t) {
                                         if ("undefined" != typeof Symbol && Symbol.iterator in Object(e)) {
                                             var r = [],
                                                 n = !0,
-                                                a = !1,
-                                                o = void 0;
+                                                o = !1,
+                                                a = void 0;
                                             try {
-                                                for (var l, i = e[Symbol.iterator](); !(n = (l = i.next()).done) && (r.push(l.value), !t || r.length !== t); n = !0);
+                                                for (var i, l = e[Symbol.iterator](); !(n = (i = l.next()).done) && (r.push(i.value), !t || r.length !== t); n = !0);
                                             } catch (e) {
-                                                a = !0, o = e
+                                                o = !0, a = e
                                             } finally {
                                                 try {
-                                                    n || null == i.return || i.return()
+                                                    n || null == l.return || l.return()
                                                 } finally {
-                                                    if (a) throw o
+                                                    if (o) throw a
                                                 }
                                             }
                                             return r
                                         }
                                     }(n, 3) || function(e, t) {
                                         if (e) {
-                                            if ("string" == typeof e) return l(e, t);
+                                            if ("string" == typeof e) return i(e, t);
                                             var r = Object.prototype.toString.call(e).slice(8, -1);
                                             if ("Object" === r && e.constructor && (r = e.constructor.name), "Map" === r || "Set" === r) return Array.from(e);
-                                            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return l(e, t)
+                                            if ("Arguments" === r || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(r)) return i(e, t)
                                         }
                                     }(n, 3) || function() {
                                         throw TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                                     }(),
-                                    o = a[1],
-                                    i = a[2];
-                                "h" === i && (t += 3600 * parseInt(o, 10)), "m" === i && (t += 60 * parseInt(o, 10)), "s" === i && (t += parseInt(o, 10)), r = s.exec(e)
+                                    a = o[1],
+                                    l = o[2];
+                                "h" === l && (t += 3600 * parseInt(a, 10)), "m" === l && (t += 60 * parseInt(a, 10)), "s" === l && (t += parseInt(a, 10)), r = s.exec(e)
                             }
                             return t
                         }(n);
                         if (c.test(n)) return parseInt(n)
                     }
                 }
             }
 
-            function f(e) {
+            function d(e) {
                 return window[e] ? window[e] : window.exports && window.exports[e] ? window.exports[e] : window.module && window.module.exports && window.module.exports[e] ? window.module.exports[e] : null
             }
             var p = {}
         }
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/699-1a88a588882ce475.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/699-a015e8646ccfaf97.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,68 @@
 "use strict";
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
     [699], {
+        8385: function(e, t, r) {
+            var n = r(7294),
+                o = r(3935),
+                i = r(3703),
+                l = r(3546),
+                a = r(7960),
+                s = r(5893);
+            let d = n.forwardRef(function(e, t) {
+                let {
+                    children: r,
+                    container: d,
+                    disablePortal: u = !1
+                } = e, [c, p] = n.useState(null), f = (0, i.Z)(n.isValidElement(r) ? r.ref : null, t);
+                return ((0, l.Z)(() => {
+                    !u && p(("function" == typeof d ? d() : d) || document.body)
+                }, [d, u]), (0, l.Z)(() => {
+                    if (c && !u) return (0, a.Z)(t, c), () => {
+                        (0, a.Z)(t, null)
+                    }
+                }, [t, c, u]), u) ? n.isValidElement(r) ? n.cloneElement(r, {
+                    ref: f
+                }) : (0, s.jsx)(n.Fragment, {
+                    children: r
+                }) : (0, s.jsx)(n.Fragment, {
+                    children: c ? o.createPortal(r, c) : c
+                })
+            });
+            t.Z = d
+        },
+        1873: function(e, t, r) {
+            r.d(t, {
+                T: function() {
+                    return i
+                }
+            });
+            var n = r(7294);
+            r(5893);
+            let o = n.createContext({
+                disableDefaultClasses: !1
+            });
+
+            function i(e) {
+                let {
+                    disableDefaultClasses: t
+                } = n.useContext(o);
+                return r => t ? "" : e(r)
+            }
+        },
         4808: function(e, t, r) {
             r.d(t, {
                 Z: function() {
                     return g
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(7294),
-                l = r(6010),
+                l = r(3680),
                 a = r(4780),
                 s = r(948),
                 d = r(1657),
                 u = r(6628),
                 c = r(1588),
                 p = r(4867);
 
@@ -123,15 +171,15 @@
                 Z: function() {
                     return R
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(7294),
-                l = r(6010),
+                l = r(3680),
                 a = r(4780),
                 s = r(1657),
                 d = r(948),
                 u = r(8712),
                 c = r(8216),
                 p = r(1579),
                 f = r(7167),
@@ -318,15 +366,15 @@
 
             function a(e) {
                 return (0, i.Z)("MuiInput", e)
             }
             let s = (0, n.Z)({}, l.Z, (0, o.Z)("MuiInput", ["root", "underline", "input"]));
             t.Z = s
         },
-        3032: function(e, t, r) {
+        3970: function(e, t, r) {
             r.d(t, {
                 rA: function() {
                     return j
                 },
                 Ej: function() {
                     return z
                 },
@@ -340,15 +388,15 @@
                     return N
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(1387),
                 l = r(7294),
-                a = r(6010),
+                a = r(3680),
                 s = r(4780),
                 d = r(3935),
                 u = r(3703),
                 c = r(4161),
                 p = r(9336),
                 f = r(3546),
                 m = r(5893);
@@ -453,20 +501,21 @@
                     }, x)), (0, m.jsx)("textarea", {
                         "aria-hidden": !0,
                         className: e.className,
                         readOnly: !0,
                         ref: S,
                         tabIndex: -1,
                         style: (0, o.Z)({}, b.shadow, s, {
-                            padding: 0
+                            paddingTop: 0,
+                            paddingBottom: 0
                         })
                     })]
                 })
             });
-            var x = r(3247),
+            var x = r(8442),
                 y = r(5704),
                 R = r(7167),
                 w = r(4423),
                 S = r(948),
                 P = r(1657),
                 k = r(8216),
                 C = r(1705),
@@ -849,15 +898,15 @@
                 Z: function() {
                     return g
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(7294),
-                l = r(6010),
+                l = r(3680),
                 a = r(4780),
                 s = r(948),
                 d = r(1657),
                 u = r(9773),
                 c = r(1588),
                 p = r(4867);
 
@@ -937,35 +986,35 @@
             var g = Z
         },
         9773: function(e, t, r) {
             var n = r(7294);
             let o = n.createContext({});
             t.Z = o
         },
-        9219: function(e, t, r) {
+        2980: function(e, t, r) {
             r.d(t, {
                 Z: function() {
                     return W
                 }
             });
             var n = r(3366),
                 o = r(7462),
                 i = r(7294),
-                l = r(6010),
+                l = r(3680),
                 a = r(3703),
                 s = r(2690),
                 d = r(9948);
 
             function u(...e) {
                 return e.reduce((e, t) => null == t ? e : function(...r) {
                     e.apply(this, r), t.apply(this, r)
                 }, () => {})
             }
             var c = r(4780),
-                p = r(8173),
+                p = r(8385),
                 f = r(4161),
                 m = r(5806);
 
             function h(e, t) {
                 t ? e.setAttribute("aria-hidden", "true") : e.removeAttribute("aria-hidden")
             }
 
@@ -1097,16 +1146,16 @@
                 },
                 w = r(1588),
                 S = r(4867);
 
             function P(e) {
                 return (0, S.Z)("MuiModal", e)
             }(0, w.Z)("MuiModal", ["root", "hidden", "backdrop"]);
-            var k = r(3249),
-                C = r(3905);
+            var k = r(9235),
+                C = r(1873);
             let E = ["children", "closeAfterTransition", "container", "disableAutoFocus", "disableEnforceFocus", "disableEscapeKeyDown", "disablePortal", "disableRestoreFocus", "disableScrollLock", "hideBackdrop", "keepMounted", "manager", "onBackdropClick", "onClose", "onKeyDown", "open", "onTransitionEnter", "onTransitionExited", "slotProps", "slots"],
                 M = e => {
                     let {
                         open: t,
                         exited: r
                     } = e;
                     return (0, c.Z)({
@@ -1126,20 +1175,20 @@
                             let t = [];
                             return [].forEach.call(e.children, e => {
                                 "true" === e.getAttribute("aria-hidden") && t.push(e)
                             }), t
                         }(t);
                         b(t, e.mount, e.modalRef, n, !0);
                         let o = Z(this.containers, e => e.container === t);
-                        return -1 !== o ? (this.containers[o].modals.push(e), r) : (this.containers.push({
+                        return -1 !== o ? this.containers[o].modals.push(e) : this.containers.push({
                             modals: [e],
                             container: t,
                             restore: null,
                             hiddenSiblings: n
-                        }), r)
+                        }), r
                     }
                     mount(e, t) {
                         let r = Z(this.containers, t => -1 !== t.modals.indexOf(e)),
                             n = this.containers[r];
                         n.restore || (n.restore = function(e, t) {
                             let r = [],
                                 n = e.container;
@@ -1311,16 +1360,16 @@
                                 isEnabled: J,
                                 open: O,
                                 children: i.cloneElement(c, en)
                             })]
                         }))
                     }) : null
                 });
-            var T = r(7488),
-                N = r(3247),
+            var T = r(1276),
+                N = r(8442),
                 O = r(948),
                 A = r(1657),
                 z = r(4808);
             let j = ["BackdropComponent", "BackdropProps", "classes", "className", "closeAfterTransition", "children", "container", "component", "components", "componentsProps", "disableAutoFocus", "disableEnforceFocus", "disableEscapeKeyDown", "disablePortal", "disableRestoreFocus", "disableScrollLock", "hideBackdrop", "keepMounted", "onBackdropClick", "onClose", "open", "slotProps", "slots", "theme"],
                 L = (0, O.ZP)("div", {
                     name: "MuiModal",
                     slot: "Root",
@@ -1500,15 +1549,15 @@
                         easing: t.transitions.easing.easeOut,
                         delay: 50
                     })
                 })));
             var f = r(4423),
                 m = r(5704),
                 h = r(4656),
-                v = r(3032),
+                v = r(3970),
                 b = r(1657);
             let Z = ["components", "fullWidth", "inputComponent", "label", "multiline", "notched", "slots", "type"],
                 g = e => {
                     let {
                         classes: t
                     } = e, r = (0, a.Z)({
                         root: ["root"],
@@ -1648,15 +1697,15 @@
                         } = c,
                         M = (0, o.Z)(c, Z),
                         I = g(c),
                         F = (0, f.Z)(),
                         T = (0, m.Z)({
                             props: c,
                             muiFormControl: F,
-                            states: ["required"]
+                            states: ["color", "disabled", "error", "focused", "hiddenLabel", "size", "required"]
                         }),
                         N = (0, i.Z)({}, c, {
                             color: T.color || "primary",
                             disabled: T.disabled,
                             error: T.error,
                             focused: T.focused,
                             formControl: F,
@@ -1717,21 +1766,21 @@
                 Z: function() {
                     return tb
                 }
             });
             var n, o, i = r(7462),
                 l = r(3366),
                 a = r(7294),
-                s = r(6010),
+                s = r(3680),
                 d = r(4780),
                 u = r(2996),
                 c = r(948),
                 p = r(1657),
                 f = r(9766),
-                m = r(3032),
+                m = r(3970),
                 h = r(7021),
                 v = r(5893);
             let b = ["disableUnderline", "components", "componentsProps", "fullWidth", "inputComponent", "multiline", "slotProps", "slots", "type"],
                 Z = e => {
                     let {
                         classes: t,
                         disableUnderline: r
@@ -2492,16 +2541,16 @@
                         p && p(e)
                     },
                     tabIndex: n ? 0 : -1
                 }, m, {
                     children: x
                 }))
             });
-            var ec = r(3249),
-                ep = r(3247),
+            var ec = r(9235),
+                ep = r(8442),
                 ef = r(7144),
                 em = r(5340),
                 eh = r(8662),
                 ev = r(2734),
                 eb = r(577);
             let eZ = ["addEndListener", "appear", "children", "easing", "in", "onEnter", "onEntered", "onEntering", "onExit", "onExited", "onExiting", "style", "timeout", "TransitionComponent"];
 
@@ -2608,15 +2657,15 @@
                                 visibility: "exited" !== e || d ? void 0 : "hidden"
                             }, ex[e], b, o.props.style),
                             ref: P
                         }, t))
                     }))
                 });
             eR.muiSupportAuto = !0;
-            var ew = r(9219),
+            var ew = r(2980),
                 eS = r(629);
 
             function eP(e) {
                 return (0, N.Z)("MuiPopover", e)
             }(0, T.Z)("MuiPopover", ["root", "paper"]);
             let ek = ["onEntering"],
                 eC = ["action", "anchorEl", "anchorOrigin", "anchorPosition", "anchorReference", "children", "className", "container", "elevation", "marginThreshold", "open", "PaperProps", "slots", "slotProps", "transformOrigin", "TransitionComponent", "transitionDuration", "TransitionProps"],
@@ -3118,16 +3167,16 @@
             var e5 = r(8712),
                 e2 = r(9299);
 
             function e7(e) {
                 return (0, N.Z)("MuiSelect", e)
             }
             let e4 = (0, T.Z)("MuiSelect", ["select", "multiple", "filled", "outlined", "standard", "disabled", "focused", "icon", "iconOpen", "iconFilled", "iconOutlined", "iconStandard", "nativeInput", "error"]),
-                e6 = ["aria-describedby", "aria-label", "autoFocus", "autoWidth", "children", "className", "defaultOpen", "defaultValue", "disabled", "displayEmpty", "error", "IconComponent", "inputRef", "labelId", "MenuProps", "multiple", "name", "onBlur", "onChange", "onClose", "onFocus", "onOpen", "open", "readOnly", "renderValue", "SelectDisplayProps", "tabIndex", "type", "value", "variant"],
-                e8 = (0, c.ZP)("div", {
+                e8 = ["aria-describedby", "aria-label", "autoFocus", "autoWidth", "children", "className", "defaultOpen", "defaultValue", "disabled", "displayEmpty", "error", "IconComponent", "inputRef", "labelId", "MenuProps", "multiple", "name", "onBlur", "onChange", "onClose", "onFocus", "onOpen", "open", "readOnly", "renderValue", "SelectDisplayProps", "tabIndex", "type", "value", "variant"],
+                e6 = (0, c.ZP)("div", {
                     name: "MuiSelect",
                     slot: "Select",
                     overridesResolver: (e, t) => {
                         let {
                             ownerState: r
                         } = e;
                         return [{
@@ -3221,15 +3270,15 @@
                         open: N,
                         readOnly: O,
                         renderValue: A,
                         SelectDisplayProps: z = {},
                         tabIndex: j,
                         value: L,
                         variant: $ = "standard"
-                    } = e, B = (0, l.Z)(e, e6), [W, D] = (0, e2.Z)({
+                    } = e, B = (0, l.Z)(e, e8), [W, D] = (0, e2.Z)({
                         controlled: L,
                         default: Z,
                         name: "Select"
                     }), [H, q] = (0, e2.Z)({
                         controlled: N,
                         default: b,
                         name: "Select"
@@ -3319,15 +3368,15 @@
                             variant: $,
                             value: W,
                             open: ea,
                             error: y
                         }),
                         em = tt(ef);
                     return (0, v.jsxs)(a.Fragment, {
-                        children: [(0, v.jsx)(e8, (0, i.Z)({
+                        children: [(0, v.jsx)(e6, (0, i.Z)({
                             ref: et,
                             tabIndex: void 0 !== j ? j : g ? null : 0,
                             role: "button",
                             "aria-disabled": g ? "true" : void 0,
                             "aria-expanded": ea ? "true" : "false",
                             "aria-haspopup": "listbox",
                             "aria-label": c,
@@ -3658,62 +3707,14 @@
             r(7294);
             var n = r(8169),
                 o = r(5893);
             t.Z = (0, n.Z)((0, o.jsx)("path", {
                 d: "M7 10l5 5 5-5z"
             }), "ArrowDropDown")
         },
-        8173: function(e, t, r) {
-            var n = r(7294),
-                o = r(3935),
-                i = r(3703),
-                l = r(3546),
-                a = r(7960),
-                s = r(5893);
-            let d = n.forwardRef(function(e, t) {
-                let {
-                    children: r,
-                    container: d,
-                    disablePortal: u = !1
-                } = e, [c, p] = n.useState(null), f = (0, i.Z)(n.isValidElement(r) ? r.ref : null, t);
-                return ((0, l.Z)(() => {
-                    !u && p(("function" == typeof d ? d() : d) || document.body)
-                }, [d, u]), (0, l.Z)(() => {
-                    if (c && !u) return (0, a.Z)(t, c), () => {
-                        (0, a.Z)(t, null)
-                    }
-                }, [t, c, u]), u) ? n.isValidElement(r) ? n.cloneElement(r, {
-                    ref: f
-                }) : (0, s.jsx)(n.Fragment, {
-                    children: r
-                }) : (0, s.jsx)(n.Fragment, {
-                    children: c ? o.createPortal(r, c) : c
-                })
-            });
-            t.Z = d
-        },
-        3905: function(e, t, r) {
-            r.d(t, {
-                T: function() {
-                    return i
-                }
-            });
-            var n = r(7294);
-            r(5893);
-            let o = n.createContext({
-                disableDefaultClasses: !1
-            });
-
-            function i(e) {
-                let {
-                    disableDefaultClasses: t
-                } = n.useContext(o);
-                return r => t ? "" : e(r)
-            }
-        },
         1579: function(e, t, r) {
             r.d(t, {
                 Z: function() {
                     return o
                 }
             });
             var n = r(7294),
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/731-eb947eaba8f94f26.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/731-b6cafe94e88ed8c7.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,134 @@
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
     [731], {
+        8442: function(e, t, l) {
+            "use strict";
+
+            function r(e) {
+                return "string" == typeof e
+            }
+            l.d(t, {
+                Z: function() {
+                    return r
+                }
+            })
+        },
+        1276: function(e, t, l) {
+            "use strict";
+
+            function r(e, t, l) {
+                return "function" == typeof e ? e(t, l) : e
+            }
+            l.d(t, {
+                Z: function() {
+                    return r
+                }
+            })
+        },
+        9235: function(e, t, l) {
+            "use strict";
+            l.d(t, {
+                Z: function() {
+                    return d
+                }
+            });
+            var r = l(7462),
+                o = l(3366),
+                n = l(3703),
+                i = l(8442),
+                a = function() {
+                    for (var e, t, l = 0, r = ""; l < arguments.length;)(e = arguments[l++]) && (t = function e(t) {
+                        var l, r, o = "";
+                        if ("string" == typeof t || "number" == typeof t) o += t;
+                        else if ("object" == typeof t) {
+                            if (Array.isArray(t))
+                                for (l = 0; l < t.length; l++) t[l] && (r = e(t[l])) && (o && (o += " "), o += r);
+                            else
+                                for (l in t) t[l] && (o && (o += " "), o += l)
+                        }
+                        return o
+                    }(e)) && (r && (r += " "), r += t);
+                    return r
+                };
+
+            function s(e) {
+                if (void 0 === e) return {};
+                let t = {};
+                return Object.keys(e).filter(t => !(t.match(/^on[A-Z]/) && "function" == typeof e[t])).forEach(l => {
+                    t[l] = e[l]
+                }), t
+            }
+            var c = l(1276);
+            let u = ["elementType", "externalSlotProps", "ownerState", "skipResolvingSlotProps"];
+
+            function d(e) {
+                var t, l;
+                let {
+                    elementType: d,
+                    externalSlotProps: f,
+                    ownerState: p,
+                    skipResolvingSlotProps: h = !1
+                } = e, b = (0, o.Z)(e, u), m = h ? {} : (0, c.Z)(f, p), {
+                    props: v,
+                    internalRef: y
+                } = function(e) {
+                    let {
+                        getSlotProps: t,
+                        additionalProps: l,
+                        externalSlotProps: o,
+                        externalForwardedProps: n,
+                        className: i
+                    } = e;
+                    if (!t) {
+                        let e = a(null == n ? void 0 : n.className, null == o ? void 0 : o.className, i, null == l ? void 0 : l.className),
+                            t = (0, r.Z)({}, null == l ? void 0 : l.style, null == n ? void 0 : n.style, null == o ? void 0 : o.style),
+                            s = (0, r.Z)({}, l, n, o);
+                        return e.length > 0 && (s.className = e), Object.keys(t).length > 0 && (s.style = t), {
+                            props: s,
+                            internalRef: void 0
+                        }
+                    }
+                    let c = function(e, t = []) {
+                            if (void 0 === e) return {};
+                            let l = {};
+                            return Object.keys(e).filter(l => l.match(/^on[A-Z]/) && "function" == typeof e[l] && !t.includes(l)).forEach(t => {
+                                l[t] = e[t]
+                            }), l
+                        }((0, r.Z)({}, n, o)),
+                        u = s(o),
+                        d = s(n),
+                        f = t(c),
+                        p = a(null == f ? void 0 : f.className, null == l ? void 0 : l.className, i, null == n ? void 0 : n.className, null == o ? void 0 : o.className),
+                        h = (0, r.Z)({}, null == f ? void 0 : f.style, null == l ? void 0 : l.style, null == n ? void 0 : n.style, null == o ? void 0 : o.style),
+                        b = (0, r.Z)({}, f, l, d, u);
+                    return p.length > 0 && (b.className = p), Object.keys(h).length > 0 && (b.style = h), {
+                        props: b,
+                        internalRef: f.ref
+                    }
+                }((0, r.Z)({}, b, {
+                    externalSlotProps: m
+                })), Z = (0, n.Z)(y, null == m ? void 0 : m.ref, null == (t = e.additionalProps) ? void 0 : t.ref), g = (l = (0, r.Z)({}, v, {
+                    ref: Z
+                }), void 0 === d || (0, i.Z)(d) ? l : (0, r.Z)({}, l, {
+                    ownerState: (0, r.Z)({}, l.ownerState, p)
+                }));
+                return g
+            }
+        },
         4267: function(e, t, l) {
             "use strict";
             l.d(t, {
                 Z: function() {
                     return y
                 }
             });
             var r = l(7462),
                 o = l(3366),
                 n = l(7294),
-                i = l(6010),
+                i = l(3680),
                 a = l(4780),
                 s = l(948),
                 c = l(1657),
                 u = l(1588),
                 d = l(4867);
 
             function f(e) {
@@ -69,15 +183,15 @@
                 Z: function() {
                     return x
                 }
             });
             var r = l(3366),
                 o = l(7462),
                 n = l(7294),
-                i = l(6010),
+                i = l(3680),
                 a = l(4780),
                 s = l(2022),
                 c = l(8216),
                 u = l(1657),
                 d = l(948),
                 f = l(1588),
                 p = l(4867);
@@ -248,17 +362,17 @@
                     return K
                 }
             });
             var o = l(3366),
                 n = l(7462),
                 i = l(7294);
             l(9864);
-            var a = l(6010),
+            var a = l(3680),
                 s = l(4780),
-                c = l(3249),
+                c = l(9235),
                 u = l(948),
                 d = l(1657),
                 f = l(2734),
                 p = l(7144);
 
             function h() {
                 if (r) return r;
@@ -317,15 +431,15 @@
                         orientation: l,
                         disabled: r
                     } = e;
                     return (0, s.Z)({
                         root: ["root", l, r && "disabled"]
                     }, E, t)
                 },
-                N = (0, u.ZP)(_.Z, {
+                k = (0, u.ZP)(_.Z, {
                     name: "MuiTabScrollButton",
                     slot: "Root",
                     overridesResolver: (e, t) => {
                         let {
                             ownerState: l
                         } = e;
                         return [t.root, l.orientation && t[l.orientation]]
@@ -342,15 +456,15 @@
                 }, "vertical" === e.orientation && {
                     width: "100%",
                     height: 40,
                     "& svg": {
                         transform: `rotate(${e.isRtl?-90:90}deg)`
                     }
                 })),
-                k = i.forwardRef(function(e, t) {
+                N = i.forwardRef(function(e, t) {
                     var l, r;
                     let i = (0, d.Z)({
                             props: e,
                             name: "MuiTabScrollButton"
                         }),
                         {
                             className: s,
@@ -379,15 +493,15 @@
                             elementType: w,
                             externalSlotProps: p.endScrollButtonIcon,
                             additionalProps: {
                                 fontSize: "small"
                             },
                             ownerState: y
                         });
-                    return (0, Z.jsx)(N, (0, n.Z)({
+                    return (0, Z.jsx)(k, (0, n.Z)({
                         component: "div",
                         className: (0, a.Z)(g.root, s),
                         ref: t,
                         role: null,
                         ownerState: y,
                         tabIndex: null
                     }, b, {
@@ -590,18 +704,18 @@
                             children: w,
                             className: S,
                             component: C = "div",
                             allowScrollButtonsMobile: _ = !1,
                             indicatorColor: B = "primary",
                             onChange: P,
                             orientation: E = "horizontal",
-                            ScrollButtonComponent: M = k,
+                            ScrollButtonComponent: M = N,
                             scrollButtons: R = "auto",
                             selectionFollowsFocus: T,
-                            slots: N = {},
+                            slots: k = {},
                             slotProps: W = {},
                             TabIndicatorProps: I = {},
                             TabScrollButtonProps: q = {},
                             textColor: K = "primary",
                             value: U,
                             variant: J = "standard",
                             visibleScrollbar: Q = !1
@@ -629,20 +743,20 @@
                             scrollableX: et && !el,
                             scrollableY: et && el,
                             centered: x && !et,
                             scrollButtonsHideMobile: !_
                         }),
                         ec = H(es),
                         eu = (0, c.Z)({
-                            elementType: N.StartScrollButtonIcon,
+                            elementType: k.StartScrollButtonIcon,
                             externalSlotProps: W.startScrollButtonIcon,
                             ownerState: es
                         }),
                         ed = (0, c.Z)({
-                            elementType: N.EndScrollButtonIcon,
+                            elementType: k.EndScrollButtonIcon,
                             externalSlotProps: W.endScrollButtonIcon,
                             ownerState: es
                         }),
                         [ef, ep] = i.useState(!1),
                         [eh, eb] = i.useState(G),
                         [em, ev] = i.useState({
                             start: !1,
@@ -709,32 +823,32 @@
                         e_ = (e, {
                             animation: t = !0
                         } = {}) => {
                             t ? function(e, t, l, r = {}, o = () => {}) {
                                 let {
                                     ease: n = m,
                                     duration: i = 300
-                                } = r, a = null, s = t[e], c = !1, u = () => {
-                                    c = !0
-                                }, d = r => {
+                                } = r, a = null, s = t[e], c = !1, u = r => {
                                     if (c) {
                                         o(Error("Animation cancelled"));
                                         return
                                     }
                                     null === a && (a = r);
-                                    let u = Math.min(1, (r - a) / i);
-                                    if (t[e] = n(u) * (l - s) + s, u >= 1) {
+                                    let d = Math.min(1, (r - a) / i);
+                                    if (t[e] = n(d) * (l - s) + s, d >= 1) {
                                         requestAnimationFrame(() => {
                                             o(null)
                                         });
                                         return
                                     }
-                                    requestAnimationFrame(d)
+                                    requestAnimationFrame(u)
                                 };
-                                return s === l ? (o(Error("Element already at target position")), u) : (requestAnimationFrame(d), u)
+                                return s === l ? o(Error("Element already at target position")) : requestAnimationFrame(u), () => {
+                                    c = !0
+                                }
                             }(er, ex.current, e, {
                                 duration: r.transitions.duration.standard
                             }) : ex.current[er] = e
                         },
                         eB = e => {
                             let t = ex.current[er];
                             el ? t += e : (t += e * (s ? -1 : 1), t *= s && "reverse" === h() ? -1 : 1), e_(t)
@@ -780,15 +894,15 @@
                                     let r = t[er] + (l[en] - t[en]);
                                     e_(r, {
                                         animation: e
                                     })
                                 }
                             }
                         }),
-                        eN = (0, j.Z)(() => {
+                        ek = (0, j.Z)(() => {
                             if (et && !1 !== R) {
                                 let e, t;
                                 let {
                                     scrollTop: l,
                                     scrollHeight: o,
                                     clientHeight: n,
                                     scrollWidth: i,
@@ -803,38 +917,38 @@
                                     end: t
                                 })
                             }
                         });
                     i.useEffect(() => {
                         let e;
                         let t = (0, p.Z)(() => {
-                                ex.current && (eC(), eN())
+                                ex.current && (eC(), ek())
                             }),
                             l = (0, y.Z)(ex.current);
                         return l.addEventListener("resize", t), "undefined" != typeof ResizeObserver && (e = new ResizeObserver(t), Array.from(ew.current.children).forEach(t => {
                             e.observe(t)
                         })), () => {
                             t.clear(), l.removeEventListener("resize", t), e && e.disconnect()
                         }
-                    }, [eC, eN]);
-                    let ek = i.useMemo(() => (0, p.Z)(() => {
-                        eN()
-                    }), [eN]);
+                    }, [eC, ek]);
+                    let eN = i.useMemo(() => (0, p.Z)(() => {
+                        ek()
+                    }), [ek]);
                     i.useEffect(() => () => {
-                        ek.clear()
-                    }, [ek]), i.useEffect(() => {
+                        eN.clear()
+                    }, [eN]), i.useEffect(() => {
                         ep(!0)
                     }, []), i.useEffect(() => {
-                        eC(), eN()
+                        eC(), ek()
                     }), i.useEffect(() => {
                         eT(G !== eh)
                     }, [eT, eh]), i.useImperativeHandle(g, () => ({
                         updateIndicator: eC,
-                        updateScrollButtons: eN
-                    }), [eC, eN]);
+                        updateScrollButtons: ek
+                    }), [eC, ek]);
                     let ej = (0, Z.jsx)(V, (0, n.Z)({}, I, {
                             className: (0, a.Z)(ec.indicator, I.className),
                             ownerState: es,
                             style: (0, n.Z)({}, eh, I.style)
                         })),
                         eW = 0,
                         eI = i.Children.map(w, e => {
@@ -860,28 +974,28 @@
                                 onChange: eR,
                                 className: (0, a.Z)(ec.scrollableX, ec.hideScrollbar)
                             }) : null;
                             let t = em.start || em.end,
                                 l = et && ("auto" === R && t || !0 === R);
                             return e.scrollButtonStart = l ? (0, Z.jsx)(M, (0, n.Z)({
                                 slots: {
-                                    StartScrollButtonIcon: N.StartScrollButtonIcon
+                                    StartScrollButtonIcon: k.StartScrollButtonIcon
                                 },
                                 slotProps: {
                                     startScrollButtonIcon: eu
                                 },
                                 orientation: E,
                                 direction: s ? "right" : "left",
                                 onClick: eE,
                                 disabled: !em.start
                             }, q, {
                                 className: (0, a.Z)(ec.scrollButtons, q.className)
                             })) : null, e.scrollButtonEnd = l ? (0, Z.jsx)(M, (0, n.Z)({
                                 slots: {
-                                    EndScrollButtonIcon: N.EndScrollButtonIcon
+                                    EndScrollButtonIcon: k.EndScrollButtonIcon
                                 },
                                 slotProps: {
                                     endScrollButtonIcon: ed
                                 },
                                 orientation: E,
                                 direction: s ? "left" : "right",
                                 onClick: eM,
@@ -900,15 +1014,15 @@
                             className: ec.scroller,
                             ownerState: es,
                             style: {
                                 overflow: ey.overflow,
                                 [el ? `margin${s?"Left":"Right"}` : "marginBottom"]: Q ? void 0 : -ey.scrollbarWidth
                             },
                             ref: ex,
-                            onScroll: ek,
+                            onScroll: eN,
                             children: [(0, Z.jsx)(X, {
                                 "aria-label": u,
                                 "aria-labelledby": v,
                                 "aria-orientation": "vertical" === E ? "vertical" : null,
                                 className: ec.flexContainer,
                                 ownerState: es,
                                 onKeyDown: e => {
@@ -937,114 +1051,14 @@
                                 children: eI
                             }), ef && ej]
                         }), eL.scrollButtonEnd]
                     }))
                 });
             var K = q
         },
-        3247: function(e, t, l) {
-            "use strict";
-
-            function r(e) {
-                return "string" == typeof e
-            }
-            l.d(t, {
-                Z: function() {
-                    return r
-                }
-            })
-        },
-        7488: function(e, t, l) {
-            "use strict";
-
-            function r(e, t) {
-                return "function" == typeof e ? e(t) : e
-            }
-            l.d(t, {
-                Z: function() {
-                    return r
-                }
-            })
-        },
-        3249: function(e, t, l) {
-            "use strict";
-            l.d(t, {
-                Z: function() {
-                    return d
-                }
-            });
-            var r = l(7462),
-                o = l(3366),
-                n = l(3703),
-                i = l(3247),
-                a = l(6010);
-
-            function s(e) {
-                if (void 0 === e) return {};
-                let t = {};
-                return Object.keys(e).filter(t => !(t.match(/^on[A-Z]/) && "function" == typeof e[t])).forEach(l => {
-                    t[l] = e[l]
-                }), t
-            }
-            var c = l(7488);
-            let u = ["elementType", "externalSlotProps", "ownerState"];
-
-            function d(e) {
-                var t, l;
-                let {
-                    elementType: d,
-                    externalSlotProps: f,
-                    ownerState: p
-                } = e, h = (0, o.Z)(e, u), b = (0, c.Z)(f, p), {
-                    props: m,
-                    internalRef: v
-                } = function(e) {
-                    let {
-                        getSlotProps: t,
-                        additionalProps: l,
-                        externalSlotProps: o,
-                        externalForwardedProps: n,
-                        className: i
-                    } = e;
-                    if (!t) {
-                        let e = (0, a.Z)(null == n ? void 0 : n.className, null == o ? void 0 : o.className, i, null == l ? void 0 : l.className),
-                            t = (0, r.Z)({}, null == l ? void 0 : l.style, null == n ? void 0 : n.style, null == o ? void 0 : o.style),
-                            s = (0, r.Z)({}, l, n, o);
-                        return e.length > 0 && (s.className = e), Object.keys(t).length > 0 && (s.style = t), {
-                            props: s,
-                            internalRef: void 0
-                        }
-                    }
-                    let c = function(e, t = []) {
-                            if (void 0 === e) return {};
-                            let l = {};
-                            return Object.keys(e).filter(l => l.match(/^on[A-Z]/) && "function" == typeof e[l] && !t.includes(l)).forEach(t => {
-                                l[t] = e[t]
-                            }), l
-                        }((0, r.Z)({}, n, o)),
-                        u = s(o),
-                        d = s(n),
-                        f = t(c),
-                        p = (0, a.Z)(null == f ? void 0 : f.className, null == l ? void 0 : l.className, i, null == n ? void 0 : n.className, null == o ? void 0 : o.className),
-                        h = (0, r.Z)({}, null == f ? void 0 : f.style, null == l ? void 0 : l.style, null == n ? void 0 : n.style, null == o ? void 0 : o.style),
-                        b = (0, r.Z)({}, f, l, d, u);
-                    return p.length > 0 && (b.className = p), Object.keys(h).length > 0 && (b.style = h), {
-                        props: b,
-                        internalRef: f.ref
-                    }
-                }((0, r.Z)({}, h, {
-                    externalSlotProps: b
-                })), y = (0, n.Z)(v, null == b ? void 0 : b.ref, null == (t = e.additionalProps) ? void 0 : t.ref), Z = (l = (0, r.Z)({}, m, {
-                    ref: y
-                }), void 0 === d || (0, i.Z)(d) ? l : (0, r.Z)({}, l, {
-                    ownerState: (0, r.Z)({}, l.ownerState, p)
-                }));
-                return Z
-            }
-        },
         2690: function(e, t, l) {
             "use strict";
 
             function r(e) {
                 return e && e.ownerDocument || document
             }
             l.d(t, {
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/75fc9c18-c0cb841eaf75495d.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1410,15 +1410,15 @@
                     if (o(e) && (t = e, e = void 0), e = e || "", null != t) return tz(e, t, n, "month");
                     var s, i = [];
                     for (s = 0; s < 12; s++) i[s] = tz(e, s, n, "month");
                     return i
                 }
 
                 function tq(e, t, n, s) {
-                    "boolean" == typeof e ? (o(t) && (n = t, t = void 0), t = t || "") : (n = t = e, e = !1, o(t) && (n = t, t = void 0), t = t || "");
+                    "boolean" == typeof e || (n = t = e, e = !1), o(t) && (n = t, t = void 0), t = t || "";
                     var i, r = eQ(),
                         a = e ? r._week.dow : 0,
                         u = [];
                     if (null != n) return tz(t, (n + a) % 7, s, "day");
                     for (i = 0; i < 7; i++) u[i] = tz(t, (i + a) % 7, s, "day");
                     return u
                 }
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/767-b6df483a2f96f15d.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/767-21712ed9071ee20e.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -6,19 +6,19 @@
                 Z: function() {
                     return W
                 }
             });
             var o = r(3366),
                 a = r(7462),
                 i = r(7294),
-                n = r(6010),
+                n = r(3680),
                 l = r(4780),
                 s = r(2996),
                 d = r(8216),
-                c = r(9219),
+                c = r(2980),
                 p = r(6628),
                 u = r(629),
                 m = r(1657),
                 Z = r(948),
                 v = r(1588),
                 f = r(4867);
 
@@ -260,15 +260,15 @@
                 Z: function() {
                     return h
                 }
             });
             var o = r(3366),
                 a = r(7462),
                 i = r(7294),
-                n = r(6010),
+                n = r(3680),
                 l = r(4780),
                 s = r(948),
                 d = r(1657),
                 c = r(1588),
                 p = r(4867);
 
             function u(e) {
@@ -334,15 +334,15 @@
                 Z: function() {
                     return y
                 }
             });
             var o = r(3366),
                 a = r(7462),
                 i = r(7294),
-                n = r(6010),
+                n = r(3680),
                 l = r(4780),
                 s = r(948),
                 d = r(1657),
                 c = r(1588),
                 p = r(4867);
 
             function u(e) {
@@ -408,15 +408,15 @@
                 });
             var y = h
         },
         7645: function(e, t, r) {
             var o = r(7462),
                 a = r(3366),
                 i = r(7294),
-                n = r(6010),
+                n = r(3680),
                 l = r(4780),
                 s = r(5861),
                 d = r(948),
                 c = r(1657),
                 p = r(4472),
                 u = r(4182),
                 m = r(5893);
@@ -482,17 +482,17 @@
                 ZP: function() {
                     return W
                 }
             });
             var o = r(3366),
                 a = r(7462),
                 i = r(7294),
-                n = r(6010),
+                n = r(3680),
                 l = r(4780),
-                s = r(3247),
+                s = r(8442),
                 d = r(1796),
                 c = r(948),
                 p = r(1657),
                 u = r(2022),
                 m = r(1579),
                 Z = r(8974),
                 v = r(1705),
@@ -723,15 +723,15 @@
                 Z: function() {
                     return y
                 }
             });
             var o = r(3366),
                 a = r(7462),
                 i = r(7294),
-                n = r(6010),
+                n = r(3680),
                 l = r(4780),
                 s = r(948),
                 d = r(1657),
                 c = r(9773),
                 p = r(1588),
                 u = r(4867);
 
@@ -796,15 +796,15 @@
                 Z: function() {
                     return x
                 }
             });
             var o = r(3366),
                 a = r(7462),
                 i = r(7294),
-                n = r(6010),
+                n = r(3680),
                 l = r(4780),
                 s = r(5861),
                 d = r(9773),
                 c = r(1657),
                 p = r(948),
                 u = r(1588),
                 m = r(4867);
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/826-e44464776abed9eb.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/826-25c5c840b401fbf5.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -6,15 +6,15 @@
                 Z: function() {
                     return b
                 }
             });
             var r = a(3366),
                 o = a(7462),
                 n = a(7294),
-                i = a(6010),
+                i = a(3680),
                 s = a(4780),
                 l = a(948),
                 d = a(1657),
                 c = a(5861),
                 u = a(1588),
                 p = a(4867);
 
@@ -65,15 +65,15 @@
                 Z: function() {
                     return $
                 }
             });
             var r, o = a(3366),
                 n = a(7462),
                 i = a(7294),
-                s = a(6010),
+                s = a(3680),
                 l = a(4780),
                 d = a(8216),
                 c = a(5861),
                 u = a(7167),
                 p = a(4423),
                 m = a(948),
                 h = a(1588),
@@ -177,15 +177,15 @@
                 });
             var $ = k
         },
         8619: function(e, t, a) {
             var r = a(3366),
                 o = a(7462),
                 n = a(7294),
-                i = a(6010),
+                i = a(3680),
                 s = a(4780),
                 l = a(1796),
                 d = a(948),
                 c = a(1657),
                 u = a(2022),
                 p = a(8974),
                 m = a(1705),
@@ -331,15 +331,15 @@
                 Z: function() {
                     return b
                 }
             });
             var r = a(3366),
                 o = a(7462),
                 n = a(7294),
-                i = a(6010),
+                i = a(3680),
                 s = a(4780),
                 l = a(948),
                 d = a(1657),
                 c = a(1588),
                 u = a(4867);
 
             function p(e) {
@@ -404,15 +404,15 @@
                 Z: function() {
                     return B
                 }
             });
             var r = a(3366),
                 o = a(7462),
                 n = a(7294),
-                i = a(6010),
+                i = a(3680),
                 s = a(4780),
                 l = a(1796),
                 d = a(8216),
                 c = a(948),
                 u = a(9299),
                 p = a(4423),
                 m = a(2022),
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/913-948b3bc7b49750f4.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/713-76d25fee0de05077.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 "use strict";
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
-    [913], {
-        3913: function(e, t, o) {
+    [713], {
+        9713: function(e, t, o) {
             o.d(t, {
                 Z: function() {
                     return tI
                 }
             });
             var r, n, a, i, l, s, c, p = o(3366),
                 u = o(7462),
                 d = o(7294),
-                f = o(6010),
+                f = o(3680),
                 m = o(4780),
                 g = o(2996),
                 h = o(9032),
                 v = e => {
                     let t = d.useRef({});
                     return d.useEffect(() => {
                         t.current = e
@@ -1042,23 +1042,23 @@
                             return e()
                         }), i = []
                     }
                     return c.setOptions(o).then(function(e) {
                         !s && o.onFirstUpdate && o.onFirstUpdate(e)
                     }), c
                 }),
-                eR = o(8173),
+                eR = o(8385),
                 eL = o(4867),
                 eA = o(1588);
 
             function eD(e) {
                 return (0, eL.Z)("MuiPopper", e)
             }(0, eA.Z)("MuiPopper", ["root"]);
-            var eE = o(3249),
-                eM = o(3905),
+            var eE = o(9235),
+                eM = o(1873),
                 eT = o(5893);
             let ej = ["anchorEl", "children", "direction", "disablePortal", "modifiers", "open", "placement", "popperOptions", "popperRef", "slotProps", "slots", "TransitionProps", "ownerState"],
                 eN = ["anchorEl", "children", "container", "direction", "disablePortal", "keepMounted", "modifiers", "open", "placement", "popperOptions", "popperRef", "style", "transition", "slotProps", "slots"];
 
             function ez(e) {
                 return "function" == typeof e ? e() : e
             }
@@ -1362,16 +1362,16 @@
                         ref: t,
                         ownerState: d
                     }, c))
                 });
             e1.muiSkipListHighlight = !0;
             var e2 = o(629),
                 e4 = o(3946),
-                e6 = o(8169),
-                e5 = (0, e6.Z)((0, eT.jsx)("path", {
+                e5 = o(8169),
+                e6 = (0, e5.Z)((0, eT.jsx)("path", {
                     d: "M12 2C6.47 2 2 6.47 2 12s4.47 10 10 10 10-4.47 10-10S17.53 2 12 2zm5 13.59L15.59 17 12 13.41 8.41 17 7 15.59 10.59 12 7 8.41 8.41 7 12 10.59 15.59 7 17 8.41 13.41 12 17 15.59z"
                 }), "Cancel"),
                 e7 = o(1705),
                 e9 = o(2022);
 
             function e3(e) {
                 return (0, eL.Z)("MuiChip", e)
@@ -1672,15 +1672,15 @@
                     }, v && {
                         disableRipple: !0
                     }) : {},
                     D = null;
                 v && (D = s && d.isValidElement(s) ? d.cloneElement(s, {
                     className: (0, f.Z)(s.props.className, L.deleteIcon),
                     onClick: S
-                }) : (0, eT.jsx)(e5, {
+                }) : (0, eT.jsx)(e6, {
                     className: (0, f.Z)(L.deleteIcon),
                     onClick: S
                 }));
                 let E = null;
                 r && d.isValidElement(r) && (E = d.cloneElement(r, {
                     className: (0, f.Z)(L.avatar, r.props.className)
                 }));
@@ -1709,15 +1709,15 @@
                     }), D]
                 }))
             });
             var ti = o(7021),
                 tl = o(5827),
                 ts = o(4656),
                 tc = o(4707),
-                tp = (0, e6.Z)((0, eT.jsx)("path", {
+                tp = (0, e5.Z)((0, eT.jsx)("path", {
                     d: "M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"
                 }), "Close"),
                 tu = o(224);
 
             function td(e) {
                 return (0, eL.Z)("MuiAutocomplete", e)
             }
@@ -2701,15 +2701,15 @@
                             });
                             return eX((0, u.Z)({}, o, {
                                 className: eK.option
                             }), e, {
                                 selected: o["aria-selected"],
                                 index: t,
                                 inputValue: eE
-                            })
+                            }, eq)
                         },
                         eJ = null != (o = eg.clearIndicator) ? o : D.clearIndicator,
                         eQ = null != (r = eg.paper) ? r : D.paper,
                         e0 = null != (n = eg.popper) ? n : D.popper,
                         e1 = null != (a = eg.popupIndicator) ? a : D.popupIndicator;
                     return (0, eT.jsxs)(d.Fragment, {
                         children: [(0, eT.jsx)(tv, (0, u.Z)({
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/framework-305cb810cde7afac.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/framework-7a7e500878b44665.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -881,15 +881,15 @@
             function nP(e, n, t, r, l, a) {
                 return null === e || e.nativeEvent !== a ? (e = {
                     blockedOn: n,
                     domEventName: t,
                     eventSystemFlags: r,
                     nativeEvent: a,
                     targetContainers: [l]
-                }, null !== n && null !== (n = rD(n)) && np(n), e) : (e.eventSystemFlags |= r, n = e.targetContainers, null !== l && -1 === n.indexOf(l) && n.push(l), e)
+                }, null !== n && null !== (n = rD(n)) && np(n)) : (e.eventSystemFlags |= r, n = e.targetContainers, null !== l && -1 === n.indexOf(l) && n.push(l)), e
             }
 
             function nN(e) {
                 var n = rO(e.target);
                 if (null !== n) {
                     var t = eW(n);
                     if (null !== t) {
@@ -2693,28 +2693,28 @@
                 }
 
                 function u(n) {
                     return e && null === n.alternate && (n.flags |= 2), n
                 }
 
                 function o(e, n, t, r) {
-                    return null === n || 6 !== n.tag ? ((n = oZ(t, e.mode, r)).return = e, n) : ((n = l(n, t)).return = e, n)
+                    return null === n || 6 !== n.tag ? (n = oZ(t, e.mode, r)).return = e : (n = l(n, t)).return = e, n
                 }
 
                 function i(e, n, t, r) {
                     var a = t.type;
-                    return a === z ? c(e, n, t.props.children, r, t.key) : null !== n && (n.elementType === a || "object" == typeof a && null !== a && a.$$typeof === U && l0(a) === n.type) ? ((r = l(n, t.props)).ref = lZ(e, n, t), r.return = e, r) : ((r = oY(t.type, t.key, t.props, null, e.mode, r)).ref = lZ(e, n, t), r.return = e, r)
+                    return a === z ? c(e, n, t.props.children, r, t.key) : (null !== n && (n.elementType === a || "object" == typeof a && null !== a && a.$$typeof === U && l0(a) === n.type) ? (r = l(n, t.props)).ref = lZ(e, n, t) : (r = oY(t.type, t.key, t.props, null, e.mode, r)).ref = lZ(e, n, t), r.return = e, r)
                 }
 
                 function s(e, n, t, r) {
-                    return null === n || 4 !== n.tag || n.stateNode.containerInfo !== t.containerInfo || n.stateNode.implementation !== t.implementation ? ((n = oJ(t, e.mode, r)).return = e, n) : ((n = l(n, t.children || [])).return = e, n)
+                    return null === n || 4 !== n.tag || n.stateNode.containerInfo !== t.containerInfo || n.stateNode.implementation !== t.implementation ? (n = oJ(t, e.mode, r)).return = e : (n = l(n, t.children || [])).return = e, n
                 }
 
                 function c(e, n, t, r, a) {
-                    return null === n || 7 !== n.tag ? ((n = oX(t, e.mode, r, a)).return = e, n) : ((n = l(n, t)).return = e, n)
+                    return null === n || 7 !== n.tag ? (n = oX(t, e.mode, r, a)).return = e : (n = l(n, t)).return = e, n
                 }
 
                 function d(e, n, t) {
                     if ("string" == typeof n && "" !== n || "number" == typeof n) return (n = oZ("" + n, e.mode, t)).return = e, n;
                     if ("object" == typeof n && null !== n) {
                         switch (n.$$typeof) {
                             case P:
@@ -2849,15 +2849,15 @@
                             for (h = r(l, h); !y.done; g++, y = o.next()) null !== (y = m(h, l, g, y.value, i)) && (e && null !== y.alternate && h.delete(null === y.key ? g : y.key), u = a(y, u, g), null === c ? s = y : c.sibling = y, c = y);
                             return e && h.forEach(function(e) {
                                 return n(l, e)
                             }), lc && ll(l, g), s
                         }(i, s, c, h);
                         lJ(i, c)
                     }
-                    return "string" == typeof c && "" !== c || "number" == typeof c ? (c = "" + c, null !== s && 6 === s.tag ? (t(i, s.sibling), (s = l(s, c)).return = i, i = s) : (t(i, s), (s = oZ(c, i.mode, h)).return = i, i = s), u(i)) : t(i, s)
+                    return "string" == typeof c && "" !== c || "number" == typeof c ? (c = "" + c, null !== s && 6 === s.tag ? (t(i, s.sibling), (s = l(s, c)).return = i) : (t(i, s), (s = oZ(c, i.mode, h)).return = i), u(i = s)) : t(i, s)
                 }
             }
             var l2 = l1(!0),
                 l3 = l1(!1),
                 l4 = {},
                 l8 = rA(l4),
                 l5 = rA(l4),
@@ -3533,15 +3533,15 @@
                     if ((n = 13 === e.tag) && (n = null === (n = e.memoizedState) || null !== n.dehydrated), n) return e;
                     e = e.return
                 } while (null !== e);
                 return null
             }
 
             function ur(e, n, t, r, l) {
-                return 0 == (1 & e.mode) ? (e === n ? e.flags |= 65536 : (e.flags |= 128, t.flags |= 131072, t.flags &= -52805, 1 === t.tag && (null === t.alternate ? t.tag = 17 : ((n = lV(-1, 1)).tag = 2, l$(t, n, 1))), t.lanes |= 1), e) : (e.flags |= 65536, e.lanes = l, e)
+                return 0 == (1 & e.mode) ? e === n ? e.flags |= 65536 : (e.flags |= 128, t.flags |= 131072, t.flags &= -52805, 1 === t.tag && (null === t.alternate ? t.tag = 17 : ((n = lV(-1, 1)).tag = 2, l$(t, n, 1))), t.lanes |= 1) : (e.flags |= 65536, e.lanes = l), e
             }
             var ul = C.ReactCurrentOwner,
                 ua = !1;
 
             function uu(e, n, t, r) {
                 n.child = null === e ? l3(n, null, t, r) : l2(n, e.child, t, r)
             }
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/main-d5c9aef8f3ea3bae.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/main-2ecf43899f8683c2.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -232,15 +232,15 @@
                     router: function() {
                         return n
                     },
                     emitter: function() {
                         return V
                     },
                     initialize: function() {
-                        return J
+                        return K
                     },
                     hydrate: function() {
                         return ec
                     }
                 });
             let g = r(8754);
             r(37);
@@ -250,48 +250,48 @@
                 v = g._(r(6595)),
                 P = r(9955),
                 w = r(3105),
                 S = r(3162),
                 j = r(3908),
                 O = r(7905),
                 E = r(9064),
-                x = r(3232),
-                R = g._(r(9623)),
+                R = r(3232),
+                x = g._(r(9623)),
                 C = g._(r(9030)),
                 M = g._(r(5108)),
                 A = r(2827),
                 L = r(6885),
-                T = r(676),
-                I = r(3341),
+                I = r(676),
+                T = r(3341),
                 N = r(9577),
                 k = r(2140),
                 D = r(4224),
                 B = r(9486),
                 H = r(8463),
                 U = g._(r(4225)),
                 F = e => t => e(t) + "",
-                q = r.u;
-            r.u = F(q);
-            let W = r.k;
-            r.k = F(W);
+                W = r.u;
+            r.u = F(W);
+            let q = r.k;
+            r.k = F(q);
             let z = r.miniCssF;
             r.miniCssF = F(z);
-            let G = "13.4.7",
+            let G = "13.4.10",
                 V = (0, v.default)(),
                 X = e => [].slice.call(e),
-                Y = !1;
+                $ = !1;
             self.__next_require__ = r;
-            class $ extends y.default.Component {
+            class Y extends y.default.Component {
                 componentDidCatch(e, t) {
                     this.props.fn(e, t)
                 }
                 componentDidMount() {
-                    this.scrollToHash(), n.isSsr && (a.isFallback || a.nextExport && ((0, S.isDynamicRoute)(n.pathname) || location.search || Y) || a.props && a.props.__N_SSG && (location.search || Y)) && n.replace(n.pathname + "?" + String((0, j.assign)((0, j.urlQueryToSearchParams)(n.query), new URLSearchParams(location.search))), o, {
+                    this.scrollToHash(), n.isSsr && (a.isFallback || a.nextExport && ((0, S.isDynamicRoute)(n.pathname) || location.search || $) || a.props && a.props.__N_SSG && (location.search || $)) && n.replace(n.pathname + "?" + String((0, j.assign)((0, j.urlQueryToSearchParams)(n.query), new URLSearchParams(location.search))), o, {
                         _h: 1,
-                        shallow: !a.isFallback && !Y
+                        shallow: !a.isFallback && !$
                     }).catch(e => {
                         if (!e.cancelled) throw e
                     })
                 }
                 componentDidUpdate() {
                     this.scrollToHash()
                 }
@@ -303,15 +303,15 @@
                     let t = document.getElementById(e);
                     t && setTimeout(() => t.scrollIntoView(), 0)
                 }
                 render() {
                     return this.props.children
                 }
             }
-            async function J(e) {
+            async function K(e) {
                 void 0 === e && (e = {}), a = JSON.parse(document.getElementById("__NEXT_DATA__").textContent), window.__NEXT_DATA__ = a, p = a.defaultLocale;
                 let t = a.assetPrefix || "";
                 if (r.p = "" + t + "/_next/", (0, O.setConfig)({
                         serverRuntimeConfig: {},
                         publicRuntimeConfig: a.runtimeConfig || {}
                     }), o = (0, E.getURL)(), (0, k.hasBasePath)(o) && (o = (0, N.removeBasePath)(o)), a.scriptLoader) {
                     let {
@@ -320,45 +320,45 @@
                     e(a.scriptLoader)
                 }
                 i = new C.default(a.buildId, t);
                 let s = e => {
                     let [t, r] = e;
                     return i.routeLoader.onEntrypoint(t, r)
                 };
-                return window.__NEXT_P && window.__NEXT_P.map(e => setTimeout(() => s(e), 0)), window.__NEXT_P = [], window.__NEXT_P.push = s, (u = (0, R.default)()).getIsSsr = () => n.isSsr, l = document.getElementById("__next"), {
+                return window.__NEXT_P && window.__NEXT_P.map(e => setTimeout(() => s(e), 0)), window.__NEXT_P = [], window.__NEXT_P.push = s, (u = (0, x.default)()).getIsSsr = () => n.isSsr, l = document.getElementById("__next"), {
                     assetPrefix: t
                 }
             }
 
-            function K(e, t) {
+            function J(e, t) {
                 return y.default.createElement(e, t)
             }
 
             function Q(e) {
                 var t;
                 let {
                     children: r
-                } = e;
-                return y.default.createElement($, {
+                } = e, a = y.default.useMemo(() => (0, B.adaptForAppRouterInstance)(n), []);
+                return y.default.createElement(Y, {
                     fn: e => ee({
                         App: f,
                         err: e
                     }).catch(e => console.error("Error rendering page: ", e))
                 }, y.default.createElement(D.AppRouterContext.Provider, {
-                    value: (0, B.adaptForAppRouterInstance)(n)
+                    value: a
                 }, y.default.createElement(H.SearchParamsContext.Provider, {
                     value: (0, B.adaptForSearchParams)(n)
                 }, y.default.createElement(B.PathnameContextProviderAdapter, {
                     router: n,
                     isAutoExport: null != (t = self.__NEXT_DATA__.autoExport) && t
                 }, y.default.createElement(P.RouterContext.Provider, {
                     value: (0, L.makePublicRouterInstance)(n)
                 }, y.default.createElement(b.HeadManagerContext.Provider, {
                     value: u
-                }, y.default.createElement(I.ImageConfigContext.Provider, {
+                }, y.default.createElement(T.ImageConfigContext.Provider, {
                     value: {
                         deviceSizes: [640, 750, 828, 1080, 1200, 1920, 2048, 3840],
                         imageSizes: [16, 32, 48, 64, 96, 128, 256, 384],
                         path: "/_next/image",
                         loader: "default",
                         dangerouslyAllowSVG: !1,
                         unoptimized: !1
@@ -368,15 +368,15 @@
             let Z = e => t => {
                 let r = {
                     ...t,
                     Component: h,
                     err: a.err,
                     router: n
                 };
-                return y.default.createElement(Q, null, K(e, r))
+                return y.default.createElement(Q, null, J(e, r))
             };
 
             function ee(e) {
                 let {
                     App: t,
                     err: l
                 } = e;
@@ -522,15 +522,15 @@
                                 y: r
                             } = e.scroll;
                             (0, w.handleSmoothScroll)(() => {
                                 window.scrollTo(t, r)
                             })
                         }
                     }
-                }), y.default.createElement(Q, null, K(r, f), y.default.createElement(x.Portal, {
+                }), y.default.createElement(Q, null, J(r, f), y.default.createElement(R.Portal, {
                     type: "next-route-announcer"
                 }, y.default.createElement(A.RouteAnnouncer, null))));
                 return ! function(e, t) {
                     E.ST && performance.mark("beforeRender");
                     let r = t(en ? eo : ei);
                     if (er) {
                         let e = y.default.startTransition;
@@ -548,15 +548,15 @@
                 if (e.err) {
                     await ee(e);
                     return
                 }
                 try {
                     await eu(e)
                 } catch (r) {
-                    let t = (0, T.getProperError)(r);
+                    let t = (0, I.getProperError)(r);
                     if (t.cancelled) throw t;
                     await ee({
                         ...e,
                         err: t
                     })
                 }
             }
@@ -591,15 +591,15 @@
                         };
                         c && (d.attribution = c), r.reportWebVitals(d)
                     });
                     let n = await i.routeLoader.whenEntrypoint(a.page);
                     if ("error" in n) throw n.error;
                     h = n.component
                 } catch (e) {
-                    t = (0, T.getProperError)(e)
+                    t = (0, I.getProperError)(e)
                 }
                 window.__NEXT_PRELOADREADY && await window.__NEXT_PRELOADREADY(a.dynamicIds), n = (0, L.createRouter)(a.page, a.query, o, {
                     initialProps: a.props,
                     pageLoader: i,
                     App: f,
                     Component: h,
                     wrapApp: Z,
@@ -610,15 +610,15 @@
                         scroll: r
                     })),
                     locale: a.locale,
                     locales: a.locales,
                     defaultLocale: p,
                     domainLocales: a.domainLocales,
                     isPreview: a.isPreview
-                }), Y = await n._initialMatchesMiddlewarePromise;
+                }), $ = await n._initialMatchesMiddlewarePromise;
                 let r = {
                     App: f,
                     initial: !0,
                     Component: h,
                     props: a.props,
                     err: t
                 };
@@ -2019,14 +2019,29 @@
                 a = r(8106);
 
             function o(e) {
                 let t = (0, a.normalizePathSep)(e);
                 return t.startsWith("/index/") && !(0, n.isDynamicRoute)(t) ? t.slice(6) : "/index" !== t ? t : "/"
             }
         },
+        7302: function(e, t) {
+            "use strict";
+
+            function r(e) {
+                return e.startsWith("/") ? e : "/" + e
+            }
+            Object.defineProperty(t, "__esModule", {
+                value: !0
+            }), Object.defineProperty(t, "ensureLeadingSlash", {
+                enumerable: !0,
+                get: function() {
+                    return r
+                }
+            })
+        },
         8106: function(e, t) {
             "use strict";
 
             function r(e) {
                 return e.replace(/\\/g, "/")
             }
             Object.defineProperty(t, "__esModule", {
@@ -2147,15 +2162,15 @@
                     default: function() {
                         return V
                     },
                     matchesMiddleware: function() {
                         return N
                     },
                     createKey: function() {
-                        return W
+                        return q
                     }
                 });
             let n = r(8754),
                 a = r(1757),
                 o = r(7734),
                 i = r(5564),
                 l = r(5442),
@@ -2176,23 +2191,23 @@
                 v = r(2080),
                 P = r(9577),
                 w = r(4266),
                 S = r(2140),
                 j = r(9423),
                 O = r(6373),
                 E = r(9473),
-                x = r(6385),
-                R = r(3353),
+                R = r(6385),
+                x = r(3353),
                 C = r(293),
                 M = r(5821),
                 A = r(4532),
                 L = r(5036),
-                T = r(3105);
+                I = r(3105);
 
-            function I() {
+            function T() {
                 return Object.assign(Error("Route Cancelled"), {
                     cancelled: !0
                 })
             }
             async function N(e) {
                 let t = await Promise.resolve(e.router.pageLoader.getMiddleware());
                 if (!t) return !1;
@@ -2335,15 +2350,15 @@
                 try {
                     return JSON.parse(e)
                 } catch (e) {
                     return null
                 }
             }
 
-            function q(e) {
+            function W(e) {
                 var t;
                 let {
                     dataHref: r,
                     inflightCache: n,
                     isPrefetch: a,
                     hasMiddleware: o,
                     isServerRender: l,
@@ -2409,15 +2424,15 @@
                     throw f || delete n[d], ("Failed to fetch" === e.message || "NetworkError when attempting to fetch resource." === e.message || "Load failed" === e.message) && (0, i.markAssetError)(e), e
                 });
                 return f && s ? h({}).then(e => (n[d] = Promise.resolve(e), e)) : void 0 !== n[d] ? n[d] : n[d] = h(c ? {
                     method: "HEAD"
                 } : {})
             }
 
-            function W() {
+            function q() {
                 return Math.random().toString(36).slice(2, 10)
             }
 
             function z(e) {
                 let {
                     url: t,
                     router: r
@@ -2491,53 +2506,53 @@
                                     }
                                 }
                             }
                     }
                     return !1
                 }
                 async change(e, t, r, n, a) {
-                    var s, c, f, j, O, E, C, A, T;
+                    var s, c, f, j, O, E, C, A, I;
                     let k, H;
-                    if (!(0, R.isLocalURL)(t)) return z({
+                    if (!(0, x.isLocalURL)(t)) return z({
                         url: t,
                         router: this
                     }), !1;
                     let F = 1 === n._h;
                     F || n.shallow || await this._bfl(r, void 0, n.locale);
-                    let q = F || n._shouldResolveHref || (0, _.parsePath)(t).pathname === (0, _.parsePath)(r).pathname,
-                        W = {
+                    let W = F || n._shouldResolveHref || (0, _.parsePath)(t).pathname === (0, _.parsePath)(r).pathname,
+                        q = {
                             ...this.state
                         },
                         G = !0 !== this.isReady;
                     this.isReady = !0;
                     let X = this.isSsr;
                     if (F || (this.isSsr = !1), F && this.clc) return !1;
-                    let Y = W.locale;
+                    let $ = q.locale;
                     d.ST && performance.mark("routeChange");
                     let {
-                        shallow: $ = !1,
-                        scroll: J = !0
-                    } = n, K = {
-                        shallow: $
+                        shallow: Y = !1,
+                        scroll: K = !0
+                    } = n, J = {
+                        shallow: Y
                     };
-                    this._inFlightRoute && this.clc && (X || V.events.emit("routeChangeError", I(), this._inFlightRoute, K), this.clc(), this.clc = null), r = (0, w.addBasePath)((0, b.addLocale)((0, S.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, n.locale, this.defaultLocale));
-                    let Q = (0, v.removeLocale)((0, S.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, W.locale);
+                    this._inFlightRoute && this.clc && (X || V.events.emit("routeChangeError", T(), this._inFlightRoute, J), this.clc(), this.clc = null), r = (0, w.addBasePath)((0, b.addLocale)((0, S.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, n.locale, this.defaultLocale));
+                    let Q = (0, v.removeLocale)((0, S.hasBasePath)(r) ? (0, P.removeBasePath)(r) : r, q.locale);
                     this._inFlightRoute = r;
-                    let Z = Y !== W.locale;
+                    let Z = $ !== q.locale;
                     if (!F && this.onlyAHashChange(Q) && !Z) {
-                        W.asPath = Q, V.events.emit("hashChangeStart", r, K), this.changeState(e, t, r, {
+                        q.asPath = Q, V.events.emit("hashChangeStart", r, J), this.changeState(e, t, r, {
                             ...n,
                             scroll: !1
-                        }), J && this.scrollToHash(Q);
+                        }), K && this.scrollToHash(Q);
                         try {
-                            await this.set(W, this.components[W.route], null)
+                            await this.set(q, this.components[q.route], null)
                         } catch (e) {
-                            throw (0, u.default)(e) && e.cancelled && V.events.emit("routeChangeError", e, Q, K), e
+                            throw (0, u.default)(e) && e.cancelled && V.events.emit("routeChangeError", e, Q, J), e
                         }
-                        return V.events.emit("hashChangeComplete", r, K), !0
+                        return V.events.emit("hashChangeComplete", r, J), !0
                     }
                     let ee = (0, p.parseRelativeUrl)(t),
                         {
                             pathname: et,
                             query: er
                         } = ee;
                     if (null == (s = this.components[et]) ? void 0 : s.__appRouter) return z({
@@ -2558,22 +2573,22 @@
                     let en = r;
                     et = et ? (0, o.removeTrailingSlash)((0, P.removeBasePath)(et)) : et;
                     let ea = (0, o.removeTrailingSlash)(et),
                         eo = r.startsWith("/") && (0, p.parseRelativeUrl)(r).pathname,
                         ei = !!(eo && ea !== eo && (!(0, h.isDynamicRoute)(ea) || !(0, m.getRouteMatcher)((0, g.getRouteRegex)(ea))(eo))),
                         el = !n.shallow && await N({
                             asPath: r,
-                            locale: W.locale,
+                            locale: q.locale,
                             router: this
                         });
-                    if (F && el && (q = !1), q && "/_error" !== et && (n._shouldResolveHref = !0, ee.pathname = B(et, k), ee.pathname === et || (et = ee.pathname, ee.pathname = (0, w.addBasePath)(et), el || (t = (0, y.formatWithValidation)(ee)))), !(0, R.isLocalURL)(r)) return z({
+                    if (F && el && (W = !1), W && "/_error" !== et && (n._shouldResolveHref = !0, ee.pathname = B(et, k), ee.pathname === et || (et = ee.pathname, ee.pathname = (0, w.addBasePath)(et), el || (t = (0, y.formatWithValidation)(ee)))), !(0, x.isLocalURL)(r)) return z({
                         url: r,
                         router: this
                     }), !1;
-                    en = (0, v.removeLocale)((0, P.removeBasePath)(en), W.locale), ea = (0, o.removeTrailingSlash)(et);
+                    en = (0, v.removeLocale)((0, P.removeBasePath)(en), q.locale), ea = (0, o.removeTrailingSlash)(et);
                     let eu = !1;
                     if ((0, h.isDynamicRoute)(ea)) {
                         let e = (0, p.parseRelativeUrl)(en),
                             n = e.pathname,
                             a = (0, g.getRouteRegex)(ea);
                         eu = (0, m.getRouteMatcher)(a)(n);
                         let o = ea === n,
@@ -2583,38 +2598,38 @@
                             query: (0, M.omit)(er, i.params)
                         })) : Object.assign(er, eu);
                         else {
                             let e = Object.keys(a.groups).filter(e => !er[e] && !a.groups[e].optional);
                             if (e.length > 0 && !el) throw Error((o ? "The provided `href` (" + t + ") value is missing query values (" + e.join(", ") + ") to be interpolated properly. " : "The provided `as` value (" + n + ") is incompatible with the `href` value (" + ea + "). ") + "Read more: https://nextjs.org/docs/messages/" + (o ? "href-interpolation-failed" : "incompatible-href-as"))
                         }
                     }
-                    F || V.events.emit("routeChangeStart", r, K);
+                    F || V.events.emit("routeChangeStart", r, J);
                     let es = "/404" === this.pathname || "/_error" === this.pathname;
                     try {
                         let o = await this.getRouteInfo({
                             route: ea,
                             pathname: et,
                             query: er,
                             as: r,
                             resolvedAs: en,
-                            routeProps: K,
-                            locale: W.locale,
-                            isPreview: W.isPreview,
+                            routeProps: J,
+                            locale: q.locale,
+                            isPreview: q.isPreview,
                             hasMiddleware: el,
                             unstable_skipClientCache: n.unstable_skipClientCache,
                             isQueryUpdating: F && !this.isFallback,
                             isMiddlewareRewrite: ei
                         });
-                        if (F || n.shallow || await this._bfl(r, "resolvedAs" in o ? o.resolvedAs : void 0, W.locale), "route" in o && el) {
-                            ea = et = o.route || ea, K.shallow || (er = Object.assign({}, o.query || {}, er));
+                        if (F || n.shallow || await this._bfl(r, "resolvedAs" in o ? o.resolvedAs : void 0, q.locale), "route" in o && el) {
+                            ea = et = o.route || ea, J.shallow || (er = Object.assign({}, o.query || {}, er));
                             let e = (0, S.hasBasePath)(ee.pathname) ? (0, P.removeBasePath)(ee.pathname) : ee.pathname;
                             if (eu && et !== e && Object.keys(eu).forEach(e => {
                                     eu && er[e] === eu[e] && delete er[e]
                                 }), (0, h.isDynamicRoute)(et)) {
-                                let e = !K.shallow && o.resolvedAs ? o.resolvedAs : (0, w.addBasePath)((0, b.addLocale)(new URL(r, location.href).pathname, W.locale), !0),
+                                let e = !J.shallow && o.resolvedAs ? o.resolvedAs : (0, w.addBasePath)((0, b.addLocale)(new URL(r, location.href).pathname, q.locale), !0),
                                     t = e;
                                 (0, S.hasBasePath)(t) && (t = (0, P.removeBasePath)(t));
                                 let n = (0, g.getRouteRegex)(et),
                                     a = (0, m.getRouteMatcher)(n)(new URL(t, location.href).pathname);
                                 a && Object.assign(er, a)
                             }
                         }
@@ -2646,15 +2661,15 @@
                                     return this.change(e, a, o, n)
                                 }
                                 return z({
                                     url: t,
                                     router: this
                                 }), new Promise(() => {})
                             }
-                            if (W.isPreview = !!o.props.__N_PREVIEW, o.props.notFound === U) {
+                            if (q.isPreview = !!o.props.__N_PREVIEW, o.props.notFound === U) {
                                 let e;
                                 try {
                                     await this.fetchComponent("/404"), e = "/404"
                                 } catch (t) {
                                     e = "/_error"
                                 }
                                 if (o = await this.getRouteInfo({
@@ -2662,29 +2677,29 @@
                                         pathname: e,
                                         query: er,
                                         as: r,
                                         resolvedAs: en,
                                         routeProps: {
                                             shallow: !1
                                         },
-                                        locale: W.locale,
-                                        isPreview: W.isPreview,
+                                        locale: q.locale,
+                                        isPreview: q.isPreview,
                                         isNotFound: !0
                                     }), "type" in o) throw Error("Unexpected middleware effect on /404")
                             }
                         }
                         F && "/_error" === this.pathname && (null == (c = self.__NEXT_DATA__.props) ? void 0 : null == (f = c.pageProps) ? void 0 : f.statusCode) === 500 && (null == (j = o.props) ? void 0 : j.pageProps) && (o.props.pageProps.statusCode = 500);
-                        let s = n.shallow && W.route === (null != (O = o.route) ? O : ea),
+                        let s = n.shallow && q.route === (null != (O = o.route) ? O : ea),
                             d = null != (E = n.scroll) ? E : !F && !s,
                             y = null != a ? a : d ? {
                                 x: 0,
                                 y: 0
                             } : null,
                             _ = {
-                                ...W,
+                                ...q,
                                 route: ea,
                                 pathname: et,
                                 query: er,
                                 asPath: Q,
                                 isFallback: !1
                             };
                         if (F && es) {
@@ -2693,59 +2708,59 @@
                                     pathname: this.pathname,
                                     query: er,
                                     as: r,
                                     resolvedAs: en,
                                     routeProps: {
                                         shallow: !1
                                     },
-                                    locale: W.locale,
-                                    isPreview: W.isPreview,
+                                    locale: q.locale,
+                                    isPreview: q.isPreview,
                                     isQueryUpdating: F && !this.isFallback
                                 }), "type" in o) throw Error("Unexpected middleware effect on " + this.pathname);
-                            "/_error" === this.pathname && (null == (C = self.__NEXT_DATA__.props) ? void 0 : null == (A = C.pageProps) ? void 0 : A.statusCode) === 500 && (null == (T = o.props) ? void 0 : T.pageProps) && (o.props.pageProps.statusCode = 500);
+                            "/_error" === this.pathname && (null == (C = self.__NEXT_DATA__.props) ? void 0 : null == (A = C.pageProps) ? void 0 : A.statusCode) === 500 && (null == (I = o.props) ? void 0 : I.pageProps) && (o.props.pageProps.statusCode = 500);
                             try {
                                 await this.set(_, o, y)
                             } catch (e) {
-                                throw (0, u.default)(e) && e.cancelled && V.events.emit("routeChangeError", e, Q, K), e
+                                throw (0, u.default)(e) && e.cancelled && V.events.emit("routeChangeError", e, Q, J), e
                             }
                             return !0
                         }
-                        V.events.emit("beforeHistoryChange", r, K), this.changeState(e, t, r, n);
-                        let v = F && !y && !G && !Z && (0, x.compareRouterStates)(_, this.state);
+                        V.events.emit("beforeHistoryChange", r, J), this.changeState(e, t, r, n);
+                        let v = F && !y && !G && !Z && (0, R.compareRouterStates)(_, this.state);
                         if (!v) {
                             try {
                                 await this.set(_, o, y)
                             } catch (e) {
                                 if (e.cancelled) o.error = o.error || e;
                                 else throw e
                             }
-                            if (o.error) throw F || V.events.emit("routeChangeError", o.error, Q, K), o.error;
-                            F || V.events.emit("routeChangeComplete", r, K), d && /#.+$/.test(r) && this.scrollToHash(r)
+                            if (o.error) throw F || V.events.emit("routeChangeError", o.error, Q, J), o.error;
+                            F || V.events.emit("routeChangeComplete", r, J), d && /#.+$/.test(r) && this.scrollToHash(r)
                         }
                         return !0
                     } catch (e) {
                         if ((0, u.default)(e) && e.cancelled) return !1;
                         throw e
                     }
                 }
                 changeState(e, t, r, n) {
                     void 0 === n && (n = {}), ("pushState" !== e || (0, d.getURL)() !== r) && (this._shallow = n.shallow, window.history[e]({
                         url: t,
                         as: r,
                         options: n,
                         __N: !0,
-                        key: this._key = "pushState" !== e ? this._key : W()
+                        key: this._key = "pushState" !== e ? this._key : q()
                     }, "", r))
                 }
                 async handleRouteInfoError(e, t, r, n, a, o) {
                     if (console.error(e), e.cancelled) throw e;
                     if ((0, i.isAssetError)(e) || o) throw V.events.emit("routeChangeError", e, n, a), z({
                         url: n,
                         router: this
-                    }), I();
+                    }), T();
                     try {
                         let n;
                         let {
                             page: a,
                             styleSheets: o
                         } = await this.fetchComponent("/_error"), i = {
                             props: n,
@@ -2810,15 +2825,15 @@
                                 inflightCache: p ? this.sbc : this.sdc,
                                 persistCache: !d,
                                 isPrefetch: !1,
                                 unstable_skipClientCache: h,
                                 isBackground: p
                             },
                             E = p && !m ? null : await H({
-                                fetchData: () => q(O),
+                                fetchData: () => W(O),
                                 asPath: g ? "/404" : i,
                                 locale: s,
                                 router: this
                             }).catch(e => {
                                 if (p) return null;
                                 throw e
                             });
@@ -2836,71 +2851,71 @@
                                 route: _
                             }
                         }
                         if ((0, j.isAPIRoute)(_)) return z({
                             url: a,
                             router: this
                         }), new Promise(() => {});
-                        let x = u || await this.fetchComponent(_).then(e => ({
+                        let R = u || await this.fetchComponent(_).then(e => ({
                                 Component: e.page,
                                 styleSheets: e.styleSheets,
                                 __N_SSG: e.mod.__N_SSG,
                                 __N_SSP: e.mod.__N_SSP
                             })),
-                            R = null == E ? void 0 : null == (S = E.response) ? void 0 : S.headers.get("x-middleware-skip"),
-                            C = x.__N_SSG || x.__N_SSP;
-                        R && (null == E ? void 0 : E.dataHref) && delete this.sdc[E.dataHref];
+                            x = null == E ? void 0 : null == (S = E.response) ? void 0 : S.headers.get("x-middleware-skip"),
+                            C = R.__N_SSG || R.__N_SSP;
+                        x && (null == E ? void 0 : E.dataHref) && delete this.sdc[E.dataHref];
                         let {
                             props: M,
                             cacheKey: A
                         } = await this._getData(async () => {
                             if (C) {
-                                if ((null == E ? void 0 : E.json) && !R) return {
+                                if ((null == E ? void 0 : E.json) && !x) return {
                                     cacheKey: E.cacheKey,
                                     props: E.json
                                 };
                                 let e = (null == E ? void 0 : E.dataHref) ? E.dataHref : this.pageLoader.getDataHref({
                                         href: (0, y.formatWithValidation)({
                                             pathname: r,
                                             query: n
                                         }),
                                         asPath: i,
                                         locale: s
                                     }),
-                                    t = await q({
+                                    t = await W({
                                         dataHref: e,
                                         isServerRender: this.isSsr,
                                         parseJSON: !0,
-                                        inflightCache: R ? {} : this.sdc,
+                                        inflightCache: x ? {} : this.sdc,
                                         persistCache: !d,
                                         isPrefetch: !1,
                                         unstable_skipClientCache: h
                                     });
                                 return {
                                     cacheKey: t.cacheKey,
                                     props: t.json || {}
                                 }
                             }
                             return {
                                 headers: {},
-                                props: await this.getInitialProps(x.Component, {
+                                props: await this.getInitialProps(R.Component, {
                                     pathname: r,
                                     query: n,
                                     asPath: a,
                                     locale: s,
                                     locales: this.locales,
                                     defaultLocale: this.defaultLocale
                                 })
                             }
                         });
-                        return x.__N_SSP && O.dataHref && A && delete this.sdc[A], this.isPreview || !x.__N_SSG || p || q(Object.assign({}, O, {
+                        return R.__N_SSP && O.dataHref && A && delete this.sdc[A], this.isPreview || !R.__N_SSG || p || W(Object.assign({}, O, {
                             isBackground: !0,
                             persistCache: !1,
                             inflightCache: this.sbc
-                        })).catch(() => {}), M.pageProps = Object.assign({}, M.pageProps), x.props = M, x.route = _, x.query = n, x.resolvedAs = i, this.components[_] = x, x
+                        })).catch(() => {}), M.pageProps = Object.assign({}, M.pageProps), R.props = M, R.route = _, R.query = n, R.resolvedAs = i, this.components[_] = R, R
                     } catch (e) {
                         return this.handleRouteInfoError((0, u.getProperError)(e), r, n, a, l)
                     }
                 }
                 set(e, t, r) {
                     return this.state = e, this.sub(t, this.components["/_app"].Component, r)
                 }
@@ -2911,25 +2926,25 @@
                     if (!this.asPath) return !1;
                     let [t, r] = this.asPath.split("#"), [n, a] = e.split("#");
                     return !!a && t === n && r === a || t === n && r !== a
                 }
                 scrollToHash(e) {
                     let [, t = ""] = e.split("#");
                     if ("" === t || "top" === t) {
-                        (0, T.handleSmoothScroll)(() => window.scrollTo(0, 0));
+                        (0, I.handleSmoothScroll)(() => window.scrollTo(0, 0));
                         return
                     }
                     let r = decodeURIComponent(t),
                         n = document.getElementById(r);
                     if (n) {
-                        (0, T.handleSmoothScroll)(() => n.scrollIntoView());
+                        (0, I.handleSmoothScroll)(() => n.scrollIntoView());
                         return
                     }
                     let a = document.getElementsByName(r)[0];
-                    a && (0, T.handleSmoothScroll)(() => a.scrollIntoView())
+                    a && (0, I.handleSmoothScroll)(() => a.scrollIntoView())
                 }
                 urlIsNew(e) {
                     return this.asPath !== e
                 }
                 async prefetch(e, t, r) {
                     if (void 0 === t && (t = e), void 0 === r && (r = {}), (0, C.isBot)(window.navigator.userAgent)) return;
                     let n = (0, p.parseRelativeUrl)(e),
@@ -2945,15 +2960,15 @@
                         d = await N({
                             asPath: t,
                             locale: f,
                             router: this
                         });
                     n.pathname = B(n.pathname, s), (0, h.isDynamicRoute)(n.pathname) && (i = n.pathname, n.pathname = i, Object.assign(l, (0, m.getRouteMatcher)((0, g.getRouteRegex)(n.pathname))((0, _.parsePath)(t).pathname) || {}), d || (e = (0, y.formatWithValidation)(n)));
                     let b = await H({
-                        fetchData: () => q({
+                        fetchData: () => W({
                             dataHref: this.pageLoader.getDataHref({
                                 href: (0, y.formatWithValidation)({
                                     pathname: u,
                                     query: l
                                 }),
                                 skipInterpolation: !0,
                                 asPath: c,
@@ -2973,15 +2988,15 @@
                     if ((null == b ? void 0 : b.effect.type) === "rewrite" && (n.pathname = b.effect.resolvedHref, i = b.effect.resolvedHref, l = {
                             ...l,
                             ...b.effect.parsedAs.query
                         }, c = b.effect.parsedAs.pathname, e = (0, y.formatWithValidation)(n)), (null == b ? void 0 : b.effect.type) === "redirect-external") return;
                     let v = (0, o.removeTrailingSlash)(i);
                     await this._bfl(t, c, r.locale, !0) && (this.components[a] = {
                         __appRouter: !0
-                    }), await Promise.all([this.pageLoader._isSsg(v).then(t => !!t && q({
+                    }), await Promise.all([this.pageLoader._isSsg(v).then(t => !!t && W({
                         dataHref: (null == b ? void 0 : b.json) ? null == b ? void 0 : b.dataHref : this.pageLoader.getDataHref({
                             href: e,
                             asPath: c,
                             locale: f
                         }),
                         isServerRender: !1,
                         parseJSON: !0,
@@ -3013,15 +3028,15 @@
                             let e = Error("Loading initial props cancelled");
                             throw e.cancelled = !0, e
                         }
                         return e
                     })
                 }
                 _getFlightData(e) {
-                    return q({
+                    return W({
                         dataHref: e,
                         isServerRender: !0,
                         parseJSON: !1,
                         inflightCache: this.sdc,
                         persistCache: !1,
                         isPrefetch: !1
                     }).then(e => {
@@ -3076,15 +3091,15 @@
                     isFallback: m,
                     locale: g,
                     locales: _,
                     defaultLocale: b,
                     domainLocales: v,
                     isPreview: P
                 }) {
-                    this.sdc = {}, this.sbc = {}, this.isFirstPopStateEvent = !0, this._key = W(), this.onPopState = e => {
+                    this.sdc = {}, this.sbc = {}, this.isFirstPopStateEvent = !0, this._key = q(), this.onPopState = e => {
                         let t;
                         let {
                             isFirstPopStateEvent: r
                         } = this;
                         this.isFirstPopStateEvent = !1;
                         let n = e.state;
                         if (!n) {
@@ -3236,14 +3251,42 @@
                     pathname: r,
                     query: a,
                     hash: o
                 } = (0, n.parsePath)(e);
                 return "" + r + t + a + o
             }
         },
+        6097: function(e, t, r) {
+            "use strict";
+            Object.defineProperty(t, "__esModule", {
+                    value: !0
+                }),
+                function(e, t) {
+                    for (var r in t) Object.defineProperty(e, r, {
+                        enumerable: !0,
+                        get: t[r]
+                    })
+                }(t, {
+                    normalizeAppPath: function() {
+                        return a
+                    },
+                    normalizeRscPath: function() {
+                        return o
+                    }
+                });
+            let n = r(7302);
+
+            function a(e) {
+                return (0, n.ensureLeadingSlash)(e.split("/").reduce((e, t, r, n) => !t || "(" === t[0] && t.endsWith(")") || "@" === t[0] || ("page" === t || "route" === t) && r === n.length - 1 ? e : e + "/" + t, ""))
+            }
+
+            function o(e, t) {
+                return t ? e.replace(/\.rsc($|\?)/, "$1") : e
+            }
+        },
         6385: function(e, t) {
             "use strict";
 
             function r(e, t) {
                 let r = Object.keys(e);
                 if (r.length !== Object.keys(t).length) return !1;
                 for (let n = r.length; n--;) {
@@ -3710,17 +3753,16 @@
                 s = r(3162),
                 c = r(5036);
 
             function f(e, t, r) {
                 let f;
                 let d = "string" == typeof t ? t : (0, a.formatWithValidation)(t),
                     h = d.match(/^[a-zA-Z]{1,}:\/\//),
-                    p = h ? d.slice(h[0].length) : d,
-                    m = p.split("?");
-                if ((m[0] || "").match(/(\/\/|\\)/)) {
+                    p = h ? d.slice(h[0].length) : d;
+                if ((p.split("?")[0] || "").match(/(\/\/|\\)/)) {
                     console.error("Invalid href '" + d + "' passed to next/router in page: '" + e.pathname + "'. Repeated forward-slashes (//) or backslashes \\ are not valid in the href.");
                     let t = (0, i.normalizeRepeatedSlashes)(p);
                     d = (h ? h[0] : "") + t
                 }
                 if (!(0, u.isLocalURL)(d)) return r ? [d] : d;
                 try {
                     f = new URL(d.startsWith("#") ? e.asPath : e.pathname, "http://n")
@@ -3797,52 +3839,66 @@
                         get: t[r]
                     })
                 }(t, {
                     getRouteRegex: function() {
                         return u
                     },
                     getNamedRouteRegex: function() {
-                        return c
+                        return f
                     },
                     getNamedMiddlewareRegex: function() {
-                        return f
+                        return d
                     }
                 });
-            let n = r(5987),
-                a = r(7734),
-                o = "nxtP";
+            let n = r(2407),
+                a = r(5987),
+                o = r(7734);
 
             function i(e) {
                 let t = e.startsWith("[") && e.endsWith("]");
                 t && (e = e.slice(1, -1));
                 let r = e.startsWith("...");
                 return r && (e = e.slice(3)), {
                     key: e,
                     repeat: r,
                     optional: t
                 }
             }
 
             function l(e) {
-                let t = (0, a.removeTrailingSlash)(e).slice(1).split("/"),
+                let t = (0, o.removeTrailingSlash)(e).slice(1).split("/"),
                     r = {},
-                    o = 1;
+                    l = 1;
                 return {
                     parameterizedRoute: t.map(e => {
-                        if (!(e.startsWith("[") && e.endsWith("]"))) return "/" + (0, n.escapeStringRegexp)(e); {
+                        let t = n.INTERCEPTION_ROUTE_MARKERS.find(t => e.startsWith(t)),
+                            o = e.match(/\[((?:\[.*\])|.+)\]/);
+                        if (t && o) {
                             let {
-                                key: t,
+                                key: e,
                                 optional: n,
-                                repeat: a
-                            } = i(e.slice(1, -1));
-                            return r[t] = {
-                                pos: o++,
-                                repeat: a,
+                                repeat: u
+                            } = i(o[1]);
+                            return r[e] = {
+                                pos: l++,
+                                repeat: u,
+                                optional: n
+                            }, "/" + (0, a.escapeStringRegexp)(t) + "([^/]+?)"
+                        }
+                        if (!o) return "/" + (0, a.escapeStringRegexp)(e); {
+                            let {
+                                key: e,
+                                repeat: t,
+                                optional: n
+                            } = i(o[1]);
+                            return r[e] = {
+                                pos: l++,
+                                repeat: t,
                                 optional: n
-                            }, a ? n ? "(?:/(.+?))?" : "/(.+?)" : "/([^/]+?)"
+                            }, t ? n ? "(?:/(.+?))?" : "/(.+?)" : "/([^/]+?)"
                         }
                     }).join(""),
                     groups: r
                 }
             }
 
             function u(e) {
@@ -3852,61 +3908,78 @@
                 } = l(e);
                 return {
                     re: RegExp("^" + t + "(?:/)?$"),
                     groups: r
                 }
             }
 
-            function s(e, t) {
-                let r, l;
-                let u = (0, a.removeTrailingSlash)(e).slice(1).split("/"),
-                    s = (r = 97, l = 1, () => {
+            function s(e) {
+                let t, r, {
+                        segment: n,
+                        routeKeys: a,
+                        keyPrefix: o
+                    } = e,
+                    l = (t = 97, r = 1, () => {
                         let e = "";
-                        for (let t = 0; t < l; t++) e += String.fromCharCode(r), ++r > 122 && (l++, r = 97);
+                        for (let n = 0; n < r; n++) e += String.fromCharCode(t), ++t > 122 && (r++, t = 97);
                         return e
                     }),
-                    c = {};
+                    {
+                        key: u,
+                        optional: s,
+                        repeat: c
+                    } = i(n),
+                    f = u.replace(/\W/g, "");
+                o && (f = "" + o + f);
+                let d = !1;
+                return (0 === f.length || f.length > 30) && (d = !0), isNaN(parseInt(f.slice(0, 1))) || (d = !0), d && (f = l()), o ? a[f] = "" + o + u : a[f] = "" + u, c ? s ? "(?:/(?<" + f + ">.+?))?" : "/(?<" + f + ">.+?)" : "/(?<" + f + ">[^/]+?)"
+            }
+
+            function c(e, t) {
+                let r = (0, o.removeTrailingSlash)(e).slice(1).split("/"),
+                    i = {};
                 return {
-                    namedParameterizedRoute: u.map(e => {
-                        if (!(e.startsWith("[") && e.endsWith("]"))) return "/" + (0, n.escapeStringRegexp)(e); {
-                            let {
-                                key: r,
-                                optional: n,
-                                repeat: a
-                            } = i(e.slice(1, -1)), l = r.replace(/\W/g, "");
-                            t && (l = "" + o + l);
-                            let u = !1;
-                            return (0 === l.length || l.length > 30) && (u = !0), isNaN(parseInt(l.slice(0, 1))) || (u = !0), u && (l = s()), t ? c[l] = "" + o + r : c[l] = "" + r, a ? n ? "(?:/(?<" + l + ">.+?))?" : "/(?<" + l + ">.+?)" : "/(?<" + l + ">[^/]+?)"
-                        }
+                    namedParameterizedRoute: r.map(e => {
+                        let r = n.INTERCEPTION_ROUTE_MARKERS.some(t => e.startsWith(t)),
+                            o = e.match(/\[((?:\[.*\])|.+)\]/);
+                        return r && o ? s({
+                            segment: o[1],
+                            routeKeys: i,
+                            keyPrefix: t ? "nxtI" : void 0
+                        }) : o ? s({
+                            segment: o[1],
+                            routeKeys: i,
+                            keyPrefix: t ? "nxtP" : void 0
+                        }) : "/" + (0, a.escapeStringRegexp)(e)
                     }).join(""),
-                    routeKeys: c
+                    routeKeys: i
                 }
             }
 
-            function c(e, t) {
-                let r = s(e, t);
+            function f(e, t) {
+                let r = c(e, t);
                 return {
                     ...u(e),
                     namedRegex: "^" + r.namedParameterizedRoute + "(?:/)?$",
                     routeKeys: r.routeKeys
                 }
             }
 
-            function f(e, t) {
+            function d(e, t) {
                 let {
                     parameterizedRoute: r
                 } = l(e), {
                     catchAll: n = !0
                 } = t;
                 if ("/" === r) return {
                     namedRegex: "^/" + (n ? ".*" : "") + "$"
                 };
                 let {
                     namedParameterizedRoute: a
-                } = s(e, !1);
+                } = c(e, !1);
                 return {
                     namedRegex: "^" + a + (n ? "(?:(/.*)?)" : "") + "$"
                 }
             }
         },
         9163: function(e, t) {
             "use strict";
@@ -4103,14 +4176,17 @@
                         return g
                     },
                     MissingStaticPage: function() {
                         return y
                     },
                     MiddlewareNotFoundError: function() {
                         return _
+                    },
+                    stringifyError: function() {
+                        return b
                     }
                 });
             let r = ["CLS", "FCP", "FID", "INP", "LCP", "TTFB"];
 
             function n(e) {
                 let t, r = !1;
                 return function() {
@@ -4178,29 +4254,36 @@
                 }
             }
             class _ extends Error {
                 constructor() {
                     super(), this.code = "ENOENT", this.message = "Cannot find the middleware module"
                 }
             }
+
+            function b(e) {
+                return JSON.stringify({
+                    message: e.message,
+                    stack: e.stack
+                })
+            }
         },
         4210: function(e, t) {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), Object.defineProperty(t, "warnOnce", {
                 enumerable: !0,
                 get: function() {
                     return r
                 }
             });
             let r = e => {}
         },
         8018: function(e) {
-            var t, r, n, a, o, i, l, u, s, c, f, d, h, p, m, g, y, _, b, v, P, w, S, j, O, E, x, R, C, M, A, L, T, I, N, k, D, B, H, U, F, q, W, z, G, V;
+            var t, r, n, a, o, i, l, u, s, c, f, d, h, p, m, g, y, _, b, v, P, w, S, j, O, E, R, x, C, M, A, L, I, T, N, k, D, B, H, U, F, W, q, z, G, V;
             (t = {}).d = function(e, r) {
                 for (var n in r) t.o(r, n) && !t.o(e, n) && Object.defineProperty(e, n, {
                     enumerable: !0,
                     get: r[n]
                 })
             }, t.o = function(e, t) {
                 return Object.prototype.hasOwnProperty.call(e, t)
@@ -4217,15 +4300,15 @@
                 getFCP: function() {
                     return v
                 },
                 getFID: function() {
                     return M
                 },
                 getINP: function() {
-                    return q
+                    return W
                 },
                 getLCP: function() {
                     return z
                 },
                 getTTFB: function() {
                     return V
                 },
@@ -4235,15 +4318,15 @@
                 onFCP: function() {
                     return v
                 },
                 onFID: function() {
                     return M
                 },
                 onINP: function() {
-                    return q
+                    return W
                 },
                 onLCP: function() {
                     return z
                 },
                 onTTFB: function() {
                     return V
                 }
@@ -4353,43 +4436,43 @@
                 }), s(function() {
                     i = 0, w = -1, n = m(a, o = d("CLS", 0), r, t.reportAllChanges)
                 }))
             }, j = {
                 passive: !0,
                 capture: !0
             }, O = new Date, E = function(e, t) {
-                n || (n = t, a = e, o = new Date, C(removeEventListener), x())
-            }, x = function() {
+                n || (n = t, a = e, o = new Date, C(removeEventListener), R())
+            }, R = function() {
                 if (a >= 0 && a < o - O) {
                     var e = {
                         entryType: "first-input",
                         name: n.type,
                         target: n.target,
                         cancelable: n.cancelable,
                         startTime: n.timeStamp,
                         processingStart: n.timeStamp + a
                     };
                     i.forEach(function(t) {
                         t(e)
                     }), i = []
                 }
-            }, R = function(e) {
+            }, x = function(e) {
                 if (e.cancelable) {
                     var t, r, n, a = (e.timeStamp > 1e12 ? new Date : performance.now()) - e.timeStamp;
                     "pointerdown" == e.type ? (t = function() {
                         E(a, e), n()
                     }, r = function() {
                         n()
                     }, n = function() {
                         removeEventListener("pointerup", t, j), removeEventListener("pointercancel", r, j)
                     }, addEventListener("pointerup", t, j), addEventListener("pointercancel", r, j)) : E(a, e)
                 }
             }, C = function(e) {
                 ["mousedown", "keydown", "touchstart", "pointerdown"].forEach(function(t) {
-                    return e(t, R, j)
+                    return e(t, x, j)
                 })
             }, M = function(e, t) {
                 t = t || {};
                 var r, o = [100, 300],
                     l = b(),
                     u = d("FID"),
                     c = function(e) {
@@ -4398,24 +4481,24 @@
                     f = function(e) {
                         e.forEach(c)
                     },
                     g = h("first-input", f);
                 r = m(e, u, o, t.reportAllChanges), g && p(function() {
                     f(g.takeRecords()), g.disconnect()
                 }, !0), g && s(function() {
-                    r = m(e, u = d("FID"), o, t.reportAllChanges), i = [], a = -1, n = null, C(addEventListener), i.push(c), x()
+                    r = m(e, u = d("FID"), o, t.reportAllChanges), i = [], a = -1, n = null, C(addEventListener), i.push(c), R()
                 })
-            }, A = 0, L = 1 / 0, T = 0, I = function(e) {
+            }, A = 0, L = 1 / 0, I = 0, T = function(e) {
                 e.forEach(function(e) {
-                    e.interactionId && (L = Math.min(L, e.interactionId), A = (T = Math.max(T, e.interactionId)) ? (T - L) / 7 + 1 : 0)
+                    e.interactionId && (L = Math.min(L, e.interactionId), A = (I = Math.max(I, e.interactionId)) ? (I - L) / 7 + 1 : 0)
                 })
             }, N = function() {
                 return l ? A : performance.interactionCount || 0
             }, k = function() {
-                "interactionCount" in performance || l || (l = h("event", I, {
+                "interactionCount" in performance || l || (l = h("event", T, {
                     type: "event",
                     buffered: !0,
                     durationThreshold: 0
                 }))
             }, D = 0, B = function() {
                 return N() - D
             }, H = [], U = {}, F = function(e) {
@@ -4433,15 +4516,15 @@
                     }
                     H.sort(function(e, t) {
                         return t.latency - e.latency
                     }), H.splice(10).forEach(function(e) {
                         delete U[e.id]
                     })
                 }
-            }, q = function(e, t) {
+            }, W = function(e, t) {
                 t = t || {};
                 var r = [200, 500];
                 k();
                 var n, a = d("INP"),
                     o = function(e) {
                         e.forEach(function(e) {
                             e.interactionId && F(e), "first-input" !== e.entryType || H.some(function(t) {
@@ -4460,15 +4543,15 @@
                     type: "first-input",
                     buffered: !0
                 }), p(function() {
                     o(i.takeRecords()), a.value < 0 && B() > 0 && (a.value = 0, a.entries = []), n(!0)
                 }), s(function() {
                     H = [], D = N(), n = m(e, a = d("INP"), r, t.reportAllChanges)
                 }))
-            }, W = {}, z = function(e, t) {
+            }, q = {}, z = function(e, t) {
                 t = t || {};
                 var r, n = [2500, 4e3],
                     a = b(),
                     o = d("LCP"),
                     i = function(e) {
                         var t = e[e.length - 1];
                         if (t) {
@@ -4476,25 +4559,25 @@
                             n < a.firstHiddenTime && (o.value = n, o.entries = [t], r())
                         }
                     },
                     l = h("largest-contentful-paint", i);
                 if (l) {
                     r = m(e, o, n, t.reportAllChanges);
                     var u = function() {
-                        W[o.id] || (i(l.takeRecords()), l.disconnect(), W[o.id] = !0, r(!0))
+                        q[o.id] || (i(l.takeRecords()), l.disconnect(), q[o.id] = !0, r(!0))
                     };
                     ["keydown", "click"].forEach(function(e) {
                         addEventListener(e, u, {
                             once: !0,
                             capture: !0
                         })
                     }), p(u, !0), s(function(a) {
                         r = m(e, o = d("LCP"), n, t.reportAllChanges), requestAnimationFrame(function() {
                             requestAnimationFrame(function() {
-                                o.value = performance.now() - a.timeStamp, W[o.id] = !0, r(!0)
+                                o.value = performance.now() - a.timeStamp, q[o.id] = !0, r(!0)
                             })
                         })
                     })
                 }
             }, G = function e(t) {
                 document.prerendering ? addEventListener("prerenderingchange", function() {
                     return e(t)
@@ -4556,14 +4639,74 @@
                 return "object" == typeof e && null !== e && "name" in e && "message" in e
             }
 
             function o(e) {
                 return a(e) ? e : Error((0, n.isPlainObject)(e) ? JSON.stringify(e) : e + "")
             }
         },
+        2407: function(e, t, r) {
+            "use strict";
+            Object.defineProperty(t, "__esModule", {
+                    value: !0
+                }),
+                function(e, t) {
+                    for (var r in t) Object.defineProperty(e, r, {
+                        enumerable: !0,
+                        get: t[r]
+                    })
+                }(t, {
+                    INTERCEPTION_ROUTE_MARKERS: function() {
+                        return a
+                    },
+                    isInterceptionRouteAppPath: function() {
+                        return o
+                    },
+                    extractInterceptionRouteInformation: function() {
+                        return i
+                    }
+                });
+            let n = r(6097),
+                a = ["(..)(..)", "(.)", "(..)", "(...)"];
+
+            function o(e) {
+                return void 0 !== e.split("/").find(e => a.find(t => e.startsWith(t)))
+            }
+
+            function i(e) {
+                let t, r, o;
+                for (let n of e.split("/"))
+                    if (r = a.find(e => n.startsWith(e))) {
+                        [t, o] = e.split(r, 2);
+                        break
+                    } if (!t || !r || !o) throw Error(`Invalid interception route: ${e}. Must be in the format /<intercepting route>/(..|...|..)(..)/<intercepted route>`);
+                switch (t = (0, n.normalizeAppPath)(t), r) {
+                    case "(.)":
+                        o = "/" === t ? `/${o}` : t + "/" + o;
+                        break;
+                    case "(..)":
+                        if ("/" === t) throw Error(`Invalid interception route: ${e}. Cannot use (..) marker at the root level, use (.) instead.`);
+                        o = t.split("/").slice(0, -1).concat(o).join("/");
+                        break;
+                    case "(...)":
+                        o = "/" + o;
+                        break;
+                    case "(..)(..)":
+                        let i = t.split("/");
+                        if (i.length <= 2) throw Error(`Invalid interception route: ${e}. Cannot use (..)(..) marker at the root level or one level up.`);
+                        o = i.slice(0, -2).concat(o).join("/");
+                        break;
+                    default:
+                        throw Error("Invariant: unexpected marker")
+                }
+                return {
+                    interceptingRoute: t,
+                    interceptedRoute: o
+                }
+            }
+        },
         2431: function() {},
         8754: function(e, t, r) {
             "use strict";
 
             function n(e) {
                 return e && e.__esModule ? e : {
                     default: e
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/_app-4638cf4f01fc5510.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2831,18 +2831,15 @@
                         theme: r
                     } = e, n = p(), a = i.useMemo(() => {
                         let e = null === n ? r : function(e, t) {
                             if ("function" == typeof t) {
                                 let r = t(e);
                                 return r
                             }
-                            return {
-                                ...e,
-                                ...t
-                            }
+                            return (0, l.Z)({}, e, t)
                         }(n, r);
                         return null != e && (e[m] = null !== n), e
                     }, [r, n]);
                     return (0, o.jsx)(f.Provider, {
                         value: a,
                         children: t
                     })
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-ea5036b8dd1a507b.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-57051d0ee30b9efa.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -164,15 +164,15 @@
                 r = n(7294),
                 a = n(1163),
                 s = n(2734),
                 o = n(5582),
                 l = n(6886),
                 c = n(8456),
                 d = n(5861),
-                u = n(3913),
+                u = n(9713),
                 p = n(699),
                 h = n(3321),
                 x = n(6154),
                 m = n(8103),
                 y = function() {
                     let e = (0, a.useRouter)().query,
                         [t, n] = (0, r.useState)(),
@@ -283,12 +283,12 @@
                         noHeader: !0,
                         children: (0, i.jsx)(y, {})
                     })
                 }
         }
     },
     function(e) {
-        e.O(0, [702, 134, 418, 498, 699, 154, 913, 774, 888, 179], function() {
+        e.O(0, [702, 134, 728, 498, 699, 154, 713, 774, 888, 179], function() {
             return e(e.s = 1328)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-7e45aefe6a4d48af.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-d4f904aedaf93672.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -436,12 +436,12 @@
                         noHeader: !0,
                         children: (0, n.jsx)(P, {})
                     })
                 }
         }
     },
     function(e) {
-        e.O(0, [702, 134, 418, 498, 699, 154, 767, 774, 888, 179], function() {
+        e.O(0, [702, 134, 728, 498, 699, 154, 767, 774, 888, 179], function() {
             return e(e.s = 8573)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/data-a3eeebdc39c5f892.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/data-59d72c465167efc4.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -177,45 +177,45 @@
                 }
                 isConnected() {
                     var e;
                     return (null === (e = this.websocket) || void 0 === e ? void 0 : e.readyState) === WebSocket.OPEN
                 }
                 getData(e) {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && (console.log("Get data:", e), this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "GET_DATA",
                         modules: e
                     })))
                 }
                 getSettings() {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && (console.log("Get settings"), this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "GET_SETTINGS"
                     })))
                 }
                 registerDataListener(e) {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && (console.log("Register data listener:", e), this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "REGISTER_DATA_LISTENER",
                         modules: e
                     })))
                 }
                 sendPlayerStatus(e) {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "MEDIA_STATUS",
                         status: e
                     }))
                 }
                 updateSetting(e, t) {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && (console.log("Update setting:", {
                         key: e,
                         value: t
                     }), this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "UPDATE_SETTING",
                         setting: e,
                         value: t
                     })))
                 }
                 constructor(e, t, s) {
                     this.port = e || 9170, this.apiKey = t, (async () => {
@@ -224,50 +224,51 @@
                 }
             }
         },
         6351: function(e, t, s) {
             "use strict";
             s.r(t), s.d(t, {
                 default: function() {
-                    return P
+                    return E
                 }
             });
             var n = s(5893),
                 i = s(7294),
                 o = s(5582),
                 a = s(1163),
                 r = s(2734),
                 c = s(6886),
                 l = s(1703),
                 d = s(44),
                 h = s(8456),
-                u = s(6486),
-                p = s(6018),
-                y = s(5152),
-                m = s.n(y),
-                g = s(4267),
-                w = s(5861);
-            let b = m()(() => s.e(171).then(s.t.bind(s, 5171, 23)), {
+                u = s(361),
+                p = s.n(u),
+                y = s(6018),
+                m = s(5152),
+                g = s.n(m),
+                w = s(4267),
+                b = s(5861);
+            let k = g()(() => s.e(171).then(s.t.bind(s, 5171, 23)), {
                 loadableGenerated: {
                     webpack: () => [5171]
                 },
                 ssr: !1
             });
-            var k = function(e) {
+            var x = function(e) {
                 let {
                     name: t,
                     data: s
                 } = e;
-                return (0, n.jsxs)(g.Z, {
-                    children: [(0, n.jsx)(w.Z, {
+                return (0, n.jsxs)(w.Z, {
+                    children: [(0, n.jsx)(b.Z, {
                         gutterBottom: !0,
                         variant: "h4",
                         component: "h3",
                         children: t
-                    }), s ? (0, n.jsx)(b, {
+                    }), s ? (0, n.jsx)(k, {
                         src: s,
                         displayDataTypes: !1,
                         displayObjectSize: !0,
                         enableClipboard: !0,
                         iconStyle: "triangle",
                         name: null,
                         collapseStringsAfterLength: 140,
@@ -280,121 +281,121 @@
                         container: !0,
                         direction: "row",
                         justifyContent: "center",
                         children: (0, n.jsx)(h.Z, {})
                     })]
                 })
             };
-            let x = ["battery", "cpu", "disk", "display", "gpu", "media", "memory", "network", "sensors", "system"],
-                f = {
+            let f = ["battery", "cpu", "disk", "display", "gpu", "media", "memory", "network", "sensors", "system"],
+                S = {
                     battery: "Battery",
                     cpu: "CPU",
                     disk: "Disk",
                     display: "Display",
                     gpu: "GPU",
                     media: "Media",
                     memory: "Memory",
                     network: "Network",
                     sensors: "Sensors",
                     system: "System"
                 },
-                S = {
+                j = {
                     battery: {},
                     cpu: {},
                     disk: {},
                     media: {},
                     memory: {},
                     network: {},
                     sensors: {},
                     system: {}
                 };
-            var j = function() {
-                    let [e, t] = (0, i.useState)(S), [s, o] = (0, i.useState)(!1), [y, m] = (0, i.useState)(0), g = (0, a.useRouter)().query, w = (0, i.useCallback)(e => {
+            var v = function() {
+                    let [e, t] = (0, i.useState)(j), [s, o] = (0, i.useState)(!1), [u, m] = (0, i.useState)(0), g = (0, a.useRouter)().query, w = (0, i.useCallback)(e => {
                         console.log("Event:", e), "DATA_UPDATE" === e.type && (console.log("Data update:", e.module, e.data), t(t => {
-                            let s = (0, u.cloneDeep)(t);
+                            let s = p()(t);
                             return "string" == typeof e.module && (s[e.module] = e.data), s
                         }))
                     }, []), b = (0, i.useCallback)((e, t) => {
                         console.log("Setup WebSocketConnection");
-                        let s = new p.C(e, t, async () => {
-                            s.getData(x), s.registerDataListener(x)
+                        let s = new y.C(e, t, async () => {
+                            s.getData(f), s.registerDataListener(f)
                         });
                         s.onEvent = w
                     }, [w]);
                     (0, i.useEffect)(() => {
                         !s && g && g.apiKey && (o(!0), b(Number(g.apiPort) || 9170, String(g.apiKey)))
                     }, [s, b, g]);
-                    let j = (0, r.Z)();
+                    let k = (0, r.Z)();
                     return (0, n.jsx)(n.Fragment, {
                         children: (0, n.jsx)(c.ZP, {
                             container: !0,
                             direction: "column",
                             spacing: 2,
                             alignItems: "stretch",
                             sx: {
-                                padding: j.spacing(2)
+                                padding: k.spacing(2)
                             },
                             children: (0, n.jsxs)(c.ZP, {
                                 container: !0,
                                 direction: "row",
                                 item: !0,
                                 xs: !0,
                                 children: [(0, n.jsx)(c.ZP, {
                                     item: !0,
                                     children: (0, n.jsx)(l.Z, {
                                         orientation: "vertical",
                                         variant: "scrollable",
-                                        value: y,
+                                        value: u,
                                         onChange: (e, t) => {
                                             m(t)
                                         },
-                                        children: x.map((e, t) => (0, n.jsx)(d.Z, {
-                                            label: f[e],
+                                        children: f.map((e, t) => (0, n.jsx)(d.Z, {
+                                            label: S[e],
                                             id: "scrollable-auto-tab-".concat(t),
                                             "aria-controls": "scrollable-auto-tabpanel-".concat(t)
                                         }, t))
                                     })
                                 }), (0, n.jsx)(c.ZP, {
                                     item: !0,
                                     xs: !0,
-                                    children: x.map((t, s) => (0, n.jsx)(i.Fragment, {
-                                        children: y === s ? (0, n.jsx)(n.Fragment, {
-                                            children: e[t] ? (0, n.jsx)(k, {
+                                    children: f.map((t, s) => (0, n.jsx)(i.Fragment, {
+                                        children: u === s ? (0, n.jsx)(n.Fragment, {
+                                            children: e[t] ? (0, n.jsx)(x, {
                                                 data: e[t],
-                                                name: f[t]
+                                                name: S[t]
                                             }) : (0, n.jsx)(c.ZP, {
                                                 container: !0,
                                                 direction: "row",
                                                 justifyContent: "center",
                                                 sx: {
-                                                    margin: j.spacing(8, 0, 14)
+                                                    margin: k.spacing(8, 0, 14)
                                                 },
                                                 children: (0, n.jsx)(h.Z, {})
                                             })
                                         }) : ""
                                     }, s))
                                 })]
                             })
                         })
                     })
                 },
-                v = s(8980),
-                P = function() {
-                    return (0, n.jsx)(v.Z, {
+                P = s(8980),
+                E = function() {
+                    return (0, n.jsx)(P.Z, {
                         title: "Data",
                         url: "https://system-bridge.timmo.dev",
                         description: "Frontend for System Bridge",
                         children: (0, n.jsx)(o.Z, {
                             component: "article",
                             maxWidth: "xl",
-                            children: (0, n.jsx)(j, {})
+                            children: (0, n.jsx)(v, {})
                         })
                     })
                 }
         }
     },
     function(e) {
-        e.O(0, [702, 662, 134, 498, 731, 774, 888, 179], function() {
+        e.O(0, [702, 134, 498, 361, 731, 774, 888, 179], function() {
             return e(e.s = 8792)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/notification-0384bbf9e77dbfb4.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/notification-416e0ab0e8597db3.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 (self.webpackChunk_N_E = self.webpackChunk_N_E || []).push([
     [723], {
-        4239: function(e, t, n) {
+        8973: function(e, t, n) {
             (window.__NEXT_P = window.__NEXT_P || []).push(["/app/notification", function() {
                 return n(154)
             }])
         },
         8980: function(e, t, n) {
             "use strict";
             n.d(t, {
                 Z: function() {
                     return k
                 }
             });
             var i = n(5893),
-                o = n(7294),
-                r = n(1163),
+                r = n(7294),
+                o = n(1163),
                 a = n(9008),
                 s = n.n(a),
                 c = n(3946),
                 l = n(8849),
                 d = n(5317),
                 u = n(8298),
                 p = n(2734),
@@ -33,21 +33,21 @@
             function j(e) {
                 let {
                     children: t
                 } = e, n = (0, u.Z)({
                     disableHysteresis: !0,
                     threshold: 24
                 });
-                return (0, o.cloneElement)(t, {
+                return (0, r.cloneElement)(t, {
                     elevation: n ? 4 : 0
                 })
             }
             var Z = function() {
-                let [e, t] = (0, o.useState)(!1);
-                (0, o.useCallback)(() => {
+                let [e, t] = (0, r.useState)(!1);
+                (0, r.useCallback)(() => {
                     t(!e)
                 }, [e]);
                 let n = (0, p.Z)();
                 return (0, i.jsx)(i.Fragment, {
                     children: (0, i.jsx)(j, {
                         children: (0, i.jsxs)(i.Fragment, {
                             children: [(0, i.jsx)(m.Z, {
@@ -95,29 +95,29 @@
                             })]
                         })
                     })
                 })
             };
             let w = !1;
             var k = function(e) {
-                let t = (0, r.useRouter)();
-                return (0, o.useEffect)(() => {
+                let t = (0, o.useRouter)();
+                return (0, r.useEffect)(() => {
                     if (t.isReady && !w) {
-                        var e, n, i, o;
+                        var e, n, i, r;
                         w = !0;
-                        let r = (null === (e = t.query) || void 0 === e ? void 0 : e.apiKey) || "",
+                        let o = (null === (e = t.query) || void 0 === e ? void 0 : e.apiKey) || "",
                             a = (null === (n = t.query) || void 0 === n ? void 0 : n.apiPort) || "9170",
                             s = !1;
-                        if ((null === (i = t.query) || void 0 === i ? void 0 : i.apiKey) || (s = !0, r = window.prompt("Please enter your API key", r)), (null === (o = t.query) || void 0 === o ? void 0 : o.apiPort) || (s = !0, a = window.prompt("Please enter your API port (default: 9170)", a)), s && r && a) {
+                        if ((null === (i = t.query) || void 0 === i ? void 0 : i.apiKey) || (s = !0, o = window.prompt("Please enter your API key", o)), (null === (r = t.query) || void 0 === r ? void 0 : r.apiPort) || (s = !0, a = window.prompt("Please enter your API port (default: 9170)", a)), s && o && a) {
                             let e = t.asPath.split("?")[0];
                             t.replace({
                                 pathname: e.includes(".html") ? e : "".concat(e, ".html"),
                                 query: {
                                     ...t.query,
-                                    apiKey: r,
+                                    apiKey: o,
                                     apiPort: a
                                 }
                             })
                         }
                     }
                 }, [t]), (0, i.jsxs)(i.Fragment, {
                     children: [(0, i.jsxs)(s(), {
@@ -153,24 +153,24 @@
                 })
             }
         },
         154: function(e, t, n) {
             "use strict";
             n.r(t), n.d(t, {
                 default: function() {
-                    return T
+                    return $
                 }
             });
             var i = n(5893),
-                o = n(7294),
-                r = n(1163),
+                r = n(7294),
+                o = n(1163),
                 a = n(2734),
                 s = n(3366),
                 c = n(7462),
-                l = n(6010),
+                l = n(209),
                 d = n(9766),
                 u = n(4780),
                 p = n(4867),
                 m = n(3264),
                 h = n(9628),
                 g = n(9707),
                 f = n(6500),
@@ -210,54 +210,54 @@
                         values: e.direction,
                         breakpoints: t.breakpoints.values
                     }), e => ({
                         flexDirection: e
                     })));
                     if (e.spacing) {
                         let i = (0, y.hB)(t),
-                            o = Object.keys(t.breakpoints.values).reduce((t, n) => (("object" == typeof e.spacing && null != e.spacing[n] || "object" == typeof e.direction && null != e.direction[n]) && (t[n] = !0), t), {}),
-                            r = (0, x.P$)({
+                            r = Object.keys(t.breakpoints.values).reduce((t, n) => (("object" == typeof e.spacing && null != e.spacing[n] || "object" == typeof e.direction && null != e.direction[n]) && (t[n] = !0), t), {}),
+                            o = (0, x.P$)({
                                 values: e.direction,
-                                base: o
+                                base: r
                             }),
                             a = (0, x.P$)({
                                 values: e.spacing,
-                                base: o
+                                base: r
                             });
-                        "object" == typeof r && Object.keys(r).forEach((e, t, n) => {
-                            let i = r[e];
+                        "object" == typeof o && Object.keys(o).forEach((e, t, n) => {
+                            let i = o[e];
                             if (!i) {
-                                let i = t > 0 ? r[n[t - 1]] : "column";
-                                r[e] = i
+                                let i = t > 0 ? o[n[t - 1]] : "column";
+                                o[e] = i
                             }
                         }), n = (0, d.Z)(n, (0, x.k9)({
                             theme: t
                         }, a, (t, n) => e.useFlexGap ? {
                             gap: (0, y.NA)(i, t)
                         } : {
-                            "& > :not(style) + :not(style)": {
+                            "& > :not(style) ~ :not(style)": {
                                 margin: 0,
-                                [`margin${k(n?r[n]:e.direction)}`]: (0, y.NA)(i, t)
+                                [`margin${k(n?o[n]:e.direction)}`]: (0, y.NA)(i, t)
                             }
                         }))
                     }
                     return (0, x.dt)(t.breakpoints, n)
                 };
             var C = n(948),
                 P = n(1657);
             let S = function(e = {}) {
                 let {
                     createStyledComponent: t = Z,
                     useThemeProps: n = w,
-                    componentName: r = "MuiStack"
+                    componentName: o = "MuiStack"
                 } = e, a = () => (0, u.Z)({
                     root: ["root"]
-                }, e => (0, p.Z)(r, e), {}), d = t(b), m = o.forwardRef(function(e, t) {
-                    let r = n(e),
-                        u = (0, g.Z)(r),
+                }, e => (0, p.Z)(o, e), {}), d = t(b), m = r.forwardRef(function(e, t) {
+                    let o = n(e),
+                        u = (0, g.Z)(o),
                         {
                             component: p = "div",
                             direction: m = "column",
                             spacing: h = 0,
                             divider: f,
                             children: x,
                             className: y,
@@ -272,17 +272,17 @@
                             spacing: h,
                             useFlexGap: j
                         },
                         ref: t,
                         className: (0, l.Z)(w.root, y)
                     }, Z, {
                         children: f ? function(e, t) {
-                            let n = o.Children.toArray(e).filter(Boolean);
-                            return n.reduce((e, i, r) => (e.push(i), r < n.length - 1 && e.push(o.cloneElement(t, {
-                                key: `separator-${r}`
+                            let n = r.Children.toArray(e).filter(Boolean);
+                            return n.reduce((e, i, o) => (e.push(i), o < n.length - 1 && e.push(r.cloneElement(t, {
+                                key: `separator-${o}`
                             })), e), [])
                         }(x, f) : x
                     }))
                 });
                 return m
             }({
                 createStyledComponent: (0, C.ZP)("div", {
@@ -291,139 +291,140 @@
                     overridesResolver: (e, t) => t.root
                 }),
                 useThemeProps: e => (0, P.Z)({
                     props: e,
                     name: "MuiStack"
                 })
             });
+            var M = n(3680);
 
-            function M(e) {
+            function N(e) {
                 return (0, p.Z)("MuiCardMedia", e)
             }(0, n(1588).Z)("MuiCardMedia", ["root", "media", "img"]);
-            let N = ["children", "className", "component", "image", "src", "style"],
-                R = e => {
+            let R = ["children", "className", "component", "image", "src", "style"],
+                _ = e => {
                     let {
                         classes: t,
                         isMediaComponent: n,
                         isImageComponent: i
                     } = e;
                     return (0, u.Z)({
                         root: ["root", n && "media", i && "img"]
-                    }, M, t)
+                    }, N, t)
                 },
-                _ = (0, C.ZP)("div", {
+                I = (0, C.ZP)("div", {
                     name: "MuiCardMedia",
                     slot: "Root",
                     overridesResolver: (e, t) => {
                         let {
                             ownerState: n
                         } = e, {
                             isMediaComponent: i,
-                            isImageComponent: o
+                            isImageComponent: r
                         } = n;
-                        return [t.root, i && t.media, o && t.img]
+                        return [t.root, i && t.media, r && t.img]
                     }
                 })(({
                     ownerState: e
                 }) => (0, c.Z)({
                     display: "block",
                     backgroundSize: "cover",
                     backgroundRepeat: "no-repeat",
                     backgroundPosition: "center"
                 }, e.isMediaComponent && {
                     width: "100%"
                 }, e.isImageComponent && {
                     objectFit: "cover"
                 })),
-                I = ["video", "audio", "picture", "iframe", "img"],
-                B = ["picture", "img"],
-                q = o.forwardRef(function(e, t) {
+                B = ["video", "audio", "picture", "iframe", "img"],
+                q = ["picture", "img"],
+                E = r.forwardRef(function(e, t) {
                     let n = (0, P.Z)({
                             props: e,
                             name: "MuiCardMedia"
                         }),
                         {
-                            children: o,
-                            className: r,
+                            children: r,
+                            className: o,
                             component: a = "div",
-                            image: d,
-                            src: u,
-                            style: p
+                            image: l,
+                            src: d,
+                            style: u
                         } = n,
-                        m = (0, s.Z)(n, N),
-                        h = -1 !== I.indexOf(a),
-                        g = !h && d ? (0, c.Z)({
-                            backgroundImage: `url("${d}")`
-                        }, p) : p,
-                        f = (0, c.Z)({}, n, {
+                        p = (0, s.Z)(n, R),
+                        m = -1 !== B.indexOf(a),
+                        h = !m && l ? (0, c.Z)({
+                            backgroundImage: `url("${l}")`
+                        }, u) : u,
+                        g = (0, c.Z)({}, n, {
                             component: a,
-                            isMediaComponent: h,
-                            isImageComponent: -1 !== B.indexOf(a)
+                            isMediaComponent: m,
+                            isImageComponent: -1 !== q.indexOf(a)
                         }),
-                        x = R(f);
-                    return (0, i.jsx)(_, (0, c.Z)({
-                        className: (0, l.Z)(x.root, r),
+                        f = _(g);
+                    return (0, i.jsx)(I, (0, c.Z)({
+                        className: (0, M.Z)(f.root, o),
                         as: a,
-                        role: !h && d ? "img" : void 0,
+                        role: !m && l ? "img" : void 0,
                         ref: t,
-                        style: g,
-                        ownerState: f,
-                        src: h ? d || u : void 0
-                    }, m, {
-                        children: o
+                        style: h,
+                        ownerState: g,
+                        src: m ? l || d : void 0
+                    }, p, {
+                        children: r
                     }))
                 });
-            var E = n(5861),
-                A = n(3321),
-                F = n(6154);
-            class O {
+            var A = n(5861),
+                F = n(3321),
+                O = n(6154);
+            class H {
                 async request(e) {
                     let {
                         body: t,
                         endpoint: n,
                         method: i,
-                        params: o
-                    } = e, r = {
+                        params: r
+                    } = e, o = {
                         baseURL: "http://localhost:".concat(this.port),
                         data: t,
                         headers: {
                             "api-key": this.apiKey
                         },
                         method: i,
-                        params: o,
+                        params: r,
                         url: "/api/".concat(n)
                     };
-                    return await F.Z.request(r)
+                    return await O.Z.request(o)
                 }
                 constructor(e, t) {
                     this.apiKey = t, this.port = e || 9170
                 }
             }
-            var H = n(8980),
-                T = function() {
-                    let e = (0, r.useRouter)(),
+            var T = n(8980),
+                $ = function() {
+                    let e = (0, o.useRouter)(),
                         {
                             apiPort: t,
                             apiKey: n,
                             title: s,
                             message: c,
                             icon: l,
                             image: d,
                             actions: u
                         } = e.query,
-                        p = (0, o.useMemo)(() => {
+                        p = (0, r.useMemo)(() => {
                             if (u) try {
                                 return JSON.parse(u)
                             } catch (e) {
                                 console.error(e)
                             }
                             return null
                         }, [u]),
                         m = (0, a.Z)();
-                    return (0, i.jsx)(H.Z, {
+                    return (0, i.jsx)(T.Z, {
                         title: "Notification",
                         url: "https://system-bridge.timmo.dev",
                         description: "Frontend for System Bridge",
                         closeButton: !0,
                         noHeader: !0,
                         children: (0, i.jsxs)(S, {
                             direction: "column",
@@ -437,40 +438,40 @@
                             children: [(0, i.jsxs)(S, {
                                 direction: "row",
                                 alignContent: "center",
                                 justifyContent: "flex-start",
                                 style: {
                                     padding: m.spacing(1, 1, 1)
                                 },
-                                children: [l && (0, i.jsx)(q, {
+                                children: [l && (0, i.jsx)(E, {
                                     component: "img",
                                     image: l,
                                     alt: "Notification Icon",
                                     sx: {
                                         height: 28,
                                         width: 28,
                                         margin: m.spacing(.5, 0, .5, 1)
                                     }
-                                }), (0, i.jsx)(E.Z, {
+                                }), (0, i.jsx)(A.Z, {
                                     component: "h1",
                                     variant: "h5",
                                     sx: {
                                         margin: m.spacing(0, 1)
                                     },
                                     children: s
                                 })]
-                            }), c && (0, i.jsx)(E.Z, {
+                            }), c && (0, i.jsx)(A.Z, {
                                 component: "div",
                                 variant: "body2",
                                 color: "text.secondary",
                                 sx: {
                                     padding: m.spacing(0, l ? 7 : 2, 1)
                                 },
                                 children: c
-                            }), d && (0, i.jsx)(q, {
+                            }), d && (0, i.jsx)(E, {
                                 component: "img",
                                 image: d,
                                 alt: "Notification Image",
                                 sx: {
                                     height: "280px",
                                     maxHeight: "280px",
                                     maxWidth: "100%",
@@ -479,24 +480,24 @@
                             }), p && (0, i.jsx)(S, {
                                 direction: "row",
                                 alignContent: "center",
                                 justifyContent: "flex-end",
                                 sx: {
                                     padding: m.spacing(1)
                                 },
-                                children: p.map(e => (0, i.jsx)(A.Z, {
+                                children: p.map(e => (0, i.jsx)(F.Z, {
                                     variant: "contained",
                                     color: "primary",
                                     sx: {
                                         margin: m.spacing(1, .5, 1, .5)
                                     },
                                     onClick: () => (function(e) {
                                         switch (console.log("Action clicked:", e), e.command) {
                                             case "api":
-                                                new O(Number(t) || 9170, String(n)).request(e.data).then(e => {
+                                                new H(Number(t) || 9170, String(n)).request(e.data).then(e => {
                                                     console.log("API Response:", e.data)
                                                 }).catch(e => {
                                                     console.error("API Error:", e)
                                                 });
                                                 break;
                                             case "close":
                                                 window.location.href = "http://close.window"
@@ -508,11 +509,11 @@
                         })
                     })
                 }
         }
     },
     function(e) {
         e.O(0, [702, 134, 154, 774, 888, 179], function() {
-            return e(e.s = 4239)
+            return e(e.s = 8973)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-8b29e9945ddce62c.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-3826169d9ca46804.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -26,12 +26,12 @@
                         })
                     })
                 })
             }
         }
     },
     function(e) {
-        e.O(0, [702, 662, 885, 134, 418, 633, 142, 774, 888, 179], function() {
+        e.O(0, [702, 885, 134, 728, 361, 514, 142, 774, 888, 179], function() {
             return e(e.s = 2134)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-b8b2ae3418f95cef.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/player/video-9c7e9646d273d6aa.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -26,12 +26,12 @@
                         })
                     })
                 })
             }
         }
     },
     function(e) {
-        e.O(0, [702, 662, 885, 134, 418, 633, 142, 774, 888, 179], function() {
+        e.O(0, [702, 885, 134, 728, 361, 514, 142, 774, 888, 179], function() {
             return e(e.s = 3049)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/app/settings-0b5df1a27de4507f.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/app/settings-c2e844bc6170d7a5.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -204,45 +204,45 @@
                 }
                 isConnected() {
                     var e;
                     return (null === (e = this.websocket) || void 0 === e ? void 0 : e.readyState) === WebSocket.OPEN
                 }
                 getData(e) {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && (console.log("Get data:", e), this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "GET_DATA",
                         modules: e
                     })))
                 }
                 getSettings() {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && (console.log("Get settings"), this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "GET_SETTINGS"
                     })))
                 }
                 registerDataListener(e) {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && (console.log("Register data listener:", e), this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "REGISTER_DATA_LISTENER",
                         modules: e
                     })))
                 }
                 sendPlayerStatus(e) {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "MEDIA_STATUS",
                         status: e
                     }))
                 }
                 updateSetting(e, t) {
                     this.websocket && this.websocket.readyState === this.websocket.OPEN && (console.log("Update setting:", {
                         key: e,
                         value: t
                     }), this.websocket.send(JSON.stringify({
-                        "api-key": this.apiKey,
+                        api_key: this.apiKey,
                         event: "UPDATE_SETTING",
                         setting: e,
                         value: t
                     })))
                 }
                 constructor(e, t, i) {
                     this.port = e || 9170, this.apiKey = t, (async () => {
@@ -277,20 +277,20 @@
                 f = i(9953),
                 v = i(3395),
                 k = i(9653),
                 b = i(4054),
                 Z = i(7709),
                 w = i(7109),
                 S = i(3946),
-                P = i(3913),
+                P = i(9713),
                 C = i(699),
                 E = i(8849),
-                I = i(8995),
-                N = i(8396),
-                _ = i(657),
+                _ = i(8995),
+                I = i(8396),
+                N = i(657),
                 A = i(7645),
                 O = i(8951),
                 T = i(6514),
                 R = i(8462),
                 z = i(1425),
                 D = i(3321),
                 W = i(6486),
@@ -318,16 +318,16 @@
                         description: x,
                         icon: v
                     } = i;
                     (0, a.useEffect)(() => {
                         !o && n && h(n)
                     }, [n, o]);
                     let k = (0, l.Z)(),
-                        b = (0, N.Z)(k.breakpoints.down("md"));
-                    return (0, s.jsxs)(_.Z, {
+                        b = (0, I.Z)(k.breakpoints.down("md"));
+                    return (0, s.jsxs)(N.Z, {
                         fullScreen: b,
                         fullWidth: !0,
                         maxWidth: "lg",
                         open: o,
                         scroll: "paper",
                         PaperProps: {
                             style: {
@@ -453,18 +453,18 @@
                 q = function(e) {
                     let {
                         keyIn: t,
                         valueIn: i,
                         handleChanged: n
                     } = e, [o, r] = (0, a.useState)(!1), [d, u] = (0, a.useState)(!1), [h, g] = (0, a.useState)(i);
 
-                    function N(e) {
+                    function I(e) {
                         g(e.target.value)
                     }
-                    let _ = (0, a.useMemo)(() => i !== h, [i, h]),
+                    let N = (0, a.useMemo)(() => i !== h, [i, h]),
                         {
                             name: A,
                             description: O,
                             icon: T,
                             containerDisabled: R,
                             isList: z,
                             isPassword: D,
@@ -539,15 +539,15 @@
                                                                 id: "generate-api-key",
                                                                 title: "Generate API Key",
                                                                 size: 1,
                                                                 path: p.VmU
                                                             })
                                                         }), (0, s.jsx)(S.Z, {
                                                             "aria-label": "Copy to clipboard",
-                                                            onClick: () => (0, I.X)(String(h)),
+                                                            onClick: () => (0, _.X)(String(h)),
                                                             size: "large",
                                                             sx: {
                                                                 margin: G.spacing(-1, -.5)
                                                             },
                                                             children: (0, s.jsx)(E.Icon, {
                                                                 id: "copy-to-clipboard",
                                                                 title: "Copy to clipboard",
@@ -572,15 +572,15 @@
                                                 },
                                                 value: h
                                             }) : "string" == typeof i && D ? (0, s.jsx)(b.Z, {
                                                 variant: "outlined",
                                                 children: (0, s.jsx)(Z.Z, {
                                                     type: d ? "text" : "password",
                                                     defaultValue: h,
-                                                    onChange: N,
+                                                    onChange: I,
                                                     endAdornment: (0, s.jsx)(w.Z, {
                                                         position: "end",
                                                         children: (0, s.jsx)(S.Z, {
                                                             "aria-label": "Toggle visibility",
                                                             onClick: function() {
                                                                 u(!d)
                                                             },
@@ -597,44 +597,44 @@
                                                         })
                                                     })
                                                 })
                                             }) : "string" == typeof i ? (0, s.jsx)(C.Z, {
                                                 type: "text",
                                                 defaultValue: h,
                                                 disabled: R,
-                                                onChange: N,
+                                                onChange: I,
                                                 variant: "outlined"
                                             }) : "number" == typeof i ? (0, s.jsx)(C.Z, {
                                                 error: !!W && Number(h) < W,
                                                 type: "number",
                                                 disabled: R,
                                                 inputProps: {
                                                     minimum: W
                                                 },
                                                 defaultValue: h,
-                                                onChange: N,
+                                                onChange: I,
                                                 variant: "outlined"
                                             }) : ""
                                         }), (0, s.jsx)(c.ZP, {
                                             item: !0,
                                             children: (0, s.jsx)(S.Z, {
-                                                disabled: !1 === _,
+                                                disabled: !1 === N,
                                                 onClick: () => {
                                                     n(t, h)
                                                 },
                                                 sx: {
                                                     margin: G.spacing(1)
                                                 },
                                                 children: (0, s.jsx)(E.Icon, {
                                                     id: "save",
                                                     title: "Save",
                                                     size: 1,
                                                     path: p.JTj,
                                                     style: {
-                                                        opacity: _ ? 1 : .25
+                                                        opacity: N ? 1 : .25
                                                     }
                                                 })
                                             })
                                         })]
                                     })
                                 })]
                             })
@@ -788,12 +788,12 @@
                             children: (0, s.jsx)(H, {})
                         })
                     })
                 }
         }
     },
     function(e) {
-        e.O(0, [702, 662, 134, 418, 498, 699, 913, 767, 826, 774, 888, 179], function() {
+        e.O(0, [702, 662, 134, 728, 498, 699, 713, 767, 826, 774, 888, 179], function() {
             return e(e.s = 4768)
         }), _N_E = e.O()
     }
 ]);
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/chunks/webpack-29bb9d3475e20ac7.js` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/chunks/webpack-8c974454c1c3cd10.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -90,15 +90,15 @@
             743: "reactPlayerVimeo",
             965: "reactPlayerVidyard"
         })[e] || e) + "." + ({
             11: "812fbc47cf3ccebc",
             55: "29aa97668baf75ea",
             121: "3663ffcf10139668",
             125: "60e72fefd71eeb25",
-            171: "64880094f51dbbf7",
+            171: "cfc407cdf8574e41",
             216: "52035ec5fd363953",
             261: "46641a0f37607223",
             439: "77a6d75e3f5e95ef",
             546: "c374322fbd4a05d5",
             596: "da042b36db7662eb",
             664: "9b535aa9cbcb0a91",
             667: "258ac8431338b78a",
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.d17f5f2b.woff` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.d17f5f2b.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.d6d4cf7b.woff` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.d6d4cf7b.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-latin-400-normal.f2894edc.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.21abc8c8.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.9600b4a6.woff` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-latin-ext-400-normal.9600b4a6.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.b339d926.woff` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.b339d926.woff`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/_next/static/media/roboto-vietnamese-400-normal.c95fc061.woff2`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/bridges/openon.html` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/bridges/setup.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Open URL On - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/418-f078369e2fd2524e.js" defer=""></script><script src="/_next/static/chunks/498-112306b4f8cd81ec.js" defer=""></script><script src="/_next/static/chunks/699-1a88a588882ce475.js" defer=""></script><script src="/_next/static/chunks/154-7942dd40332ec4bf.js" defer=""></script><script src="/_next/static/chunks/913-948b3bc7b49750f4.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/openon-ea5036b8dd1a507b.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/openon","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Bridges - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/498-c0ac8cca5a5197e4.js" defer=""></script><script src="/_next/static/chunks/699-a015e8646ccfaf97.js" defer=""></script><script src="/_next/static/chunks/154-454aae7a1f6cc481.js" defer=""></script><script src="/_next/static/chunks/767-21712ed9071ee20e.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/setup-d4f904aedaf93672.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_buildManifest.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/setup","query":{},"buildId":"iX_HmcWE_KZJ1V0jDuyN4","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/bridges/setup.html` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/bridges/openon.html`

 * *Files 7% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Bridges - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/418-f078369e2fd2524e.js" defer=""></script><script src="/_next/static/chunks/498-112306b4f8cd81ec.js" defer=""></script><script src="/_next/static/chunks/699-1a88a588882ce475.js" defer=""></script><script src="/_next/static/chunks/154-7942dd40332ec4bf.js" defer=""></script><script src="/_next/static/chunks/767-b6df483a2f96f15d.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/setup-7e45aefe6a4d48af.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/setup","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Open URL On - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/498-c0ac8cca5a5197e4.js" defer=""></script><script src="/_next/static/chunks/699-a015e8646ccfaf97.js" defer=""></script><script src="/_next/static/chunks/154-454aae7a1f6cc481.js" defer=""></script><script src="/_next/static/chunks/713-76d25fee0de05077.js" defer=""></script><script src="/_next/static/chunks/pages/app/bridges/openon-57051d0ee30b9efa.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_buildManifest.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css 1qsxih2">.css-1qsxih2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1qsxih2{padding-left:24px;padding-right:24px;}}@media (min-width:1200px){.css-1qsxih2{max-width:1200px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthLg css-1qsxih2"><style data-emotion="css jybjss">.css-jybjss{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:80px 0px 64px;}</style><div class="MuiGrid-root MuiGrid-container css-jybjss"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/bridges/openon","query":{},"buildId":"iX_HmcWE_KZJ1V0jDuyN4","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/data.html` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/data.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Data - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/498-112306b4f8cd81ec.js" defer=""></script><script src="/_next/static/chunks/731-eb947eaba8f94f26.js" defer=""></script><script src="/_next/static/chunks/pages/app/data-a3eeebdc39c5f892.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css stiot1">.css-stiot1{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;padding:16px;}.css-stiot1>.MuiGrid-item{max-width:none;}.css-stiot1>.MuiGrid-item{padding-top:16px;}.css-stiot1>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-stiot1"><style data-emotion="css 1ag80em">.css-1ag80em{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-grid-xs-true css-1ag80em"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 6x4ics">.css-6x4ics{overflow:hidden;min-height:48px;-webkit-overflow-scrolling:touch;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}@media (max-width:599.95px){.css-6x4ics .MuiTabs-scrollButtons{display:none;}}</style><div class="MuiTabs-root MuiTabs-vertical css-6x4ics"><style data-emotion="css oqr85h">.css-oqr85h{overflow-x:auto;overflow-y:hidden;scrollbar-width:none;}.css-oqr85h::-webkit-scrollbar{display:none;}</style><div style="width:99px;height:99px;position:absolute;top:-9999px;overflow:scroll" class="MuiTabs-hideScrollbar css-oqr85h"></div><style data-emotion="css ccrt04">.css-ccrt04{position:relative;display:inline-block;-webkit-flex:1 1 auto;-ms-flex:1 1 auto;flex:1 1 auto;white-space:nowrap;scrollbar-width:none;overflow-y:auto;overflow-x:hidden;}.css-ccrt04::-webkit-scrollbar{display:none;}</style><div class="MuiTabs-scroller MuiTabs-hideScrollbar MuiTabs-scrollableY css-ccrt04" style="overflow:hidden;margin-right:0"><style data-emotion="css j7qwjs">.css-j7qwjs{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}</style><div aria-orientation="vertical" class="MuiTabs-flexContainer MuiTabs-flexContainerVertical css-j7qwjs" role="tablist"><style data-emotion="css y235a3">.css-y235a3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-y235a3.Mui-selected{color:#512da8;}.css-y235a3.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><style data-emotion="css yt5x7b">.css-yt5x7b{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-yt5x7b::-moz-focus-inner{border-style:none;}.css-yt5x7b.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-yt5x7b{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-yt5x7b.Mui-selected{color:#512da8;}.css-yt5x7b.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary Mui-selected css-yt5x7b" tabindex="0" type="button" role="tab" aria-selected="true" id="scrollable-auto-tab-0" aria-controls="scrollable-auto-tabpanel-0">Battery<style data-emotion="css 14srzcc">.css-14srzcc{position:absolute;height:100%;bottom:0;width:2px;-webkit-transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;background-color:#512da8;right:0;}</style><span class="MuiTabs-indicator css-14srzcc"></span></button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-1" aria-controls="scrollable-auto-tabpanel-1">CPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-2" aria-controls="scrollable-auto-tabpanel-2">Disk</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-3" aria-controls="scrollable-auto-tabpanel-3">Display</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-4" aria-controls="scrollable-auto-tabpanel-4">GPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-5" aria-controls="scrollable-auto-tabpanel-5">Media</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-6" aria-controls="scrollable-auto-tabpanel-6">Memory</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-7" aria-controls="scrollable-auto-tabpanel-7">Network</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-8" aria-controls="scrollable-auto-tabpanel-8">Sensors</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-9" aria-controls="scrollable-auto-tabpanel-9">System</button></div></div></div></div><style data-emotion="css kxu0dz">.css-kxu0dz{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-true css-kxu0dz"><style data-emotion="css iaoeqv">.css-iaoeqv{padding:16px;padding:24px 32px;}.css-iaoeqv:last-child{padding-bottom:24px;}.css-iaoeqv:last-child{padding-bottom:16px;}</style><div class="MuiCardContent-root css-iaoeqv"><style data-emotion="css 177hlju">.css-177hlju{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;margin-bottom:0.35em;}@media (min-width:600px){.css-177hlju{font-size:1.8219rem;}}@media (min-width:900px){.css-177hlju{font-size:2.0243rem;}}@media (min-width:1200px){.css-177hlju{font-size:2.0243rem;}}</style><h3 class="MuiTypography-root MuiTypography-h4 MuiTypography-gutterBottom css-177hlju">Battery</h3></div></div></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/data","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Data - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/498-c0ac8cca5a5197e4.js" defer=""></script><script src="/_next/static/chunks/361-70173883768cacf6.js" defer=""></script><script src="/_next/static/chunks/731-b6cafe94e88ed8c7.js" defer=""></script><script src="/_next/static/chunks/pages/app/data-59d72c465167efc4.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_buildManifest.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css stiot1">.css-stiot1{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;padding:16px;}.css-stiot1>.MuiGrid-item{max-width:none;}.css-stiot1>.MuiGrid-item{padding-top:16px;}.css-stiot1>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-stiot1"><style data-emotion="css 1ag80em">.css-1ag80em{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-1ag80em{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-item MuiGrid-grid-xs-true css-1ag80em"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 6x4ics">.css-6x4ics{overflow:hidden;min-height:48px;-webkit-overflow-scrolling:touch;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}@media (max-width:599.95px){.css-6x4ics .MuiTabs-scrollButtons{display:none;}}</style><div class="MuiTabs-root MuiTabs-vertical css-6x4ics"><style data-emotion="css oqr85h">.css-oqr85h{overflow-x:auto;overflow-y:hidden;scrollbar-width:none;}.css-oqr85h::-webkit-scrollbar{display:none;}</style><div style="width:99px;height:99px;position:absolute;top:-9999px;overflow:scroll" class="MuiTabs-hideScrollbar css-oqr85h"></div><style data-emotion="css ccrt04">.css-ccrt04{position:relative;display:inline-block;-webkit-flex:1 1 auto;-ms-flex:1 1 auto;flex:1 1 auto;white-space:nowrap;scrollbar-width:none;overflow-y:auto;overflow-x:hidden;}.css-ccrt04::-webkit-scrollbar{display:none;}</style><div class="MuiTabs-scroller MuiTabs-hideScrollbar MuiTabs-scrollableY css-ccrt04" style="overflow:hidden;margin-right:0"><style data-emotion="css j7qwjs">.css-j7qwjs{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;}</style><div aria-orientation="vertical" class="MuiTabs-flexContainer MuiTabs-flexContainerVertical css-j7qwjs" role="tablist"><style data-emotion="css y235a3">.css-y235a3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-y235a3.Mui-selected{color:#512da8;}.css-y235a3.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><style data-emotion="css yt5x7b">.css-yt5x7b{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.25;letter-spacing:0.02857em;text-transform:uppercase;max-width:360px;min-width:90px;position:relative;min-height:48px;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;padding:12px 16px;overflow:hidden;white-space:normal;text-align:center;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;color:rgba(255, 255, 255, 0.7);}.css-yt5x7b::-moz-focus-inner{border-style:none;}.css-yt5x7b.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-yt5x7b{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-yt5x7b.Mui-selected{color:#512da8;}.css-yt5x7b.Mui-disabled{color:rgba(255, 255, 255, 0.5);}</style><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary Mui-selected css-yt5x7b" tabindex="0" type="button" role="tab" aria-selected="true" id="scrollable-auto-tab-0" aria-controls="scrollable-auto-tabpanel-0">Battery<style data-emotion="css 14srzcc">.css-14srzcc{position:absolute;height:100%;bottom:0;width:2px;-webkit-transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:all 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;background-color:#512da8;right:0;}</style><span class="MuiTabs-indicator css-14srzcc"></span></button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-1" aria-controls="scrollable-auto-tabpanel-1">CPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-2" aria-controls="scrollable-auto-tabpanel-2">Disk</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-3" aria-controls="scrollable-auto-tabpanel-3">Display</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-4" aria-controls="scrollable-auto-tabpanel-4">GPU</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-5" aria-controls="scrollable-auto-tabpanel-5">Media</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-6" aria-controls="scrollable-auto-tabpanel-6">Memory</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-7" aria-controls="scrollable-auto-tabpanel-7">Network</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-8" aria-controls="scrollable-auto-tabpanel-8">Sensors</button><button class="MuiButtonBase-root MuiTab-root MuiTab-textColorPrimary css-yt5x7b" tabindex="-1" type="button" role="tab" aria-selected="false" id="scrollable-auto-tab-9" aria-controls="scrollable-auto-tabpanel-9">System</button></div></div></div></div><style data-emotion="css kxu0dz">.css-kxu0dz{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}@media (min-width:600px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:900px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1200px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}@media (min-width:1536px){.css-kxu0dz{-webkit-flex-basis:0;-ms-flex-preferred-size:0;flex-basis:0;-webkit-box-flex:1;-webkit-flex-grow:1;-ms-flex-positive:1;flex-grow:1;max-width:100%;}}</style><div class="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-true css-kxu0dz"><style data-emotion="css iaoeqv">.css-iaoeqv{padding:16px;padding:24px 32px;}.css-iaoeqv:last-child{padding-bottom:24px;}.css-iaoeqv:last-child{padding-bottom:16px;}</style><div class="MuiCardContent-root css-iaoeqv"><style data-emotion="css 177hlju">.css-177hlju{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;margin-bottom:0.35em;}@media (min-width:600px){.css-177hlju{font-size:1.8219rem;}}@media (min-width:900px){.css-177hlju{font-size:2.0243rem;}}@media (min-width:1200px){.css-177hlju{font-size:2.0243rem;}}</style><h3 class="MuiTypography-root MuiTypography-h4 MuiTypography-gutterBottom css-177hlju">Battery</h3></div></div></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/data","query":{},"buildId":"iX_HmcWE_KZJ1V0jDuyN4","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/notification.html` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/notification.html`

 * *Files 5% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Notification - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/154-7942dd40332ec4bf.js" defer=""></script><script src="/_next/static/chunks/pages/app/notification-0384bbf9e77dbfb4.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button><style data-emotion="css tqjkiw">.css-tqjkiw{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-tqjkiw" style="height:100vh;width:100%;overflow:hidden"><style data-emotion="css 1vj4tmr">.css-1vj4tmr{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-1vj4tmr" style="padding:8px 8px 8px"><style data-emotion="css qtssx">.css-qtssx{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.25rem;line-height:1.334;letter-spacing:0em;margin:0px 8px;}@media (min-width:600px){.css-qtssx{font-size:1.3118rem;}}@media (min-width:900px){.css-qtssx{font-size:1.4993rem;}}@media (min-width:1200px){.css-qtssx{font-size:1.4993rem;}}</style><h1 class="MuiTypography-root MuiTypography-h5 css-qtssx"></h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/notification","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Notification - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/154-454aae7a1f6cc481.js" defer=""></script><script src="/_next/static/chunks/pages/app/notification-416e0ab0e8597db3.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_buildManifest.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button><style data-emotion="css tqjkiw">.css-tqjkiw{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-tqjkiw" style="height:100vh;width:100%;overflow:hidden"><style data-emotion="css 1vj4tmr">.css-1vj4tmr{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-align-content:center;-ms-flex-line-pack:center;align-content:center;-webkit-box-pack:start;-ms-flex-pack:start;-webkit-justify-content:flex-start;justify-content:flex-start;}</style><div class="MuiStack-root css-1vj4tmr" style="padding:8px 8px 8px"><style data-emotion="css qtssx">.css-qtssx{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.25rem;line-height:1.334;letter-spacing:0em;margin:0px 8px;}@media (min-width:600px){.css-qtssx{font-size:1.3118rem;}}@media (min-width:900px){.css-qtssx{font-size:1.4993rem;}}@media (min-width:1200px){.css-qtssx{font-size:1.4993rem;}}</style><h1 class="MuiTypography-root MuiTypography-h5 css-qtssx"></h1></div></div></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/notification","query":{},"buildId":"iX_HmcWE_KZJ1V0jDuyN4","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/player/audio.html` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/player/audio.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Audio Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/418-f078369e2fd2524e.js" defer=""></script><script src="/_next/static/chunks/633-a2b446f38d34df6a.js" defer=""></script><script src="/_next/static/chunks/142-b511304dc754f6ca.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/audio-8b29e9945ddce62c.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/audio","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Audio Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-c0cb841eaf75495d.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/361-70173883768cacf6.js" defer=""></script><script src="/_next/static/chunks/514-17895623628db944.js" defer=""></script><script src="/_next/static/chunks/142-6fa2d4be01c7dab9.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/audio-3826169d9ca46804.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_buildManifest.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/audio","query":{},"buildId":"iX_HmcWE_KZJ1V0jDuyN4","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/player/video.html` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/player/video.html`

 * *Files 6% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Video Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/418-f078369e2fd2524e.js" defer=""></script><script src="/_next/static/chunks/633-a2b446f38d34df6a.js" defer=""></script><script src="/_next/static/chunks/142-b511304dc754f6ca.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/video-b8b2ae3418f95cef.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/video","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Video Player - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/75fc9c18-c0cb841eaf75495d.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/361-70173883768cacf6.js" defer=""></script><script src="/_next/static/chunks/514-17895623628db944.js" defer=""></script><script src="/_next/static/chunks/142-6fa2d4be01c7dab9.js" defer=""></script><script src="/_next/static/chunks/pages/app/player/video-9c7e9646d273d6aa.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_buildManifest.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css vvp5f9">.css-vvp5f9{text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-vvp5f9:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-vvp5f9:hover{background-color:transparent;}}.css-vvp5f9.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 17pbrtl">.css-17pbrtl{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;text-align:center;-webkit-flex:0 0 auto;-ms-flex:0 0 auto;flex:0 0 auto;font-size:1.5rem;padding:8px;border-radius:50%;overflow:visible;color:#fff;-webkit-transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 150ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;padding:5px;font-size:1.125rem;position:absolute;top:4px;right:4px;z-index:1000;}.css-17pbrtl::-moz-focus-inner{border-style:none;}.css-17pbrtl.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-17pbrtl{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-17pbrtl:hover{background-color:rgba(255, 255, 255, 0.08);}@media (hover: none){.css-17pbrtl:hover{background-color:transparent;}}.css-17pbrtl.Mui-disabled{background-color:transparent;color:rgba(255, 255, 255, 0.3);}</style><button class="MuiButtonBase-root MuiIconButton-root MuiIconButton-sizeSmall css-17pbrtl" tabindex="0" type="button"><svg viewBox="0 0 24 24" style="width:1.5rem;height:1.5rem" role="presentation"><path d="M19,6.41L17.59,5L12,10.59L6.41,5L5,6.41L10.59,12L5,17.59L6.41,19L12,13.41L17.59,19L19,17.59L13.41,12L19,6.41Z" style="fill:currentColor"></path></svg></button></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/player/video","query":{},"buildId":"iX_HmcWE_KZJ1V0jDuyN4","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/app/settings.html` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/app/settings.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Settings - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/418-f078369e2fd2524e.js" defer=""></script><script src="/_next/static/chunks/498-112306b4f8cd81ec.js" defer=""></script><script src="/_next/static/chunks/699-1a88a588882ce475.js" defer=""></script><script src="/_next/static/chunks/913-948b3bc7b49750f4.js" defer=""></script><script src="/_next/static/chunks/767-b6df483a2f96f15d.js" defer=""></script><script src="/_next/static/chunks/826-e44464776abed9eb.js" defer=""></script><script src="/_next/static/chunks/pages/app/settings-0b5df1a27de4507f.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css hm04cy">.css-hm04cy{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;margin-bottom:64px;padding:16px;}.css-hm04cy>.MuiGrid-item{max-width:none;}.css-hm04cy>.MuiGrid-item{padding-top:16px;}.css-hm04cy>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-hm04cy"><style data-emotion="css 8uezpq">.css-8uezpq{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:16px 0px 80px;}</style><div class="MuiGrid-root MuiGrid-container css-8uezpq"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/settings","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Settings - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/29107295-809b6f0b05884bf7.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/728-4d1eeb7a2f426351.js" defer=""></script><script src="/_next/static/chunks/498-c0ac8cca5a5197e4.js" defer=""></script><script src="/_next/static/chunks/699-a015e8646ccfaf97.js" defer=""></script><script src="/_next/static/chunks/713-76d25fee0de05077.js" defer=""></script><script src="/_next/static/chunks/767-21712ed9071ee20e.js" defer=""></script><script src="/_next/static/chunks/826-25c5c840b401fbf5.js" defer=""></script><script src="/_next/static/chunks/pages/app/settings-c2e844bc6170d7a5.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_buildManifest.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"><style data-emotion="css hm04cy">.css-hm04cy{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;margin-top:-16px;width:calc(100% + 16px);margin-left:-16px;-webkit-align-items:stretch;-webkit-box-align:stretch;-ms-flex-align:stretch;align-items:stretch;margin-bottom:64px;padding:16px;}.css-hm04cy>.MuiGrid-item{max-width:none;}.css-hm04cy>.MuiGrid-item{padding-top:16px;}.css-hm04cy>.MuiGrid-item{padding-left:16px;}</style><div class="MuiGrid-root MuiGrid-container MuiGrid-spacing-xs-2 MuiGrid-direction-xs-column css-hm04cy"><style data-emotion="css 8uezpq">.css-8uezpq{box-sizing:border-box;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:wrap;-webkit-flex-wrap:wrap;-ms-flex-wrap:wrap;flex-wrap:wrap;width:100%;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;margin:16px 0px 80px;}</style><div class="MuiGrid-root MuiGrid-container css-8uezpq"><style data-emotion="css a5m0jp animation-61bdi0">.css-a5m0jp{display:inline-block;color:#512da8;-webkit-animation:animation-61bdi0 1.4s linear infinite;animation:animation-61bdi0 1.4s linear infinite;}@-webkit-keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}@keyframes animation-61bdi0{0%{-webkit-transform:rotate(0deg);-moz-transform:rotate(0deg);-ms-transform:rotate(0deg);transform:rotate(0deg);}100%{-webkit-transform:rotate(360deg);-moz-transform:rotate(360deg);-ms-transform:rotate(360deg);transform:rotate(360deg);}}</style><span class="MuiCircularProgress-root MuiCircularProgress-indeterminate MuiCircularProgress-colorPrimary css-a5m0jp" style="width:40px;height:40px" role="progressbar"><style data-emotion="css 13o7eu2">.css-13o7eu2{display:block;}</style><svg class="MuiCircularProgress-svg css-13o7eu2" viewBox="22 22 44 44"><style data-emotion="css 14891ef animation-1p2h4ri">.css-14891ef{stroke:currentColor;stroke-dasharray:80px,200px;stroke-dashoffset:0;-webkit-animation:animation-1p2h4ri 1.4s ease-in-out infinite;animation:animation-1p2h4ri 1.4s ease-in-out infinite;}@-webkit-keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}@keyframes animation-1p2h4ri{0%{stroke-dasharray:1px,200px;stroke-dashoffset:0;}50%{stroke-dasharray:100px,200px;stroke-dashoffset:-15px;}100%{stroke-dasharray:100px,200px;stroke-dashoffset:-125px;}}</style><circle class="MuiCircularProgress-circle MuiCircularProgress-circleIndeterminate css-14891ef" cx="44" cy="44" r="20.2" fill="none" stroke-width="3.6"></circle></svg></span></div></div></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/app/settings","query":{},"buildId":"iX_HmcWE_KZJ1V0jDuyN4","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/favicon.svg` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/favicon.svg`

 * *Files identical despite different names*

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend/out/index.html` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend/out/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Placeholder - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-29bb9d3475e20ac7.js" defer=""></script><script src="/_next/static/chunks/framework-305cb810cde7afac.js" defer=""></script><script src="/_next/static/chunks/main-d5c9aef8f3ea3bae.js" defer=""></script><script src="/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-8b4cf5ad285047cd.js" defer=""></script><script src="/_next/static/chunks/pages/index-f934b9a030f633a0.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js" defer=""></script><script src="/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"7cCNYQwxkasei7aJF3BXn","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
+<!DOCTYPE html><html lang="en"><head><meta charSet="utf-8"/><meta name="viewport" content="minimum-scale=1, initial-scale=1, width=device-width"/><title>Placeholder - System Bridge</title><link rel="canonical" href="https://system-bridge.timmo.dev"/><meta name="description" content="Frontend for System Bridge"/><meta name="keywords" content="system-bridge, system, bridge, typescript"/><meta name="next-head-count" content="6"/><meta name="author" content="Aidan Timson &lt;contact@timmo.xyz&gt;"/><meta name="theme-color" content="#512da8"/><link rel="icon" type="image/svg+xml" href="/favicon.svg"/><link data-next-font="" rel="preconnect" href="/" crossorigin="anonymous"/><link rel="preload" href="/_next/static/css/7c971015b368f9b1.css" as="style"/><link rel="stylesheet" href="/_next/static/css/7c971015b368f9b1.css" data-n-g=""/><noscript data-n-css=""></noscript><script defer="" nomodule="" src="/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js"></script><script src="/_next/static/chunks/webpack-8c974454c1c3cd10.js" defer=""></script><script src="/_next/static/chunks/framework-7a7e500878b44665.js" defer=""></script><script src="/_next/static/chunks/main-2ecf43899f8683c2.js" defer=""></script><script src="/_next/static/chunks/pages/_app-4638cf4f01fc5510.js" defer=""></script><script src="/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js" defer=""></script><script src="/_next/static/chunks/134-be8afb194db80d1f.js" defer=""></script><script src="/_next/static/chunks/pages/index-f934b9a030f633a0.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_buildManifest.js" defer=""></script><script src="/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_ssgManifest.js" defer=""></script><style id="jss-server-side"></style></head><body><div id="__next"><style data-emotion="css-global uox009">html{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;box-sizing:border-box;-webkit-text-size-adjust:100%;}*,*::before,*::after{box-sizing:inherit;}strong,b{font-weight:700;}body{margin:0;color:#fff;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1rem;line-height:1.5;letter-spacing:0.00938em;background-color:#212121;}@media print{body{background-color:#fff;}}body::backdrop{background-color:#212121;}</style><style data-emotion="css hnqd2s">.css-hnqd2s{display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-hnqd2s{position:absolute;}}</style><style data-emotion="css 1gtczq1">.css-1gtczq1{background-color:#212121;color:#fff;-webkit-transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:box-shadow 300ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;box-shadow:none;background-image:linear-gradient(rgba(255, 255, 255, 0), rgba(255, 255, 255, 0));display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-flex-direction:column;-ms-flex-direction:column;flex-direction:column;width:100%;box-sizing:border-box;-webkit-flex-shrink:0;-ms-flex-negative:0;flex-shrink:0;position:fixed;z-index:1100;top:0;left:auto;right:0;background-color:transparent;color:inherit;background-image:none;}@media print{.css-1gtczq1{position:absolute;}}</style><header class="MuiPaper-root MuiPaper-elevation MuiPaper-elevation0 MuiAppBar-root MuiAppBar-colorTransparent MuiAppBar-positionFixed mui-fixed css-1gtczq1"><style data-emotion="css 1wbqjz2">.css-1wbqjz2{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;padding:0px;}@media (min-width:600px){.css-1wbqjz2{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1wbqjz2{max-width:1536px;}}</style><div class="MuiContainer-root MuiContainer-maxWidthXl css-1wbqjz2"><style data-emotion="css y3hjov">.css-y3hjov{position:relative;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;padding-left:16px;padding-right:16px;min-height:56px;min-height:50px;max-height:50px;padding:0px;-webkit-flex:1;-ms-flex:1;flex:1;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:justify;-webkit-justify-content:space-between;justify-content:space-between;display:-webkit-box;display:-webkit-flex;display:-ms-flexbox;display:flex;-webkit-box-flex-wrap:nowrap;-webkit-flex-wrap:nowrap;-ms-flex-wrap:nowrap;flex-wrap:nowrap;}@media (min-width:600px){.css-y3hjov{padding-left:24px;padding-right:24px;}}@media (min-width:0px){@media (orientation: landscape){.css-y3hjov{min-height:48px;}}}@media (min-width:600px){.css-y3hjov{min-height:64px;}}</style><div class="MuiToolbar-root MuiToolbar-gutters MuiToolbar-regular css-y3hjov"><style data-emotion="css 1wxaqej">.css-1wxaqej{box-sizing:border-box;margin:0;-webkit-flex-direction:row;-ms-flex-direction:row;flex-direction:row;}</style><div class="MuiGrid-root MuiGrid-item css-1wxaqej"><style data-emotion="css 1x6trl3">.css-1x6trl3{font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1x6trl3:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1x6trl3:hover{background-color:transparent;}}.css-1x6trl3.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><style data-emotion="css 1o7udr7">.css-1o7udr7{display:-webkit-inline-box;display:-webkit-inline-flex;display:-ms-inline-flexbox;display:inline-flex;-webkit-align-items:center;-webkit-box-align:center;-ms-flex-align:center;align-items:center;-webkit-box-pack:center;-ms-flex-pack:center;-webkit-justify-content:center;justify-content:center;position:relative;box-sizing:border-box;-webkit-tap-highlight-color:transparent;background-color:transparent;outline:0;border:0;margin:0;border-radius:0;padding:0;cursor:pointer;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;vertical-align:middle;-moz-appearance:none;-webkit-appearance:none;-webkit-text-decoration:none;text-decoration:none;color:inherit;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:500;font-size:0.875rem;line-height:1.75;letter-spacing:0.02857em;text-transform:uppercase;min-width:64px;padding:6px 8px;border-radius:4px;-webkit-transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;transition:background-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,border-color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms,color 250ms cubic-bezier(0.4, 0, 0.2, 1) 0ms;color:#512da8;}.css-1o7udr7::-moz-focus-inner{border-style:none;}.css-1o7udr7.Mui-disabled{pointer-events:none;cursor:default;}@media print{.css-1o7udr7{-webkit-print-color-adjust:exact;color-adjust:exact;}}.css-1o7udr7:hover{-webkit-text-decoration:none;text-decoration:none;background-color:rgba(81, 45, 168, 0.08);}@media (hover: none){.css-1o7udr7:hover{background-color:transparent;}}.css-1o7udr7.Mui-disabled{color:rgba(255, 255, 255, 0.3);}</style><a class="MuiButtonBase-root MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium MuiButton-root MuiButton-text MuiButton-textPrimary MuiButton-sizeMedium MuiButton-textSizeMedium css-1o7udr7" tabindex="0" href="https://system-bridge.timmo.dev" target="_blank"><style data-emotion="css 1lcbag5">.css-1lcbag5{margin:0;font-family:"Roboto","Helvetica","Arial",sans-serif;font-weight:400;font-size:1.5625rem;line-height:1.235;letter-spacing:0.00735em;color:#fff;text-transform:none;-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none;}@media (min-width:600px){.css-1lcbag5{font-size:1.8219rem;}}@media (min-width:900px){.css-1lcbag5{font-size:2.0243rem;}}@media (min-width:1200px){.css-1lcbag5{font-size:2.0243rem;}}</style><div class="MuiTypography-root MuiTypography-h4 css-1lcbag5">System Bridge</div></a></div></div></div></header><style data-emotion="css 1pm3cft">.css-1pm3cft{height:144px;}</style><div class="MuiBox-root css-1pm3cft"></div><style data-emotion="css 1ekb41w">.css-1ekb41w{width:100%;margin-left:auto;box-sizing:border-box;margin-right:auto;display:block;padding-left:16px;padding-right:16px;}@media (min-width:600px){.css-1ekb41w{padding-left:24px;padding-right:24px;}}@media (min-width:1536px){.css-1ekb41w{max-width:1536px;}}</style><article class="MuiContainer-root MuiContainer-maxWidthXl css-1ekb41w"></article></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{}},"page":"/","query":{},"buildId":"iX_HmcWE_KZJ1V0jDuyN4","nextExport":true,"autoExport":true,"isFallback":false,"scriptLoader":[]}</script></body></html>
```

### Comparing `systembridgefrontend-3.7.0.dev1/systembridgefrontend.egg-info/SOURCES.txt` & `systembridgefrontend-3.8.0.dev5/systembridgefrontend.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,59 +5,60 @@
 systembridgefrontend.egg-info/PKG-INFO
 systembridgefrontend.egg-info/SOURCES.txt
 systembridgefrontend.egg-info/dependency_links.txt
 systembridgefrontend.egg-info/top_level.txt
 systembridgefrontend/out/404.html
 systembridgefrontend/out/favicon.svg
 systembridgefrontend/out/index.html
-systembridgefrontend/out/_next/static/7cCNYQwxkasei7aJF3BXn/_buildManifest.js
-systembridgefrontend/out/_next/static/7cCNYQwxkasei7aJF3BXn/_ssgManifest.js
-systembridgefrontend/out/_next/static/chunks/134-8b4cf5ad285047cd.js
-systembridgefrontend/out/_next/static/chunks/142-b511304dc754f6ca.js
-systembridgefrontend/out/_next/static/chunks/154-7942dd40332ec4bf.js
-systembridgefrontend/out/_next/static/chunks/171.64880094f51dbbf7.js
-systembridgefrontend/out/_next/static/chunks/29107295-8f8fd7e7e27aa6a2.js
-systembridgefrontend/out/_next/static/chunks/418-f078369e2fd2524e.js
-systembridgefrontend/out/_next/static/chunks/498-112306b4f8cd81ec.js
-systembridgefrontend/out/_next/static/chunks/633-a2b446f38d34df6a.js
-systembridgefrontend/out/_next/static/chunks/699-1a88a588882ce475.js
-systembridgefrontend/out/_next/static/chunks/731-eb947eaba8f94f26.js
-systembridgefrontend/out/_next/static/chunks/75fc9c18-058f7f136d59a7a6.js
-systembridgefrontend/out/_next/static/chunks/767-b6df483a2f96f15d.js
-systembridgefrontend/out/_next/static/chunks/826-e44464776abed9eb.js
-systembridgefrontend/out/_next/static/chunks/913-948b3bc7b49750f4.js
+systembridgefrontend/out/_next/static/chunks/134-be8afb194db80d1f.js
+systembridgefrontend/out/_next/static/chunks/142-6fa2d4be01c7dab9.js
+systembridgefrontend/out/_next/static/chunks/154-454aae7a1f6cc481.js
+systembridgefrontend/out/_next/static/chunks/171.cfc407cdf8574e41.js
+systembridgefrontend/out/_next/static/chunks/29107295-809b6f0b05884bf7.js
+systembridgefrontend/out/_next/static/chunks/361-70173883768cacf6.js
+systembridgefrontend/out/_next/static/chunks/498-c0ac8cca5a5197e4.js
+systembridgefrontend/out/_next/static/chunks/514-17895623628db944.js
+systembridgefrontend/out/_next/static/chunks/699-a015e8646ccfaf97.js
+systembridgefrontend/out/_next/static/chunks/713-76d25fee0de05077.js
+systembridgefrontend/out/_next/static/chunks/728-4d1eeb7a2f426351.js
+systembridgefrontend/out/_next/static/chunks/731-b6cafe94e88ed8c7.js
+systembridgefrontend/out/_next/static/chunks/75fc9c18-c0cb841eaf75495d.js
+systembridgefrontend/out/_next/static/chunks/767-21712ed9071ee20e.js
+systembridgefrontend/out/_next/static/chunks/826-25c5c840b401fbf5.js
 systembridgefrontend/out/_next/static/chunks/b2e984c5-f44d94ec783f59d4.js
-systembridgefrontend/out/_next/static/chunks/framework-305cb810cde7afac.js
-systembridgefrontend/out/_next/static/chunks/main-d5c9aef8f3ea3bae.js
+systembridgefrontend/out/_next/static/chunks/framework-7a7e500878b44665.js
+systembridgefrontend/out/_next/static/chunks/main-2ecf43899f8683c2.js
 systembridgefrontend/out/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerDailyMotion.da042b36db7662eb.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerFacebook.3663ffcf10139668.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerFilePlayer.812fbc47cf3ccebc.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerKaltura.46641a0f37607223.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerMixcloud.258ac8431338b78a.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerPreview.9b535aa9cbcb0a91.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerSoundCloud.60e72fefd71eeb25.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerStreamable.c374322fbd4a05d5.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerTwitch.52035ec5fd363953.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerVidyard.8c3ec4a7a5b4aac4.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerVimeo.5a5700a7f86e58a2.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerWistia.29aa97668baf75ea.js
 systembridgefrontend/out/_next/static/chunks/reactPlayerYouTube.77a6d75e3f5e95ef.js
-systembridgefrontend/out/_next/static/chunks/webpack-29bb9d3475e20ac7.js
-systembridgefrontend/out/_next/static/chunks/pages/_app-d13b8fcca9a8fc8a.js
+systembridgefrontend/out/_next/static/chunks/webpack-8c974454c1c3cd10.js
+systembridgefrontend/out/_next/static/chunks/pages/_app-4638cf4f01fc5510.js
 systembridgefrontend/out/_next/static/chunks/pages/_error-54de1933a164a1ff.js
 systembridgefrontend/out/_next/static/chunks/pages/index-f934b9a030f633a0.js
-systembridgefrontend/out/_next/static/chunks/pages/app/data-a3eeebdc39c5f892.js
-systembridgefrontend/out/_next/static/chunks/pages/app/notification-0384bbf9e77dbfb4.js
-systembridgefrontend/out/_next/static/chunks/pages/app/settings-0b5df1a27de4507f.js
-systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-ea5036b8dd1a507b.js
-systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-7e45aefe6a4d48af.js
-systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-8b29e9945ddce62c.js
-systembridgefrontend/out/_next/static/chunks/pages/app/player/video-b8b2ae3418f95cef.js
+systembridgefrontend/out/_next/static/chunks/pages/app/data-59d72c465167efc4.js
+systembridgefrontend/out/_next/static/chunks/pages/app/notification-416e0ab0e8597db3.js
+systembridgefrontend/out/_next/static/chunks/pages/app/settings-c2e844bc6170d7a5.js
+systembridgefrontend/out/_next/static/chunks/pages/app/bridges/openon-57051d0ee30b9efa.js
+systembridgefrontend/out/_next/static/chunks/pages/app/bridges/setup-d4f904aedaf93672.js
+systembridgefrontend/out/_next/static/chunks/pages/app/player/audio-3826169d9ca46804.js
+systembridgefrontend/out/_next/static/chunks/pages/app/player/video-9c7e9646d273d6aa.js
 systembridgefrontend/out/_next/static/css/7c971015b368f9b1.css
+systembridgefrontend/out/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_buildManifest.js
+systembridgefrontend/out/_next/static/iX_HmcWE_KZJ1V0jDuyN4/_ssgManifest.js
 systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.19f93502.woff
 systembridgefrontend/out/_next/static/media/roboto-cyrillic-400-normal.2d9c9d60.woff2
 systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.02e18372.woff
 systembridgefrontend/out/_next/static/media/roboto-cyrillic-ext-400-normal.d7827ae3.woff2
 systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.63e6dc18.woff2
 systembridgefrontend/out/_next/static/media/roboto-greek-400-normal.e3b5876b.woff
 systembridgefrontend/out/_next/static/media/roboto-greek-ext-400-normal.2b547ded.woff2
```

