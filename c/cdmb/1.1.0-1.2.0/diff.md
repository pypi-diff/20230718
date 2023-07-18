# Comparing `tmp/cdmb-1.1.0.tar.gz` & `tmp/cdmb-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdmb-1.1.0.tar", max compression
+gzip compressed data, was "cdmb-1.2.0.tar", max compression
```

## Comparing `cdmb-1.1.0.tar` & `cdmb-1.2.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0    19345 2023-07-14 11:35:03.439263 cdmb-1.1.0/LICENSE
--rw-r--r--   0        0        0    35035 2023-07-14 11:35:03.439263 cdmb-1.1.0/README.md
--rw-r--r--   0        0        0    64829 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/CommonDataModel.py
--rw-r--r--   0        0        0      991 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/__init__.py
--rw-r--r--   0        0        0     8532 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/cohort/Cohort.py
--rw-r--r--   0        0        0     4576 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/cohort/Crosswalks.py
--rw-r--r--   0        0        0      120 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/cohort/__init__.py
--rw-r--r--   0        0        0     2921 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/entities/Catalog.py
--rw-r--r--   0        0        0    15180 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/entities/Entity.py
--rw-r--r--   0        0        0    22831 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/entities/Rule.py
--rw-r--r--   0        0        0    10189 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/entities/RuleSet.py
--rw-r--r--   0        0        0    11975 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/entities/Variable.py
--rw-r--r--   0        0        0      498 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/entities/__init__.py
--rw-r--r--   0        0        0     4637 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/project/Author.py
--rw-r--r--   0        0        0    12717 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/project/Metadata.py
--rw-r--r--   0        0        0       33 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/project/__init__.py
--rw-r--r--   0        0        0     6027 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/relationships/Relationship.py
--rw-r--r--   0        0        0       28 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/relationships/__init__.py
--rw-r--r--   0        0        0     1659 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/Utils.py
--rw-r--r--   0        0        0       21 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/__init__.py
--rw-r--r--   0        0        0       50 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/.gitignore
--rw-r--r--   0        0        0    18656 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/LICENSE.md
--rw-r--r--   0        0        0     5920 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/README.md
--rw-r--r--   0        0        0       41 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/_quarto.yml
--rw-r--r--   0        0        0    10224 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/check_load.py
--rw-r--r--   0        0        0     2947 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/dqa.py
--rw-r--r--   0        0        0      151 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/man_container_deployment.md
--rw-r--r--   0        0        0     2855 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/r_report_template.qmd
--rw-r--r--   0        0        0    10161 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/validator.py
--rw-r--r--   0        0        0     3228 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/templates/files/validator_report.qmd
--rw-r--r--   0        0        0      554 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/typing/CommonDataModelTyping.py
--rw-r--r--   0        0        0       36 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/typing/__init__.py
--rw-r--r--   0        0        0    12472 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/UILauncher.py
--rw-r--r--   0        0        0       65 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/__init__.py
--rw-r--r--   0        0        0   111554 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/0.83e0eb50.css
--rw-r--r--   0        0        0      412 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/2.b838d5a7.css
--rw-r--r--   0        0        0     4495 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/4.18440754.css
--rw-r--r--   0        0        0     3111 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/6.bf404883.css
--rw-r--r--   0        0        0       34 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/Indicator.1d121e74.css
--rw-r--r--   0        0        0   111782 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_layout.f2858481.css
--rw-r--r--   0        0        0     4491 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_page.11cd5570.css
--rw-r--r--   0        0        0      412 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_page.b838d5a7.css
--rw-r--r--   0        0        0     3111 2023-07-14 11:35:03.439263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_page.bf404883.css
--rw-r--r--   0        0        0    12580 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/eu_flag.c3360867.jpg
--rw-r--r--   0        0        0    25582 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/favicon.157dca14.png
--rw-r--r--   0        0        0    77364 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff
--rw-r--r--   0        0        0     9104 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2
--rw-r--r--   0        0        0    15772 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2
--rw-r--r--   0        0        0    10520 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2
--rw-r--r--   0        0        0     7508 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2
--rw-r--r--   0        0        0    16284 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2
--rw-r--r--   0        0        0    11364 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2
--rw-r--r--   0        0        0     1753 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/github.1ea8d62e.svg
--rw-r--r--   0        0        0    21305 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.15dffd2d.png
--rw-r--r--   0        0        0    11196 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.dcd54a0d.webp
--rw-r--r--   0        0        0     3663 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Alert.2febe6fa.js
--rw-r--r--   0        0        0    10431 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Button.68ac352c.js
--rw-r--r--   0        0        0     6362 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/CloseButton.0aecb936.js
--rw-r--r--   0        0        0    13044 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Divider.623c8765.js
--rw-r--r--   0        0        0     2206 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Fileupload.78d706fe.js
--rw-r--r--   0        0        0    15049 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/FloatingLabelInput.21cd1ebc.js
--rw-r--r--   0        0        0     1844 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Heading.759b5df3.js
--rw-r--r--   0        0        0      817 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Indicator.svelte_svelte_type_style_lang.e2c519f7.js
--rw-r--r--   0        0        0     9203 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Modal.b90503ef.js
--rw-r--r--   0        0        0    45009 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/SimpleGrid.f308d3bd.js
--rw-r--r--   0        0        0    41583 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Space.5d3c5051.js
--rw-r--r--   0        0        0     9044 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/TableHeadCell.a7fa45f2.js
--rw-r--r--   0        0        0     4606 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Textarea.17eddb3d.js
--rw-r--r--   0        0        0     1484 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Trash.33219cd3.js
--rw-r--r--   0        0        0    15089 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/combinator.becf7b0b.js
--rw-r--r--   0        0        0       27 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/environment.9aa685ef.js
--rw-r--r--   0        0        0      820 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/index.5b757cee.js
--rw-r--r--   0        0        0     1667 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/index.b7a14a97.js
--rw-r--r--   0        0        0    16042 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/index.d8ca07a9.js
--rw-r--r--   0        0        0     9918 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/navigation.8bb60df9.js
--rw-r--r--   0        0        0     2496 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/singletons.3dbe6478.js
--rw-r--r--   0        0        0      414 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.247e7f87.js
--rw-r--r--   0        0        0    11736 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.4d7a1ebc.js
--rw-r--r--   0        0        0      814 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.6cd3ab0e.js
--rw-r--r--   0        0        0     1379 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.c28f1804.js
--rw-r--r--   0        0        0      266 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/stores.d0e64236.js
--rw-r--r--   0        0        0     9868 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/entry/app.34f7a124.js
--rw-r--r--   0        0        0    23923 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/entry/start.07ad94a0.js
--rw-r--r--   0        0        0    13097 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/0.51906aee.js
--rw-r--r--   0        0        0      800 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/1.e22fd99e.js
--rw-r--r--   0        0        0    20534 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/2.7284b9d4.js
--rw-r--r--   0        0        0    27325 2023-07-14 11:35:03.443263 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/3.510394aa.js
--rw-r--r--   0        0        0    56093 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/4.828fc947.js
--rw-r--r--   0        0        0   122218 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/5.faf63ad8.js
--rw-r--r--   0        0        0    68782 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/6.c31223f5.js
--rw-r--r--   0        0        0    61580 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/7.56d911fb.js
--rw-r--r--   0        0        0    28637 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/8.ed4ac5b3.js
--rw-r--r--   0        0        0       27 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/_app/version.json
--rw-r--r--   0        0        0    13602 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/about.html
--rw-r--r--   0        0        0    17310 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/cohort.html
--rw-r--r--   0        0        0     5151 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/entities.html
--rw-r--r--   0        0        0    25582 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/favicon.png
--rw-r--r--   0        0        0    10045 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/index.html
--rw-r--r--   0        0        0    21009 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/project.html
--rw-r--r--   0        0        0       67 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/robots.txt
--rw-r--r--   0        0        0    15250 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/summary.html
--rw-r--r--   0        0        0     8887 2023-07-14 11:35:03.447264 cdmb-1.1.0/cdmb/ui/static_ui/validation.html
--rw-r--r--   0        0        0     1472 2023-07-14 11:35:03.447264 cdmb-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    36684 1970-01-01 00:00:00.000000 cdmb-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    19345 2023-07-18 08:48:03.514975 cdmb-1.2.0/LICENSE
+-rw-r--r--   0        0        0    35035 2023-07-18 08:48:03.514975 cdmb-1.2.0/README.md
+-rw-r--r--   0        0        0    65792 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/CommonDataModel.py
+-rw-r--r--   0        0        0      991 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/__init__.py
+-rw-r--r--   0        0        0     8532 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/cohort/Cohort.py
+-rw-r--r--   0        0        0     4576 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/cohort/Crosswalks.py
+-rw-r--r--   0        0        0      120 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/cohort/__init__.py
+-rw-r--r--   0        0        0     2921 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/entities/Catalog.py
+-rw-r--r--   0        0        0    15180 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/entities/Entity.py
+-rw-r--r--   0        0        0    22831 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/entities/Rule.py
+-rw-r--r--   0        0        0    10189 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/entities/RuleSet.py
+-rw-r--r--   0        0        0    11975 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/entities/Variable.py
+-rw-r--r--   0        0        0      498 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/entities/__init__.py
+-rw-r--r--   0        0        0     4637 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/project/Author.py
+-rw-r--r--   0        0        0    12717 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/project/Metadata.py
+-rw-r--r--   0        0        0       33 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/project/__init__.py
+-rw-r--r--   0        0        0     6027 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/relationships/Relationship.py
+-rw-r--r--   0        0        0       28 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/relationships/__init__.py
+-rw-r--r--   0        0        0     1786 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/Utils.py
+-rw-r--r--   0        0        0       21 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/__init__.py
+-rw-r--r--   0        0        0       50 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/.gitignore
+-rw-r--r--   0        0        0    18656 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/LICENSE.md
+-rw-r--r--   0        0        0     6080 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/README.md
+-rw-r--r--   0        0        0       41 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/_quarto.yml
+-rw-r--r--   0        0        0    10224 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/check_load.py
+-rw-r--r--   0        0        0     2947 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/dqa.py
+-rw-r--r--   0        0        0      151 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/man_container_deployment.md
+-rw-r--r--   0        0        0     2855 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/r_report_template.qmd
+-rw-r--r--   0        0        0    10161 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/validator.py
+-rw-r--r--   0        0        0     3228 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/templates/files/validator_report.qmd
+-rw-r--r--   0        0        0      554 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/typing/CommonDataModelTyping.py
+-rw-r--r--   0        0        0       36 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/typing/__init__.py
+-rw-r--r--   0        0        0    12526 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/UILauncher.py
+-rw-r--r--   0        0        0       65 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/__init__.py
+-rw-r--r--   0        0        0   111554 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/0.83e0eb50.css
+-rw-r--r--   0        0        0      412 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/2.b838d5a7.css
+-rw-r--r--   0        0        0     4495 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/4.18440754.css
+-rw-r--r--   0        0        0     3111 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/6.bf404883.css
+-rw-r--r--   0        0        0       34 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/Indicator.1d121e74.css
+-rw-r--r--   0        0        0   111782 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_layout.f2858481.css
+-rw-r--r--   0        0        0     4491 2023-07-18 08:48:03.514975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_page.11cd5570.css
+-rw-r--r--   0        0        0      412 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_page.b838d5a7.css
+-rw-r--r--   0        0        0     3111 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_page.bf404883.css
+-rw-r--r--   0        0        0    12580 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/eu_flag.c3360867.jpg
+-rw-r--r--   0        0        0    25582 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/favicon.157dca14.png
+-rw-r--r--   0        0        0    77364 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff
+-rw-r--r--   0        0        0     9104 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2
+-rw-r--r--   0        0        0    15772 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2
+-rw-r--r--   0        0        0    10520 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2
+-rw-r--r--   0        0        0     7508 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2
+-rw-r--r--   0        0        0    16284 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2
+-rw-r--r--   0        0        0    11364 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2
+-rw-r--r--   0        0        0     1753 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/github.1ea8d62e.svg
+-rw-r--r--   0        0        0    21305 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.15dffd2d.png
+-rw-r--r--   0        0        0    11196 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.dcd54a0d.webp
+-rw-r--r--   0        0        0     3663 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Alert.2febe6fa.js
+-rw-r--r--   0        0        0    10431 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Button.68ac352c.js
+-rw-r--r--   0        0        0     6362 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/CloseButton.0aecb936.js
+-rw-r--r--   0        0        0    13044 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Divider.623c8765.js
+-rw-r--r--   0        0        0     2206 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Fileupload.78d706fe.js
+-rw-r--r--   0        0        0    15049 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/FloatingLabelInput.21cd1ebc.js
+-rw-r--r--   0        0        0     1844 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Heading.759b5df3.js
+-rw-r--r--   0        0        0      817 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Indicator.svelte_svelte_type_style_lang.e2c519f7.js
+-rw-r--r--   0        0        0     9203 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Modal.b90503ef.js
+-rw-r--r--   0        0        0    45009 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/SimpleGrid.f308d3bd.js
+-rw-r--r--   0        0        0    41583 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Space.5d3c5051.js
+-rw-r--r--   0        0        0     9044 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/TableHeadCell.a7fa45f2.js
+-rw-r--r--   0        0        0     4606 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Textarea.17eddb3d.js
+-rw-r--r--   0        0        0     1484 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Trash.33219cd3.js
+-rw-r--r--   0        0        0    15089 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/combinator.becf7b0b.js
+-rw-r--r--   0        0        0       27 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/environment.9aa685ef.js
+-rw-r--r--   0        0        0      820 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/index.5b757cee.js
+-rw-r--r--   0        0        0     1667 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/index.b7a14a97.js
+-rw-r--r--   0        0        0    16042 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/index.d8ca07a9.js
+-rw-r--r--   0        0        0     9918 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/navigation.8bb60df9.js
+-rw-r--r--   0        0        0     2496 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/singletons.3dbe6478.js
+-rw-r--r--   0        0        0      414 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.247e7f87.js
+-rw-r--r--   0        0        0    11736 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.4d7a1ebc.js
+-rw-r--r--   0        0        0      814 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.6cd3ab0e.js
+-rw-r--r--   0        0        0     1379 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.c28f1804.js
+-rw-r--r--   0        0        0      266 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/stores.d0e64236.js
+-rw-r--r--   0        0        0     9868 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/entry/app.34f7a124.js
+-rw-r--r--   0        0        0    23923 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/entry/start.07ad94a0.js
+-rw-r--r--   0        0        0    13097 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/0.51906aee.js
+-rw-r--r--   0        0        0      800 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/1.e22fd99e.js
+-rw-r--r--   0        0        0    20534 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/2.7284b9d4.js
+-rw-r--r--   0        0        0    27325 2023-07-18 08:48:03.518975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/3.510394aa.js
+-rw-r--r--   0        0        0    56093 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/4.828fc947.js
+-rw-r--r--   0        0        0   122218 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/5.faf63ad8.js
+-rw-r--r--   0        0        0    68782 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/6.c31223f5.js
+-rw-r--r--   0        0        0    61580 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/7.56d911fb.js
+-rw-r--r--   0        0        0    28637 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/8.ed4ac5b3.js
+-rw-r--r--   0        0        0       27 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/_app/version.json
+-rw-r--r--   0        0        0    13602 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/about.html
+-rw-r--r--   0        0        0    17310 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/cohort.html
+-rw-r--r--   0        0        0     5151 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/entities.html
+-rw-r--r--   0        0        0    25582 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/favicon.png
+-rw-r--r--   0        0        0    10045 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/index.html
+-rw-r--r--   0        0        0    21009 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/project.html
+-rw-r--r--   0        0        0       67 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/robots.txt
+-rw-r--r--   0        0        0    15250 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/summary.html
+-rw-r--r--   0        0        0     8887 2023-07-18 08:48:03.522975 cdmb-1.2.0/cdmb/ui/static_ui/validation.html
+-rw-r--r--   0        0        0     1472 2023-07-18 08:48:03.522975 cdmb-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    36684 1970-01-01 00:00:00.000000 cdmb-1.2.0/PKG-INFO
```

### Comparing `cdmb-1.1.0/LICENSE` & `cdmb-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/README.md` & `cdmb-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/CommonDataModel.py` & `cdmb-1.2.0/cdmb/CommonDataModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,37 @@
 from .entities.Entity import Entity
 from .entities.Rule import DummyRule
 from .entities.Variable import Variable
 from .project.Author import Author
 from .project.Metadata import Metadata
 from .relationships.Relationship import Relationship
 from .templates import Utils
+from dateutil.parser import parse
 
+def is_float(param: str):
+    try:
+        float(param)
+        return True
+    except ValueError:
+        return False
+
+
+def is_int(param: str):
+    try:
+        int(param)
+        return True
+    except ValueError:
+        return False
+
+def is_date(string, fuzzy=False):
+    try:
+        parse(string, fuzzy=fuzzy)
+        return True
+    except ValueError:
+        return False
 
 class CommonDataModel:
     def __init__(self,
                  metadata_definition: Metadata,
                  cohort_definition: Cohort,
                  entities: list[Entity],
                  relationships: list[Relationship] = None
@@ -183,15 +205,15 @@
          out_dir (String): Output directory.
 
         """
         with tempfile.TemporaryDirectory(dir=out_dir) as tmpdirname:
             self.save_project(str(tmpdirname))
             time.sleep(1)
             uuid_zip = str(uuid.uuid4())
-            shutil.make_archive(os.path.join(out_dir, uuid_zip), 'zip', root_dir=str(tmpdirname),
+            shutil.make_archive(os.path.join(out_dir, self.folder_code), 'zip', root_dir=str(tmpdirname),
                                 base_dir=self.folder_code)
             time.sleep(1)
             return uuid_zip
 
     def generate_json_structure(self) -> dict:
         response = {
             "created_dt": self._created_dt,
@@ -414,15 +436,14 @@
                 response = relationship.left_column
                 break
             elif relationship.right_entity is not None and relationship.right_entity == entity.name:
                 response = relationship.right_column
                 break
         return response
 
-
     def __generate_synthetic(self, num_registries: int = 1000):
         database_ = os.path.join(self.__getInputPath(), 'data.duckdb')
         con = duckdb.connect(database=database_, read_only=False)
         fake = Faker()
         for entity in self.entities:
             # If related entity reset seed to match.
             Faker.seed(1234)
@@ -463,14 +484,22 @@
                     elif label in rules_set and format_ != "Boolean":
                         ## check if label in rules
                         rule = rules_set[label][0]
                         if rule['category'] == "restricted":
                             data_[label] = choices(rule["values"],
                                                    k=num_registries)
                         else:
+                            # String Categorical variable that takes numerical/date variables.
+                            if format_ == "String" and (is_int(rule['min_value']) or is_int(rule['max_value'])):
+                                format_ = "Integer"
+                            elif format_ == "String" and (is_float(rule['min_value']) or is_float(rule['max_value'])):
+                                format_ = "Double"
+                            elif format_ == "String" and (is_date(rule['min_value']) or is_date(rule['max_value'])):
+                                format_ = "Datetime"
+
                             if 'interval_comparison' in rule['category'] and rule['negative'] is True:
                                 # not between X and Y
                                 left_side_registries = int(num_registries / 2)
                                 right_side_registries = num_registries - left_side_registries
                                 if format_ == "Date":
                                     data_[label] = [fake.date_between_dates(date_end=rule['min_value'])
                                                     for _ in range(left_side_registries)] + \
@@ -594,16 +623,14 @@
             for child in tree_dependencies.children:
                 change_dependency_values(child, None)
 
             if str(entity.name).strip() == "":
                 raise ValueError("The entity name cannot be an empty string.")
 
             df.to_csv(path_, index=False)
-            # TODO Establecer el tipo de datos de la tabla
-
 
             con.sql("CREATE TABLE " + entity.name + " AS SELECT * FROM df")
 
     def __create_rog(self):
         crate = ROCrate()
         authors = []
         orcid_prefix = "https://orcid.org/"
```

### Comparing `cdmb-1.1.0/cdmb/__init__.py` & `cdmb-1.2.0/cdmb/__init__.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/cohort/Cohort.py` & `cdmb-1.2.0/cdmb/cohort/Cohort.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/cohort/Crosswalks.py` & `cdmb-1.2.0/cdmb/cohort/Crosswalks.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/entities/Catalog.py` & `cdmb-1.2.0/cdmb/entities/Catalog.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/entities/Entity.py` & `cdmb-1.2.0/cdmb/entities/Entity.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/entities/Rule.py` & `cdmb-1.2.0/cdmb/entities/Rule.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/entities/RuleSet.py` & `cdmb-1.2.0/cdmb/entities/RuleSet.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/entities/Variable.py` & `cdmb-1.2.0/cdmb/entities/Variable.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/project/Author.py` & `cdmb-1.2.0/cdmb/project/Author.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/project/Metadata.py` & `cdmb-1.2.0/cdmb/project/Metadata.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/relationships/Relationship.py` & `cdmb-1.2.0/cdmb/relationships/Relationship.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/templates/Utils.py` & `cdmb-1.2.0/cdmb/templates/Utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,21 @@
     copyFilesTemplates(out_dir)
     copyFileValidator(out_dir)
     copyFileDqa(out_dir)
     copyFileCheckLoad(out_dir)
 
 
 def copyFileDoc(out_dir: str):
-    docs = ["man_container_deployment.md", "README.md", "LICENSE.md",".gitignore"]
+    docs = ["man_container_deployment.md", "README.md", "LICENSE.md"]
     for doc in docs:
         original = os.path.join(os.path.dirname(__file__), 'files', doc)
         target = os.path.join(out_dir, doc)
         shutil.copyfile(original, target)
-
+    original = os.path.join(os.path.dirname(__file__), 'files', ".gitignore")
+    shutil.copy(original, os.path.join(out_dir, ".gitignore"))
 
 def copyFileDqa(out_dir: str):
     filename = "dqa.py"
     original = os.path.join(os.path.dirname(__file__), "files", filename)
     target = os.path.join(out_dir, "src", "dqa-scripts", filename)
     shutil.copyfile(original, target)
```

### Comparing `cdmb-1.1.0/cdmb/templates/files/LICENSE.md` & `cdmb-1.2.0/cdmb/templates/files/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/templates/files/README.md` & `cdmb-1.2.0/cdmb/templates/files/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Logo of the project](https://cienciadedatosysalud.org/wp-content/uploads/Data-Science-and-VPM.png)
+![Logo of the project](https://cienciadedatosysalud.org/wp-content/uploads/logo-Data-Science-VPM.png)
 
 <small><i>This project follows the structure build using the [Common Data Model Builder](https://github.com/cienciadedatosysalud/cdmb), a tool that allows you to create common data models to facilitate interoperability and reproducibility of the analyses.</i></small>
 
 
 # Your project title
 
 ---
@@ -80,13 +80,15 @@
 
 # How to contribute
 - Repository: https://github.com/your_user/your_repository/
 - Issue tracker: https://github.com/your_user/your_repository/issues
 
 # References
 - Data Science for Health Services and Policy Research group: https://cienciadedatosysalud.org/en/
+- Common Data Model Builder library :https://github.com/cienciadedatosysalud/cdmb
 - Analytic Software Pipeline Interface for Reproducible Execution (ASPIRE): https://github.com/cienciadedatosysalud/ASPIRE
 - ORCID: https://orcid.org/
 - Zenodo: https://zenodo.org/
+- Research Object Crate (RO-Crate): https://www.researchobject.org/ro-crate/
 
 <a href="https://creativecommons.org/licenses/by/4.0/" target="_blank" ><img src="https://img.shields.io/badge/license-CC--BY%204.0-lightgrey" alt="License: CC-BY 4.0"></a>
```

### Comparing `cdmb-1.1.0/cdmb/templates/files/check_load.py` & `cdmb-1.2.0/cdmb/templates/files/check_load.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/templates/files/dqa.py` & `cdmb-1.2.0/cdmb/templates/files/dqa.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/templates/files/r_report_template.qmd` & `cdmb-1.2.0/cdmb/templates/files/r_report_template.qmd`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/templates/files/validator.py` & `cdmb-1.2.0/cdmb/templates/files/validator.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/templates/files/validator_report.qmd` & `cdmb-1.2.0/cdmb/templates/files/validator_report.qmd`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/typing/CommonDataModelTyping.py` & `cdmb-1.2.0/cdmb/typing/CommonDataModelTyping.py`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/UILauncher.py` & `cdmb-1.2.0/cdmb/ui/UILauncher.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         configuration_ = json.loads(configuration)
         metadata_, cohort_, entities_, relationships_ = CommonDataModel.load_previous_configuration_from_web(
             configuration_,
             files)
         cdm = CommonDataModel(metadata_, cohort_, entities_, relationships_)
         with tempfile.TemporaryDirectory(dir='.') as output_dir:
             cdm.save_project(output_dir)
-            file_list = glob.glob(output_dir + "/**", recursive=True)
+            file_list = glob.glob(output_dir + "/**", recursive=True) + glob.glob(output_dir + "/**/.git*", recursive=True)
             return zipfiles(file_list, output_dir)
     except Exception as e:
         raise HTTPException(status_code=400, detail=str(e))
 
 
 @app.post("/api/rules/template")
 def create_rules_template(variables: Annotated[str, Form(media_type="multipart/form-data")]):
```

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/0.83e0eb50.css` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/0.83e0eb50.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/4.18440754.css` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/4.18440754.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/6.bf404883.css` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/6.bf404883.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_layout.f2858481.css` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_layout.f2858481.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_page.11cd5570.css` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_page.11cd5570.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/_page.bf404883.css` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/_page.bf404883.css`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/eu_flag.c3360867.jpg` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/eu_flag.c3360867.jpg`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/favicon.157dca14.png` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/favicon.157dca14.png`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-all-400-normal.1e3b098c.woff`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-400-normal.c7d433fd.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-cyrillic-ext-400-normal.3df7909e.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-400-normal.a8be01ce.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-greek-ext-400-normal.9e2fe623.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-400-normal.e43b3538.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/fira-mono-latin-ext-400-normal.6bfabd30.woff2`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/github.1ea8d62e.svg` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/github.1ea8d62e.svg`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.15dffd2d.png` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.15dffd2d.png`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.dcd54a0d.webp` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/assets/logo_Data_Science_VPM.dcd54a0d.webp`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Alert.2febe6fa.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Alert.2febe6fa.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Button.68ac352c.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Button.68ac352c.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/CloseButton.0aecb936.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/CloseButton.0aecb936.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Divider.623c8765.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Divider.623c8765.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Fileupload.78d706fe.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Fileupload.78d706fe.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/FloatingLabelInput.21cd1ebc.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/FloatingLabelInput.21cd1ebc.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Heading.759b5df3.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Heading.759b5df3.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Indicator.svelte_svelte_type_style_lang.e2c519f7.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Indicator.svelte_svelte_type_style_lang.e2c519f7.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Modal.b90503ef.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Modal.b90503ef.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/SimpleGrid.f308d3bd.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/SimpleGrid.f308d3bd.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Space.5d3c5051.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Space.5d3c5051.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/TableHeadCell.a7fa45f2.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/TableHeadCell.a7fa45f2.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Textarea.17eddb3d.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Textarea.17eddb3d.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/Trash.33219cd3.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/Trash.33219cd3.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/combinator.becf7b0b.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/combinator.becf7b0b.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/index.5b757cee.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/index.5b757cee.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/index.b7a14a97.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/index.b7a14a97.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/index.d8ca07a9.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/index.d8ca07a9.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/navigation.8bb60df9.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/navigation.8bb60df9.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/singletons.3dbe6478.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/singletons.3dbe6478.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.4d7a1ebc.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.4d7a1ebc.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.6cd3ab0e.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.6cd3ab0e.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/chunks/store.c28f1804.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/chunks/store.c28f1804.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/entry/app.34f7a124.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/entry/app.34f7a124.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/entry/start.07ad94a0.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/entry/start.07ad94a0.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/0.51906aee.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/0.51906aee.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/1.e22fd99e.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/1.e22fd99e.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/2.7284b9d4.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/2.7284b9d4.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/3.510394aa.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/3.510394aa.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/4.828fc947.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/4.828fc947.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/5.faf63ad8.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/5.faf63ad8.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/6.c31223f5.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/6.c31223f5.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/7.56d911fb.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/7.56d911fb.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/_app/immutable/nodes/8.ed4ac5b3.js` & `cdmb-1.2.0/cdmb/ui/static_ui/_app/immutable/nodes/8.ed4ac5b3.js`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/about.html` & `cdmb-1.2.0/cdmb/ui/static_ui/about.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/cohort.html` & `cdmb-1.2.0/cdmb/ui/static_ui/cohort.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/entities.html` & `cdmb-1.2.0/cdmb/ui/static_ui/entities.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/favicon.png` & `cdmb-1.2.0/cdmb/ui/static_ui/favicon.png`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/index.html` & `cdmb-1.2.0/cdmb/ui/static_ui/index.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/project.html` & `cdmb-1.2.0/cdmb/ui/static_ui/project.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/summary.html` & `cdmb-1.2.0/cdmb/ui/static_ui/summary.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/cdmb/ui/static_ui/validation.html` & `cdmb-1.2.0/cdmb/ui/static_ui/validation.html`

 * *Files identical despite different names*

### Comparing `cdmb-1.1.0/pyproject.toml` & `cdmb-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdmb"
-version = "1.1.0"
+version = "1.2.0"
 description = "Common Data Model Builder library"
 authors = [
     "Javier González-Galindo <jgonzalezga.iacs@aragon.es>",
     "Francisco Estupiñan-Romero <festupinnan.iacs@aragon.es>",
     "Santiago Royo-Sierra <sroyo.iacs@aragon.es>"
 ]
```

### Comparing `cdmb-1.1.0/PKG-INFO` & `cdmb-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdmb
-Version: 1.1.0
+Version: 1.2.0
 Summary: Common Data Model Builder library
 Home-page: https://github.com/cienciadedatosysalud/cdmb
 License: CC-BY-NC-4.0
 Keywords: common data model,real-world data,health data,synthetic data,secondary use,health,healthcare
 Author: Javier González-Galindo
 Author-email: jgonzalezga.iacs@aragon.es
 Maintainer: Javier González-Galindo
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cdmb Version: 1.1.0 Summary: Common Data Model
+Metadata-Version: 2.1 Name: cdmb Version: 1.2.0 Summary: Common Data Model
 Builder library Home-page: https://github.com/cienciadedatosysalud/cdmb
 License: CC-BY-NC-4.0 Keywords: common data model,real-world data,health
 data,synthetic data,secondary use,health,healthcare Author: Javier GonzÃ¡lez-
 Galindo Author-email: jgonzalezga.iacs@aragon.es Maintainer: Javier GonzÃ¡lez-
 Galindo Maintainer-email: jgonzalezga.iacs@aragon.es Requires-Python:
 >=3.9,<4.0 Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Healthcare Industry Classifier: Intended Audience :: Science/
```

