# Comparing `tmp/pyqrlew-0.1.0.tar.gz` & `tmp/pyqrlew-0.2.0.tar.gz`

## Comparing `pyqrlew-0.1.0.tar` & `pyqrlew-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,35 @@
--rw-r--r--   0        0        0      313 1970-01-01 00:00:00.000000 pyqrlew-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     2785 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3539 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/.gitignore
--rw-r--r--   0     1001      123    11357 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/LICENSE
--rw-r--r--   0     1001      123    38299 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/examples/Sarus SQL.ipynb
--rw-r--r--   0     1001      123      495 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/examples/simple.py
--rw-r--r--   0     1001      123      393 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123      112 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/python/pyqrlew/__init__.py
--rw-r--r--   0     1001      123      513 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/python/pyqrlew/data/retail_demo/dataset.json
--rw-r--r--   0     1001      123    77231 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/python/pyqrlew/data/retail_demo/schema.json
--rw-r--r--   0     1001      123    50408 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/python/pyqrlew/data/retail_demo/size.json
--rw-r--r--   0     1001      123     2420 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123     1019 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/tests/conftest.py
--rw-r--r--   0     1001      123     2481 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/tests/queries/sql_unlimited_queries.sql
--rw-r--r--   0     1001      123     6706 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/tests/queries/valid_queries.sql
--rw-r--r--   0     1001      123    17129 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/tests/ressources/bounds.json
--rw-r--r--   0     1001      123      431 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/tests/ressources/dataset.json
--rw-r--r--   0     1001      123     3411 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/tests/ressources/generate_mocks.py
--rw-r--r--   0     1001      123      366 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/tests/ressources/names.py
--rw-r--r--   0     1001      123    42353 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/tests/ressources/schema.json
--rw-r--r--   0     1001      123    17913 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/tests/ressources/size.json
--rw-r--r--   0     1001      123     1217 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/tests/test_results.py
--rw-r--r--   0     1001      123    45207 2023-05-26 16:40:55.000000 pyqrlew-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      278 1970-01-01 00:00:00.000000 pyqrlew-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 pyqrlew-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123     4542 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     3539 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/.gitignore
+-rw-r--r--   0     1001      123      818 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/.readthedocs.yaml
+-rw-r--r--   0     1001      123      655 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/CHANGELOG.md
+-rw-r--r--   0     1001      123    11357 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/LICENSE
+-rw-r--r--   0     1001      123     1466 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/README.md
+-rw-r--r--   0     1001      123      634 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/docs/Makefile
+-rw-r--r--   0     1001      123     1212 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/docs/conf.py
+-rw-r--r--   0     1001      123      224 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/docs/contributing.md
+-rw-r--r--   0     1001      123     1786 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/docs/index.md
+-rw-r--r--   0     1001      123      800 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/docs/make.bat
+-rw-r--r--   0     1001      123       61 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/docs/requirements.txt
+-rw-r--r--   0     1001      123    49678 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/PyQrlew.ipynb
+-rw-r--r--   0     1001      123   146621 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/demo/demo.ipynb
+-rw-r--r--   0     1001      123      431 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/demo/retail_data/dataset.json
+-rw-r--r--   0     1001      123     1032 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/demo/retail_data/install_db.sql
+-rw-r--r--   0     1001      123      234 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/demo/retail_data/install_db_on_docker.sh
+-rw-r--r--   0     1001      123    84990 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/demo/retail_data/schema.json
+-rw-r--r--   0     1001      123    11484 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/demo/retail_data/size.json
+-rw-r--r--   0     1001      123      133 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/requirements.txt
+-rw-r--r--   0     1001      123      317 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/examples/simple.py
+-rw-r--r--   0     1001      123     1139 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123      112 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/python/pyqrlew/__init__.py
+-rw-r--r--   0     1001      123       45 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/python/pyqrlew/io/__init__.py
+-rw-r--r--   0     1001      123    10178 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/python/pyqrlew/io/database.py
+-rw-r--r--   0     1001      123     2612 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/python/pyqrlew/io/postgresql.py
+-rw-r--r--   0     1001      123    13493 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123      136 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/tests/conftest.py
+-rw-r--r--   0     1001      123     2481 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/tests/queries/sql_unlimited_queries.sql
+-rw-r--r--   0     1001      123     7054 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/tests/queries/valid_queries.sql
+-rw-r--r--   0     1001      123      178 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/tests/requirements.txt
+-rw-r--r--   0     1001      123     1399 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/tests/test_financial_dataset.py
+-rw-r--r--   0     1001      123    45460 2023-07-18 11:51:55.000000 pyqrlew-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 pyqrlew-0.2.0/PKG-INFO
```

### Comparing `pyqrlew-0.1.0/.github/workflows/CI.yml` & `pyqrlew-0.2.0/.github/workflows/CI.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,118 +1,150 @@
 # This file is autogenerated by maturin v0.14.16
 # To update, run
 #
 #    maturin init
 #
 on:
-  push:
-    branches:
-      - main
-      - master
-    tags:
-      - '*'
-  pull_request:
-  workflow_dispatch:
+    push:
+        branches:
+            - main
+            - master
+        tags:
+            - "v*"
+    pull_request:
+    workflow_dispatch:
 
 permissions:
-  contents: read
+    contents: read
 
 jobs:
-  linux:
-    runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        target: [x86_64, x86, aarch64, armv7, s390x, ppc64le]
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-        with:
-          python-version: '3.10'
-      - name: Build wheels
-        uses: PyO3/maturin-action@v1
-        with:
-          target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
-          sccache: 'true'
-          manylinux: auto
-      - name: Upload wheels
-        uses: actions/upload-artifact@v3
-        with:
-          name: wheels
-          path: dist
-
-  windows:
-    runs-on: windows-latest
-    strategy:
-      matrix:
-        target: [x64, x86]
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-        with:
-          python-version: '3.10'
-          architecture: ${{ matrix.target }}
-      - name: Build wheels
-        uses: PyO3/maturin-action@v1
-        with:
-          target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
-          sccache: 'true'
-      - name: Upload wheels
-        uses: actions/upload-artifact@v3
-        with:
-          name: wheels
-          path: dist
-
-  macos:
-    runs-on: macos-latest
-    strategy:
-      matrix:
-        target: [x86_64, aarch64]
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-        with:
-          python-version: '3.10'
-      - name: Build wheels
-        uses: PyO3/maturin-action@v1
-        with:
-          target: ${{ matrix.target }}
-          args: --release --out dist --find-interpreter
-          sccache: 'true'
-      - name: Upload wheels
-        uses: actions/upload-artifact@v3
-        with:
-          name: wheels
-          path: dist
-
-  sdist:
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v3
-      - name: Build sdist
-        uses: PyO3/maturin-action@v1
-        with:
-          command: sdist
-          args: --out dist
-      - name: Upload sdist
-        uses: actions/upload-artifact@v3
-        with:
-          name: wheels
-          path: dist
-
-  release:
-    name: Release
-    runs-on: ubuntu-latest
-    if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [linux, windows, macos, sdist]
-    steps:
-      - uses: actions/download-artifact@v3
-        with:
-          name: wheels
-      - name: Publish to PyPI
-        uses: PyO3/maturin-action@v1
-        env:
-          MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
-        with:
-          command: upload
-          args: --skip-existing *
+    # See: https://github.com/pydantic/pydantic-core/blob/main/.github/workflows/ci.yml
+    test-python:
+        name: test ${{ matrix.python-version }}
+        strategy:
+            fail-fast: false
+            matrix:
+                python-version:
+                    - '3.10'
+        runs-on: ubuntu-latest
+        steps:
+            - uses: actions/checkout@v3
+            - name: install rust stable
+              uses: dtolnay/rust-toolchain@stable
+            - name: cache rust
+              uses: Swatinem/rust-cache@v2
+              with:
+                  key: test-v3
+            - name: set up python
+              uses: actions/setup-python@v4
+              with:
+                  python-version: ${{ matrix.python-version }}
+            - run: pip install -r tests/requirements.txt
+            - run: pip install -e .
+              env:
+                  RUST_BACKTRACE: 1
+            - run: pip freeze
+            - run: pytest
+
+    linux:
+        runs-on: ubuntu-latest
+        if: startsWith(github.ref, 'refs/tags/')
+        strategy:
+            matrix:
+                target: [x86_64, x86, aarch64, armv7, s390x, ppc64le]
+        steps:
+            - uses: actions/checkout@v3
+            - uses: actions/setup-python@v4
+              with:
+                  python-version: '3.10'
+            - name: Build wheels
+              uses: PyO3/maturin-action@v1
+              with:
+                  target: ${{ matrix.target }}
+                  args: --release --out dist --find-interpreter
+                  sccache: "true"
+                  manylinux: auto
+            - name: Upload wheels
+              uses: actions/upload-artifact@v3
+              with:
+                  name: wheels
+                  path: dist
+
+    windows:
+        runs-on: windows-latest
+        if: startsWith(github.ref, 'refs/tags/')
+        strategy:
+            matrix:
+                target: [x64, x86]
+        steps:
+            - uses: actions/checkout@v3
+            - uses: actions/setup-python@v4
+              with:
+                  python-version: '3.10'
+                  architecture: ${{ matrix.target }}
+            - name: Build wheels
+              uses: PyO3/maturin-action@v1
+              with:
+                  target: ${{ matrix.target }}
+                  args: --release --out dist --find-interpreter
+                  sccache: "true"
+            - name: Upload wheels
+              uses: actions/upload-artifact@v3
+              with:
+                  name: wheels
+                  path: dist
+
+    macos:
+        runs-on: macos-latest
+        if: startsWith(github.ref, 'refs/tags/')
+        strategy:
+            matrix:
+                target: [x86_64, aarch64]
+        steps:
+            - uses: actions/checkout@v3
+            - uses: actions/setup-python@v4
+              with:
+                  python-version: "3.10"
+            - name: Build wheels
+              uses: PyO3/maturin-action@v1
+              with:
+                  target: ${{ matrix.target }}
+                  args: --release --out dist --find-interpreter
+                  sccache: "true"
+            - name: Upload wheels
+              uses: actions/upload-artifact@v3
+              with:
+                  name: wheels
+                  path: dist
+
+    sdist:
+        runs-on: ubuntu-latest
+        if: startsWith(github.ref, 'refs/tags/')
+        steps:
+            - uses: actions/checkout@v3
+            - name: Build sdist
+              uses: PyO3/maturin-action@v1
+              with:
+                  command: sdist
+                  args: --out dist
+            - name: Upload sdist
+              uses: actions/upload-artifact@v3
+              with:
+                  name: wheels
+                  path: dist
+
+    release:
+        name: Release
+        runs-on: ubuntu-latest
+        if: startsWith(github.ref, 'refs/tags/')
+        needs: [linux, windows, macos, sdist]
+        steps:
+            - uses: actions/download-artifact@v3
+              with:
+                  name: wheels
+            - name: Publish to PyPI
+              uses: PyO3/maturin-action@v1
+              env:
+                  MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
+              with:
+                  command: upload
+                  args: --skip-existing *
```

### Comparing `pyqrlew-0.1.0/.gitignore` & `pyqrlew-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.1.0/LICENSE` & `pyqrlew-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.1.0/tests/queries/sql_unlimited_queries.sql` & `pyqrlew-0.2.0/tests/queries/sql_unlimited_queries.sql`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.1.0/tests/queries/valid_queries.sql` & `pyqrlew-0.2.0/tests/queries/valid_queries.sql`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 -- SELECT COUNT(*) AS count_all FROM census;
 SELECT COUNT(age) AS count_all FROM census;
 SELECT SUM(education_num) AS sum_education_num FROM census;
 SELECT AVG(education_num) AS my_avg FROM census;
 SELECT STDDEV(education_num) AS my_std FROM census;
-SELECT VARIANCE(education_num)FROM census;
+SELECT VARIANCE(education_num) AS my_var FROM census;
 SELECT SUM(education_num * age + 4 + LOG(age + 2)) AS my_sum FROM census;
-SELECT age, sex, SUM(education_num) AS sum_education_num FROM census GROUP BY age, sex ORDER BY age DESC;
--- SELECT COUNT(*) AS count_all, SUM(education_num) AS sum_education_num, AVG(education_num) AS avg_education_num, VARIANCE(education_num) AS var_education_num, STDDEV(education_num) AS stddev_education_num FROM census;
+-- SELECT age, sex, SUM(education_num) AS sum_education_num FROM census GROUP BY age, sex ORDER BY age DESC; -- Problem with the order by
+-- SELECT COUNT(*) AS count_all, SUM(education_num) AS sum_education_num, AVG(education_num) AS avg_education_num, VARIANCE(education_num) AS var_education_num, STDDEV(education_num) AS stddev_education_num FROM census; -- COUNT(*)
 SELECT SUM(education_num * age + 4 + LOG(age + 3)) AS my_sum FROM census;
 SELECT VARIANCE(education_num) AS my_var, marital_status FROM census GROUP BY marital_status;
 SELECT (VARIANCE(education_num)) AS my_var, marital_status FROM census GROUP BY marital_status;
-SELECT sex, SUM(capital_gain / 10000) AS my_sum, SUM(education_num) AS sum_education_num FROM census GROUP BY sex HAVING NOT ( sex = 'Female' ) ORDER BY my_sum DESC LIMIT 10;
-SELECT marital_status, SUM(capital_gain / 100000) AS my_sum, SUM(education_num) AS sum_education_num FROM census GROUP BY marital_status HAVING marital_status = 'Divorced';
-SELECT POWER(AVG(age), 2) FROM census;
-SELECT 1 + AVG(age) FROM census;
-SELECT SUM(age) FROM census as p;
--- SELECT COUNT(*) FROM census WHERE workclass LIKE 'Married%'
--- SELECT SUM(education_num) FROM census GROUP BY LOG(CASE WHEN age < 50 THEN 50 ELSE 1 END);
--- SELECT CASE WHEN age < 50 THEN 50 ELSE 1 END, COUNT(education_num) FROM census GROUP BY WHEN age < 50 THEN 50 ELSE 1 END;
-SELECT age, SUM(education_num) AS my_sum, SUM(education_num) AS sum_education_num FROM census GROUP BY age HAVING SUM(education_num) > 1 ORDER BY age;
+-- SELECT sex, SUM(capital_gain / 10000) AS my_sum, SUM(education_num) AS sum_education_num FROM census GROUP BY sex HAVING NOT ( sex = 'Female' ) ORDER BY my_sum DESC LIMIT 10; -- HAVING not supported
+-- SELECT marital_status, SUM(capital_gain / 100000) AS my_sum, SUM(education_num) AS sum_education_num FROM census GROUP BY marital_status HAVING marital_status = 'Divorced'; -- HAVING not supported
+SELECT POWER(AVG(age), 2) AS my_res FROM census;
+SELECT 1 + AVG(age) AS my_res FROM census;
+SELECT SUM(age)  AS my_res FROM census as p;
+-- SELECT COUNT(*) FROM census WHERE workclass LIKE 'Married%' -- COUNT(*)
+SELECT SUM(education_num) AS my_sum FROM census GROUP BY LOG(CASE WHEN age < 50 THEN 50 ELSE 1 END);
+SELECT COUNT(education_num) As my_sum FROM census GROUP BY CASE WHEN age < 50 THEN 50 ELSE 1 END;
+-- SELECT CASE WHEN age < 50 THEN 50 ELSE 1 END, COUNT(education_num) AS my_sum FROM census GROUP BY CASE WHEN age < 50 THEN 50 ELSE 1 END;
+-- SELECT age, SUM(education_num) AS my_sum, SUM(education_num) AS sum_education_num FROM census GROUP BY age HAVING SUM(education_num) > 1 ORDER BY age; -- HAVING
 -- SELECT age AS age1, SUM(education_num) FROM census GROUP BY age1 ORDER BY age1;
--- SELECT SUM(age) AS my_sum FROM census GROUP BY marital_status, CASE WHEN age > 90 THEN 1 ELSE 0 END ORDER BY my_sum;
+SELECT SUM(age) AS my_sum FROM census GROUP BY marital_status, CASE WHEN age > 90 THEN 1 ELSE 0 END ORDER BY my_sum;
 -- SELECT CASE WHEN age > 90 THEN 1 ELSE 0 END, SUM(age) AS my_sum FROM census GROUP BY marital_status, CASE WHEN age > 90 THEN 1 ELSE 0 END ORDER BY my_sum;
 -- SELECT CASE WHEN age > 90 THEN 1 ELSE 0 END AS my_col, SUM(age) AS my_sum FROM census GROUP BY my_col ORDER BY my_sum;
--- SELECT SUM(CASE WHEN age > 90 THEN 1 ELSE 0 END), SUM(age) FROM census;
--- SELECT SUM(CASE WHEN age > 90 THEN 1 ELSE 0 END), SUM(age) FROM census;
--- SELECT ( 2 * (SUM(CASE WHEN age > 90 THEN 1 ELSE 0 END))) FROM census;
+SELECT SUM(CASE WHEN age > 90 THEN 1 ELSE 0 END) AS s1, SUM(age) AS s2 FROM census;
+SELECT ( 2 * (SUM(CASE WHEN age > 90 THEN 1 ELSE 0 END))) AS s1 FROM census;
 -- SELECT capital_gain, COUNT(*) FROM census GROUP BY capital_gain;
-SELECT capital_gain, COUNT(1) FROM census GROUP BY capital_gain;
-SELECT capital_gain, COUNT(age) FROM census GROUP BY capital_gain;
+-- SELECT capital_gain, COUNT(1) FROM census GROUP BY capital_gain;
+SELECT capital_gain, COUNT(age) AS count_all FROM census GROUP BY capital_gain;
 -- SELECT EXTRACT( YEAR FROM "検知日時" ) AS _year, COUNT(*) FROM beacon GROUP BY EXTRACT(YEAR FROM "検知日時");
 -- SELECT age AS "my age", 3 * COS(COUNT(*)) AS my_ln_count, AVG(education_num) AS "my avg" FROM census GROUP BY age ORDER BY age, "my avg";
 -- SELECT age AS "my age", 3 * COS(COUNT(*)) AS my_ln_count, AVG(education_num) AS "my avg" FROM census GROUP BY "my age" ORDER BY "my age", "my avg";
 -- SELECT age, COUNT(*) FROM census WHERE age BETWEEN 18 AND 30 GROUP BY age;
 -- SELECT age, COUNT(*) FROM census WHERE age NOT BETWEEN 18 AND 30 GROUP BY age;
 -- SELECT COUNT(*) FROM census WHERE native_country IN ('Holand-Netherlands', 'Cuba', 'Italy', 'England');
 -- SELECT native_country, COUNT(*) FROM census WHERE native_country NOT IN ('Holand-Netherlands', 'Cuba', 'Italy', 'England') GROUP BY native_country;
@@ -41,35 +41,36 @@
 -- SELECT LOWER(marital_status), COUNT(*) FROM census GROUP BY marital_status;
 -- SELECT CONCAT(age, marital_status), COUNT(*) FROM census GROUP BY age, marital_status;
 -- SELECT COALESCE(age, 1) AS new_age, COUNT(*) FROM census GROUP BY COALESCE(age, 1) ORDER BY new_age;
 -- SELECT TRIM(education) AS new_income, COUNT(*) FROM census GROUP BY TRIM(education);
 -- SELECT SUBSTRING(education FROM 1 FOR 4), COUNT(*) FROM census GROUP BY education;
 -- SELECT POSITION('m' in education), COUNT(*) FROM census GROUP BY education;
 -- SELECT CHAR_LENGTH(education), COUNT(*) FROM census GROUP BY education;
-SELECT SUM(census.age), SUM(age) FROM census;
-SELECT table1.sex, SUM(table1.age), SUM(age) FROM census AS table1 GROUP BY table1.sex;
+-- SELECT SUM(census.age) AS s1, SUM(age) AS s2 FROM census;
+SELECT table1.sex AS c1, SUM(table1.age) AS c2, SUM(age) AS c2 FROM census AS table1 GROUP BY table1.sex;
 -- SELECT COUNT(*) FROM census WHERE marital_status LIKE 'W%';
--- SELECT age AS age1, SUM(education_num) FROM census WHERE age IS NOT NULL GROUP BY age1 ORDER BY age1;
+-- SELECT age AS age1, SUM(education_num) AS s1 FROM census WHERE age IS NOT NULL GROUP BY age;
+-- SELECT SUM("マップのY座標") FROM beacon; -- Does not handle '"'"
 -- SELECT "所属部署", COUNT("マップのY座標") FROM beacon GROUP BY "所属部署";
 -- SELECT 2 * SUM (3 * LOG("マップのY座標" + 5)) FROM beacon GROUP BY 3 * "マップのY座標";
 -- SELECT "所属部署" AS "MY_COL", COUNT(*) FROM beacon GROUP BY "所属部署";
 -- SELECT "所属部署" AS "MY_COL", COUNT(*) FROM beacon GROUP BY "MY_COL";
 -- SELECT CURRENT_TIMESTAMP - "検知日時", COUNT(*) FROM beacon GROUP BY "検知日時";
-SELECT COUNT("table_alias"."age") AS "count_alias"  FROM census AS "table_alias";
+-- SELECT COUNT("table_alias"."age") AS "count_alias"  FROM census AS "table_alias";
 -- SELECT age, 3 * COUNT(*), CASE WHEN COUNT(*) > 10 THEN 'large' ELSE 'small' END, COUNT(*) FROM census GROUP BY age;
 -- SELECT age, COUNT(*) FROM census WHERE age IN (20, 30, 40, 50) GROUP BY age;
 -- SELECT age, CASE WHEN age IN (20, 30, 40, 50) THEN 'decade' ELSE '-' END, COUNT(*) FROM census GROUP BY age;
 -- SELECT age, CASE WHEN age BETWEEN 10 AND 40 THEN 0 ELSE 1 END, COUNT(*) FROM census GROUP BY age;
 -- SELECT age, CASE WHEN age IS Null THEN 'Null' ELSE 'NotNull' END, COUNT(*) FROM census GROUP BY age;
 -- SELECT age, CASE WHEN COUNT(*) BETWEEN 0 AND 10 THEN 0 ELSE 1 END, COUNT(*) FROM census GROUP BY age;
 -- SELECT COUNT(*) FROM beacon WHERE "検知日時" BETWEEN '1900-01-01' AND '2025-01-01';
 -- SELECT CASE WHEN SUM(capital_gain) < 10 THEN SUM(capital_gain) ELSE SUM(capital_gain) END FROM census;
 -- SELECT CASE WHEN SUM(age) > 90 THEN 90 WHEN SUM(age) < 10 THEN 10 ELSE 0 END FROM census;
 -- SELECT CASE WHEN SUM(age) > 90 THEN 90 ELSE SUM(age) END FROM census;
-SELECT SUM("age"), STDDEV("age"), VARIANCE("age") FROM census;
+-- SELECT SUM("age"), STDDEV("age"), VARIANCE("age") FROM census;
 -- SELECT SUM("Code Client Patient"), AVG("Code Client Patient"), STDDEV("Code Client Patient") FROM "suivi-patients";
 -- SELECT COUNT(*) AS count_all FROM census LIMIT 30 OFFSET 5;
 -- SELECT COUNT(*) FROM census WHERE marital_status ILIKE 'W%';
 -- SELECT EXTRACT( HOUR FROM "検知日時" ), COUNT(*) FROM beacon GROUP BY "検知日時";
-SELECT SUM(capital_gain) FROM census GROUP BY capital_gain;
-SELECT SUM(100 * age) FROM census WHERE age = 40
-SELECT SUM(-100 * age) FROM census WHERE age = 40
+-- SELECT SUM(capital_gain) FROM census GROUP BY capital_gain;
+-- SELECT SUM(100 * age) FROM census WHERE age = 40
+-- SELECT SUM(-100 * age) FROM census WHERE age = 40
```

### Comparing `pyqrlew-0.1.0/Cargo.lock` & `pyqrlew-0.2.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -548,14 +548,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
@@ -616,17 +625,17 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.6"
@@ -877,115 +886,116 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyqrlew"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "pyo3",
  "qrlew",
  "qrlew-sarus",
+ "serde_json",
 ]
 
 [[package]]
 name = "qrlew"
-version = "0.1.1"
+version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a3cdc65a1dde95348dec96cf6e9aa9fc47693510f7397913482247e9c5956d7"
+checksum = "6481b0b1b1e2e9fce9fffb3626959b8f9445c83e1caa8593745455899b33be16"
 dependencies = [
  "base64",
  "chrono",
  "colored",
  "dot",
  "env_logger",
- "itertools",
+ "itertools 0.10.5",
  "log",
  "paste",
  "postgres",
  "rand",
  "rust_decimal",
  "serde",
  "serde_json",
  "sqlparser",
 ]
 
 [[package]]
 name = "qrlew-sarus"
-version = "0.1.0"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7c9cc4da44ad674d22345d43c43352e644c1c2e818dbf6094b8e89069d2b43a"
+checksum = "53055cfd1efb7aeeb2ad31ddefe40d661cf778fa44b92e8ddaa8b55930b38e52"
 dependencies = [
  "anyhow",
  "chrono",
  "colored",
  "env_logger",
  "glob",
- "itertools",
+ "itertools 0.11.0",
  "log",
  "paste",
  "protobuf",
  "protobuf-codegen",
  "protobuf-json-mapping",
  "qrlew",
  "serde",
```

