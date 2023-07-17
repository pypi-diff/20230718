# Comparing `tmp/jupysql_plugin-0.1.6.tar.gz` & `tmp/jupysql_plugin-0.1.7.tar.gz`

## Comparing `jupysql_plugin-0.1.6.tar` & `jupysql_plugin-0.1.7.tar`

### file list

```diff
@@ -1,83 +1,71 @@
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/CHANGELOG.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/babel.config.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/environment.yml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jest.config.js
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/noxfile.py
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/package.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/setup.cfg
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/setup.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/tsconfig.json
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/doc/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/_version.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/_widgets.py
--rw-r--r--   0        0        0    21640 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/build_log.json
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/package.json
--rw-r--r--   0        0        0    93905 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/lib_index_js.14d44517f1c252c0cba4.js
--rw-r--r--   0        0        0   105089 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/lib_index_js.14d44517f1c252c0cba4.js.map
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_memoize_dist_emotion-m-27ec560.b32b1b0849b462d4402e.js
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_memoize_dist_emotion-m-27ec560.b32b1b0849b462d4402e.js.map
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_memoize_dist_emotion-m-27ec561.2d54dcba41685bb662c2.js
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/node_modules_babel_runtime_helpers_esm_extends_js-node_modules_emotion_memoize_dist_emotion-m-27ec561.2d54dcba41685bb662c2.js.map
--rw-r--r--   0        0        0    42299 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/remoteEntry.80d9644794491b9cb99c.js
--rw-r--r--   0        0        0    41233 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/remoteEntry.80d9644794491b9cb99c.js.map
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/style.js
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/style_index_js.d2d1cdf7cc4936cb793a.js
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/style_index_js.d2d1cdf7cc4936cb793a.js.map
--rw-r--r--   0        0        0   298220 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.96fcc0d596d862afebe5.js
--rw-r--r--   0        0        0   389840 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_bootstrap_dist_js_bootstrap_esm_js.96fcc0d596d862afebe5.js.map
--rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.4552f03d4f09d840178e.js
--rw-r--r--   0        0        0    13790 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.4552f03d4f09d840178e.js.map
--rw-r--r--   0        0        0    80087 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_emotion_cache_dist_emotion-cache_browser_esm_js-node_modules_react-is_index_js.8c54e7818c50a340e116.js
--rw-r--r--   0        0        0    74398 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_emotion_cache_dist_emotion-cache_browser_esm_js-node_modules_react-is_index_js.8c54e7818c50a340e116.js.map
--rw-r--r--   0        0        0   310637 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_emotion_memoize_dist_emotion-memoize_esm_js-node_modules_mui_material_ut-b38a82.5815c11c9daf7417d735.js
--rw-r--r--   0        0        0   260448 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_emotion_memoize_dist_emotion-memoize_esm_js-node_modules_mui_material_ut-b38a82.5815c11c9daf7417d735.js.map
--rw-r--r--   0        0        0    35993 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js.8760b7f6f1a9e478e9d2.js
--rw-r--r--   0        0        0    33847 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_emotion_react_dist_emotion-react_browser_esm_js.8760b7f6f1a9e478e9d2.js.map
--rw-r--r--   0        0        0    20137 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_emotion_serialize_dist_emotion-serialize_browser_esm_js-node_modules_emo-cbc221.8bece0dcdce335387905.js
--rw-r--r--   0        0        0    19960 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_emotion_serialize_dist_emotion-serialize_browser_esm_js-node_modules_emo-cbc221.8bece0dcdce335387905.js.map
--rw-r--r--   0        0        0    18639 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js.e1295841c98f873355ce.js
--rw-r--r--   0        0        0    14893 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_emotion_styled_dist_emotion-styled_browser_esm_js.e1295841c98f873355ce.js.map
--rw-r--r--   0        0        0   915898 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_mui_icons-material_CloudQueue_js-node_modules_css-loader_dist_runtime_ge-e0889f.9559d46693239cb52684.js
--rw-r--r--   0        0        0  1131567 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_mui_icons-material_CloudQueue_js-node_modules_css-loader_dist_runtime_ge-e0889f.9559d46693239cb52684.js.map
--rw-r--r--   0        0        0  2857874 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_mui_material_index_js.020b86048099472a1075.js
--rw-r--r--   0        0        0  2068653 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_mui_material_index_js.020b86048099472a1075.js.map
--rw-r--r--   0        0        0   449129 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.9c76b210f008568ff588.js
--rw-r--r--   0        0        0   725067 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_sql-formatter_lib_index_js.9c76b210f008568ff588.js.map
--rw-r--r--   0        0        0   272574 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_underscore_modules_index-all_js.8220176670f4f625110f.js
--rw-r--r--   0        0        0   120157 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/labextension/static/vendors-node_modules_underscore_modules_index-all_js.8220176670f4f625110f.js.map
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/server_handlers/dashboard.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/widgets/__init__.py
--rw-r--r--   0        0        0    10534 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupysql_plugin/widgets/connector_widget.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupyter-config/jupyter_notebook_config.d/jupysql_plugin.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/jupyter-config/jupyter_server_config.d/jupysql_plugin.json
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/comm.ts
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/connector.ts
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/customconnector.ts
--rw-r--r--   0        0        0    10369 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/dialog.tsx
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/extension.ts
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/formatter.ts
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/index-widgets.ts
--rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/index.ts
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/keywords.json
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/version.ts
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/__tests__/jupysql_plugin.spec.ts
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/const/env.ts
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/utils/util.ts
--rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/widgets/connector.ts
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/widgets/form.ts
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/src/widgets/table.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/style/base.css
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/style/connector.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/style/index.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/style/widget.css
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/style/icons/add_primary.svg
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/style/icons/delete_outline_black.svg
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/README.md
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/CHANGELOG.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/babel.config.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/environment.yml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jest.config.js
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/noxfile.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/package.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/setup.cfg
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/setup.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/tsconfig.json
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/doc/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/_version.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/_widgets.py
+-rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/package.json
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/122.83febd31f97f409ed32e.js
+-rw-r--r--   0        0        0   448079 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js.LICENSE.txt
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/171.256ff36dbd88e97f7d85.js
+-rw-r--r--   0        0        0    32377 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/238.248c93b1dc2fa4a4015a.js
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/282.1bb9d755cf1f2c786d16.js
+-rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js.LICENSE.txt
+-rw-r--r--   0        0        0    11027 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/378.d4abe61f25a998d75e66.js
+-rw-r--r--   0        0        0    39339 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/40.4f257c905f8cbcacb158.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/40.4f257c905f8cbcacb158.js.LICENSE.txt
+-rw-r--r--   0        0        0    60929 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/520.482c287db47780739825.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/520.482c287db47780739825.js.LICENSE.txt
+-rw-r--r--   0        0        0   237389 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/646.2440cc17aba449886588.js
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/747.233d2b03fe10fa309835.js
+-rw-r--r--   0        0        0    22082 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/794.a07de7512354fbf79bee.js
+-rw-r--r--   0        0        0    23542 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/804.d8cbf6a18594a5e5e734.js
+-rw-r--r--   0        0        0     9732 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/846.1e01de8e428bb8d890c8.js
+-rw-r--r--   0        0        0   228074 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/906.0dfaf4363c1e58ef89b0.js
+-rw-r--r--   0        0        0    10014 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/remoteEntry.e80d3b8b00f5114eb1bb.js
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/style.js
+-rw-r--r--   0        0        0    42216 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/server_handlers/dashboard.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/widgets/__init__.py
+-rw-r--r--   0        0        0    10534 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupysql_plugin/widgets/connector_widget.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupyter-config/jupyter_notebook_config.d/jupysql_plugin.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/jupyter-config/jupyter_server_config.d/jupysql_plugin.json
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/comm.ts
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/connector.ts
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/customconnector.ts
+-rw-r--r--   0        0        0    10369 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/dialog.tsx
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/extension.ts
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/formatter.ts
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/index-widgets.ts
+-rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/index.ts
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/keywords.json
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/version.ts
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/__tests__/jupysql_plugin.spec.ts
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/const/env.ts
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/utils/util.ts
+-rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/widgets/connector.ts
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/widgets/form.ts
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/src/widgets/table.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/base.css
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/connector.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/index.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/widget.css
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/icons/add_primary.svg
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/style/icons/delete_outline_black.svg
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/README.md
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.7/PKG-INFO
```

### Comparing `jupysql_plugin-0.1.6/RELEASE.md` & `jupysql_plugin-0.1.7/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/jest.config.js` & `jupysql_plugin-0.1.7/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/noxfile.py` & `jupysql_plugin-0.1.7/noxfile.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/package.json` & `jupysql_plugin-0.1.7/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'0.1.7'"}*

```diff
@@ -117,15 +117,15 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.6",
+    "version": "0.1.7",
     "workspaces": {
         "packages": [
             "jupysql_plugin",
             "ui-tests"
         ]
     }
 }
```

### Comparing `jupysql_plugin-0.1.6/tsconfig.json` & `jupysql_plugin-0.1.7/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/doc/README.md` & `jupysql_plugin-0.1.7/doc/README.md`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/jupysql_plugin/__init__.py` & `jupysql_plugin-0.1.7/jupysql_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/jupysql_plugin/_widgets.py` & `jupysql_plugin-0.1.7/jupysql_plugin/_widgets.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/jupysql_plugin/labextension/package.json` & `jupysql_plugin-0.1.7/jupysql_plugin/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9778079710144927%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e80d3b8b00f5114eb1bb.js'}}",*

 * * "'version'": "'0.1.7'"}*

```diff
@@ -60,15 +60,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/ploomber/jupysql-plugin.git",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.80d9644794491b9cb99c.js",
+            "load": "static/remoteEntry.e80d3b8b00f5114eb1bb.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupysql_plugin/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
@@ -122,15 +122,15 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.5",
+    "version": "0.1.7",
     "workspaces": {
         "packages": [
             "jupysql_plugin",
             "ui-tests"
         ]
     }
 }
```

### Comparing `jupysql_plugin-0.1.6/jupysql_plugin/server_handlers/dashboard.py` & `jupysql_plugin-0.1.7/jupysql_plugin/server_handlers/dashboard.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/jupysql_plugin/widgets/connector_widget.py` & `jupysql_plugin-0.1.7/jupysql_plugin/widgets/connector_widget.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/src/comm.ts` & `jupysql_plugin-0.1.7/src/comm.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/src/connector.ts` & `jupysql_plugin-0.1.7/src/connector.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/src/customconnector.ts` & `jupysql_plugin-0.1.7/src/customconnector.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/src/dialog.tsx` & `jupysql_plugin-0.1.7/src/dialog.tsx`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/src/formatter.ts` & `jupysql_plugin-0.1.7/src/formatter.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/src/index.ts` & `jupysql_plugin-0.1.7/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/src/keywords.json` & `jupysql_plugin-0.1.7/src/keywords.json`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/src/utils/util.ts` & `jupysql_plugin-0.1.7/src/utils/util.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/src/widgets/connector.ts` & `jupysql_plugin-0.1.7/src/widgets/connector.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/src/widgets/form.ts` & `jupysql_plugin-0.1.7/src/widgets/form.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/src/widgets/table.ts` & `jupysql_plugin-0.1.7/src/widgets/table.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/style/connector.css` & `jupysql_plugin-0.1.7/style/connector.css`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/.gitignore` & `jupysql_plugin-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/LICENSE` & `jupysql_plugin-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/README.md` & `jupysql_plugin-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/pyproject.toml` & `jupysql_plugin-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.6/PKG-INFO` & `jupysql_plugin-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql-plugin
-Version: 0.1.6
+Version: 0.1.7
 Summary: Jupyterlab extension for JupySQL
 Project-URL: Homepage, https://github.com/ploomber/jupysql-plugin.git
 Project-URL: Bug Tracker, https://github.com/ploomber/jupysql-plugin.git/issues
 Project-URL: Repository, https://github.com/ploomber/jupysql-plugin.git.git
 Author-email: Ploomber <contact@ploomber.io>
 License: BSD 3-Clause License
```

