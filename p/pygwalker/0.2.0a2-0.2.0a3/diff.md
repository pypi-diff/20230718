# Comparing `tmp/pygwalker-0.2.0a2.tar.gz` & `tmp/pygwalker-0.2.0a3.tar.gz`

## Comparing `pygwalker-0.2.0a2.tar` & `pygwalker-0.2.0a3.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/.gitignore
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/index.html
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/package.json
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/postcss.config.js
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/tailwind.config.js
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/tsconfig.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/vite.config.ts
--rw-r--r--   0        0        0   133942 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/yarn.lock
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/index.css
--rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/index.tsx
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/components/defaultTab.tsx
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/components/loadingIcon.tsx
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/components/modal.tsx
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/components/options.tsx
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/components/button/base.ts
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/components/button/default.tsx
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/components/button/primary.tsx
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/components/codeExportModal/index.tsx
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/components/codeExportModal/saveConfigButton.tsx
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/components/initModal/index.tsx
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/dataSource/index.ts
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/interfaces/index.ts
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/notify/index.tsx
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/store/common.ts
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/store/communication.ts
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/tools/exportTool.tsx
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/tools/loginTool.tsx
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/tools/saveTool.tsx
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/utils/communication.ts
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/utils/graphicWalkerParser.ts
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/utils/save.ts
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/utils/screenshot.ts
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/app/src/utils/userConfig.ts
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/_constants.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/_typing.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/api/__init__.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/api/gwalker.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/api/html.py
--rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/api/pygwalker.py
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/api/walker.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/communications/__init__.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/communications/base.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/communications/hacker_comm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/data_parsers/__init__.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/data_parsers/base.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/data_parsers/modin_parser.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/data_parsers/pandas_parser.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/data_parsers/polars_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/services/__init__.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/services/check_update.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/services/data_parsers.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/services/fname_encodings.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/services/format_invoke_walk_code.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/services/global_var.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/services/preview_image.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/services/render.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/services/spec.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/services/tip_tools.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/services/upload_data.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/.gitignore
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/index.html
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/preview.html
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/pygwalker_iframe.html
--rw-r--r--   0        0        0   358324 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/tailwind.js
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/walk.js
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/index.d.ts
--rw-r--r--   0        0        0  1935594 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/pygwalker-app.iife.js
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/components/defaultTab.d.ts
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/components/loadingIcon.d.ts
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/components/modal.d.ts
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/components/options.d.ts
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/components/button/base.d.ts
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/components/button/default.d.ts
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/components/button/primary.d.ts
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/components/codeExportModal/index.d.ts
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/components/codeExportModal/saveConfigButton.d.ts
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/components/initModal/index.d.ts
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/dataSource/index.d.ts
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/interfaces/index.d.ts
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/notify/index.d.ts
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/store/common.d.ts
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/store/communication.d.ts
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/tools/exportTool.d.ts
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/tools/loginTool.d.ts
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/tools/saveTool.d.ts
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/utils/communication.d.ts
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/utils/graphicWalkerParser.d.ts
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/utils/save.d.ts
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/utils/screenshot.d.ts
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/templates/dist/utils/userConfig.d.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/utils/__init__.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/utils/display.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/utils/encode.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker/utils/randoms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker_utils/__init__.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker_utils/__main__.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker_utils/config.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pygwalker_utils/defaults.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/scripts/__init__.py
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/scripts/compile.sh
--rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/scripts/develop.sh
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/scripts/test-init.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/scripts/test-init.sh
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/.gitignore
--rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/LICENSE
--rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/README.md
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0    14558 2020-02-02 00:00:00.000000 pygwalker-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/.gitignore
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/index.html
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/package.json
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/postcss.config.js
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/tailwind.config.js
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/tsconfig.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/vite.config.ts
+-rw-r--r--   0        0        0   133942 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/yarn.lock
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/index.css
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/index.tsx
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/defaultTab.tsx
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/loadingIcon.tsx
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/modal.tsx
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/options.tsx
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/button/base.ts
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/button/default.tsx
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/button/primary.tsx
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/codeExportModal/index.tsx
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/codeExportModal/saveConfigButton.tsx
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/components/initModal/index.tsx
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/dataSource/index.ts
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/interfaces/index.ts
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/notify/index.tsx
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/store/common.ts
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/store/communication.ts
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/tools/exportTool.tsx
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/tools/loginTool.tsx
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/tools/saveTool.tsx
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/utils/communication.ts
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/utils/graphicWalkerParser.ts
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/utils/save.ts
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/utils/screenshot.ts
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/app/src/utils/userConfig.ts
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/_constants.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/_typing.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/api/__init__.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/api/gwalker.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/api/html.py
+-rw-r--r--   0        0        0     9214 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/api/pygwalker.py
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/api/walker.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/communications/__init__.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/communications/base.py
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/communications/hacker_comm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/data_parsers/__init__.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/data_parsers/base.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/data_parsers/modin_parser.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/data_parsers/pandas_parser.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/data_parsers/polars_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/__init__.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/check_update.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/data_parsers.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/fname_encodings.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/format_invoke_walk_code.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/global_var.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/preview_image.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/render.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/spec.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/tip_tools.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/services/upload_data.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/.gitignore
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/index.html
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/preview.html
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/preview_list.html
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/pygwalker_iframe.html
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/walk.js
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/index.d.ts
+-rw-r--r--   0        0        0  1935613 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/pygwalker-app.iife.js
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/defaultTab.d.ts
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/loadingIcon.d.ts
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/modal.d.ts
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/options.d.ts
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/button/base.d.ts
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/button/default.d.ts
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/button/primary.d.ts
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/codeExportModal/index.d.ts
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/codeExportModal/saveConfigButton.d.ts
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/components/initModal/index.d.ts
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/dataSource/index.d.ts
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/interfaces/index.d.ts
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/notify/index.d.ts
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/store/common.d.ts
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/store/communication.d.ts
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/tools/exportTool.d.ts
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/tools/loginTool.d.ts
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/tools/saveTool.d.ts
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/utils/communication.d.ts
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/utils/graphicWalkerParser.d.ts
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/utils/save.d.ts
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/utils/screenshot.d.ts
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/templates/dist/utils/userConfig.d.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/utils/__init__.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/utils/display.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/utils/encode.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker/utils/randoms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker_utils/__init__.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker_utils/__main__.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker_utils/config.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pygwalker_utils/defaults.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/scripts/__init__.py
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/scripts/compile.sh
+-rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/scripts/develop.sh
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/scripts/test-init.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/scripts/test-init.sh
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/.gitignore
+-rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/LICENSE
+-rw-r--r--   0        0        0    13064 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/README.md
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/pyproject.toml
+-rw-r--r--   0        0        0    14582 2020-02-02 00:00:00.000000 pygwalker-0.2.0a3/PKG-INFO
```

### Comparing `pygwalker-0.2.0a2/app/package.json` & `pygwalker-0.2.0a3/app/package.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/tsconfig.json` & `pygwalker-0.2.0a3/app/tsconfig.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/vite.config.ts` & `pygwalker-0.2.0a3/app/vite.config.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/yarn.lock` & `pygwalker-0.2.0a3/app/yarn.lock`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/index.tsx` & `pygwalker-0.2.0a3/app/src/index.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import { getLoginTool } from './tools/loginTool';
 import { domToPng } from "./utils/screenshot"
 
 // @ts-ignore
 import style from './index.css?inline'
 
 
-const initChart = async (gwRef: React.MutableRefObject<IGWHandler | null>, total: number) => {
+const initChart = async (gwRef: React.MutableRefObject<IGWHandler | null>, total: number, gid: string) => {
     if (total !== 0) {
         commonStore.initModalOpen = true;
         commonStore.setInitModalInfo({
             title: "Recover Charts",
             curIndex: 0,
             total: total,
         });
@@ -41,14 +41,15 @@
             const singleChart = await domToPng(chart.data.container()!);
             await communicationStore.comm?.sendMsg("save_chart", {...chart.data, singleChart});
             commonStore.setInitModalInfo({
                 title: "Recover Charts",
                 curIndex: chart.index + 1,
                 total: chart.total,
             });
+            hidePreview(gid);
         }
     }
     commonStore.initModalOpen = false;
 }
 
 /** App does not consider props.storeRef */
 const App: React.FC<IAppProps> = observer((propsIn) => {
@@ -93,15 +94,15 @@
           name: 'Dataset',
           rawFields: rawFields,
           dataSource: data,
         } as IDataSetInfo);
         storeRef?.current?.commonStore?.commitTempDS();
       }
       if (!props.needLoadDatas && props.env === "jupyter_widgets") {
-        setTimeout(() => { initChart(gwRef, specList.length) }, 0);
+        setTimeout(() => { initChart(gwRef, specList.length, props.id) }, 0);
       }
   }, [storeRef])
 
   useEffect(() => {
     setData({ data: dataSource, rawFields, visSpec });
   }, [dataSource, rawFields, visSpec]);
 
@@ -112,15 +113,15 @@
   const updateDataSource = useCallback(async () => {
 
     // TODO: don't always update visSpec when appending data
     await loadDataSource(dataSourceProps).then(ds => {
       const data = ds;
       setData({ data, rawFields, visSpec });
       if (props.env === "jupyter_widgets") {
-        initChart(gwRef, specList.length);
+        initChart(gwRef, specList.length, props.id);
       } else {
         commonStore.setInitModalOpen(false);
       }
     }).catch(e => {
       console.error('Load DataSource Error', e);
     });
   }, [dataSource, dataSourceProps, rawFields, visSpec, setData]);
```

### Comparing `pygwalker-0.2.0a2/app/src/components/defaultTab.tsx` & `pygwalker-0.2.0a3/app/src/components/defaultTab.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/components/loadingIcon.tsx` & `pygwalker-0.2.0a3/app/src/components/loadingIcon.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/components/modal.tsx` & `pygwalker-0.2.0a3/app/src/components/modal.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/components/options.tsx` & `pygwalker-0.2.0a3/app/src/components/options.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/components/button/default.tsx` & `pygwalker-0.2.0a3/app/src/components/button/default.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/components/button/primary.tsx` & `pygwalker-0.2.0a3/app/src/components/button/primary.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/components/codeExportModal/index.tsx` & `pygwalker-0.2.0a3/app/src/components/codeExportModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/components/codeExportModal/saveConfigButton.tsx` & `pygwalker-0.2.0a3/app/src/components/codeExportModal/saveConfigButton.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/components/initModal/index.tsx` & `pygwalker-0.2.0a3/app/src/components/initModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/dataSource/index.ts` & `pygwalker-0.2.0a3/app/src/dataSource/index.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/interfaces/index.ts` & `pygwalker-0.2.0a3/app/src/interfaces/index.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/notify/index.tsx` & `pygwalker-0.2.0a3/app/src/notify/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/store/common.ts` & `pygwalker-0.2.0a3/app/src/store/common.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/tools/exportTool.tsx` & `pygwalker-0.2.0a3/app/src/tools/exportTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/tools/loginTool.tsx` & `pygwalker-0.2.0a3/app/src/tools/loginTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/tools/saveTool.tsx` & `pygwalker-0.2.0a3/app/src/tools/saveTool.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/utils/communication.ts` & `pygwalker-0.2.0a3/app/src/utils/communication.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/utils/graphicWalkerParser.ts` & `pygwalker-0.2.0a3/app/src/utils/graphicWalkerParser.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/app/src/utils/save.ts` & `pygwalker-0.2.0a3/app/src/utils/save.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/__init__.py` & `pygwalker-0.2.0a3/pygwalker/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 from pygwalker.utils.randoms import rand_str as __rand_str
 from pygwalker_utils.config import get_config as __get_config
 
-__version__ = "0.2.0a2"
+__version__ = "0.2.0a3"
 __hash__ = __rand_str()
 
 from pygwalker.api.walker import walk
 from pygwalker.api.gwalker import GWalker
 from pygwalker.api.html import to_html
 from pygwalker.data_parsers.base import FieldSpec
```

### Comparing `pygwalker-0.2.0a2/pygwalker/_typing.py` & `pygwalker-0.2.0a3/pygwalker/_typing.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/api/gwalker.py` & `pygwalker-0.2.0a3/pygwalker/api/gwalker.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/api/html.py` & `pygwalker-0.2.0a3/pygwalker/api/html.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/api/pygwalker.py` & `pygwalker-0.2.0a3/pygwalker/api/pygwalker.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pygwalker.services.global_var import GlobalVarManager
 from pygwalker.services.tip_tools import TipOnStartTool
 from pygwalker.services.render import (
     render_gwalker_html,
     render_gwalker_iframe,
     get_max_limited_datas
 )
-from pygwalker.services.preview_image import PreviewImageTool, render_preview_html
+from pygwalker.services.preview_image import PreviewImageTool, render_preview_html, ChartData
 from pygwalker.services.upload_data import (
     BatchUploadDatasToolOnWidgets,
     BatchUploadDatasToolOnJupyter
 )
 from pygwalker.services.spec import get_spec_json
 from pygwalker.communications.hacker_comm import HackerCommunication, BaseCommunication
 from pygwalker._constants import JUPYTER_BYTE_LIMIT, JUPYTER_WIDGETS_BYTE_LIMIT
@@ -55,15 +55,18 @@
         self.dark = dark
         self.data_source_id = rand_str()
         self.other_props = kwargs
         self.vis_spec, self.spec_type = get_spec_json(spec)
         self.tunnel_id = "tunnel!"
         self.show_cloud_tool = show_cloud_tool
         self.use_preview = use_preview
-        self._chart_map = {}
+        self._chart_map = self._init_chart_map()
+
+    def _init_chart_map(self) -> Dict[str, ChartData]:
+        return {}
 
     def to_html(self) -> str:
         props = self._get_props()
         return self._get_render_iframe(props)
 
     def display_on_streamlit(self):
         display_on_streamlit(self.to_html())
@@ -122,17 +125,23 @@
         self._init_callback(comm, preview_tool)
 
         display_html(html_widgets)
         preview_tool.init_display()
 
     @property
     def chart_list(self) -> List[str]:
+        """
+        Get the list of saved charts.
+        """
         return list(self._chart_map.keys())
 
     def save_chart_to_file(self, chart_name: str, path: str, save_type: Literal["html", "png"] = "png"):
+        """
+        Save the chart to a file.
+        """
         if save_type == "html":
             content = self.export_chart_html(chart_name)
             write_mode = "w"
             encoding = "utf-8"
         elif save_type == "png":
             content = self.export_chart_png(chart_name)
             write_mode = "wb"
@@ -140,49 +149,49 @@
         else:
             raise ValueError(f"save_type must be html or png, but got {save_type}")
 
         with open(path, write_mode, encoding=encoding) as f:
             f.write(content)
 
     def export_chart_html(self, chart_name: str) -> str:
+        """
+        Export the chart as a html string.
+        """
         chart_data = self._get_chart_by_name(chart_name)
 
         return render_preview_html(
             chart_data,
             f"{self.gid}-{chart_name}",
             custom_title="",
             desc=""
         )
 
     def export_chart_png(self, chart_name: str) -> bytes:
+        """
+        Export the chart as a png bytes.
+        """
         chart_data = self._get_chart_by_name(chart_name)
 
-        with urllib.request.urlopen(chart_data["singleChart"]) as png_string:
+        with urllib.request.urlopen(chart_data.single_chart) as png_string:
             return png_string.read()
 
     def display_chart(self, chart_name: str, *, title: Optional[str] = None, desc: str = ""):
+        """
+        Display the chart in the notebook.
+        """
         chart_data = self._get_chart_by_name(chart_name)
         html = render_preview_html(
             chart_data,
             f"{self.gid}-{chart_name}",
             custom_title=title,
             desc=desc
         )
         display_html(html)
 
-    def _get_chart_by_name(self, chart_name: str) -> Dict[str, Any]:
-        """
-        datas: {
-            "charts": {"rowIndex": int, ""colIndex": int, "data": str, "height": int, "width": int, "canvasHeight": int, "canvasWidth": int},
-            "singleChart": str,
-            "nRows": int,
-            "nCols": int,
-            "title": str
-        }
-        """
+    def _get_chart_by_name(self, chart_name: str) -> ChartData:
         if chart_name not in self._chart_map:
             raise ValueError(f"chart_name: {chart_name} not found, please confirm whether to save")
         return self._chart_map[chart_name]
 
     def _init_callback(self, comm: BaseCommunication, preview_tool: PreviewImageTool):
         upload_tool = BatchUploadDatasToolOnWidgets(comm)
 
@@ -199,17 +208,18 @@
             return {"visSpec": vis_spec}
 
         def update_spec(data: Dict[str, Any]):
             with open(self.spec, "w", encoding="utf-8") as f:
                 f.write(data["content"])
 
         def save_chart_endpoint(data: Dict[str, Any]):
-            self._chart_map[data["title"]] = data
+            chart_data = ChartData.parse_obj(data)
+            self._chart_map[data["title"]] = chart_data
             if self.use_preview:
-                preview_tool.render(data)
+                preview_tool.render(self._chart_map)
 
         comm.register("request_data", reuqest_data_callback)
         comm.register("get_latest_vis_spec", get_latest_vis_spec)
         comm.register("update_vis_spec", update_spec)
         comm.register("save_chart", save_chart_endpoint)
 
     def _get_props(
```

### Comparing `pygwalker-0.2.0a2/pygwalker/api/walker.py` & `pygwalker-0.2.0a3/pygwalker/api/walker.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/communications/base.py` & `pygwalker-0.2.0a3/pygwalker/communications/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/communications/hacker_comm.py` & `pygwalker-0.2.0a3/pygwalker/communications/hacker_comm.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/data_parsers/base.py` & `pygwalker-0.2.0a3/pygwalker/data_parsers/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/data_parsers/modin_parser.py` & `pygwalker-0.2.0a3/pygwalker/data_parsers/modin_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/data_parsers/pandas_parser.py` & `pygwalker-0.2.0a3/pygwalker/data_parsers/pandas_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/data_parsers/polars_parser.py` & `pygwalker-0.2.0a3/pygwalker/data_parsers/polars_parser.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/services/check_update.py` & `pygwalker-0.2.0a3/pygwalker/services/check_update.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/services/data_parsers.py` & `pygwalker-0.2.0a3/pygwalker/services/data_parsers.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/services/format_invoke_walk_code.py` & `pygwalker-0.2.0a3/pygwalker/services/format_invoke_walk_code.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/services/render.py` & `pygwalker-0.2.0a3/pygwalker/services/render.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/services/spec.py` & `pygwalker-0.2.0a3/pygwalker/services/spec.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/services/tip_tools.py` & `pygwalker-0.2.0a3/pygwalker/services/tip_tools.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/services/upload_data.py` & `pygwalker-0.2.0a3/pygwalker/services/upload_data.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/templates/preview.html` & `pygwalker-0.2.0a3/pygwalker/templates/preview.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,60 @@
-00000000: 3c68 746d 6c3e 0a3c 626f 6479 3e0a 2020  <html>.<body>.  
-00000010: 2020 3c64 6976 2069 643d 227b 7b20 6469    <div id="{{ di
-00000020: 765f 6964 207d 7d22 2073 7479 6c65 3d22  v_id }}" style="
-00000030: 7769 6474 683a 2031 3030 253b 206d 6178  width: 100%; max
-00000040: 2d68 6569 6768 743a 2036 3030 7078 3b22  -height: 600px;"
-00000050: 3e0a 2020 2020 2020 2020 7b25 2069 6620  >.        {% if 
-00000060: 7469 746c 6520 213d 2027 2720 257d 0a20  title != '' %}. 
-00000070: 2020 2020 2020 203c 6831 2073 7479 6c65         <h1 style
-00000080: 3d22 6d61 7267 696e 2d74 6f70 3a20 3172  ="margin-top: 1r
-00000090: 656d 3b20 636f 6c6f 723a 2023 3333 333b  em; color: #333;
-000000a0: 2066 6f6e 742d 7369 7a65 3a20 312e 3172   font-size: 1.1r
-000000b0: 656d 3b20 6d61 7267 696e 2d62 6f74 746f  em; margin-botto
-000000c0: 6d3a 2030 2e35 7265 6d3b 2070 6164 6469  m: 0.5rem; paddi
-000000d0: 6e67 2d69 6e6c 696e 652d 7374 6172 743a  ng-inline-start:
-000000e0: 2031 7265 6d3b 223e 7b7b 2074 6974 6c65   1rem;">{{ title
-000000f0: 207d 7d3c 2f68 313e 0a20 2020 2020 2020   }}</h1>.       
-00000100: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-00000110: 2020 2020 203c 7020 7374 796c 653d 2263       <p style="c
-00000120: 6f6c 6f72 3a20 2336 3636 3b20 666f 6e74  olor: #666; font
-00000130: 2d77 6569 6768 743a 2033 3030 3b20 7061  -weight: 300; pa
-00000140: 6464 696e 672d 696e 6c69 6e65 2d73 7461  dding-inline-sta
-00000150: 7274 3a20 3172 656d 3b22 3e7b 7b20 6465  rt: 1rem;">{{ de
-00000160: 7363 207d 7d3c 2f70 3e0a 2020 2020 2020  sc }}</p>.      
-00000170: 2020 3c21 2d2d 203c 703e 556e 6465 7220    <!-- <p>Under 
-00000180: 6365 7274 6169 6e20 4a75 7079 7465 7220  certain Jupyter 
-00000190: 656e 7669 726f 6e6d 656e 7473 2c20 6166  environments, af
-000001a0: 7465 7220 6c61 756e 6368 696e 6720 7079  ter launching py
-000001b0: 6777 616c 6b65 722c 2074 6865 2070 7265  gwalker, the pre
-000001c0: 7669 6577 206d 6179 206e 6f74 2061 7574  view may not aut
-000001d0: 6f6d 6174 6963 616c 6c79 2068 6964 652e  omatically hide.
-000001e0: 2059 6f75 2063 616e 206d 616e 7561 6c6c   You can manuall
-000001f0: 7920 636c 6963 6b20 7468 6520 6275 7474  y click the butt
-00000200: 6f6e 2074 6f20 6869 6465 2069 742e 3c2f  on to hide it.</
-00000210: 703e 202d 2d3e 0a20 2020 2020 2020 203c  p> -->.        <
-00000220: 6469 7620 636c 6173 733d 226d 6169 6e2d  div class="main-
-00000230: 626f 7822 3e0a 2020 2020 2020 2020 2020  box">.          
-00000240: 2020 7b25 2066 6f72 2072 6f77 2069 6e20    {% for row in 
-00000250: 696d 6167 655f 6c69 7374 2025 7d0a 2020  image_list %}.  
-00000260: 2020 2020 2020 2020 2020 3c64 6976 2073            <div s
-00000270: 7479 6c65 3d22 6469 7370 6c61 793a 2066  tyle="display: f
-00000280: 6c65 783b 223e 0a20 2020 2020 2020 2020  lex;">.         
-00000290: 2020 2020 2020 207b 2520 666f 7220 696d         {% for im
-000002a0: 6167 6520 696e 2072 6f77 2025 7d0a 2020  age in row %}.  
-000002b0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000002c0: 6976 2073 7479 6c65 3d22 7769 6474 683a  iv style="width:
-000002d0: 207b 7b20 696d 6167 655b 2777 6964 7468   {{ image['width
-000002e0: 275d 207d 7d70 783b 2068 6569 6768 743a  '] }}px; height:
-000002f0: 207b 7b20 696d 6167 655b 2768 6569 6768   {{ image['heigh
-00000300: 7427 5d20 7d7d 7078 223e 0a20 2020 2020  t'] }}px">.     
-00000310: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000320: 696d 6720 7374 796c 653d 226d 6178 2d77  img style="max-w
-00000330: 6964 7468 3a20 6e6f 6e65 3b22 2068 6569  idth: none;" hei
-00000340: 6768 743d 227b 7b20 696d 6167 655b 2763  ght="{{ image['c
-00000350: 616e 7661 7348 6569 6768 7427 5d20 7d7d  anvasHeight'] }}
-00000360: 2220 7769 6474 683d 227b 7b20 696d 6167  " width="{{ imag
-00000370: 655b 2763 616e 7661 7357 6964 7468 275d  e['canvasWidth']
-00000380: 207d 7d22 2073 7263 3d22 7b7b 2069 6d61   }}" src="{{ ima
-00000390: 6765 5b27 6461 7461 275d 207d 7d22 202f  ge['data'] }}" /
-000003a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000003b0: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-000003c0: 2020 2020 2020 2020 207b 2520 656e 6466           {% endf
-000003d0: 6f72 2025 7d0a 2020 2020 2020 2020 2020  or %}.          
-000003e0: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-000003f0: 2020 2020 207b 2520 656e 6466 6f72 2025       {% endfor %
-00000400: 7d0a 2020 2020 2020 2020 3c2f 6469 763e  }.        </div>
-00000410: 0a20 2020 203c 2f64 6976 3e0a 3c2f 626f  .    </div>.</bo
-00000420: 6479 3e0a 3c2f 6874 6d6c 3e0a            dy>.</html>.
+00000000: 3c64 6976 2069 643d 227b 7b20 6469 765f  <div id="{{ div_
+00000010: 6964 207d 7d22 2073 7479 6c65 3d22 7769  id }}" style="wi
+00000020: 6474 683a 2031 3030 253b 206d 6178 2d68  dth: 100%; max-h
+00000030: 6569 6768 743a 2036 3030 7078 3b22 3e0a  eight: 600px;">.
+00000040: 2020 2020 7b25 2069 6620 7469 746c 6520      {% if title 
+00000050: 213d 2027 2720 257d 0a20 2020 203c 6831  != '' %}.    <h1
+00000060: 2073 7479 6c65 3d22 6d61 7267 696e 2d74   style="margin-t
+00000070: 6f70 3a20 3172 656d 3b20 636f 6c6f 723a  op: 1rem; color:
+00000080: 2023 3333 333b 2066 6f6e 742d 7369 7a65   #333; font-size
+00000090: 3a20 312e 3172 656d 3b20 6d61 7267 696e  : 1.1rem; margin
+000000a0: 2d62 6f74 746f 6d3a 2030 2e35 7265 6d3b  -bottom: 0.5rem;
+000000b0: 2070 6164 6469 6e67 2d69 6e6c 696e 652d   padding-inline-
+000000c0: 7374 6172 743a 2031 7265 6d3b 223e 7b7b  start: 1rem;">{{
+000000d0: 2074 6974 6c65 207d 7d3c 2f68 313e 0a20   title }}</h1>. 
+000000e0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
+000000f0: 2020 203c 7020 7374 796c 653d 2263 6f6c     <p style="col
+00000100: 6f72 3a20 2336 3636 3b20 666f 6e74 2d77  or: #666; font-w
+00000110: 6569 6768 743a 2033 3030 3b20 7061 6464  eight: 300; padd
+00000120: 696e 672d 696e 6c69 6e65 2d73 7461 7274  ing-inline-start
+00000130: 3a20 3172 656d 3b22 3e7b 7b20 6465 7363  : 1rem;">{{ desc
+00000140: 207d 7d3c 2f70 3e0a 2020 2020 3c21 2d2d   }}</p>.    <!--
+00000150: 203c 703e 556e 6465 7220 6365 7274 6169   <p>Under certai
+00000160: 6e20 4a75 7079 7465 7220 656e 7669 726f  n Jupyter enviro
+00000170: 6e6d 656e 7473 2c20 6166 7465 7220 6c61  nments, after la
+00000180: 756e 6368 696e 6720 7079 6777 616c 6b65  unching pygwalke
+00000190: 722c 2074 6865 2070 7265 7669 6577 206d  r, the preview m
+000001a0: 6179 206e 6f74 2061 7574 6f6d 6174 6963  ay not automatic
+000001b0: 616c 6c79 2068 6964 652e 2059 6f75 2063  ally hide. You c
+000001c0: 616e 206d 616e 7561 6c6c 7920 636c 6963  an manually clic
+000001d0: 6b20 7468 6520 6275 7474 6f6e 2074 6f20  k the button to 
+000001e0: 6869 6465 2069 742e 3c2f 703e 202d 2d3e  hide it.</p> -->
+000001f0: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
+00000200: 226d 6169 6e2d 626f 7822 3e0a 2020 2020  "main-box">.    
+00000210: 2020 2020 7b25 2066 6f72 2072 6f77 2069      {% for row i
+00000220: 6e20 696d 6167 655f 6c69 7374 2025 7d0a  n image_list %}.
+00000230: 2020 2020 2020 2020 3c64 6976 2073 7479          <div sty
+00000240: 6c65 3d22 6469 7370 6c61 793a 2066 6c65  le="display: fle
+00000250: 783b 223e 0a20 2020 2020 2020 2020 2020  x;">.           
+00000260: 207b 2520 666f 7220 696d 6167 6520 696e   {% for image in
+00000270: 2072 6f77 2025 7d0a 2020 2020 2020 2020   row %}.        
+00000280: 2020 2020 3c64 6976 2073 7479 6c65 3d22      <div style="
+00000290: 7769 6474 683a 207b 7b20 696d 6167 652e  width: {{ image.
+000002a0: 7769 6474 6820 7d7d 7078 3b20 6865 6967  width }}px; heig
+000002b0: 6874 3a20 7b7b 2069 6d61 6765 2e68 6569  ht: {{ image.hei
+000002c0: 6768 7420 7d7d 7078 223e 0a20 2020 2020  ght }}px">.     
+000002d0: 2020 2020 2020 2020 2020 203c 696d 6720             <img 
+000002e0: 7374 796c 653d 226d 6178 2d77 6964 7468  style="max-width
+000002f0: 3a20 6e6f 6e65 3b22 2068 6569 6768 743d  : none;" height=
+00000300: 227b 7b20 696d 6167 652e 6361 6e76 6173  "{{ image.canvas
+00000310: 5f68 6569 6768 7420 7d7d 2220 7769 6474  _height }}" widt
+00000320: 683d 227b 7b20 696d 6167 652e 6361 6e76  h="{{ image.canv
+00000330: 6173 5f77 6964 7468 207d 7d22 2073 7263  as_width }}" src
+00000340: 3d22 7b7b 2069 6d61 6765 2e64 6174 6120  ="{{ image.data 
+00000350: 7d7d 2220 2f3e 0a20 2020 2020 2020 2020  }}" />.         
+00000360: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000370: 2020 2020 2020 7b25 2065 6e64 666f 7220        {% endfor 
+00000380: 257d 0a20 2020 2020 2020 203c 2f64 6976  %}.        </div
+00000390: 3e0a 2020 2020 2020 2020 7b25 2065 6e64  >.        {% end
+000003a0: 666f 7220 257d 0a20 2020 203c 2f64 6976  for %}.    </div
+000003b0: 3e0a 3c2f 6469 763e 0a                   >.</div>.
```

### Comparing `pygwalker-0.2.0a2/pygwalker/templates/pygwalker_iframe.html` & `pygwalker-0.2.0a3/pygwalker/templates/pygwalker_iframe.html`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/templates/walk.js` & `pygwalker-0.2.0a3/pygwalker/templates/walk.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/templates/dist/pygwalker-app.iife.js` & `pygwalker-0.2.0a3/pygwalker/templates/dist/pygwalker-app.iife.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -83493,32 +83493,32 @@
 
     function _Xe(e) {
         setTimeout((() => {
             var t;
             null == (t = window.parent.document.getElementById(`pygwalker-preview-${e}`)) || t.remove()
         }), 500)
     }
-    const kXe = async (e, t) => {
-        var n, r;
+    const kXe = async (e, t, n) => {
+        var r, i;
         if (0 !== t) {
             kGe.initModalOpen = !0, kGe.setInitModalInfo({
                 title: "Recover Charts",
                 curIndex: 0,
                 total: t
             });
-            for await (const t of null == (n = e.current) ? void 0 : n.exportChartList("data-url")) {
+            for await (const t of null == (r = e.current) ? void 0 : r.exportChartList("data-url")) {
                 const e = await xXe(t.data.container());
-                await (null == (r = AGe.comm) ? void 0 : r.sendMsg("save_chart", {
+                await (null == (i = AGe.comm) ? void 0 : i.sendMsg("save_chart", {
                     ...t.data,
                     singleChart: e
                 })), kGe.setInitModalInfo({
                     title: "Recover Charts",
                     curIndex: t.index + 1,
                     total: t.total
-                })
+                }), _Xe(n)
             }
         }
         kGe.initModalOpen = !1
     }, SXe = bm((e => {
         var t;
         const n = xe.useRef(null),
             r = xe.useRef(null),
@@ -83581,15 +83581,15 @@
                 }],
                 specList: m
             }) : (null == (s = null == (a = null == n ? void 0 : n.current) ? void 0 : a.commonStore) || s.updateTempSTDDS({
                 name: "Dataset",
                 rawFields: d,
                 dataSource: u
             }), null == (c = null == (l = null == n ? void 0 : n.current) ? void 0 : l.commonStore) || c.commitTempDS()), o.needLoadDatas || "jupyter_widgets" !== o.env || setTimeout((() => {
-                kXe(r, m.length)
+                kXe(r, m.length, o.id)
             }), 0)
         }), [n]);
         ye.useEffect((() => {
             g({
                 data: i,
                 rawFields: l,
                 visSpec: a
@@ -83625,15 +83625,15 @@
                     window.addEventListener("message", a)
                 }))
             }(s).then((e => {
                 g({
                     data: e,
                     rawFields: l,
                     visSpec: a
-                }), "jupyter_widgets" === o.env ? kXe(r, m.length) : kGe.setInitModalOpen(!1)
+                }), "jupyter_widgets" === o.env ? kXe(r, m.length, o.id) : kGe.setInitModalOpen(!1)
             })).catch((e => {
                 console.error("Load DataSource Error", e)
             }))
         }), [i, s, l, a, g]);
         ye.useEffect((() => {
             if (n.current) try {
                 b()
```

### Comparing `pygwalker-0.2.0a2/pygwalker/templates/dist/interfaces/index.d.ts` & `pygwalker-0.2.0a3/pygwalker/templates/dist/interfaces/index.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/templates/dist/tools/saveTool.d.ts` & `pygwalker-0.2.0a3/pygwalker/templates/dist/tools/saveTool.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/templates/dist/utils/communication.d.ts` & `pygwalker-0.2.0a3/pygwalker/templates/dist/utils/communication.d.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker/utils/display.py` & `pygwalker-0.2.0a3/pygwalker/utils/display.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker_utils/__main__.py` & `pygwalker-0.2.0a3/pygwalker_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pygwalker_utils/config.py` & `pygwalker-0.2.0a3/pygwalker_utils/config.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/scripts/test-init.py` & `pygwalker-0.2.0a3/scripts/test-init.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/scripts/test-init.sh` & `pygwalker-0.2.0a3/scripts/test-init.sh`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/.gitignore` & `pygwalker-0.2.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/LICENSE` & `pygwalker-0.2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/README.md` & `pygwalker-0.2.0a3/README.md`

 * *Files identical despite different names*

### Comparing `pygwalker-0.2.0a2/pyproject.toml` & `pygwalker-0.2.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
     "jinja2",
     "ipython",
     "astor",
     "typing_extensions",
-    "ipywidgets"
+    "ipywidgets",
+    "pydantic"
 ]
 [project.urls]
 homepage = "https://github.com/Kanaries/pygwalker"
 repository = "https://github.com/Kanaries/pygwalker"
 # changelog, documentation
 
 [project.optional-dependencies]
```

### Comparing `pygwalker-0.2.0a2/PKG-INFO` & `pygwalker-0.2.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pygwalker
-Version: 0.2.0a2
+Version: 0.2.0a3
 Summary: pygwalker: Combining Jupyter Notebook with a Tableau-like UI
 Project-URL: homepage, https://github.com/Kanaries/pygwalker
 Project-URL: repository, https://github.com/Kanaries/pygwalker
 Author-email: "Asm.Def" <woojson@zju.edu.cn>
 License-File: LICENSE
 Keywords: data-analysis,data-exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: astor
 Requires-Dist: ipython
 Requires-Dist: ipywidgets
 Requires-Dist: jinja2
+Requires-Dist: pydantic
 Requires-Dist: typing-extensions
 Provides-Extra: all
 Requires-Dist: pygwalker[pandas,polars,streamlit]; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Provides-Extra: labv4
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: pygwalker Version: 0.2.0a2 Summary: pygwalker:
+Metadata-Version: 2.1 Name: pygwalker Version: 0.2.0a3 Summary: pygwalker:
 Combining Jupyter Notebook with a Tableau-like UI Project-URL: homepage, https:
 //github.com/Kanaries/pygwalker Project-URL: repository, https://github.com/
 Kanaries/pygwalker Author-email: "Asm.Def"
 zju.edu.cn> License-File: LICENSE Keywords: data-analysis,data-
 exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist: astor
 Requires-Dist: ipython Requires-Dist: ipywidgets Requires-Dist: jinja2
-Requires-Dist: typing-extensions Provides-Extra: all Requires-Dist: pygwalker
-[pandas,polars,streamlit]; extra == 'all' Provides-Extra: dev Requires-Dist:
-build; extra == 'dev' Requires-Dist: twine; extra == 'dev' Provides-Extra:
-labv4 Requires-Dist: ipywidgets>=8.0.0; extra == 'labv4' Requires-Dist:
-jupyter-client>7.4.9; extra == 'labv4' Requires-Dist: jupyter-server>2.5.0;
-extra == 'labv4' Provides-Extra: notebook Requires-Dist:
+Requires-Dist: pydantic Requires-Dist: typing-extensions Provides-Extra: all
+Requires-Dist: pygwalker[pandas,polars,streamlit]; extra == 'all' Provides-
+Extra: dev Requires-Dist: build; extra == 'dev' Requires-Dist: twine; extra ==
+'dev' Provides-Extra: labv4 Requires-Dist: ipywidgets>=8.0.0; extra == 'labv4'
+Requires-Dist: jupyter-client>7.4.9; extra == 'labv4' Requires-Dist: jupyter-
+server>2.5.0; extra == 'labv4' Provides-Extra: notebook Requires-Dist:
 ipywidgets<8.0.0,>7.0.0; extra == 'notebook' Requires-Dist: jupyter-
 client<=7.4.9,>6.0.0; extra == 'notebook' Requires-Dist: jupyter-server<=2.5.0;
 extra == 'notebook' Provides-Extra: pandas Requires-Dist: pandas; extra ==
 'pandas' Provides-Extra: polars Requires-Dist: polars; extra == 'polars'
 Provides-Extra: streamlit Requires-Dist: streamlit; extra == 'streamlit'
 Description-Content-Type: text/markdown   [English](README.md) | [ä¸­æ](./
 docs/README.zh.md)
```

