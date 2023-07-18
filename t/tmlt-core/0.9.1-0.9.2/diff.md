# Comparing `tmp/tmlt_core-0.9.1.tar.gz` & `tmp/tmlt_core-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmlt_core-0.9.1.tar", max compression
+gzip compressed data, was "tmlt_core-0.9.2.tar", max compression
```

## Comparing `tmlt_core-0.9.1.tar` & `tmlt_core-0.9.2.tar`

### file list

```diff
@@ -1,186 +1,186 @@
--rw-r--r--   0        0        0    10213 2023-04-20 16:47:33.903353 tmlt_core-0.9.1/CHANGELOG.rst
--rw-r--r--   0        0        0    11358 2023-04-20 16:47:33.903353 tmlt_core-0.9.1/LICENSE
--rw-r--r--   0        0        0    20138 2023-04-20 16:47:33.903353 tmlt_core-0.9.1/LICENSE.docs
--rw-r--r--   0        0        0      116 2023-04-20 16:47:33.903353 tmlt_core-0.9.1/NOTICE
--rw-r--r--   0        0        0     1868 2023-04-20 16:47:33.903353 tmlt_core-0.9.1/README.md
--rw-r--r--   0        0        0    11481 2023-04-20 16:47:33.903353 tmlt_core-0.9.1/benchmark/benchmark_count_sum.py
--rw-r--r--   0        0        0     3838 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmark_noise_mechanism.py
--rw-r--r--   0        0        0     8652 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmark_private_join.py
--rw-r--r--   0        0        0    15676 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmark_public_join.py
--rw-r--r--   0        0        0     8873 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmark_quantile.py
--rw-r--r--   0        0        0    10207 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmark_sparkflatmap.py
--rw-r--r--   0        0        0     9446 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmark_sparkmap.py
--rw-r--r--   0        0        0      731 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/benchmark/benchmarking_utils.py
--rw-r--r--   0        0        0      951 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_static/css/custom.css
--rw-r--r--   0        0        0    12470 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_static/favicon.ico
--rw-r--r--   0        0        0     1001 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_static/js/version-banner.js
--rw-r--r--   0        0        0    30903 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_static/logo.png
--rw-r--r--   0        0        0       50 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_templates/build-info.html
--rw-r--r--   0        0        0      408 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_templates/layout.html
--rw-r--r--   0        0        0       23 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/_templates/package-name.html
--rw-r--r--   0        0        0      210 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/additional-resources/index.rst
--rw-r--r--   0        0        0      660 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/additional-resources/license.rst
--rw-r--r--   0        0        0     3159 2023-04-20 16:47:33.904353 tmlt_core-0.9.1/doc/additional-resources/privacy_policy.rst
--rw-r--r--   0        0        0     6889 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/conf.py
--rw-r--r--   0        0        0     1836 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/images/index_api.svg
--rw-r--r--   0        0        0     1186 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/images/index_more.svg
--rw-r--r--   0        0        0      596 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/images/index_topic_guides.svg
--rw-r--r--   0        0        0     1363 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/images/index_tutorials.svg
--rw-r--r--   0        0        0    30903 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/images/logo.png
--rw-r--r--   0        0        0     3186 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/index.rst
--rw-r--r--   0        0        0     4541 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/installation.rst
--rw-r--r--   0        0        0     8472 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/ref.bib
--rw-r--r--   0        0        0     2006 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/templates/python/class.rst
--rw-r--r--   0        0        0     3244 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/templates/python/module.rst
--rw-r--r--   0        0        0    16713 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/architecture.rst
--rw-r--r--   0        0        0      345 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/index.rst
--rw-r--r--   0        0        0     1424 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/known-vulnerabilities.rst
--rw-r--r--   0        0        0     6510 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/privacy-guarantee.rst
--rw-r--r--   0        0        0     2289 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/real-numbers.rst
--rw-r--r--   0        0        0     6151 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/spark.rst
--rw-r--r--   0        0        0     8100 2023-04-20 16:47:33.905353 tmlt_core-0.9.1/doc/topic-guides/special-values.rst
--rw-r--r--   0        0        0     7334 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/doc/tutorials/first-tutorial.rst
--rw-r--r--   0        0        0      231 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/doc/tutorials/index.rst
--rw-r--r--   0        0        0       88 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/doc/zcitations.rst
--rw-r--r--   0        0        0      363 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/ext/build.py
--rw-r--r--   0        0        0     3175 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/ext/build.sh
--rw-r--r--   0        0        0      150 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/ext/dependency_versions.sh
--rw-r--r--   0        0        0     4909 2023-04-20 16:48:10.329370 tmlt_core-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      103 2023-04-20 16:47:33.906353 tmlt_core-0.9.1/test/__init__.py
--rw-r--r--   0        0        0      110 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/__init__.py
--rw-r--r--   0        0        0     3889 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/measurements/test_interactive_measurements.py
--rw-r--r--   0        0        0      654 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/__init__.py
--rw-r--r--   0        0        0     5468 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_average.py
--rw-r--r--   0        0        0    11426 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_base_mechanisms.py
--rw-r--r--   0        0        0     4671 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_count.py
--rw-r--r--   0        0        0     4849 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_count_distinct.py
--rw-r--r--   0        0        0     5670 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_quantile.py
--rw-r--r--   0        0        0      844 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_samplers.py
--rw-r--r--   0        0        0     6706 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_standard_deviation.py
--rw-r--r--   0        0        0     5197 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_sum.py
--rw-r--r--   0        0        0     7067 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/system/noise_distribution_tests/test_variance.py
--rw-r--r--   0        0        0      108 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/unit/__init__.py
--rw-r--r--   0        0        0      116 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/unit/domains/__init__.py
--rw-r--r--   0        0        0     1176 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/unit/domains/test_base.py
--rw-r--r--   0        0        0     6558 2023-04-20 16:47:33.907353 tmlt_core-0.9.1/test/unit/domains/test_collections.py
--rw-r--r--   0        0        0     8866 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/domains/test_numpy_domains.py
--rw-r--r--   0        0        0     9857 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/domains/test_pandas_domains.py
--rw-r--r--   0        0        0    26425 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/domains/test_spark_domains.py
--rw-r--r--   0        0        0      121 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/__init__.py
--rw-r--r--   0        0        0      141 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/pandas_measurements/__init__.py
--rw-r--r--   0        0        0    13818 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/pandas_measurements/test_dataframe.py
--rw-r--r--   0        0        0    10203 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/pandas_measurements/test_series.py
--rw-r--r--   0        0        0    42343 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_aggregations.py
--rw-r--r--   0        0        0     7429 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_chaining.py
--rw-r--r--   0        0        0    17787 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_composition.py
--rw-r--r--   0        0        0     8003 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_converters.py
--rw-r--r--   0        0        0    80698 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_interactive_measurements.py
--rw-r--r--   0        0        0    13139 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_noise_mechanisms.py
--rw-r--r--   0        0        0     9458 2023-04-20 16:47:33.908353 tmlt_core-0.9.1/test/unit/measurements/test_postprocess.py
--rw-r--r--   0        0        0    17510 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/measurements/test_spark_measurements.py
--rw-r--r--   0        0        0      115 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/__init__.py
--rw-r--r--   0        0        0     1833 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/test_continuous_gaussian.py
--rw-r--r--   0        0        0     1235 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/test_discrete_gaussian.py
--rw-r--r--   0        0        0      707 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/test_inverse_cdf.py
--rw-r--r--   0        0        0     1957 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/test_laplace.py
--rw-r--r--   0        0        0     1590 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/test_rng.py
--rw-r--r--   0        0        0      753 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/random/test_uniform.py
--rw-r--r--   0        0        0    15212 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/test_measures.py
--rw-r--r--   0        0        0    91233 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/test_metrics.py
--rw-r--r--   0        0        0      124 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/__init__.py
--rw-r--r--   0        0        0      146 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/__init__.py
--rw-r--r--   0        0        0    22382 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_add_remove_keys.py
--rw-r--r--   0        0        0    37109 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_agg.py
--rw-r--r--   0        0        0     4748 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_filter.py
--rw-r--r--   0        0        0    16386 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_groupby.py
--rw-r--r--   0        0        0     6832 2023-04-20 16:47:33.909353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_id.py
--rw-r--r--   0        0        0    50620 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_join.py
--rw-r--r--   0        0        0    27295 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_map.py
--rw-r--r--   0        0        0    34292 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_nan.py
--rw-r--r--   0        0        0    12670 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_partition.py
--rw-r--r--   0        0        0     3331 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_persist.py
--rw-r--r--   0        0        0     6053 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_rename.py
--rw-r--r--   0        0        0     4811 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_select.py
--rw-r--r--   0        0        0    17751 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_truncation.py
--rw-r--r--   0        0        0     8000 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/test_chaining.py
--rw-r--r--   0        0        0     3922 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/test_converters.py
--rw-r--r--   0        0        0    39837 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/test_dictionary.py
--rw-r--r--   0        0        0     1936 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/transformations/test_identity.py
--rw-r--r--   0        0        0      114 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/utils/__init__.py
--rw-r--r--   0        0        0     8396 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/utils/test_arb.py
--rw-r--r--   0        0        0     5700 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/utils/test_cleanup.py
--rw-r--r--   0        0        0    10005 2023-04-20 16:47:33.910353 tmlt_core-0.9.1/test/unit/utils/test_configuration.py
--rw-r--r--   0        0        0     8733 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_distributions.py
--rw-r--r--   0        0        0     6032 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_exact_number.py
--rw-r--r--   0        0        0    13458 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_grouped_dataframe.py
--rw-r--r--   0        0        0    37873 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_join.py
--rw-r--r--   0        0        0     2424 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_misc.py
--rw-r--r--   0        0        0     1054 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_testing.py
--rw-r--r--   0        0        0     4466 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_truncation.py
--rw-r--r--   0        0        0     1837 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test/unit/utils/test_type_utils.py
--rw-r--r--   0        0        0       37 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/test_requirements.txt
--rw-r--r--   0        0        0      376 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/__init__.py
--rw-r--r--   0        0        0       83 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/domains/__init__.py
--rw-r--r--   0        0        0      992 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/domains/base.py
--rw-r--r--   0        0        0     3425 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/domains/collections.py
--rw-r--r--   0        0        0     3926 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/domains/numpy_domains.py
--rw-r--r--   0        0        0     4489 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/domains/pandas_domains.py
--rw-r--r--   0        0        0    25759 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/domains/spark_domains.py
--rw-r--r--   0        0        0       88 2023-04-20 16:47:33.911353 tmlt_core-0.9.1/tmlt/core/measurements/__init__.py
--rw-r--r--   0        0        0    83528 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/aggregations.py
--rw-r--r--   0        0        0     2931 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/base.py
--rw-r--r--   0        0        0     5020 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/chaining.py
--rw-r--r--   0        0        0     6728 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/composition.py
--rw-r--r--   0        0        0     8463 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/converters.py
--rw-r--r--   0        0        0    73838 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/interactive_measurements.py
--rw-r--r--   0        0        0    17009 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/noise_mechanisms.py
--rw-r--r--   0        0        0      120 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/pandas_measurements/__init__.py
--rw-r--r--   0        0        0    10135 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/pandas_measurements/dataframe.py
--rw-r--r--   0        0        0    15934 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/pandas_measurements/series.py
--rw-r--r--   0        0        0     7411 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/postprocess.py
--rw-r--r--   0        0        0    22812 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measurements/spark_measurements.py
--rw-r--r--   0        0        0    14858 2023-04-20 16:47:33.912353 tmlt_core-0.9.1/tmlt/core/measures.py
--rw-r--r--   0        0        0    54917 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/metrics.py
--rw-r--r--   0        0        0        0 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/py.typed
--rw-r--r--   0        0        0      119 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/__init__.py
--rw-r--r--   0        0        0     2551 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/continuous_gaussian.py
--rw-r--r--   0        0        0    16941 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/discrete_gaussian.py
--rw-r--r--   0        0        0     1497 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/inverse_cdf.py
--rw-r--r--   0        0        0     2132 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/laplace.py
--rw-r--r--   0        0        0      619 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/rng.py
--rw-r--r--   0        0        0     1673 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/random/uniform.py
--rw-r--r--   0        0        0       91 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/__init__.py
--rw-r--r--   0        0        0     4029 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/base.py
--rw-r--r--   0        0        0     4653 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/chaining.py
--rw-r--r--   0        0        0     3277 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/converters.py
--rw-r--r--   0        0        0    27820 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/dictionary.py
--rw-r--r--   0        0        0     1160 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/identity.py
--rw-r--r--   0        0        0      125 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/__init__.py
--rw-r--r--   0        0        0    34915 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/add_remove_keys.py
--rw-r--r--   0        0        0    44303 2023-04-20 16:47:33.913353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/agg.py
--rw-r--r--   0        0        0     5860 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/filter.py
--rw-r--r--   0        0        0    16865 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/groupby.py
--rw-r--r--   0        0        0     5680 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/id.py
--rw-r--r--   0        0        0    39943 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/join.py
--rw-r--r--   0        0        0    40011 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/map.py
--rw-r--r--   0        0        0    40713 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/nan.py
--rw-r--r--   0        0        0     9724 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/partition.py
--rw-r--r--   0        0        0     3862 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/persist.py
--rw-r--r--   0        0        0     6769 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/rename.py
--rw-r--r--   0        0        0     5800 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/select.py
--rw-r--r--   0        0        0    22134 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/truncation.py
--rw-r--r--   0        0        0       85 2023-04-20 16:47:33.914353 tmlt_core-0.9.1/tmlt/core/utils/__init__.py
--rw-r--r--   0        0        0    16349 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/arb.py
--rw-r--r--   0        0        0     1181 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/cleanup.py
--rw-r--r--   0        0        0     6030 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/configuration.py
--rw-r--r--   0        0        0     9303 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/distributions.py
--rw-r--r--   0        0        0    15026 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/exact_number.py
--rw-r--r--   0        0        0     9403 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/grouped_dataframe.py
--rw-r--r--   0        0        0    20371 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/join.py
--rw-r--r--   0        0        0     3190 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/misc.py
--rw-r--r--   0        0        0     3551 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/parameters.py
--rw-r--r--   0        0        0    32413 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/testing.py
--rw-r--r--   0        0        0     7707 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/truncation.py
--rw-r--r--   0        0        0     2796 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/type_utils.py
--rw-r--r--   0        0        0     6215 2023-04-20 16:47:33.915353 tmlt_core-0.9.1/tmlt/core/utils/validation.py
--rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 tmlt_core-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    10764 2023-05-16 14:11:23.605574 tmlt_core-0.9.2/CHANGELOG.rst
+-rw-r--r--   0        0        0    11358 2023-05-16 14:11:23.605574 tmlt_core-0.9.2/LICENSE
+-rw-r--r--   0        0        0    20138 2023-05-16 14:11:23.605574 tmlt_core-0.9.2/LICENSE.docs
+-rw-r--r--   0        0        0      116 2023-05-16 14:11:23.605574 tmlt_core-0.9.2/NOTICE
+-rw-r--r--   0        0        0     1868 2023-05-16 14:11:23.605574 tmlt_core-0.9.2/README.md
+-rw-r--r--   0        0        0    11481 2023-05-16 14:11:23.605574 tmlt_core-0.9.2/benchmark/benchmark_count_sum.py
+-rw-r--r--   0        0        0     3838 2023-05-16 14:11:23.605574 tmlt_core-0.9.2/benchmark/benchmark_noise_mechanism.py
+-rw-r--r--   0        0        0     8652 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/benchmark/benchmark_private_join.py
+-rw-r--r--   0        0        0    15676 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/benchmark/benchmark_public_join.py
+-rw-r--r--   0        0        0     8873 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/benchmark/benchmark_quantile.py
+-rw-r--r--   0        0        0    10207 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/benchmark/benchmark_sparkflatmap.py
+-rw-r--r--   0        0        0     9446 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/benchmark/benchmark_sparkmap.py
+-rw-r--r--   0        0        0      731 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/benchmark/benchmarking_utils.py
+-rw-r--r--   0        0        0      951 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/doc/_static/css/custom.css
+-rw-r--r--   0        0        0    12470 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/doc/_static/favicon.ico
+-rw-r--r--   0        0        0     1001 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/doc/_static/js/version-banner.js
+-rw-r--r--   0        0        0    30903 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/doc/_static/logo.png
+-rw-r--r--   0        0        0       50 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/doc/_templates/build-info.html
+-rw-r--r--   0        0        0      408 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/doc/_templates/layout.html
+-rw-r--r--   0        0        0       23 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/doc/_templates/package-name.html
+-rw-r--r--   0        0        0      210 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/doc/additional-resources/index.rst
+-rw-r--r--   0        0        0      660 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/doc/additional-resources/license.rst
+-rw-r--r--   0        0        0     3159 2023-05-16 14:11:23.606574 tmlt_core-0.9.2/doc/additional-resources/privacy_policy.rst
+-rw-r--r--   0        0        0     6889 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/conf.py
+-rw-r--r--   0        0        0     1836 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/images/index_api.svg
+-rw-r--r--   0        0        0     1186 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/images/index_more.svg
+-rw-r--r--   0        0        0      596 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/images/index_topic_guides.svg
+-rw-r--r--   0        0        0     1363 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/images/index_tutorials.svg
+-rw-r--r--   0        0        0    30903 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/images/logo.png
+-rw-r--r--   0        0        0     3186 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/index.rst
+-rw-r--r--   0        0        0     4541 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/installation.rst
+-rw-r--r--   0        0        0     8472 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/ref.bib
+-rw-r--r--   0        0        0     2006 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/templates/python/class.rst
+-rw-r--r--   0        0        0     3244 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/templates/python/module.rst
+-rw-r--r--   0        0        0    16713 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/topic-guides/architecture.rst
+-rw-r--r--   0        0        0      345 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/topic-guides/index.rst
+-rw-r--r--   0        0        0     1424 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/topic-guides/known-vulnerabilities.rst
+-rw-r--r--   0        0        0     6510 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/topic-guides/privacy-guarantee.rst
+-rw-r--r--   0        0        0     2289 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/topic-guides/real-numbers.rst
+-rw-r--r--   0        0        0     6151 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/topic-guides/spark.rst
+-rw-r--r--   0        0        0     8100 2023-05-16 14:11:23.607574 tmlt_core-0.9.2/doc/topic-guides/special-values.rst
+-rw-r--r--   0        0        0     7334 2023-05-16 14:11:23.608574 tmlt_core-0.9.2/doc/tutorials/first-tutorial.rst
+-rw-r--r--   0        0        0      231 2023-05-16 14:11:23.608574 tmlt_core-0.9.2/doc/tutorials/index.rst
+-rw-r--r--   0        0        0       88 2023-05-16 14:11:23.608574 tmlt_core-0.9.2/doc/zcitations.rst
+-rw-r--r--   0        0        0      363 2023-05-16 14:11:23.608574 tmlt_core-0.9.2/ext/build.py
+-rw-r--r--   0        0        0     3175 2023-05-16 14:11:23.608574 tmlt_core-0.9.2/ext/build.sh
+-rw-r--r--   0        0        0      150 2023-05-16 14:11:23.608574 tmlt_core-0.9.2/ext/dependency_versions.sh
+-rw-r--r--   0        0        0     4909 2023-05-16 14:12:03.094840 tmlt_core-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      103 2023-05-16 14:11:23.609574 tmlt_core-0.9.2/test/__init__.py
+-rw-r--r--   0        0        0      110 2023-05-16 14:11:23.609574 tmlt_core-0.9.2/test/system/__init__.py
+-rw-r--r--   0        0        0     3889 2023-05-16 14:11:23.609574 tmlt_core-0.9.2/test/system/measurements/test_interactive_measurements.py
+-rw-r--r--   0        0        0      654 2023-05-16 14:11:23.609574 tmlt_core-0.9.2/test/system/noise_distribution_tests/__init__.py
+-rw-r--r--   0        0        0     5468 2023-05-16 14:11:23.609574 tmlt_core-0.9.2/test/system/noise_distribution_tests/test_average.py
+-rw-r--r--   0        0        0    11463 2023-05-16 14:11:23.609574 tmlt_core-0.9.2/test/system/noise_distribution_tests/test_base_mechanisms.py
+-rw-r--r--   0        0        0     4671 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/system/noise_distribution_tests/test_count.py
+-rw-r--r--   0        0        0     4849 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/system/noise_distribution_tests/test_count_distinct.py
+-rw-r--r--   0        0        0     5670 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/system/noise_distribution_tests/test_quantile.py
+-rw-r--r--   0        0        0      844 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/system/noise_distribution_tests/test_samplers.py
+-rw-r--r--   0        0        0     6706 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/system/noise_distribution_tests/test_standard_deviation.py
+-rw-r--r--   0        0        0     5197 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/system/noise_distribution_tests/test_sum.py
+-rw-r--r--   0        0        0     7067 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/system/noise_distribution_tests/test_variance.py
+-rw-r--r--   0        0        0      108 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/unit/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/unit/domains/__init__.py
+-rw-r--r--   0        0        0     1230 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/unit/domains/test_base.py
+-rw-r--r--   0        0        0     6610 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/unit/domains/test_collections.py
+-rw-r--r--   0        0        0     8866 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/unit/domains/test_numpy_domains.py
+-rw-r--r--   0        0        0     9857 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/unit/domains/test_pandas_domains.py
+-rw-r--r--   0        0        0    26347 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/unit/domains/test_spark_domains.py
+-rw-r--r--   0        0        0      121 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/unit/measurements/__init__.py
+-rw-r--r--   0        0        0      141 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/unit/measurements/pandas_measurements/__init__.py
+-rw-r--r--   0        0        0    13923 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/unit/measurements/pandas_measurements/test_dataframe.py
+-rw-r--r--   0        0        0    10203 2023-05-16 14:11:23.610574 tmlt_core-0.9.2/test/unit/measurements/pandas_measurements/test_series.py
+-rw-r--r--   0        0        0    45235 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/measurements/test_aggregations.py
+-rw-r--r--   0        0        0     7429 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/measurements/test_chaining.py
+-rw-r--r--   0        0        0    17787 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/measurements/test_composition.py
+-rw-r--r--   0        0        0     8003 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/measurements/test_converters.py
+-rw-r--r--   0        0        0    80698 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/measurements/test_interactive_measurements.py
+-rw-r--r--   0        0        0    13139 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/measurements/test_noise_mechanisms.py
+-rw-r--r--   0        0        0     9458 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/measurements/test_postprocess.py
+-rw-r--r--   0        0        0    26417 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/measurements/test_spark_measurements.py
+-rw-r--r--   0        0        0      115 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/random/__init__.py
+-rw-r--r--   0        0        0     1978 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/random/test_continuous_gaussian.py
+-rw-r--r--   0        0        0     1235 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/random/test_discrete_gaussian.py
+-rw-r--r--   0        0        0      707 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/random/test_inverse_cdf.py
+-rw-r--r--   0        0        0     1957 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/random/test_laplace.py
+-rw-r--r--   0        0        0     1590 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/random/test_rng.py
+-rw-r--r--   0        0        0      753 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/random/test_uniform.py
+-rw-r--r--   0        0        0    15212 2023-05-16 14:11:23.611574 tmlt_core-0.9.2/test/unit/test_measures.py
+-rw-r--r--   0        0        0    91233 2023-05-16 14:11:23.612574 tmlt_core-0.9.2/test/unit/test_metrics.py
+-rw-r--r--   0        0        0      124 2023-05-16 14:11:23.612574 tmlt_core-0.9.2/test/unit/transformations/__init__.py
+-rw-r--r--   0        0        0      146 2023-05-16 14:11:23.612574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/__init__.py
+-rw-r--r--   0        0        0    22404 2023-05-16 14:11:23.612574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_add_remove_keys.py
+-rw-r--r--   0        0        0    37174 2023-05-16 14:11:23.612574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_agg.py
+-rw-r--r--   0        0        0     4788 2023-05-16 14:11:23.612574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_filter.py
+-rw-r--r--   0        0        0    16328 2023-05-16 14:11:23.612574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_groupby.py
+-rw-r--r--   0        0        0     6832 2023-05-16 14:11:23.612574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_id.py
+-rw-r--r--   0        0        0    50698 2023-05-16 14:11:23.612574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_join.py
+-rw-r--r--   0        0        0    27295 2023-05-16 14:11:23.612574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_map.py
+-rw-r--r--   0        0        0    34441 2023-05-16 14:11:23.612574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_nan.py
+-rw-r--r--   0        0        0    12670 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_partition.py
+-rw-r--r--   0        0        0     3331 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_persist.py
+-rw-r--r--   0        0        0     6204 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_rename.py
+-rw-r--r--   0        0        0     4872 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_select.py
+-rw-r--r--   0        0        0    17751 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_truncation.py
+-rw-r--r--   0        0        0     8000 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/transformations/test_chaining.py
+-rw-r--r--   0        0        0     3922 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/transformations/test_converters.py
+-rw-r--r--   0        0        0    39942 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/transformations/test_dictionary.py
+-rw-r--r--   0        0        0     1936 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/transformations/test_identity.py
+-rw-r--r--   0        0        0      114 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/utils/__init__.py
+-rw-r--r--   0        0        0     8396 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/utils/test_arb.py
+-rw-r--r--   0        0        0     5700 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/utils/test_cleanup.py
+-rw-r--r--   0        0        0    10005 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/utils/test_configuration.py
+-rw-r--r--   0        0        0     8733 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/utils/test_distributions.py
+-rw-r--r--   0        0        0     6032 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/utils/test_exact_number.py
+-rw-r--r--   0        0        0    13458 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/utils/test_grouped_dataframe.py
+-rw-r--r--   0        0        0    37873 2023-05-16 14:11:23.613574 tmlt_core-0.9.2/test/unit/utils/test_join.py
+-rw-r--r--   0        0        0     2424 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/test/unit/utils/test_misc.py
+-rw-r--r--   0        0        0     1054 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/test/unit/utils/test_testing.py
+-rw-r--r--   0        0        0     5509 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/test/unit/utils/test_truncation.py
+-rw-r--r--   0        0        0     1837 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/test/unit/utils/test_type_utils.py
+-rw-r--r--   0        0        0       37 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/test_requirements.txt
+-rw-r--r--   0        0        0      376 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/tmlt/core/__init__.py
+-rw-r--r--   0        0        0       83 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/tmlt/core/domains/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/tmlt/core/domains/base.py
+-rw-r--r--   0        0        0     4093 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/tmlt/core/domains/collections.py
+-rw-r--r--   0        0        0     3978 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/tmlt/core/domains/numpy_domains.py
+-rw-r--r--   0        0        0     4692 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/tmlt/core/domains/pandas_domains.py
+-rw-r--r--   0        0        0    26725 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/tmlt/core/domains/spark_domains.py
+-rw-r--r--   0        0        0       88 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/tmlt/core/measurements/__init__.py
+-rw-r--r--   0        0        0    86542 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/tmlt/core/measurements/aggregations.py
+-rw-r--r--   0        0        0     2931 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/tmlt/core/measurements/base.py
+-rw-r--r--   0        0        0     5020 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/tmlt/core/measurements/chaining.py
+-rw-r--r--   0        0        0     6728 2023-05-16 14:11:23.614574 tmlt_core-0.9.2/tmlt/core/measurements/composition.py
+-rw-r--r--   0        0        0     8463 2023-05-16 14:11:23.615574 tmlt_core-0.9.2/tmlt/core/measurements/converters.py
+-rw-r--r--   0        0        0    73838 2023-05-16 14:11:23.615574 tmlt_core-0.9.2/tmlt/core/measurements/interactive_measurements.py
+-rw-r--r--   0        0        0    17009 2023-05-16 14:11:23.615574 tmlt_core-0.9.2/tmlt/core/measurements/noise_mechanisms.py
+-rw-r--r--   0        0        0      120 2023-05-16 14:11:23.615574 tmlt_core-0.9.2/tmlt/core/measurements/pandas_measurements/__init__.py
+-rw-r--r--   0        0        0    10305 2023-05-16 14:11:23.615574 tmlt_core-0.9.2/tmlt/core/measurements/pandas_measurements/dataframe.py
+-rw-r--r--   0        0        0    15934 2023-05-16 14:11:23.615574 tmlt_core-0.9.2/tmlt/core/measurements/pandas_measurements/series.py
+-rw-r--r--   0        0        0     7411 2023-05-16 14:11:23.615574 tmlt_core-0.9.2/tmlt/core/measurements/postprocess.py
+-rw-r--r--   0        0        0    32413 2023-05-16 14:11:23.615574 tmlt_core-0.9.2/tmlt/core/measurements/spark_measurements.py
+-rw-r--r--   0        0        0    14858 2023-05-16 14:11:23.615574 tmlt_core-0.9.2/tmlt/core/measures.py
+-rw-r--r--   0        0        0    55188 2023-05-16 14:11:23.615574 tmlt_core-0.9.2/tmlt/core/metrics.py
+-rw-r--r--   0        0        0        0 2023-05-16 14:11:23.615574 tmlt_core-0.9.2/tmlt/core/py.typed
+-rw-r--r--   0        0        0      119 2023-05-16 14:11:23.615574 tmlt_core-0.9.2/tmlt/core/random/__init__.py
+-rw-r--r--   0        0        0     2553 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/random/continuous_gaussian.py
+-rw-r--r--   0        0        0    16941 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/random/discrete_gaussian.py
+-rw-r--r--   0        0        0     1497 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/random/inverse_cdf.py
+-rw-r--r--   0        0        0     2132 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/random/laplace.py
+-rw-r--r--   0        0        0      619 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/random/rng.py
+-rw-r--r--   0        0        0     1673 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/random/uniform.py
+-rw-r--r--   0        0        0       91 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/transformations/__init__.py
+-rw-r--r--   0        0        0     4029 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/transformations/base.py
+-rw-r--r--   0        0        0     4653 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/transformations/chaining.py
+-rw-r--r--   0        0        0     3365 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/transformations/converters.py
+-rw-r--r--   0        0        0    28130 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/transformations/dictionary.py
+-rw-r--r--   0        0        0     1160 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/transformations/identity.py
+-rw-r--r--   0        0        0      125 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/__init__.py
+-rw-r--r--   0        0        0    34986 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/add_remove_keys.py
+-rw-r--r--   0        0        0    44496 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/agg.py
+-rw-r--r--   0        0        0     5950 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/filter.py
+-rw-r--r--   0        0        0    16865 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/groupby.py
+-rw-r--r--   0        0        0     5680 2023-05-16 14:11:23.616574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/id.py
+-rw-r--r--   0        0        0    40142 2023-05-16 14:11:23.617574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/join.py
+-rw-r--r--   0        0        0    40011 2023-05-16 14:11:23.617574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/map.py
+-rw-r--r--   0        0        0    41582 2023-05-16 14:11:23.617574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/nan.py
+-rw-r--r--   0        0        0     9848 2023-05-16 14:11:23.617574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/partition.py
+-rw-r--r--   0        0        0     3862 2023-05-16 14:11:23.617574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/persist.py
+-rw-r--r--   0        0        0     6863 2023-05-16 14:11:23.617574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/rename.py
+-rw-r--r--   0        0        0     5894 2023-05-16 14:11:23.617574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/select.py
+-rw-r--r--   0        0        0    22134 2023-05-16 14:11:23.617574 tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/truncation.py
+-rw-r--r--   0        0        0       85 2023-05-16 14:11:23.617574 tmlt_core-0.9.2/tmlt/core/utils/__init__.py
+-rw-r--r--   0        0        0    16349 2023-05-16 14:11:23.617574 tmlt_core-0.9.2/tmlt/core/utils/arb.py
+-rw-r--r--   0        0        0     1341 2023-05-16 14:11:23.617574 tmlt_core-0.9.2/tmlt/core/utils/cleanup.py
+-rw-r--r--   0        0        0     6030 2023-05-16 14:11:23.617574 tmlt_core-0.9.2/tmlt/core/utils/configuration.py
+-rw-r--r--   0        0        0     9303 2023-05-16 14:11:23.617574 tmlt_core-0.9.2/tmlt/core/utils/distributions.py
+-rw-r--r--   0        0        0    15026 2023-05-16 14:11:23.618574 tmlt_core-0.9.2/tmlt/core/utils/exact_number.py
+-rw-r--r--   0        0        0     9403 2023-05-16 14:11:23.618574 tmlt_core-0.9.2/tmlt/core/utils/grouped_dataframe.py
+-rw-r--r--   0        0        0    20371 2023-05-16 14:11:23.618574 tmlt_core-0.9.2/tmlt/core/utils/join.py
+-rw-r--r--   0        0        0     3190 2023-05-16 14:11:23.618574 tmlt_core-0.9.2/tmlt/core/utils/misc.py
+-rw-r--r--   0        0        0     3551 2023-05-16 14:11:23.618574 tmlt_core-0.9.2/tmlt/core/utils/parameters.py
+-rw-r--r--   0        0        0    32450 2023-05-16 14:11:23.618574 tmlt_core-0.9.2/tmlt/core/utils/testing.py
+-rw-r--r--   0        0        0     7735 2023-05-16 14:11:23.618574 tmlt_core-0.9.2/tmlt/core/utils/truncation.py
+-rw-r--r--   0        0        0     2796 2023-05-16 14:11:23.618574 tmlt_core-0.9.2/tmlt/core/utils/type_utils.py
+-rw-r--r--   0        0        0     6215 2023-05-16 14:11:23.618574 tmlt_core-0.9.2/tmlt/core/utils/validation.py
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 tmlt_core-0.9.2/PKG-INFO
```

### Comparing `tmlt_core-0.9.1/CHANGELOG.rst` & `tmlt_core-0.9.2/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,51 @@
 .. _core-changelog:
 
 Changelog
 =========
 
+0.9.2 - 2023-05-16
+------------------
+
+Fixed
+~~~~~
+- Fixed bug in :func:`~.limit_keys_per_group`.
+- Fixed bug in :func:`~.gaussian`.
+
+Fixed
+~~~~~
+- :func:`~tmlt.core.utils.cleanup.cleanup` now emits a warning rather than an exception if it fails to get a Spark session.
+  This should prevent unexpected exceptions in the ``atexit`` cleanup handler.
+
 0.9.1 - 2023-04-20
 ------------------
 
 Added
 ~~~~~
 - Subclasses of :class:`~.Measure` now have equations defining the distance they represent.
 
+Changed
+~~~~~~~
+
+- Replaced many existing exceptions in Core to use new classes that contain meta-data about the inputs causing the exception.
+
 0.9.0 - 2023-04-14
 ------------------
 
 Added
 ~~~~~
 
 - :mod:`~.utils.join`, which contains utilities for validating join parameters, propogating domains through joins, and joining dataframes.
 
 Changed
 ~~~~~~~
 
 - :func:`~.truncate_large_groups` does not clump identical records together in hash-based ordering.
 - :class:`~.TransformValue` no longer fails when renaming the id column using :class:`~.RenameValue`.
+- Added the :class:`~.BoundSelection` spark measurement.
 
 Fixed
 ~~~~~
 
 - groupby no longer outputs nan values when both tables are views on the same original table
 - private join no longer drops Nulls on non-join columns when join_on_nulls=False
 - groupby average and variance no longer drops groups containing null values
```

### Comparing `tmlt_core-0.9.1/LICENSE` & `tmlt_core-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/LICENSE.docs` & `tmlt_core-0.9.2/LICENSE.docs`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/README.md` & `tmlt_core-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/benchmark/benchmark_count_sum.py` & `tmlt_core-0.9.2/benchmark/benchmark_count_sum.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/benchmark/benchmark_noise_mechanism.py` & `tmlt_core-0.9.2/benchmark/benchmark_noise_mechanism.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/benchmark/benchmark_private_join.py` & `tmlt_core-0.9.2/benchmark/benchmark_private_join.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/benchmark/benchmark_public_join.py` & `tmlt_core-0.9.2/benchmark/benchmark_public_join.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/benchmark/benchmark_quantile.py` & `tmlt_core-0.9.2/benchmark/benchmark_quantile.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/benchmark/benchmark_sparkflatmap.py` & `tmlt_core-0.9.2/benchmark/benchmark_sparkflatmap.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/benchmark/benchmark_sparkmap.py` & `tmlt_core-0.9.2/benchmark/benchmark_sparkmap.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/benchmark/benchmarking_utils.py` & `tmlt_core-0.9.2/benchmark/benchmarking_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/_static/css/custom.css` & `tmlt_core-0.9.2/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/_static/favicon.ico` & `tmlt_core-0.9.2/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/_static/js/version-banner.js` & `tmlt_core-0.9.2/doc/_static/js/version-banner.js`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/_static/logo.png` & `tmlt_core-0.9.2/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/additional-resources/license.rst` & `tmlt_core-0.9.2/doc/additional-resources/license.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/additional-resources/privacy_policy.rst` & `tmlt_core-0.9.2/doc/additional-resources/privacy_policy.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/conf.py` & `tmlt_core-0.9.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/images/index_api.svg` & `tmlt_core-0.9.2/doc/images/index_api.svg`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/images/index_more.svg` & `tmlt_core-0.9.2/doc/images/index_more.svg`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/images/index_topic_guides.svg` & `tmlt_core-0.9.2/doc/images/index_topic_guides.svg`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/images/index_tutorials.svg` & `tmlt_core-0.9.2/doc/images/index_tutorials.svg`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/images/logo.png` & `tmlt_core-0.9.2/doc/images/logo.png`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/index.rst` & `tmlt_core-0.9.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/installation.rst` & `tmlt_core-0.9.2/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/ref.bib` & `tmlt_core-0.9.2/doc/ref.bib`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/templates/python/class.rst` & `tmlt_core-0.9.2/doc/templates/python/class.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/templates/python/module.rst` & `tmlt_core-0.9.2/doc/templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/topic-guides/architecture.rst` & `tmlt_core-0.9.2/doc/topic-guides/architecture.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/topic-guides/known-vulnerabilities.rst` & `tmlt_core-0.9.2/doc/topic-guides/known-vulnerabilities.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/topic-guides/privacy-guarantee.rst` & `tmlt_core-0.9.2/doc/topic-guides/privacy-guarantee.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/topic-guides/real-numbers.rst` & `tmlt_core-0.9.2/doc/topic-guides/real-numbers.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/topic-guides/spark.rst` & `tmlt_core-0.9.2/doc/topic-guides/spark.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/topic-guides/special-values.rst` & `tmlt_core-0.9.2/doc/topic-guides/special-values.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/doc/tutorials/first-tutorial.rst` & `tmlt_core-0.9.2/doc/tutorials/first-tutorial.rst`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/ext/build.sh` & `tmlt_core-0.9.2/ext/build.sh`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/pyproject.toml` & `tmlt_core-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Tumult's differential privacy primitives"
 readme = "README.md"
 authors = []
 license = "Apache-2.0"
 repository = "https://gitlab.com/tumult-labs/core"
 documentation = "https://docs.tmlt.dev/core/latest"
 # The version field is required in this file format, even though it's ignored because of poetry-dynamic-versioning.
-version = "0.9.1"
+version = "0.9.2"
 
 classifiers = [
    "Development Status :: 4 - Beta",
    "Intended Audience :: Developers",
    "Intended Audience :: Science/Research",
    "Natural Language :: English",
    "Topic :: Software Development :: Libraries",
```

### Comparing `tmlt_core-0.9.1/test/system/measurements/test_interactive_measurements.py` & `tmlt_core-0.9.2/test/system/measurements/test_interactive_measurements.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/system/noise_distribution_tests/__init__.py` & `tmlt_core-0.9.2/test/system/noise_distribution_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_average.py` & `tmlt_core-0.9.2/test/system/noise_distribution_tests/test_average.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_base_mechanisms.py` & `tmlt_core-0.9.2/test/system/noise_distribution_tests/test_base_mechanisms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Tests that base mechanisms add noise sampled from the correct distributions."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
 # pylint: disable=no-member, no-self-use
 
+import math
 from typing import Callable, Dict
 
 import numpy as np
 import pandas as pd
 from nose.plugins.attrib import attr
 from parameterized import parameterized
 from scipy.stats import kstest, laplace, norm
@@ -57,15 +58,17 @@
 
 
 def _create_discrete_gaussian_pmf(loc: int):
     return lambda k, noise_scale: discrete_gaussian_pmf(k - loc, noise_scale)
 
 
 def _create_gaussian_cdf(loc: float):
-    return lambda value, noise_scale: norm.cdf(value, loc=loc, scale=noise_scale)
+    return lambda value, noise_scale: norm.cdf(
+        value, loc=loc, scale=math.sqrt(noise_scale)
+    )
 
 
 # Base Mechanisms Test Instances
 def _create_base_laplace_sampler(
     loc: float, noise_scale: ExactNumberInput, sample_size: int
 ):
     laplace_map_func = np.vectorize(
```

### Comparing `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_count.py` & `tmlt_core-0.9.2/test/system/noise_distribution_tests/test_count.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_count_distinct.py` & `tmlt_core-0.9.2/test/system/noise_distribution_tests/test_count_distinct.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_quantile.py` & `tmlt_core-0.9.2/test/system/noise_distribution_tests/test_quantile.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_samplers.py` & `tmlt_core-0.9.2/test/system/noise_distribution_tests/test_samplers.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_standard_deviation.py` & `tmlt_core-0.9.2/test/system/noise_distribution_tests/test_standard_deviation.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_sum.py` & `tmlt_core-0.9.2/test/system/noise_distribution_tests/test_sum.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/system/noise_distribution_tests/test_variance.py` & `tmlt_core-0.9.2/test/system/noise_distribution_tests/test_variance.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/domains/test_base.py` & `tmlt_core-0.9.2/test/unit/domains/test_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,11 +28,13 @@
 
     @parameterized.expand([(True,), (False,)])
     @patch.object(NewDomain, "validate", autospec=True, return_value=None)
     def test_contains(self, in_domain: bool, domain_validate):
         """Tests that __contains__ works correctly."""
         candidate = Mock()
         if not in_domain:
-            domain_validate.side_effect = OutOfDomainError("Test")
+            domain_validate.side_effect = OutOfDomainError(
+                self.domain, candidate, "Test"
+            )
 
         self.assertEqual(candidate in self.domain, in_domain)
         domain_validate.assert_called_with(self.domain, candidate)
```

### Comparing `tmlt_core-0.9.1/test/unit/domains/test_collections.py` & `tmlt_core-0.9.2/test/unit/domains/test_collections.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,20 +97,20 @@
             ({"A": Mock(), "B": Mock(), "C": Mock()}, True, True),
             ({"A": Mock()}, True, True),
         ]
     )
     def test_validate(self, candidate: Dict[str, Any], in_A: bool, in_B: bool):
         """Tests that validate works correctly."""
         self.domain_a.validate = (
-            Mock(side_effect=OutOfDomainError("Test"))
+            Mock(side_effect=OutOfDomainError(self.domain_a, candidate, "Test"))
             if not in_A
             else Mock(return_value=None)
         )
         self.domain_b.validate = (
-            Mock(side_effect=OutOfDomainError("Test"))
+            Mock(side_effect=OutOfDomainError(self.domain_b, candidate, "Test"))
             if not in_B
             else Mock(return_value=None)
         )
 
         if (in_A and in_B) and set(candidate) == {"A", "B"}:
             self.dict_domain.validate(candidate)
         else:
```

### Comparing `tmlt_core-0.9.1/test/unit/domains/test_numpy_domains.py` & `tmlt_core-0.9.2/test/unit/domains/test_numpy_domains.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/domains/test_pandas_domains.py` & `tmlt_core-0.9.2/test/unit/domains/test_pandas_domains.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/domains/test_spark_domains.py` & `tmlt_core-0.9.2/test/unit/domains/test_spark_domains.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,15 +379,15 @@
             (
                 {
                     "A": SparkIntegerColumnDescriptor(),
                     "B": SparkStringColumnDescriptor(),
                 },
                 pd.DataFrame({"B": [1, 2]}),
                 "Column must be StringType",
-                OutOfDomainError,
+                ValueError,
             ),
         ]
     )
     def test_post_init(
         self,
         schema: SparkColumnsDescriptor,
         group_keys: pd.DataFrame,
@@ -611,68 +611,66 @@
     )
     def test_validate_column(self, col_name: str, col_type: str):
         """Tests that validate_column works correctly."""
         if col_type == "int32":
             self.int32_column_descriptor.validate_column(self.test_df, col_name)
         else:
             with self.assertRaisesRegex(
-                OutOfDomainError,
+                ValueError,
                 r"Column must be IntegerType(\(\))?, instead it is "
                 f"{self.test_df.schema[col_name].dataType}.",
             ):
                 self.int32_column_descriptor.validate_column(self.test_df, col_name)
 
         if col_type == "int64":
             self.int64_column_descriptor.validate_column(self.test_df, col_name)
         else:
             with self.assertRaisesRegex(
-                OutOfDomainError,
+                ValueError,
                 r"Column must be LongType(\(\))?, instead it is "
                 f"{self.test_df.schema[col_name].dataType}.",
             ):
                 self.int64_column_descriptor.validate_column(self.test_df, col_name)
 
         if col_type == "float32":
             self.float32_column_descriptor.validate_column(self.test_df, col_name)
         else:
             with self.assertRaisesRegex(
-                OutOfDomainError,
+                ValueError,
                 r"Column must be FloatType(\(\))?, instead it is "
                 f"{self.test_df.schema[col_name].dataType}.",
             ):
                 self.float32_column_descriptor.validate_column(self.test_df, col_name)
 
         if col_type == "str":
-            with self.assertRaisesRegex(
-                OutOfDomainError, "Column contains null values."
-            ):
+            with self.assertRaisesRegex(ValueError, "Column contains null values."):
                 self.str_column_descriptor.validate_column(self.test_df, col_name)
         else:
             with self.assertRaisesRegex(
-                OutOfDomainError,
+                ValueError,
                 r"Column must be StringType(\(\))?, instead it is "
                 f"{self.test_df.schema[col_name].dataType}.",
             ):
                 self.str_column_descriptor.validate_column(self.test_df, col_name)
 
         if col_type == "date":
             self.date_column_descriptor.validate_column(self.test_df, col_name)
         else:
             with self.assertRaisesRegex(
-                OutOfDomainError,
+                ValueError,
                 r"Column must be DateType(\(\))?, instead it is "
                 f"{self.test_df.schema[col_name].dataType}.",
             ):
                 self.date_column_descriptor.validate_column(self.test_df, col_name)
 
         if col_type == "timestamp":
             self.timestamp_column_descriptor.validate_column(self.test_df, col_name)
         else:
             with self.assertRaisesRegex(
-                OutOfDomainError,
+                ValueError,
                 r"Column must be TimestampType(\(\))?, instead it is "
                 f"{self.test_df.schema[col_name].dataType}.",
             ):
                 self.timestamp_column_descriptor.validate_column(self.test_df, col_name)
 
     @parameterized.expand(
         [
```

### Comparing `tmlt_core-0.9.1/test/unit/measurements/pandas_measurements/test_dataframe.py` & `tmlt_core-0.9.2/test/unit/measurements/pandas_measurements/test_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from tmlt.core.domains.numpy_domains import (
     NumpyFloatDomain,
     NumpyIntegerDomain,
     NumpyStringDomain,
 )
 from tmlt.core.domains.pandas_domains import PandasDataFrameDomain, PandasSeriesDomain
+from tmlt.core.domains.spark_domains import DomainColumnError
 from tmlt.core.measurements.pandas_measurements.dataframe import AggregateByColumn
 from tmlt.core.measurements.pandas_measurements.series import Aggregate, NoisyQuantile
 from tmlt.core.measures import ApproxDP, Measure, PureDP, RhoZCDP
 from tmlt.core.metrics import (
     AbsoluteDifference,
     HammingDistance,
     Metric,
@@ -221,15 +222,17 @@
     def test_input_validation(
         self,
         column_to_aggregation: Dict[str, Aggregate],
         schema: Dict[str, PandasSeriesDomain],
         expected_error_message: str,
     ) -> None:
         """Init correctly validates aggregation functions."""
-        with self.assertRaisesRegex(ValueError, expected_error_message):
+        with self.assertRaisesRegex(
+            (ValueError, DomainColumnError), expected_error_message
+        ):
             AggregateByColumn(
                 input_domain=PandasDataFrameDomain(schema),
                 column_to_aggregation=column_to_aggregation,
             )
 
     def test_correctness_quantile(self) -> None:
         """Test correctness for a quantile aggregation and infinite budget."""
```

### Comparing `tmlt_core-0.9.1/test/unit/measurements/pandas_measurements/test_series.py` & `tmlt_core-0.9.2/test/unit/measurements/pandas_measurements/test_series.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/measurements/test_aggregations.py` & `tmlt_core-0.9.2/test/unit/measurements/test_aggregations.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,32 @@
     SparkDataFrameDomain,
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
 )
 from tmlt.core.measurements.aggregations import (
     NoiseMechanism,
     create_average_measurement,
+    create_bound_selection_measurement,
     create_count_distinct_measurement,
     create_count_measurement,
     create_partition_selection_measurement,
     create_quantile_measurement,
     create_standard_deviation_measurement,
     create_sum_measurement,
     create_variance_measurement,
 )
-from tmlt.core.measures import ApproxDP, PrivacyBudgetInput, PureDP, RhoZCDP
+from tmlt.core.measurements.converters import PureDPToApproxDP, PureDPToRhoZCDP
+from tmlt.core.measurements.spark_measurements import BoundSelection
+from tmlt.core.measures import (
+    ApproxDP,
+    PrivacyBudget,
+    PrivacyBudgetInput,
+    PureDP,
+    RhoZCDP,
+)
 from tmlt.core.metrics import (
     HammingDistance,
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
@@ -965,14 +974,65 @@
         if count_column is not None:
             self.assertEqual(measurement.count_column, count_column)
         # Check that measurement.privacy_function(d_in) = (epsilon, delta)
         measurement_epsilon, measurement_delta = measurement.privacy_function(d_in)
         self.assertEqual(measurement_epsilon, epsilon)
         self.assertEqual(measurement_delta, delta)
 
+    @parameterized.expand(
+        [
+            (PureDP(), 1, "B", 0.7, 1),
+            (RhoZCDP(), 1, "B", 0.7, 1),
+            (ApproxDP(), (1, 0), "B", 0.7, 1),
+        ]
+    )
+    def test_create_bound_selection_measurement(
+        self,
+        output_measure: Union[PureDP, RhoZCDP, ApproxDP],
+        d_out: PrivacyBudgetInput,
+        bound_column: str,
+        threshold: float,
+        d_in: ExactNumberInput = 1,
+    ):
+        """Test create_bound_selection_measurement works correctly."""
+        measurement = create_bound_selection_measurement(
+            input_domain=self.input_domain,
+            output_measure=output_measure,
+            d_out=d_out,
+            bound_column=bound_column,
+            threshold=threshold,
+            d_in=d_in,
+        )
+        d_out = PrivacyBudget.cast(output_measure, d_out).value
+        if isinstance(measurement, PureDPToRhoZCDP):
+            measurement = measurement.pure_dp_measurement
+            epsilon = sp.sqrt(ExactNumber(sp.Integer(2) * d_out).expr)
+        elif isinstance(measurement, PureDPToApproxDP):
+            measurement = measurement.pure_dp_measurement
+            assert isinstance(d_out, tuple)
+            epsilon = d_out[0]
+        else:
+            epsilon = d_out
+        # Appease mypy
+        if not isinstance(measurement, BoundSelection):
+            raise TypeError(
+                f"Expected measurement to be a BoundSelection, got {measurement}"
+            )
+        d_in = ExactNumber(d_in)
+        self.assertEqual(measurement.input_domain, self.input_domain)
+        self.assertEqual(measurement.output_measure, PureDP())
+        self.assertEqual(measurement.privacy_function(d_in), epsilon)
+        if d_out == float("inf"):
+            expected_alpha = ExactNumber(0)
+        else:
+            expected_alpha = (4 / epsilon) * d_in
+        self.assertEqual(measurement.alpha, expected_alpha)
+        self.assertEqual(measurement.bound_column, bound_column)
+        self.assertEqual(measurement.threshold, threshold)
+
 
 INPUT_DOMAIN = SparkDataFrameDomain(
     {"A": SparkStringColumnDescriptor(), "B": SparkIntegerColumnDescriptor()}
 )
 
 
 class TestBadDelta(unittest.TestCase):
@@ -1044,20 +1104,41 @@
     def test_functions_with_noise_mechanism(
         self, noise_mechanism: NoiseMechanism, d_out: PrivacyBudgetInput, f: Callable
     ) -> None:
         """Test error is raised for invalid delta/noise mechanism combination."""
         with self.assertRaises(ValueError):
             f(noise_mechanism=noise_mechanism, d_out=d_out)
 
-    def test_quantile(self) -> None:
-        """Test error is raised for nonzero delta for create quantile."""
+    @parameterized.expand(
+        [
+            (d_out, f)
+            for d_out in [
+                (sp.Integer(1), sp.Rational(1, 2)),
+                (sp.Integer(1), sp.Rational(1, 3)),
+            ]
+            for f in [
+                functools.partial(
+                    create_bound_selection_measurement,
+                    input_domain=INPUT_DOMAIN,
+                    bound_column="B",
+                    threshold=0.5,
+                    output_measure=ApproxDP(),
+                ),
+                functools.partial(
+                    create_quantile_measurement,
+                    input_domain=INPUT_DOMAIN,
+                    input_metric=SymmetricDifference(),
+                    measure_column="B",
+                    quantile=0.5,
+                    upper=10,
+                    lower=0,
+                    output_measure=ApproxDP(),
+                ),
+            ]
+        ]
+    )
+    def test_functions_without_noise_mechanism(
+        self, d_out: PrivacyBudgetInput, f: Callable
+    ) -> None:
+        """Test error is raised for invalid deltas."""
         with self.assertRaises(ValueError):
-            create_quantile_measurement(
-                input_domain=INPUT_DOMAIN,
-                input_metric=SymmetricDifference(),
-                measure_column="B",
-                quantile=0.5,
-                upper=10,
-                lower=0,
-                d_out=(sp.Integer(1), sp.Rational(1, 2)),
-                output_measure=ApproxDP(),
-            )
+            f(d_out=d_out)
```

### Comparing `tmlt_core-0.9.1/test/unit/measurements/test_chaining.py` & `tmlt_core-0.9.2/test/unit/measurements/test_chaining.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/measurements/test_composition.py` & `tmlt_core-0.9.2/test/unit/measurements/test_composition.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/measurements/test_converters.py` & `tmlt_core-0.9.2/test/unit/measurements/test_converters.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/measurements/test_interactive_measurements.py` & `tmlt_core-0.9.2/test/unit/measurements/test_interactive_measurements.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/measurements/test_noise_mechanisms.py` & `tmlt_core-0.9.2/test/unit/measurements/test_noise_mechanisms.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/measurements/test_postprocess.py` & `tmlt_core-0.9.2/test/unit/measurements/test_postprocess.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/measurements/test_spark_measurements.py` & `tmlt_core-0.9.2/tmlt/core/measurements/noise_mechanisms.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,452 +1,519 @@
-"""Unit tests for :mod:`~tmlt.core.measurements.spark_measurements`."""
+"""Measurements for adding noise to individual numbers."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
-# pylint: disable=no-self-use
-from typing import Dict, List
+import random
+from fractions import Fraction
+from typing import Union, cast
 
 import numpy as np
-import pandas as pd
-import sympy as sp
-from parameterized import parameterized
-from pyspark.sql import functions as sf
-from pyspark.sql.types import IntegerType, StringType, StructField, StructType
-
-from tmlt.core.domains.numpy_domains import NumpyIntegerDomain
-from tmlt.core.domains.pandas_domains import PandasDataFrameDomain, PandasSeriesDomain
-from tmlt.core.domains.spark_domains import (
-    SparkColumnDescriptor,
-    SparkDataFrameDomain,
-    SparkFloatColumnDescriptor,
-    SparkGroupedDataFrameDomain,
-    SparkIntegerColumnDescriptor,
-    SparkStringColumnDescriptor,
+from pyspark.sql.types import DataType, DoubleType, LongType
+from scipy import stats
+from typeguard import typechecked
+
+from tmlt.core.domains.numpy_domains import (
+    NumpyDomain,
+    NumpyFloatDomain,
+    NumpyIntegerDomain,
 )
-from tmlt.core.measurements.noise_mechanisms import AddGeometricNoise, AddLaplaceNoise
-from tmlt.core.measurements.pandas_measurements.dataframe import AggregateByColumn
-from tmlt.core.measurements.pandas_measurements.series import (
-    AddNoiseToSeries,
-    NoisyQuantile,
+from tmlt.core.measurements.base import Measurement
+from tmlt.core.measures import PureDP, RhoZCDP
+from tmlt.core.metrics import AbsoluteDifference
+from tmlt.core.random.continuous_gaussian import gaussian
+from tmlt.core.random.discrete_gaussian import (
+    _sample_dlaplace,
+    _sample_geometric_exp_slow,
+    sample_dgauss,
 )
-from tmlt.core.measurements.spark_measurements import (
-    AddNoiseToColumn,
-    ApplyInPandas,
-    GeometricPartitionSelection,
-    _get_materialized_df,
+from tmlt.core.random.laplace import laplace
+from tmlt.core.random.rng import prng
+from tmlt.core.utils.distributions import (
+    discrete_gaussian_inverse_cmf,
+    double_sided_geometric_inverse_cmf,
 )
-from tmlt.core.measures import ApproxDP, PureDP
-from tmlt.core.metrics import SumOf, SymmetricDifference
-from tmlt.core.utils.distributions import double_sided_geometric_cmf_exact
-from tmlt.core.utils.exact_number import ExactNumber
-from tmlt.core.utils.grouped_dataframe import GroupedDataFrame
-from tmlt.core.utils.testing import (
-    FakeAggregate,
-    PySparkTest,
-    assert_property_immutability,
-    get_all_props,
-)
-
+from tmlt.core.utils.exact_number import ExactNumber, ExactNumberInput
+from tmlt.core.utils.misc import RNGWrapper
+from tmlt.core.utils.validation import validate_exact_number
 
-class TestApplyInPandas(PySparkTest):
-    """Tests for ApplyInPandas."""
 
-    def setUp(self):
-        """Setup."""
-        self.aggregation_function = AggregateByColumn(
-            input_domain=PandasDataFrameDomain(
-                {"B": PandasSeriesDomain(NumpyIntegerDomain())}
-            ),
-            column_to_aggregation={
-                "B": NoisyQuantile(
-                    PandasSeriesDomain(NumpyIntegerDomain()),
-                    output_measure=PureDP(),
-                    quantile=0.5,
-                    lower=22,
-                    upper=29,
-                    epsilon=sp.Integer(1),
-                )
-            },
-        )
-        self.domain = SparkGroupedDataFrameDomain(
-            schema={
-                "A": SparkStringColumnDescriptor(),
-                "B": SparkIntegerColumnDescriptor(),
-            },
-            group_keys=self.spark.createDataFrame([("x1",), ("x2",)], schema=["A"]),
-        )
-        self.measurement = ApplyInPandas(
-            input_domain=self.domain,
-            input_metric=SumOf(SymmetricDifference()),
-            aggregation_function=self.aggregation_function,
-        )
+class AddLaplaceNoise(Measurement):
+    """Add Laplace noise to a number."""
 
-    @parameterized.expand(get_all_props(ApplyInPandas))
-    def test_property_immutability(self, prop_name: str):
-        """Tests that given property is immutable."""
-        assert_property_immutability(self.measurement, prop_name)
-
-    def test_properties(self):
-        """ApplyInPandas's properties have the expected values."""
-        aggregation_function = FakeAggregate()
-        input_domain = SparkGroupedDataFrameDomain(
-            schema={
-                "A": SparkStringColumnDescriptor(),
-                "B": SparkFloatColumnDescriptor(allow_nan=True),
-            },
-            group_keys=self.spark.createDataFrame([("x1",), ("x2",)], schema=["A"]),
-        )
-        measurement = ApplyInPandas(
-            input_domain=input_domain,
-            input_metric=SumOf(SymmetricDifference()),
-            aggregation_function=aggregation_function,
-        )
-        self.assertEqual(measurement.input_domain, input_domain)
-        self.assertEqual(measurement.input_metric, SumOf(SymmetricDifference()))
-        self.assertEqual(measurement.output_measure, PureDP())
-        self.assertEqual(measurement.is_interactive, False)
-        self.assertEqual(measurement.aggregation_function, aggregation_function)
-
-    @parameterized.expand(
-        [
-            # test with one groupby column
-            (
-                {
-                    "A": ["1", "2", "2", "3"],
-                    "B": [1.0, 2.0, 1.0, np.nan],
-                    "C": [np.nan] * 4,
-                    "D": [np.nan] * 4,
-                },
-                {
-                    "A": SparkStringColumnDescriptor(),
-                    "B": SparkFloatColumnDescriptor(allow_nan=True),
-                    "C": SparkFloatColumnDescriptor(allow_nan=True),
-                    "D": SparkFloatColumnDescriptor(allow_nan=True),
-                },
-                {"A": ["1", "2", "3", "4"]},
-                {
-                    "A": ["1", "2", "3", "4"],
-                    "C": [1.0, 3.0, None, -1.0],
-                    "C_str": ["1.0", "3.0", "nan", "-1.0"],
-                },
-            ),
-            # test with two groupby columns
-            (
-                {
-                    "A_1": ["1", "2", "2", "3"],
-                    "A_2": ["1", "2", "2", "1"],
-                    "B": [1.0, 2.0, 1.0, np.nan],
-                    "C": [np.nan] * 4,
-                    "D": [np.nan] * 4,
-                },
-                {
-                    "A_1": SparkStringColumnDescriptor(),
-                    "A_2": SparkStringColumnDescriptor(),
-                    "B": SparkFloatColumnDescriptor(allow_nan=True),
-                    "C": SparkFloatColumnDescriptor(allow_nan=True),
-                    "D": SparkFloatColumnDescriptor(allow_nan=True),
-                },
-                {"A_1": ["1", "1", "2", "2"], "A_2": ["1", "2", "1", "2"]},
-                {
-                    "A_1": ["1", "1", "2", "2"],
-                    "A_2": ["1", "2", "1", "2"],
-                    "C": [1.0, -1.0, -1.0, 3.0],
-                    "C_str": ["1.0", "-1.0", "-1.0", "3.0"],
-                },
-            ),
-        ]
-    )
-    def test_correctness_test_measure(
+    @typechecked
+    def __init__(
         self,
-        df_dict: Dict[str, List],
-        schema: Dict[str, SparkColumnDescriptor],
-        groupby_domains: Dict[str, List],
-        expected_dict: Dict[str, List],
+        input_domain: Union[NumpyIntegerDomain, NumpyFloatDomain],
+        scale: ExactNumberInput,
     ):
-        """Test correctness for a GroupByApplyInPandas aggregation."""
-        group_keys = self.spark.createDataFrame(pd.DataFrame(groupby_domains))
-        input_domain = SparkGroupedDataFrameDomain(schema=schema, group_keys=group_keys)
-        grouped_dataframe = GroupedDataFrame(
-            dataframe=self.spark.createDataFrame(pd.DataFrame(df_dict)),
-            group_keys=group_keys,
-        )
-        actual = ApplyInPandas(
-            input_domain=input_domain,
-            input_metric=SumOf(SymmetricDifference()),
-            aggregation_function=FakeAggregate(),
-        )(grouped_dataframe).toPandas()
-        expected = pd.DataFrame(expected_dict)
-        # It looks like python nans get converted to nulls when the return value
-        # from a python udf gets converted back to spark land.
-        self.assert_frame_equal_with_sort(actual, expected)
+        """Constructor.
 
-    def test_privacy_function_and_relation(self):
-        """Test that the privacy function and relation are computed correctly."""
+        Args:
+            input_domain: Input Domain.
+            scale: Noise scale.
+        """
+        try:
+            validate_exact_number(
+                value=scale,
+                allow_nonintegral=True,
+                minimum=0,
+                minimum_is_inclusive=True,
+            )
+        except ValueError as e:
+            raise ValueError(f"Invalid scale: {e}") from e
 
-        quantile_measurement = NoisyQuantile(
-            PandasSeriesDomain(NumpyIntegerDomain()),
+        if isinstance(input_domain, NumpyFloatDomain) and (
+            input_domain.allow_nan or input_domain.allow_inf
+        ):
+            raise ValueError("Input domain must not contain infs or nans")
+        super().__init__(
+            input_domain=input_domain,
+            input_metric=AbsoluteDifference(),
             output_measure=PureDP(),
-            quantile=0.5,
-            lower=22,
-            upper=29,
-            epsilon=sp.Integer(2),
+            is_interactive=False,
         )
+        self._scale = ExactNumber(scale)
+        self._output_type = DoubleType()
 
-        df_aggregation_function = AggregateByColumn(
-            input_domain=PandasDataFrameDomain(
-                {"Age": PandasSeriesDomain(NumpyIntegerDomain())}
-            ),
-            column_to_aggregation={"Age": quantile_measurement},
-        )
-        measurement = ApplyInPandas(
-            input_domain=SparkGroupedDataFrameDomain(
-                schema={
-                    "Gender": SparkStringColumnDescriptor(),
-                    "Age": SparkIntegerColumnDescriptor(),
-                },
-                group_keys=self.spark.createDataFrame(
-                    pd.DataFrame({"Gender": ["M", "F"]})
-                ),
-            ),
-            input_metric=SumOf(SymmetricDifference()),
-            aggregation_function=df_aggregation_function,
-        )
+    @property
+    def input_domain(self) -> NumpyDomain:
+        """Return input domain for the measurement."""
+        return cast(NumpyDomain, super().input_domain)
 
-        self.assertTrue(measurement.privacy_function(sp.Integer(1)), sp.Integer(2))
-        self.assertTrue(measurement.privacy_relation(sp.Integer(1), sp.Integer(2)))
-        self.assertFalse(
-            measurement.privacy_relation(sp.Integer(1), sp.Rational("1.99999"))
-        )
+    @property
+    def scale(self) -> ExactNumber:
+        """Returns the noise scale."""
+        return self._scale
 
+    @property
+    def output_type(self) -> DataType:
+        """Return the output data type after being used as a UDF."""
+        return self._output_type
 
-class TestAddNoiseToColumn(PySparkTest):
-    """Tests for AddNoiseToColumn.
+    @typechecked
+    def privacy_function(self, d_in: ExactNumberInput) -> ExactNumber:
+        r"""Returns the smallest d_out satisfied by the measurement.
 
-    Tests :class:`~tmlt.core.measurements.spark_measurements.AddNoiseToColumn`.
-    """
+        The returned d_out is :math:`\frac{d_{in}}{b}`
+        (:math:`\infty` if :math:`b = 0`).
 
-    def setUp(self):
-        """Test Setup."""
-        self.input_domain = SparkDataFrameDomain(
-            {
-                "A": SparkStringColumnDescriptor(),
-                "count": SparkIntegerColumnDescriptor(),
-            }
-        )
+        where:
 
-    @parameterized.expand(get_all_props(AddNoiseToColumn))
-    def test_property_immutability(self, prop_name: str):
-        """Tests that given property is immutable."""
-        measurement = AddNoiseToColumn(
-            input_domain=self.input_domain,
-            measurement=AddNoiseToSeries(
-                AddLaplaceNoise(input_domain=NumpyIntegerDomain(), scale=sp.Integer(1))
-            ),
-            measure_column="count",
-        )
-        assert_property_immutability(measurement, prop_name)
+        * :math:`d_{in}` is the input argument "d_in"
+        * :math:`b` is the property "scale"
 
-    def test_correctness(self):
-        """Tests that AddNoiseToColumn works correctly."""
-        expected = pd.DataFrame({"A": [0, 1, 2, 3], "count": [0, 1, 2, 3]})
-        sdf = self.spark.createDataFrame(expected)
-        measurement = AddNoiseToColumn(
-            input_domain=self.input_domain,
-            measurement=AddNoiseToSeries(AddGeometricNoise(alpha=0)),
-            measure_column="count",
-        )
-        actual = measurement(sdf).toPandas()
-        self.assert_frame_equal_with_sort(actual, expected)
+        Args:
+            d_in: Distance between inputs under input_metric.
+        """
+        self.input_metric.validate(d_in)
+        if self.scale == 0:
+            return ExactNumber(float("inf"))
+        return d_in / self.scale
 
+    def __call__(
+        self, val: Union[np.int32, np.int64, np.float32, np.float64, float, int]
+    ) -> float:
+        r"""Returns the value with laplace noise added.
 
-class TestGeometricPartitionSelection(PySparkTest):
-    """Tests for GeometricPartitionSelection.
+        The added laplace noise has the probability density function
 
-    Tests
-    :class:`~tmlt.core.measurements.spark_measurements.GeometricPartitionSelection`.
-    """
+        :math:`f(x) = \frac{1}{2 b} e ^ {\frac{-\mid x \mid}{b}}`
 
-    def setUp(self):
-        """Test Setup."""
-        self.input_domain = SparkDataFrameDomain(
-            {"A": SparkStringColumnDescriptor(), "B": SparkIntegerColumnDescriptor()}
-        )
-        self.threshold = 5
-        self.alpha = ExactNumber(3)
-        self.count_column = "noisy counts"
-        self.measurement = GeometricPartitionSelection(
-            input_domain=self.input_domain,
-            alpha=self.alpha,
-            threshold=self.threshold,
-            count_column=self.count_column,
-        )
+        where:
 
-    @parameterized.expand(get_all_props(GeometricPartitionSelection))
-    def test_property_immutability(self, prop_name: str):
-        """Tests that given property is immutable."""
-        assert_property_immutability(self.measurement, prop_name)
-
-    def test_properties(self):
-        """GeometricPartitionSelection has the expected properties."""
-        self.assertEqual(self.measurement.input_domain, self.input_domain)
-        self.assertEqual(self.measurement.input_metric, SymmetricDifference())
-        self.assertEqual(self.measurement.output_measure, ApproxDP())
-        self.assertEqual(self.measurement.alpha, self.alpha)
-        self.assertEqual(self.measurement.threshold, self.threshold)
-        self.assertEqual(self.measurement.count_column, self.count_column)
-
-    def test_empty(self):
-        """Tests that empty inputs/outputs don't cause any issues."""
-        sdf = self.spark.createDataFrame(
-            [],
-            schema=StructType(
-                [StructField("A", StringType()), StructField("B", IntegerType())]
-            ),
-        )
-        expected = pd.DataFrame(
-            {
-                "A": pd.Series(dtype=str),
-                "B": pd.Series(dtype=int),
-                self.count_column: pd.Series(dtype=int),
-            }
-        )
-        actual = self.measurement(sdf).toPandas()
-        self.assert_frame_equal_with_sort(actual, expected)
+        * :math:`x` is a real number
+        * :math:`b` is the property "scale"
 
-    def test_negative_threshold(self):
-        """Tests that negative thresholds don't cause any issues."""
-        sdf = self.spark.createDataFrame(
-            pd.DataFrame({"A": ["a1"] * 100, "B": [1] * 100})
-        )
-        measurement = GeometricPartitionSelection(
-            input_domain=self.input_domain,
-            alpha=1,
-            threshold=-1,
-            count_column=self.count_column,
-        )
-        actual = measurement(sdf).toPandas()
-        expected_without_count = pd.DataFrame({"A": ["a1"], "B": [1]})
-        self.assertIsInstance(actual, pd.DataFrame)
-        assert isinstance(actual, pd.DataFrame)
-        self.assert_frame_equal_with_sort(actual[["A", "B"]], expected_without_count)
-        # Threshold -1 should give worse guarantee than for threshold of 0 or 1
-        measurement_threshold_0 = GeometricPartitionSelection(
-            input_domain=self.input_domain,
-            alpha=1,
-            threshold=0,
-            count_column=self.count_column,
-        )
-        measurement_threshold_1 = GeometricPartitionSelection(
-            input_domain=self.input_domain,
-            alpha=1,
-            threshold=1,
-            count_column=self.count_column,
-        )
-        # Guarantee isn't infinitely bad
-        self.assertFalse(
-            ApproxDP().compare((sp.oo, 1), measurement.privacy_function(1))
-        )
-        # But is worse than for 0, which is worse than for 1
-        self.assertFalse(
-            ApproxDP().compare(
-                measurement.privacy_function(1),
-                measurement_threshold_0.privacy_function(1),
+        Args:
+            val: Value to add Laplace noise to.
+        """
+        if not self.scale.is_finite:
+            return random.choice([float("inf"), -float("inf")])
+        float_scale = self.scale.to_float(round_up=True)
+        return laplace(u=float(val), b=float_scale)
+
+    @classmethod
+    def inverse_cdf(cls, scale: float, probability: float) -> float:
+        """Inverse CDF function.
+
+        Given a probability, returns a point x in the range such that
+        the noise generated by this measurement will be <= x with
+        probability probability.
+
+        Args:
+            scale: The noise scale.
+            probability: The probability that noise generated by this class
+                should fall below the threshold it returns. Must be in [0, 1].
+        """
+        if probability < 0 or probability > 1:
+            raise ValueError(
+                "Probabilities input to the inverse CDF must be in [0, 1], but got"
+                f" {probability}"
             )
-        )
-        self.assertFalse(
-            ApproxDP().compare(
-                measurement.privacy_function(1),
-                measurement_threshold_1.privacy_function(1),
+        if probability == 0:
+            return -float("inf")
+        if probability == 1:
+            return float("inf")
+        if not scale:
+            return float("inf")
+
+        return stats.laplace.ppf(q=probability, loc=0, scale=scale)
+
+
+class AddGeometricNoise(Measurement):
+    """Add Geometric noise to a number."""
+
+    @typechecked
+    def __init__(self, alpha: ExactNumberInput):
+        """Constructor.
+
+        Args:
+            alpha: Noise scale.
+        """
+        try:
+            validate_exact_number(
+                value=alpha,
+                allow_nonintegral=True,
+                minimum=0,
+                minimum_is_inclusive=True,
+                maximum=float("inf"),
+                maximum_is_inclusive=False,
             )
+        except ValueError as e:
+            raise ValueError(f"Invalid alpha: {e}") from e
+
+        super().__init__(
+            input_domain=NumpyIntegerDomain(),
+            input_metric=AbsoluteDifference(),
+            output_measure=PureDP(),
+            is_interactive=False,
         )
-        self.assertFalse(
-            ApproxDP().compare(
-                measurement_threshold_0.privacy_function(1),
-                measurement_threshold_1.privacy_function(1),
+        self._alpha = ExactNumber(alpha)
+        self._output_type = LongType()
+
+    @property
+    def input_domain(self) -> NumpyIntegerDomain:
+        """Return input domain for the measurement."""
+        return cast(NumpyIntegerDomain, super().input_domain)
+
+    @property
+    def output_type(self) -> DataType:
+        """Return the output data type after being used as a UDF."""
+        return self._output_type
+
+    @property
+    def alpha(self) -> ExactNumber:
+        """Returns the noise scale."""
+        return self._alpha
+
+    @typechecked
+    def privacy_function(self, d_in: ExactNumberInput) -> ExactNumber:
+        r"""Returns the smallest d_out satisfied by the measurement.
+
+        The returned d_out is :math:`\frac{d_{in}}{\alpha}`
+        (:math:`\infty` if :math:`\alpha = 0`).
+
+        where:
+
+        * :math:`d_{in}` is the input argument "d_in"
+        * :math:`\alpha` is :attr:`~.alpha`
+
+        Args:
+            d_in: Distance between inputs under input_metric.
+        """
+        self.input_metric.validate(d_in)
+        if self.alpha == 0:
+            return ExactNumber(float("inf"))
+        return d_in / self.alpha
+
+    def __call__(self, value: Union[np.int32, np.int64, float, int]) -> int:
+        r"""Returns the value with double sided geometric noise added.
+
+        The added noise has the probability mass function
+
+        .. math::
+
+            f(k)=
+            \frac
+                {e^{1 / \alpha} - 1}
+                {e^{1 / \alpha} + 1}
+            \cdot
+            e^{\frac{-\mid k \mid}{\alpha}}
+
+        where:
+
+        * :math:`k` is an integer
+        * :math:`\alpha` is :attr:`~.alpha`
+
+        A double sided geometric distribution is the difference between two geometric
+        distributions (It can be sampled from by sampling a two values from a geometric
+        distribution, and taking their difference).
+
+        See section 4.1 in :cite:`BalcerV18`, remark 2 in
+        `this paper <https://arxiv.org/pdf/1707.01189.pdf>`_, or scipy.stats.geom for
+        more information. (Note that the parameter :math:`p` used in scipy.stats.geom
+        is related to :math:`\alpha` through :math:`p = 1 - e^{-1 / \alpha}`).
+
+        Args:
+            value: Value to add geometric noise to.
+        """
+        if self.alpha == 0:
+            return int(value)
+        float_scale = self.alpha.to_float(round_up=True)
+        # The following two statements produce the same noise distribution,
+        # but _sample_geometric_exp_slow performs better for small noise scales,
+        # and _sample_dlaplace performs better for larger noise scales
+        if float_scale < 10:
+            x = 1 / Fraction(float_scale)
+            noise = _sample_geometric_exp_slow(
+                x, RNGWrapper(prng())
+            ) - _sample_geometric_exp_slow(x, RNGWrapper(prng()))
+        # for very large noise scales, _sample_geometric_exp_slow is *very* slow
+        else:
+            # _sample_dlaplace produces a noise distribution that
+            # matches the equation above.
+            noise = _sample_dlaplace(float_scale, RNGWrapper(prng()))
+        return int(value + noise)
+
+    @classmethod
+    def inverse_cdf(cls, alpha: float, probability: float) -> float:
+        """Inverse CDF function.
+
+        Given a probability, returns a point x in the range such that
+        the noise generated by this measurement will be <= x with
+        probability probability.
+
+        Args:
+            alpha: The noise scale.
+            probability: The probability that noise generated by this class
+                should fall below the threshold it returns. Must be in [0, 1].
+        """
+        if probability < 0 or probability > 1:
+            raise ValueError(
+                "Probabilities input to the inverse CDF must be in [0, 1], but got"
+                f" {probability}"
             )
-        )
+        if probability == 0:
+            return -float("inf")
+        if probability == 1:
+            return float("inf")
+
+        return double_sided_geometric_inverse_cmf(probability, alpha)
 
-    def test_no_noise(self):
-        """Tests that the no noise works correctly."""
-        sdf = self.spark.createDataFrame(
-            pd.DataFrame(
-                {"A": ["a1", "a2", "a2", "a3", "a3", "a3"], "B": [1, 2, 2, 3, 3, 3]}
+
+class AddDiscreteGaussianNoise(Measurement):
+    """Add discrete Gaussian noise to a number."""
+
+    @typechecked
+    def __init__(self, sigma_squared: ExactNumberInput):
+        r"""Constructor.
+
+        Args:
+            sigma_squared: Noise scale. This is the variance of the discrete Gaussian
+                distribution to be used for sampling noise.
+        """
+        try:
+            validate_exact_number(
+                value=sigma_squared,
+                allow_nonintegral=True,
+                minimum=0,
+                minimum_is_inclusive=True,
+                maximum=float("inf"),
+                maximum_is_inclusive=False,
             )
-        )
-        expected = pd.DataFrame({"A": ["a2", "a3"], "B": [2, 3], "count": [2, 3]})
-        measurement = GeometricPartitionSelection(
-            input_domain=self.input_domain, alpha=0, threshold=2
-        )
-        actual = measurement(sdf).toPandas()
-        self.assert_frame_equal_with_sort(actual, expected)
+        except ValueError as e:
+            raise ValueError(f"Invalid sigma_squared: {e}") from e
 
-    def test_privacy_function(self):
-        """GeometricPartitionSelection's privacy function is correct."""
-        alpha = ExactNumber(3)
-        threshold = 100
-        measurement = GeometricPartitionSelection(
-            input_domain=self.input_domain, alpha=alpha, threshold=threshold
-        )
-        self.assertEqual(measurement.privacy_function(0), (0, 0))
-        base_epsilon = 1 / alpha
-        base_delta = 1 - double_sided_geometric_cmf_exact(threshold - 2, alpha)
-        self.assertEqual(measurement.privacy_function(1), (base_epsilon, base_delta))
-
-        self.assertEqual(
-            measurement.privacy_function(3),
-            (
-                3 * base_epsilon,
-                3 * ExactNumber(sp.E) ** (3 * base_epsilon) * base_delta,
-            ),
+        super().__init__(
+            input_domain=NumpyIntegerDomain(),
+            input_metric=AbsoluteDifference(),
+            output_measure=RhoZCDP(),
+            is_interactive=False,
         )
+        self._sigma_squared = ExactNumber(sigma_squared)
+        self._output_type = LongType()
 
+    @property
+    def input_domain(self) -> NumpyIntegerDomain:
+        """Return input domain for the measurement."""
+        return cast(NumpyIntegerDomain, super().input_domain)
 
-class TestSanitization(PySparkTest):
-    """Output DataFrames from Spark measurements are correctly sanitized."""
+    @property
+    def output_type(self) -> DataType:
+        """Return the output data type after being used as a UDF."""
+        return self._output_type
 
-    @parameterized.expand(
-        [
-            (
-                pd.DataFrame({"col1": [1, 2, 3], "col2": ["abc", "def", "ghi"]}),
-                "simple_table",
-            ),
-            (
-                pd.DataFrame(
-                    {
-                        "bad;column;name": ["a", "b", "c"],
-                        "big_numbers": [
-                            100000000000000,
-                            100000000000000000,
-                            99999999999999999,
-                        ],
-                    }
-                ),
-                "table_123456",
-            ),
-        ]
-    )
-    def test_get_materialized_df(self, df, table_name):
-        """Tests that _get_materialized_df works correctly."""
-        current_db = self.spark.catalog.currentDatabase()
-        sdf = self.spark.createDataFrame(df)
-        materialized_df = _get_materialized_df(sdf, table_name)
-        self.assertEqual(current_db, self.spark.catalog.currentDatabase())
-        self.assert_frame_equal_with_sort(materialized_df.toPandas(), df)
-
-    def test_repartition_works_as_expected(self):
-        """Tests that repartitioning randomly works as expected.
-
-        Note: This is a sanity test that checks repartition by a random
-        column works as expected regardless of the internal representation of
-        the DataFrame being repartitioned. This does not test any unit
-        in :mod:`~tmlt.core.measurements.spark_measurements`.
+    @property
+    def sigma_squared(self) -> ExactNumber:
+        """Returns the noise scale."""
+        return self._sigma_squared
+
+    @typechecked
+    def privacy_function(self, d_in: ExactNumberInput) -> ExactNumber:
+        r"""Returns the smallest d_out satisfied by the measurement.
+
+        The returned d_out is :math:`\frac{d_{in}^2}{2 \cdot \sigma^2}`
+        (:math:`\infty` if :math:`\sigma^2 = 0`).
+
+        where:
+
+        * :math:`d_{in}` is the input argument "d_in"
+        * :math:`\sigma^2` is :attr:`~.sigma_squared`
+
+        See Proposition 1.6 in `this <https://arxiv.org/pdf/1605.02065.pdf>`_ paper.
+
+        Args:
+            d_in: Distance between inputs under input_metric.
         """
-        df = self.spark.createDataFrame(
-            [(i, f"{j}") for i in range(10) for j in range(20)]
+        self.input_metric.validate(d_in)
+        if self.sigma_squared == 0:
+            return ExactNumber(float("inf"))
+        return (ExactNumber(d_in) ** 2) / (2 * self._sigma_squared)
+
+    def __call__(self, value: Union[np.int32, np.int64, float, int]) -> int:
+        r"""Adds discrete Gaussian noise with specified scale.
+
+        The added noise has the probability mass function
+
+        .. math::
+
+            f(k) = \frac
+            {e^{k^2/2\sigma^2}}
+            {
+                \sum_{n\in \mathbb{Z}}
+                e^{n^2/2\sigma^2}
+            }
+
+        where:
+
+        * :math:`k` is an integer
+        * :math:`\sigma^2` is :attr:`~.sigma_squared`
+
+        See :cite:`Canonne0S20` for more information. The formula above is based on
+        Definition 1.
+        """
+        float_scale = self.sigma_squared.to_float(round_up=True)
+        return int(value + sample_dgauss(float_scale, RNGWrapper(prng())))
+
+    @classmethod
+    def inverse_cdf(cls, sigma_squared: float, probability: float) -> float:
+        """Inverse CDF function.
+
+        Given a probability, returns a point x in the range such that
+        the noise generated by this measurement will be <= x with
+        probability probability.
+
+        Args:
+            sigma_squared: The noise scale.
+            probability: The probability that noise generated by this class
+                should fall below the threshold it returns. Must be in [0, 1].
+        """
+        if probability < 0 or probability > 1:
+            raise ValueError(
+                "Probabilities input to the inverse CDF must be in [0, 1], but got"
+                f" {probability}"
+            )
+        if probability == 0:
+            return -float("inf")
+        if probability == 1:
+            return float("inf")
+
+        return discrete_gaussian_inverse_cmf(p=probability, sigma_squared=sigma_squared)
+
+
+class AddGaussianNoise(Measurement):
+    """Add Gaussian noise to a number."""
+
+    @typechecked
+    def __init__(
+        self,
+        input_domain: Union[NumpyIntegerDomain, NumpyFloatDomain],
+        sigma_squared: ExactNumberInput,
+    ):
+        """Constructor.
+
+        Args:
+            input_domain: Domain of the input.
+            sigma_squared: Noise scale. This is the variance of the Gaussian
+                distribution to be used for sampling noise.
+        """
+        try:
+            validate_exact_number(
+                value=sigma_squared,
+                allow_nonintegral=True,
+                minimum=0,
+                minimum_is_inclusive=True,
+                maximum=float("inf"),
+                maximum_is_inclusive=True,
+            )
+        except ValueError as e:
+            raise ValueError(f"Invalid sigma_squared: {e}") from e
+
+        super().__init__(
+            input_domain=input_domain,
+            input_metric=AbsoluteDifference(),
+            output_measure=RhoZCDP(),
+            is_interactive=False,
         )
-        df = df.withColumn("partitioningColumn", sf.round(sf.rand() * 1000))
-        # Random partitioning column
-        partitions1 = df.repartition("partitioningColumn").rdd.glom().collect()
-        df_shuffled = df.repartition(1000)
-        partitions2 = df_shuffled.repartition("partitioningColumn").rdd.glom().collect()
-        self.assertListEqual(partitions1, partitions2)
+        self._sigma_squared = ExactNumber(sigma_squared)
+        self._output_type = DoubleType()
+
+    @property
+    def input_domain(self) -> NumpyDomain:
+        """Return input domain for the measurement."""
+        return cast(NumpyDomain, super().input_domain)
+
+    @property
+    def output_type(self) -> DataType:
+        """Return the output data type after being used as a UDF."""
+        return self._output_type
+
+    @property
+    def sigma_squared(self) -> ExactNumber:
+        """Returns the noise scale."""
+        return self._sigma_squared
+
+    @typechecked
+    def privacy_function(self, d_in: ExactNumberInput) -> ExactNumber:
+        r"""Returns the smallest d_out satisfied by the measurement.
+
+        The returned d_out is :math:`\frac{d_{in}^2}{2 \cdot \sigma^2}`
+        (:math:`\infty` if :math:`\sigma^2 = 0`).
+
+        where:
+
+        * :math:`d_{in}` is the input argument "d_in"
+        * :math:`\sigma^2` is :attr:`~.sigma_squared`
+
+        See Proposition 1.6 in `this <https://arxiv.org/pdf/1605.02065.pdf>`_ paper.
+
+        Args:
+            d_in: Distance between inputs under input_metric.
+        """
+        self.input_metric.validate(d_in)
+        if self.sigma_squared == 0:
+            return ExactNumber(float("inf"))
+        return (ExactNumber(d_in) ** 2) / (2 * self._sigma_squared)
+
+    def __call__(
+        self, value: Union[np.int32, np.int64, np.float32, np.float64, float, int]
+    ) -> float:
+        r"""Adds Gaussian noise with specified scale.
+
+        The added noise has the probability density function
+
+        .. math::
+
+            f(x) = \frac
+            {e^{-(x-\mu)^2/2\sigma^2}}
+            {\sqrt{2\pi}\sigma}
+
+        If :math:`\sigma^2 = \infty`) then the
+        value returned is (:math:`\infty` with probability 1/2 and
+        :math:`-\infty` with probability 1/2
+        """
+        if not self.sigma_squared.is_finite:
+            return random.choice([float("inf"), -float("inf")])
+
+        float_scale = self.sigma_squared.to_float(round_up=True)
+        return float(value + gaussian(u=0, sigma_squared=float_scale))
```

### Comparing `tmlt_core-0.9.1/test/unit/random/test_continuous_gaussian.py` & `tmlt_core-0.9.2/test/unit/random/test_continuous_gaussian.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests for :mod:`~tmlt.core.random.continuous_gaussian`."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
+import math
 from unittest import TestCase
 
 from parameterized import parameterized
 from scipy.stats import norm
 
 from tmlt.core.random.continuous_gaussian import gaussian_inverse_cdf
 from tmlt.core.utils.arb import Arb
@@ -30,20 +31,23 @@
         """`gaussian_inverse_cdf` raises error when called with bad arguments."""
         with self.assertRaisesRegex(ValueError, error_msg):
             gaussian_inverse_cdf(u, b, Arb.from_float(p), 63)
 
     @parameterized.expand(
         [
             (0, 1, 0.5),
+            (10, 100, 0.1),
             (10, 100, 0.5),
-            (10, 100, 0.5),
+            (10, 100, 0.9),
             (0, 1, 0.9),
-            (0, 1, 0.1),
-            (-10, 0.5, 0.2),
+            (0, 5, 0.1),
+            (2000, 5, 0.1),
+            (-10, 0.5, 0.5),
+            (-10, 0.5, 0.09),
         ]
     )
-    def test_correctness(self, u: float, b: float, p: float):
+    def test_correctness(self, u: float, sigma_squared: float, p: float):
         """Sanity tests for :func:`gaussian_inverse_cdf`."""
         self.assertAlmostEqual(
-            float(gaussian_inverse_cdf(u, b, Arb.from_float(p), 63)),
-            norm.ppf(p, loc=u, scale=b),
+            float(gaussian_inverse_cdf(u, sigma_squared, Arb.from_float(p), 63)),
+            norm.ppf(p, loc=u, scale=math.sqrt(sigma_squared)),
         )
```

### Comparing `tmlt_core-0.9.1/test/unit/random/test_discrete_gaussian.py` & `tmlt_core-0.9.2/test/unit/random/test_discrete_gaussian.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/random/test_inverse_cdf.py` & `tmlt_core-0.9.2/test/unit/random/test_inverse_cdf.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/random/test_laplace.py` & `tmlt_core-0.9.2/test/unit/random/test_laplace.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/random/test_rng.py` & `tmlt_core-0.9.2/test/unit/random/test_rng.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/random/test_uniform.py` & `tmlt_core-0.9.2/test/unit/random/test_uniform.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/test_measures.py` & `tmlt_core-0.9.2/test/unit/test_measures.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/test_metrics.py` & `tmlt_core-0.9.2/test/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_add_remove_keys.py` & `tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_add_remove_keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # <placeholder: boilerplate>
 import re
 from typing import Dict, Type
 
 import pandas as pd
 from parameterized import parameterized, parameterized_class
 
-from tmlt.core.domains.collections import DictDomain, ListDomain
+from tmlt.core.domains.collections import DictDomain, DomainKeyError, ListDomain
 from tmlt.core.domains.numpy_domains import NumpyIntegerDomain
 from tmlt.core.domains.spark_domains import (
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkIntegerColumnDescriptor,
     SparkRowDomain,
     SparkStringColumnDescriptor,
@@ -405,15 +405,15 @@
         )
         self.assertTrue(self.mock_filter_value.stability_relation(d_in, expected_d_out))
 
     @parameterized.expand(
         [
             (
                 "'key4' is not one of the input domain's keys",
-                KeyError,
+                DomainKeyError,
                 {"key": "key4"},
                 {},
             ),
             (
                 "'key2' is already a key in the input domain",
                 ValueError,
                 {"new_key": "key2"},
```

### Comparing `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_agg.py` & `tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_agg.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import numpy as np
 import pandas as pd
 from parameterized import parameterized
 
 from tmlt.core.domains.numpy_domains import NumpyIntegerDomain
 from tmlt.core.domains.spark_domains import (
+    DomainColumnError,
     SparkColumnsDescriptor,
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkGroupedDataFrameDomain,
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
 )
@@ -589,15 +590,15 @@
         self,
         sum_column: str,
         lower: ExactNumberInput,
         upper: ExactNumberInput,
         error_message: str,
     ):
         """Sum raises appropriate error when constructor arguments are invalid."""
-        with self.assertRaisesRegex(ValueError, error_message):
+        with self.assertRaisesRegex((ValueError, DomainColumnError), error_message):
             Sum(
                 input_domain=SparkDataFrameDomain(
                     {
                         "A": SparkStringColumnDescriptor(),
                         "B": SparkIntegerColumnDescriptor(),
                         "C": SparkFloatColumnDescriptor(allow_nan=True),
                         "D": SparkIntegerColumnDescriptor(allow_null=True),
@@ -801,15 +802,15 @@
         if schema is None:
             schema = {
                 "A": SparkStringColumnDescriptor(),
                 "B": SparkIntegerColumnDescriptor(),
                 "C": SparkFloatColumnDescriptor(allow_nan=True),
                 "D": SparkIntegerColumnDescriptor(allow_null=True),
             }
-        with self.assertRaisesRegex(ValueError, error_msg):
+        with self.assertRaisesRegex((ValueError, DomainColumnError), error_msg):
             SumGrouped(
                 input_domain=SparkGroupedDataFrameDomain(
                     schema=schema,
                     group_keys=self.spark.createDataFrame(
                         pd.DataFrame({"A": ["x1", "x2"]})
                     ),
                 ),
```

### Comparing `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_filter.py` & `tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 from typing import Union
 
 import pandas as pd
 from parameterized import parameterized
 
-from tmlt.core.domains.spark_domains import SparkDataFrameDomain
+from tmlt.core.domains.spark_domains import DomainColumnError, SparkDataFrameDomain
 from tmlt.core.metrics import (
     HammingDistance,
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
@@ -114,13 +114,13 @@
     def test_if_grouped_by_invalid_parameters(
         self,
         groupby_col: str,
         inner_metric: Union[HammingDistance, SymmetricDifference],
         error_msg: str,
     ):
         """Tests that Filter raises appropriate error with invalid parameters."""
-        with self.assertRaisesRegex(ValueError, error_msg):
+        with self.assertRaisesRegex((ValueError, DomainColumnError), error_msg):
             Filter(
                 domain=SparkDataFrameDomain(self.schema_a),
                 metric=IfGroupedBy(groupby_col, SumOf(inner_metric)),
                 filter_expr="A < 0",
             )
```

### Comparing `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_groupby.py` & `tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_groupby.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     DoubleType,
     LongType,
     StringType,
     StructField,
     StructType,
 )
 
-from tmlt.core.domains.base import OutOfDomainError
 from tmlt.core.domains.spark_domains import (
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkGroupedDataFrameDomain,
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
 )
@@ -102,15 +101,15 @@
     @parameterized.expand(
         [
             (
                 IfGroupedBy("A", SumOf(SymmetricDifference())),
                 [("1",), ("2",)],
                 StructType([StructField("A", StringType())]),
                 r"Column must be LongType(\(\))?, instead it is StringType(\(\))?.",
-                OutOfDomainError,
+                ValueError,
             ),
             (
                 IfGroupedBy("A", RootSumOfSquared(SymmetricDifference())),
                 [(1,), (2,), (3,)],
                 StructType([StructField("A", LongType())]),
                 (
                     "Input metric does not have the expected inner metric. Maybe "
```

### Comparing `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_id.py` & `tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_id.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_join.py` & `tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_join.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import re
 from typing import List, Optional, Union, cast
 
 import pandas as pd
 from parameterized import parameterized
 from pyspark.sql import types as st
 
-from tmlt.core.domains.collections import DictDomain
+from tmlt.core.domains.collections import DictDomain, DomainKeyError
 from tmlt.core.domains.spark_domains import (
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
 )
 from tmlt.core.metrics import (
@@ -818,16 +818,18 @@
                             {"A": SparkIntegerColumnDescriptor()}
                         ),
                     }
                 ),
                 "df1",
                 "df2",
                 ["A"],
-                "'A' has different data types in left (StringType) and right "
-                "(LongType) domains.",
+                (
+                    "'A' has different data types in left (StringType) and right "
+                    "(LongType) domains."
+                ),
             ),
             (  # _right column already exists
                 DictDomain(
                     {
                         "df1": SparkDataFrameDomain(
                             {
                                 "A": SparkStringColumnDescriptor(),
@@ -855,15 +857,15 @@
         input_domain: DictDomain,
         left: str,
         right: str,
         join_cols: Optional[List[str]],
         error_msg: str,
     ):
         """Tests that PrivateJoin cannot be constructed with invalid arguments."""
-        with self.assertRaisesRegex(ValueError, re.escape(error_msg)):
+        with self.assertRaisesRegex((ValueError, DomainKeyError), re.escape(error_msg)):
             PrivateJoin(
                 input_domain=input_domain,
                 left_key=left,
                 right_key=right,
                 left_truncation_strategy=TruncationStrategy.TRUNCATE,
                 right_truncation_strategy=TruncationStrategy.TRUNCATE,
                 left_truncation_threshold=1,
```

### Comparing `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_map.py` & `tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_map.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_nan.py` & `tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_nan.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import re
 from typing import Any, Dict, List, Tuple, Union
 
 from parameterized import parameterized
 from pyspark.sql import Row
 
 from tmlt.core.domains.spark_domains import (
+    DomainColumnError,
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
 )
 from tmlt.core.metrics import (
     AbsoluteDifference,
@@ -151,15 +152,15 @@
     def test_invalid_constructor_args(
         self,
         error_msg: str,
         columns: List[str],
         input_metric: Union[SymmetricDifference, IfGroupedBy] = SymmetricDifference(),
     ) -> None:
         """DropInfs raises an appropriate error on invalid constructor arguments."""
-        with self.assertRaisesRegex(ValueError, error_msg):
+        with self.assertRaisesRegex((ValueError, DomainColumnError), error_msg):
             DropInfs(
                 input_domain=self.input_domain, metric=input_metric, columns=columns
             )
 
     @parameterized.expand(
         [
             (SymmetricDifference(),),
@@ -263,15 +264,15 @@
     def test_invalid_constructor_args(
         self,
         error_msg: str,
         columns: List[str],
         input_metric: Union[SymmetricDifference, IfGroupedBy] = SymmetricDifference(),
     ):
         """DropNaNs raises appropriate errors on invalid constructor arguments."""
-        with self.assertRaisesRegex(ValueError, error_msg):
+        with self.assertRaisesRegex((ValueError, DomainColumnError), error_msg):
             DropNaNs(
                 input_domain=self.input_domain, metric=input_metric, columns=columns
             )
 
     @parameterized.expand(
         [
             (SymmetricDifference(),),
@@ -402,15 +403,15 @@
     def test_invalid_constructor_args(
         self,
         error_msg: str,
         columns: List[str],
         input_metric: Union[SymmetricDifference, IfGroupedBy] = SymmetricDifference(),
     ):
         """DropNulls raises appropriate errors on invalid constructor arguments."""
-        with self.assertRaisesRegex(ValueError, error_msg):
+        with self.assertRaisesRegex((ValueError, DomainColumnError), error_msg):
             DropNulls(
                 input_domain=self.input_domain, metric=input_metric, columns=columns
             )
 
     @parameterized.expand(
         [
             (SymmetricDifference(),),
@@ -570,15 +571,15 @@
     def test_invalid_constructor_args(
         self,
         error_msg: str,
         replace_map: Dict[str, Tuple[float, float]],
         input_metric: Union[SymmetricDifference, IfGroupedBy] = SymmetricDifference(),
     ) -> None:
         """ReplaceInfs raises appropriate errors on invalid constructor arguments."""
-        with self.assertRaisesRegex(ValueError, error_msg):
+        with self.assertRaisesRegex((ValueError, DomainColumnError), error_msg):
             ReplaceInfs(
                 input_domain=self.input_domain,
                 metric=input_metric,
                 replace_map=replace_map,
             )
 
     @parameterized.expand(
@@ -727,15 +728,15 @@
     def test_invalid_constructor_args(
         self,
         error_msg: str,
         replace_map: Dict[str, Any],
         input_metric: Union[SymmetricDifference, IfGroupedBy] = SymmetricDifference(),
     ):
         """ReplaceNaNs raises appropriate errors on invalid constructor arguments."""
-        with self.assertRaisesRegex(ValueError, error_msg):
+        with self.assertRaisesRegex((ValueError, DomainColumnError), error_msg):
             ReplaceNaNs(
                 input_domain=self.input_domain,
                 metric=input_metric,
                 replace_map=replace_map,
             )
 
     @parameterized.expand(
@@ -884,15 +885,15 @@
     def test_invalid_constructor_args(
         self,
         error_msg: str,
         replace_map: Dict[str, Any],
         input_metric: Union[SymmetricDifference, IfGroupedBy] = SymmetricDifference(),
     ):
         """ReplaceNulls raises appropriate errors on invalid constructor arguments."""
-        with self.assertRaisesRegex(ValueError, error_msg):
+        with self.assertRaisesRegex((ValueError, DomainColumnError), error_msg):
             ReplaceNulls(
                 input_domain=self.input_domain,
                 metric=input_metric,
                 replace_map=replace_map,
             )
 
     @parameterized.expand(
```

### Comparing `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_partition.py` & `tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_partition.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_persist.py` & `tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_persist.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_rename.py` & `tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_rename.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright Tumult Labs 2022
 
 from typing import Dict, Union
 
 import pandas as pd
 from parameterized import parameterized
 
-from tmlt.core.domains.spark_domains import SparkDataFrameDomain
+from tmlt.core.domains.spark_domains import DomainColumnError, SparkDataFrameDomain
 from tmlt.core.metrics import (
     HammingDistance,
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
@@ -118,16 +118,20 @@
             [[1.2, "X"]],
             columns=[rename_mapping.get("A", "A"), rename_mapping.get("B", "B")],
         )
         self.assert_frame_equal_with_sort(actual_df, expected_df)
 
     @parameterized.expand([({"D": "E"},), ({"A": "B"},)])
     def test_rename_fails_on_bad_columns(self, rename_mapping: Dict[str, str]):
-        """Tests that rename transformation fails when column doesn not exist."""
-        with self.assertRaises(ValueError):
+        """Tests that rename transformation fails when column doesn not exist.
+
+        Also tests that rename transformation fails when the new column name
+        already exists.
+        """
+        with self.assertRaises((DomainColumnError, ValueError)):
             Rename(
                 input_domain=SparkDataFrameDomain(self.schema_a),
                 metric=SymmetricDifference(),
                 rename_mapping=rename_mapping,
             )
 
     @parameterized.expand(
```

### Comparing `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_select.py` & `tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright Tumult Labs 2022
 
 from typing import List, Union
 
 import pandas as pd
 from parameterized import parameterized
 
-from tmlt.core.domains.spark_domains import SparkDataFrameDomain
+from tmlt.core.domains.spark_domains import DomainColumnError, SparkDataFrameDomain
 from tmlt.core.metrics import (
     HammingDistance,
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
@@ -96,15 +96,15 @@
         actual_df = select_transformation(self.df_a).toPandas()
         expected_df = pd.DataFrame({"B": ["X"]})
         self.assert_frame_equal_with_sort(actual_df, expected_df)
 
     @parameterized.expand([(["A", "D"],), (["D"],), (["A", "A", "B"],)])
     def test_select_fails_on_bad_columns(self, columns: List[str]):
         """Tests that rename transformation fails when columns are invalid."""
-        with self.assertRaises(ValueError):
+        with self.assertRaises((ValueError, DomainColumnError)):
             Select(
                 input_domain=SparkDataFrameDomain(self.schema_a),
                 metric=SymmetricDifference(),
                 columns=columns,
             )
 
     @parameterized.expand(
@@ -123,13 +123,13 @@
         self,
         select_columns: List[str],
         groupby_col: str,
         inner_metric: Union[SumOf, RootSumOfSquared, SymmetricDifference],
         error_msg: str,
     ):
         """Tests that Select raises appropriate errors with invalid params."""
-        with self.assertRaisesRegex(ValueError, error_msg):
+        with self.assertRaisesRegex((ValueError, DomainColumnError), error_msg):
             Select(
                 input_domain=SparkDataFrameDomain(self.schema_a),
                 metric=IfGroupedBy(groupby_col, inner_metric),
                 columns=select_columns,
             )
```

### Comparing `tmlt_core-0.9.1/test/unit/transformations/spark_transformations/test_truncation.py` & `tmlt_core-0.9.2/test/unit/transformations/spark_transformations/test_truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/transformations/test_chaining.py` & `tmlt_core-0.9.2/test/unit/transformations/test_chaining.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/transformations/test_converters.py` & `tmlt_core-0.9.2/test/unit/transformations/test_converters.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/transformations/test_dictionary.py` & `tmlt_core-0.9.2/test/unit/transformations/test_dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from unittest.case import TestCase
 from unittest.mock import call
 
 import numpy as np
 from parameterized import parameterized
 
 from tmlt.core.domains.base import Domain
-from tmlt.core.domains.collections import DictDomain
+from tmlt.core.domains.collections import DictDomain, DomainKeyError
 from tmlt.core.domains.numpy_domains import NumpyFloatDomain, NumpyIntegerDomain
 from tmlt.core.domains.spark_domains import (
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
 )
@@ -319,15 +319,17 @@
         self,
         error_regex: str,
         input_domain: DictDomain,
         input_metric: DictMetric,
         key: str,
     ):
         """Tests that GetValue raises errors appropriately."""
-        with self.assertRaisesRegex((ValueError, KeyError), re.escape(error_regex)):
+        with self.assertRaisesRegex(
+            (ValueError, DomainKeyError), re.escape(error_regex)
+        ):
             GetValue(input_domain=input_domain, input_metric=input_metric, key=key)
 
     @parameterized.expand(
         [
             (
                 DictMetric(
                     {
@@ -525,15 +527,17 @@
         self,
         error_message: str,
         input_domain: DictDomain,
         input_metric: DictMetric,
         keys: List[str],
     ):
         """Tests that Subset raises errors appropriately."""
-        with self.assertRaisesRegex(ValueError, re.escape(error_message)):
+        with self.assertRaisesRegex(
+            (ValueError, DomainKeyError), re.escape(error_message)
+        ):
             Subset(input_domain=input_domain, input_metric=input_metric, keys=keys)
 
     @parameterized.expand(
         [
             (
                 DictMetric(
                     {"key1": SymmetricDifference(), "key2": SymmetricDifference()}
@@ -755,15 +759,15 @@
                 "ignore_me": "nothing to see here",
                 "halved": np.float64(1),
             },
         )
 
     def test_create_copy_and_transform_value_invalid_key(self):
         """Raises an error if key is not in the domain."""
-        with self.assertRaisesRegex(ValueError, "key is not in the domain"):
+        with self.assertRaisesRegex(DomainKeyError, "key .* is not in the domain"):
             create_copy_and_transform_value(
                 input_domain=DictDomain(
                     {
                         "halve_me": NumpyIntegerDomain(),
                         "ignore_me": NumpyIntegerDomain(),
                     }
                 ),
@@ -845,15 +849,15 @@
         )
         self.assertEqual(
             rename(data), {"renamed": np.int64(2), "ignore_me": "nothing to see here"}
         )
 
     def test_create_rename_invalid_key(self):
         """Raises an error if key is not in the domain."""
-        with self.assertRaisesRegex(ValueError, "key is not in the domain"):
+        with self.assertRaisesRegex(DomainKeyError, "key .* is not in the domain"):
             create_rename(
                 input_domain=DictDomain(
                     {
                         "rename_me": NumpyIntegerDomain(),
                         "ignore_me": NumpyIntegerDomain(),
                     }
                 ),
@@ -983,15 +987,15 @@
         self.assertEqual(
             transform_value(data),
             {"halve_me": np.float64(1), "ignore_me": "nothing to see here"},
         )
 
     def test_create_transform_value_invalid_key(self):
         """Raises an error if key is not in the domain."""
-        with self.assertRaisesRegex(ValueError, "key is not in the domain"):
+        with self.assertRaisesRegex(DomainKeyError, "key .* is not in the domain"):
             create_transform_value(
                 input_domain=DictDomain(
                     {
                         "halve_me": NumpyIntegerDomain(),
                         "ignore_me": NumpyIntegerDomain(),
                     }
                 ),
```

### Comparing `tmlt_core-0.9.1/test/unit/transformations/test_identity.py` & `tmlt_core-0.9.2/test/unit/transformations/test_identity.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/utils/test_arb.py` & `tmlt_core-0.9.2/test/unit/utils/test_arb.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/utils/test_cleanup.py` & `tmlt_core-0.9.2/test/unit/utils/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/utils/test_configuration.py` & `tmlt_core-0.9.2/test/unit/utils/test_configuration.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/utils/test_distributions.py` & `tmlt_core-0.9.2/test/unit/utils/test_distributions.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/utils/test_exact_number.py` & `tmlt_core-0.9.2/test/unit/utils/test_exact_number.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/utils/test_grouped_dataframe.py` & `tmlt_core-0.9.2/test/unit/utils/test_grouped_dataframe.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/utils/test_join.py` & `tmlt_core-0.9.2/test/unit/utils/test_join.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/utils/test_misc.py` & `tmlt_core-0.9.2/test/unit/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/utils/test_testing.py` & `tmlt_core-0.9.2/test/unit/utils/test_testing.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/test/unit/utils/test_truncation.py` & `tmlt_core-0.9.2/test/unit/utils/test_truncation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 """Tests for :mod:`~tmlt.core.utils.truncation`."""
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
 import itertools
 from typing import List, Tuple
+from unittest.mock import patch
 
 import pandas as pd
 from parameterized import parameterized
+from pyspark.sql.functions import udf
+from pyspark.sql.types import IntegerType
 
 from tmlt.core.utils.testing import PySparkTest
-from tmlt.core.utils.truncation import drop_large_groups, truncate_large_groups
+from tmlt.core.utils.truncation import (
+    drop_large_groups,
+    limit_keys_per_group,
+    truncate_large_groups,
+)
 
 
 class TestTruncateLargeGroups(PySparkTest):
     """Tests for :meth:`~tmlt.core.utils.truncation.truncate_large_groups`."""
 
     @parameterized.expand(
         [
@@ -107,7 +114,28 @@
         self, threshold: int, input_rows: List[Tuple], expected: List[Tuple]
     ) -> None:
         """Tests that drop_large_groups works correctly."""
         df = self.spark.createDataFrame(input_rows, schema=["A", "B"])
         actual = drop_large_groups(df, ["A"], threshold).toPandas()
         expected = pd.DataFrame.from_records(expected, columns=["A", "B"])
         self.assert_frame_equal_with_sort(actual, expected)
+
+
+class TestLimitKeysPerGroup(PySparkTest):
+    """Tests for :func:`~tmlt.core.utils.truncation.limit_keys_per_group`."""
+
+    def test_hash_collisions(self):
+        """Test :func:`~.limit_keys_per_group` works when there are hash collisions.
+
+        This test fails for a previous, incorrect version of
+        :func:`~.limit_keys_per_group`. See
+        https://gitlab.com/tumult-labs/tumult/-/issues/2455 for more details.
+        """
+
+        df = self.spark.createDataFrame(
+            pd.DataFrame({"A": [1, 1, 1, 1, 2, 2, 2, 2], "B": [1, 1, 2, 2, 1, 2, 3, 4]})
+        )
+        # replace the hash function with one that always returns 1
+        hash_collision_mock = udf(lambda _, __: 1, IntegerType())
+        with patch("pyspark.sql.functions.hash", hash_collision_mock):
+            actual = limit_keys_per_group(df, ["A"], ["B"], 1)
+        self.assertEqual(actual.count(), 3)
```

### Comparing `tmlt_core-0.9.1/test/unit/utils/test_type_utils.py` & `tmlt_core-0.9.2/test/unit/utils/test_type_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/domains/base.py` & `tmlt_core-0.9.2/tmlt/core/domains/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,48 @@
 """Base class for input/output domains."""
 
 # SPDX-License-Identifier: Apache-2.0
-# Copyright Tumult Labs 2022
+# Copyright Tumult Labs 2023
+from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Any
 
 
 class OutOfDomainError(Exception):
     """Exception type that indicates a validation error in a Domain."""
 
+    def __init__(self, domain: Domain, value: Any, msg: str):
+        """Constructor.
+
+        Args:
+            domain: The domain on which the exception was raised.
+            value: The value that is not in the domain.
+            msg: The error message.
+        """
+        self.domain = domain
+        self.value = value
+        super().__init__(msg)
+
 
 class Domain(ABC):
     """Base class for input/output domains."""
 
     @property
     @abstractmethod
     def carrier_type(self) -> type:
         """Returns the type of elements in the domain."""
 
     def validate(self, value: Any):
         """Raises an error if value is not in the domain."""
         if value.__class__ is not self.carrier_type:
             raise OutOfDomainError(
-                f"Value must be {self.carrier_type}, instead it is {value.__class__}."
+                self,
+                value,
+                f"Value must be {self.carrier_type}, instead it is {value.__class__}.",
             )
 
     def __contains__(self, value: Any) -> bool:
         """Returns True if value is in the domain."""
         try:
             self.validate(value)
         except OutOfDomainError:
```

### Comparing `tmlt_core-0.9.1/tmlt/core/domains/collections.py` & `tmlt_core-0.9.2/tmlt/core/domains/collections.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,31 @@
 from typing import Any, Dict, Mapping, Optional
 
 from typeguard import check_type, typechecked
 
 from tmlt.core.domains.base import Domain, OutOfDomainError
 
 
+class DomainKeyError(Exception):
+    """Exception type that indicates that a key is not in the given domain."""
+
+    def __init__(self, domain: Domain, key: Any, msg: str):
+        """Constructor.
+
+        Args:
+            domain: The domain on which this error was raised.
+            key: The key that's not in the domain (or a collection of keys that
+                aren't in the domain).
+            msg: The error message.
+        """
+        self.key = key
+        self.domain = domain
+        super().__init__(domain, key, msg)
+
+
 @dataclass(frozen=True, eq=True)
 class ListDomain(Domain):
     """Domain of lists of elements of a particular domain."""
 
     element_domain: Domain
     """Domain of list elements."""
 
@@ -35,15 +52,15 @@
         """Raises error if value is not a row with matching schema."""
         super().validate(value)
         for elem in value:
             try:
                 self.element_domain.validate(elem)
             except OutOfDomainError as exception:
                 raise OutOfDomainError(
-                    f"Found invalid value in list: {exception}"
+                    self, exception.value, f"Found invalid value in list: {exception}"
                 ) from exception
 
 
 class DictDomain(Domain):
     """Domain of dictionaries."""
 
     @typechecked
@@ -86,18 +103,22 @@
 
     def validate(self, value: Any):
         """Raises error if value is not in the domain."""
         super().validate(value)
         value_keys, domain_keys = sorted(set(value)), sorted(set(self.key_to_domain))
         if value_keys != domain_keys:
             raise OutOfDomainError(
-                "Keys are not as expected, value must match domain.\nValue "
-                f"keys: {value_keys}\nDomain keys: {domain_keys}"
+                self,
+                value_keys,
+                (
+                    "Keys are not as expected, value must match domain.\nValue "
+                    f"keys: {value_keys}\nDomain keys: {domain_keys}"
+                ),
             )
 
         for key in value:
             try:
                 self.key_to_domain[key].validate(value[key])
             except OutOfDomainError as exception:
                 raise OutOfDomainError(
-                    f"Found invalid value at '{key}': {exception}"
+                    self, key, f"Found invalid value at '{key}': {exception}"
                 ) from exception
```

### Comparing `tmlt_core-0.9.1/tmlt/core/domains/numpy_domains.py` & `tmlt_core-0.9.2/tmlt/core/domains/numpy_domains.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,17 +78,17 @@
             return np.float32
         return np.float64
 
     def validate(self, value: Any):
         """Raises error if value is not a member of the domain."""
         super().validate(value)
         if not self.allow_inf and np.isinf(value):
-            raise OutOfDomainError("Value is infinite.")
+            raise OutOfDomainError(self, value, "Value is infinite.")
         if not self.allow_nan and np.isnan(value):
-            raise OutOfDomainError("Value is NaN.")
+            raise OutOfDomainError(self, value, "Value is NaN.")
 
 
 @dataclass(frozen=True)
 class NumpyStringDomain(NumpyDomain):
     """Domain of NumPy strings.
 
     Note:
@@ -103,16 +103,16 @@
         """Checks arguments to constructor."""
         check_type("allow_null", self.allow_null, bool)
 
     def validate(self, value: Any):
         """Raises error if value is not in domain."""
         if not isinstance(value, self.carrier_type) and value.__class__ is not str:
             raise OutOfDomainError(
-                f"Value must be {str}, instead it is {value.__class__}."
+                self, value, f"Value must be {str}, instead it is {value.__class__}."
             )
         if value is None and not self.allow_null:
-            raise OutOfDomainError("Value is null.")
+            raise OutOfDomainError(self, value, "Value is null.")
 
     @property
     def carrier_type(self) -> type:  # pylint: disable=no-self-use
         """Returns carrier types for members of NumpyStringDomain."""
         return object
```

### Comparing `tmlt_core-0.9.1/tmlt/core/domains/pandas_domains.py` & `tmlt_core-0.9.2/tmlt/core/domains/pandas_domains.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         # retrieving the corresponding python object
         super().validate(value)
         for i in range(len(value)):  # pylint: disable=consider-using-enumerate
             try:
                 self.element_domain.validate(value[i])
             except OutOfDomainError as exception:
                 raise OutOfDomainError(
-                    f"Found invalid value in Series: {exception}"
+                    self, value, f"Found invalid value in Series: {exception}"
                 ) from exception
 
     @classmethod
     def from_numpy_type(cls, dtype: np.dtype) -> "PandasSeriesDomain":
         """Returns a Pandas Series from a NumPy type."""
         return PandasSeriesDomain(NumpyDomain.from_np_type(dtype))
 
@@ -89,30 +89,38 @@
         """Raises error if value is not a Pandas DataFrame with matching schema."""
         super().validate(value)
         value_columns = list(value.columns)
         if len(value_columns) > len(set(value_columns)):
             duplicates = set(
                 col for col in value_columns if value_columns.count(col) > 1
             )
-            raise OutOfDomainError(f"Some columns are duplicated, {sorted(duplicates)}")
+            raise OutOfDomainError(
+                self, value, f"Some columns are duplicated, {sorted(duplicates)}"
+            )
 
         schema_columns = list(self.schema.keys())
         if value_columns != schema_columns:
             raise OutOfDomainError(
-                "Columns are not as expected. DataFrame and Domain must contain the "
-                f"same columns in the same order.\nDataFrame columns: {value_columns}\n"
-                f"Domain columns: {schema_columns}"
+                self,
+                value,
+                (
+                    "Columns are not as expected. DataFrame and Domain must contain"
+                    " the same columns in the same order.\nDataFrame columns:"
+                    f" {value_columns}\nDomain columns: {schema_columns}"
+                ),
             )
 
         for column in self.schema:
             try:
                 self.schema[column].validate(value[column])
             except OutOfDomainError as exception:
                 raise OutOfDomainError(
-                    f"Found invalid value in column '{column}': {exception}"
+                    self,
+                    value,
+                    f"Found invalid value in column '{column}': {exception}",
                 ) from exception
 
     def __eq__(self, other: Any) -> bool:
         """Return True if the classes are equivalent."""
         if self.__class__ != other.__class__:
             return False
         return OrderedDict(self.schema) == OrderedDict(other.schema)
```

### Comparing `tmlt_core-0.9.1/tmlt/core/domains/spark_domains.py` & `tmlt_core-0.9.2/tmlt/core/domains/spark_domains.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright Tumult Labs 2022
 
 import datetime
 import warnings
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from dataclasses import dataclass
-from typing import Any, Mapping, Optional, Sequence
+from typing import Any, Collection, Mapping, Optional, Sequence, Union
 
 import numpy as np
 from pyspark import Row
 from pyspark.sql import DataFrame
 from pyspark.sql.types import (
     DataType,
     DateType,
@@ -33,14 +33,31 @@
     NumpyFloatDomain,
     NumpyIntegerDomain,
     NumpyStringDomain,
 )
 from tmlt.core.domains.pandas_domains import PandasDataFrameDomain
 
 
+class DomainColumnError(Exception):
+    """Exception type for when a column is not in the given domain's schema."""
+
+    def __init__(self, domain: Domain, column: Union[str, Collection[str]], msg: str):
+        """Constructor.
+
+        Args:
+            domain: The domain on which this error was raised.
+            column: The column that's not in the domain's schema, or a collection of
+                columns that are not in the domain's schema.
+            msg: The error message.
+        """
+        self.domain = domain
+        self.column = column
+        super().__init__(msg)
+
+
 class SparkColumnDescriptor(ABC):
     """Base class for describing Spark column types.
 
     Attributes:
         allow_null: If True, null values are permitted in the domain.
     """
 
@@ -54,23 +71,23 @@
         """Raises error if not all values in given DataFrame column match descriptor.
 
         Args:
             sdf: Spark DataFrame to check.
             col_name: Name of column in sdf to be checked.
         """
         if col_name not in sdf.schema.fieldNames():
-            raise OutOfDomainError(f"'{col_name}' is not in the DataFrame")
+            raise ValueError(f"'{col_name}' is not in the DataFrame")
         if sdf.schema[col_name].dataType.__class__ is not self.data_type.__class__:
-            raise OutOfDomainError(
+            raise ValueError(
                 f"Column must be {self.data_type}, instead it is "
                 f"{sdf.schema[col_name].dataType}."
             )
         if not self.allow_null:
             if sdf.filter(sdf[col_name].isNull()).first():
-                raise OutOfDomainError("Column contains null values.")
+                raise ValueError("Column contains null values.")
 
     @abstractmethod
     def valid_py_value(self, val: Any) -> bool:
         """Returns True if `val` is valid for described Spark column."""
 
     @property
     @abstractmethod
@@ -174,21 +191,21 @@
         Args:
             sdf: Spark DataFrame to check.
             col_name: Name of column in sdf to be checked.
         """
         super().validate_column(sdf, col_name)
         if not self.allow_nan:
             if sdf.filter(sdf[col_name].contains(float("nan"))).first():
-                raise OutOfDomainError("Column contains NaN values.")
+                raise ValueError("Column contains NaN values.")
         if not self.allow_inf:
             if sdf.filter(
                 sdf[col_name].contains(float("inf"))
                 | sdf[col_name].contains(-float("inf"))
             ).first():
-                raise OutOfDomainError("Column contains infinite values.")
+                raise ValueError("Column contains infinite values.")
 
     def valid_py_value(self, val: Any):
         """Returns True if value is a valid python value for the descriptor.
 
         In particular, this returns True only if one of the following is true:
 
         - val is `float("nan")` and NaN is allowed.
@@ -361,30 +378,38 @@
         """Raises error if value is not a DataFrame with matching schema."""
         super().validate(value)
         value_columns = list(value.schema.fieldNames())
         if len(value_columns) > len(set(value_columns)):
             duplicates = set(
                 col for col in value_columns if value_columns.count(col) > 1
             )
-            raise OutOfDomainError(f"Some columns are duplicated, {sorted(duplicates)}")
+            raise OutOfDomainError(
+                self, value, f"Some columns are duplicated, {sorted(duplicates)}"
+            )
 
         schema_columns = list(self.schema.keys())
         if value_columns != schema_columns:
             raise OutOfDomainError(
-                "Columns are not as expected. DataFrame and Domain must contain the "
-                f"same columns in the same order.\nDataFrame columns: {value_columns}\n"
-                f"Domain columns: {schema_columns}"
+                self,
+                value,
+                (
+                    "Columns are not as expected. DataFrame and Domain must contain"
+                    " the same columns in the same order.\nDataFrame columns:"
+                    f" {value_columns}\nDomain columns: {schema_columns}"
+                ),
             )
 
         for column in self.schema:
             try:
                 self.schema[column].validate_column(value, column)
-            except OutOfDomainError as exception:
+            except ValueError as exception:
                 raise OutOfDomainError(
-                    f"Found invalid value in column '{column}': {exception}"
+                    self,
+                    value,
+                    f"Found invalid value in column '{column}': {exception}",
                 ) from exception
 
     def __eq__(self, other: Any) -> bool:
         """Return True if the classes are equivalent."""
         if self.__class__ != other.__class__:
             return False
         return OrderedDict(self.schema) == OrderedDict(other.schema)
@@ -550,16 +575,20 @@
             GroupedDataFrame,
         )
 
         super().validate(value)
         assert isinstance(value, GroupedDataFrame)
         if value.group_keys.schema != self.group_keys.schema:
             raise OutOfDomainError(
-                "Group keys dataframe does not have expected schema."
-                f"Expected: {self.group_keys.schema}. Got: {value.group_keys.schema}"
+                self,
+                value,
+                (
+                    "Group keys dataframe does not have expected schema.Expected:"
+                    f" {self.group_keys.schema}. Got: {value.group_keys.schema}"
+                ),
             )
 
         if not self.group_keys.columns:
             # Other checks are not necessary if there are no columns.
             return
 
         # Note that we are using an inner join instead of intersect
@@ -581,31 +610,35 @@
         # this join duplicates columns, drop the duplicates
         for column in value_group_keys.columns:
             intersection = intersection.drop(value_group_keys[column])
         invalid_group_keys = self.group_keys.union(value_group_keys).subtract(
             intersection
         )
         if invalid_group_keys.first():
-            raise OutOfDomainError("Groups keys do not match")
+            raise OutOfDomainError(self, value, "Groups keys do not match")
 
         if value._dataframe.columns != list(  # pylint: disable=protected-access
             self.schema.keys()
         ):
             raise OutOfDomainError(
-                "Dataframe does not match domain SparkGroupedDataFrame schema."
+                self,
+                value,
+                "Dataframe does not match domain SparkGroupedDataFrame schema.",
             )
 
         for column in self.schema:
             try:
                 self.schema[column].validate_column(
                     value._dataframe, column  # pylint: disable=protected-access
                 )
             except OutOfDomainError as exception:
                 raise OutOfDomainError(
-                    f"Found invalid value in column '{column}': {exception}"
+                    self,
+                    value,
+                    f"Found invalid value in column '{column}': {exception}",
                 ) from exception
 
     def get_group_domain(self) -> SparkDataFrameDomain:
         """Return the domain for one of the groups."""
         groupby_columns = self.group_keys.columns
         group_schema = {
             column: v
```

### Comparing `tmlt_core-0.9.1/tmlt/core/measurements/aggregations.py` & `tmlt_core-0.9.2/tmlt/core/measurements/aggregations.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,23 +37,25 @@
     AddNoiseToSeries,
     NoisyQuantile,
 )
 from tmlt.core.measurements.postprocess import PostProcess
 from tmlt.core.measurements.spark_measurements import (
     AddNoiseToColumn,
     ApplyInPandas,
+    BoundSelection,
     GeometricPartitionSelection,
 )
 from tmlt.core.measures import (
     ApproxDP,
     ApproxDPBudget,
     PrivacyBudget,
     PrivacyBudgetInput,
     PureDP,
     RhoZCDP,
+    RhoZCDPBudget,
 )
 from tmlt.core.metrics import (
     HammingDistance,
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
@@ -1919,7 +1921,94 @@
         )
     return GeometricPartitionSelection(
         input_domain=input_domain,
         threshold=threshold,
         alpha=alpha,
         count_column=count_column,
     )
+
+
+@typechecked
+def create_bound_selection_measurement(
+    input_domain: SparkDataFrameDomain,
+    output_measure: Union[PureDP, ApproxDP, RhoZCDP],
+    d_out: PrivacyBudgetInput,
+    bound_column: str,
+    threshold: float,
+    d_in: ExactNumberInput = 1,
+) -> Measurement:
+    """Returns a bound selection measurement.
+
+    A bound selection measurement created by this function will have a
+    privacy guarantee such that
+    ``measurement.privacy_function(d_in) = epsilon``.
+
+    Args:
+        input_domain: Domain of the input Spark DataFrames.
+        output_measure: Desired privacy guarantee.
+        d_out: Desired distance between output distributions w.r.t. `d_in`. This is
+            interpreted as "epsilon" if output_measure is :class:`~.PureDP`, "rho" if it
+            is :class:`~.RhoZCDP`, and ("epsilon", "delta") if it is
+            :class:`~.ApproxDP`.
+        bound_column: Column name to calculate the bounds for. The column
+            must be an integer or floating point column.
+        threshold: The threshold for the bound selection measurement.
+        d_in: The given d_in such that
+            ``measurement.privacy_function(d_in) = epsilon``.
+    """
+    d_in = ExactNumber(d_in)
+    alpha: ExactNumber
+
+    if isinstance(output_measure, ApproxDP):
+        epsilon, delta = ApproxDPBudget(d_out).value
+        if delta > 0:
+            raise ValueError(
+                "Cannot spend an ApproxDP budget with delta > 0."
+                "Use RhoZCDP, ApproxDP with delta = 0, or PureDP."
+            )
+        return PureDPToApproxDP(
+            create_bound_selection_measurement(
+                input_domain=input_domain,
+                output_measure=PureDP(),
+                d_out=epsilon,
+                bound_column=bound_column,
+                threshold=threshold,
+                d_in=d_in,
+            )
+        )
+
+    if isinstance(output_measure, RhoZCDP):
+        rho = RhoZCDPBudget(d_out).value
+        epsilon = sp.sqrt(ExactNumber(sp.Integer(2) * rho).expr)
+        return PureDPToRhoZCDP(
+            create_bound_selection_measurement(
+                input_domain=input_domain,
+                output_measure=PureDP(),
+                d_out=epsilon,
+                bound_column=bound_column,
+                threshold=threshold,
+                d_in=d_in,
+            )
+        )
+
+    if isinstance(output_measure, PureDP):
+        d_out = PrivacyBudget.cast(output_measure, d_out).value
+    else:
+        assert False
+    if d_in < 1:
+        raise NotImplementedError(
+            "Creating a partition selection measurement with d_in < 1 is not yet"
+            " supported."
+        )
+
+    # Special case for infinite privacy budget
+    if d_out == float("inf"):
+        alpha = ExactNumber(0)
+    # Normal cases
+    else:
+        alpha = (4 / d_out) * d_in
+    return BoundSelection(
+        input_domain=input_domain,
+        threshold=threshold,
+        alpha=alpha,
+        bound_column=bound_column,
+    )
```

### Comparing `tmlt_core-0.9.1/tmlt/core/measurements/base.py` & `tmlt_core-0.9.2/tmlt/core/measurements/base.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/measurements/chaining.py` & `tmlt_core-0.9.2/tmlt/core/measurements/chaining.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/measurements/composition.py` & `tmlt_core-0.9.2/tmlt/core/measurements/composition.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/measurements/converters.py` & `tmlt_core-0.9.2/tmlt/core/measurements/converters.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/measurements/interactive_measurements.py` & `tmlt_core-0.9.2/tmlt/core/measurements/interactive_measurements.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/measurements/pandas_measurements/dataframe.py` & `tmlt_core-0.9.2/tmlt/core/measurements/pandas_measurements/dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Callable, Dict, Mapping, Optional, Union, cast
 
 import pandas as pd
 from pyspark.sql.types import StructField, StructType
 from typeguard import check_type, typechecked
 
 from tmlt.core.domains.pandas_domains import PandasDataFrameDomain
+from tmlt.core.domains.spark_domains import DomainColumnError
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measurements.pandas_measurements.series import (
     Aggregate as AggregateSeries,
 )
 from tmlt.core.measures import Measure, PureDP, RhoZCDP
 from tmlt.core.metrics import HammingDistance, SymmetricDifference
 from tmlt.core.utils.exact_number import ExactNumber, ExactNumberInput
@@ -96,15 +97,19 @@
         """
         if not column_to_aggregation:
             raise ValueError("No aggregations provided.")
         # Check that the aggregation functions are compatible with DataFrame
         # aggregation.
         for column, aggregation_function in column_to_aggregation.items():
             if column not in input_domain.schema:
-                raise ValueError(f"Column '{column}' is not in the input schema.")
+                raise DomainColumnError(
+                    input_domain,
+                    column,
+                    f"Column '{column}' is not in the input schema.",
+                )
             if input_domain.schema[column] != aggregation_function.input_domain:
                 raise ValueError(
                     "The input domain is not compatible with the input domains of the"
                     " aggregation functions."
                 )
 
         # Check that all aggregation functions have the same input metric, and that
```

### Comparing `tmlt_core-0.9.1/tmlt/core/measurements/pandas_measurements/series.py` & `tmlt_core-0.9.2/tmlt/core/measurements/pandas_measurements/series.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/measurements/postprocess.py` & `tmlt_core-0.9.2/tmlt/core/measurements/postprocess.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/measurements/spark_measurements.py` & `tmlt_core-0.9.2/tmlt/core/measurements/spark_measurements.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,37 +2,42 @@
 # TODO(#1320): Add link to privacy and stability tutorial
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
 import uuid
 from abc import abstractmethod
+from itertools import accumulate
 from threading import Lock
-from typing import Any, Optional, Tuple, Union, cast
+from typing import Any, List, Optional, Tuple, Union, cast
 
+import numpy as np
+import pandas as pd
 import sympy as sp
+from pyspark.ml.feature import Bucketizer
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql import functions as sf
 from typeguard import typechecked
 
 # cleanup is imported just so its cleanup function runs at exit
 import tmlt.core.utils.cleanup  # pylint: disable=unused-import
 from tmlt.core.domains.spark_domains import (
+    SparkColumnDescriptor,
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkGroupedDataFrameDomain,
     SparkIntegerColumnDescriptor,
     SparkStringColumnDescriptor,
     convert_pandas_domain,
 )
 from tmlt.core.measurements.base import Measurement
 from tmlt.core.measurements.noise_mechanisms import AddGeometricNoise
 from tmlt.core.measurements.pandas_measurements.dataframe import Aggregate
 from tmlt.core.measurements.pandas_measurements.series import AddNoiseToSeries
-from tmlt.core.measures import ApproxDP
+from tmlt.core.measures import ApproxDP, PureDP
 from tmlt.core.metrics import OnColumn, RootSumOfSquared, SumOf, SymmetricDifference
 from tmlt.core.utils.configuration import Config
 from tmlt.core.utils.distributions import double_sided_geometric_cmf_exact
 from tmlt.core.utils.exact_number import ExactNumber, ExactNumberInput
 from tmlt.core.utils.grouped_dataframe import GroupedDataFrame
 from tmlt.core.utils.misc import get_nonconflicting_string
 from tmlt.core.utils.validation import validate_exact_number
@@ -542,14 +547,268 @@
             measurement=AddNoiseToSeries(AddGeometricNoise(self.alpha)),
             measure_column=self.count_column,
         )
         noisy_count_df = internal_measurement(count_df)
         return noisy_count_df.filter(sf.col(self.count_column) >= self.threshold)
 
 
+class BoundSelection(Measurement):
+    r"""Discovers a noisy bound based on a DataFrame Column.
+
+    Example:
+        ..
+            >>> import pandas as pd
+            >>> from tmlt.core.utils.misc import print_sdf
+            >>> spark = SparkSession.builder.getOrCreate()
+            >>> spark_dataframe = spark.createDataFrame(
+            ...     pd.DataFrame(
+            ...         {
+            ...             "A": ["a1"] * 100,
+            ...             "B": [10] * 10 + [20] * 20 + [30] * 30 + [40] * 40,
+            ...         }
+            ...     )
+            ... )
+            >>> min_bound, max_bound = -64, 64
+
+        >>> # Example input
+        >>> print_sdf(spark_dataframe)
+             A   B
+        0   a1  10
+        1   a1  10
+        2   a1  10
+        3   a1  10
+        4   a1  10
+        ..  ..  ..
+        95  a1  40
+        96  a1  40
+        97  a1  40
+        98  a1  40
+        99  a1  40
+        <BLANKLINE>
+        [100 rows x 2 columns]
+        >>> measurement = BoundSelection(
+        ...     input_domain=SparkDataFrameDomain(
+        ...         schema={
+        ...             "A": SparkStringColumnDescriptor(),
+        ...             "B": SparkIntegerColumnDescriptor(),
+        ...         },
+        ...     ),
+        ...     bound_column="B",
+        ...     alpha=1,
+        ...     threshold=0.95,
+        ... )
+        >>> min_bound, max_bound = measurement(spark_dataframe) # doctest: +SKIP
+        >>> print(f"Min: {min_bound}, Max: {max_bound}")  # doctest: +NORMALIZE_WHITESPACE
+        Min: -64, Max: 64
+
+    Measurement Contract:
+        * Input domain - :class:`~.SparkDataFrameDomain`
+        * Output type - Tuple[int, int] if the :attr:`~.bound_column` is int, else Tuple[float, float]
+        * Input metric - :class:`~.SymmetricDifference`
+        * Output measure - :class:`~.PureDP`
+
+        >>> measurement.input_domain
+        SparkDataFrameDomain(schema={'A': SparkStringColumnDescriptor(allow_null=False), 'B': SparkIntegerColumnDescriptor(allow_null=False, size=64)})
+        >>> measurement.input_metric
+        SymmetricDifference()
+        >>> measurement.output_measure
+        PureDP()
+
+        Privacy Guarantee:
+            For :math:`d_{in} = 0`, returns :math:`0`
+
+            For :math:`d_{in} > 0`, returns :math:`(4/\alpha) * d_{in}`
+
+            where:
+
+            * :math:`\alpha` is :attr:`~.alpha`
+
+            >>> measurement.privacy_function(1)
+            4
+            >>> measurement.privacy_function(2)
+            8
+    """  # pylint: disable=line-too-long
+
+    @typechecked
+    def __init__(
+        self,
+        input_domain: SparkDataFrameDomain,
+        bound_column: str,
+        alpha: ExactNumberInput,
+        threshold: float = 0.95,
+    ):
+        r"""Constructor.
+
+        Args:
+            input_domain: Domain of the input Spark DataFrames. Input must either be
+                a column of floating point numbers or a column of integers.
+            bound_column: Column name for finding the bounds.
+                The column values must be between [-2^64 + 1, 2^64 - 1] for
+                64 bit integers, [-2^32 + 1, 2^32 - 1] for 32 bit integers
+                and between [-2^100, 2^100] for floats.
+            alpha: The noise scale parameter for Geometric noise that will be added
+                to true number of values falling between the tested bounds on each
+                round of the algorithm.
+                Noise with scale of :math:`\alpha / 2` will be added
+                to compute the threshold.
+                See :class:`~.AddGeometricNoise` for more information.
+            threshold: The fraction of the total count to use as the threshold.
+                This value should be between (0, 1]. By default it is set to 0.95.
+        """
+        if bound_column not in input_domain.schema:
+            raise ValueError(
+                f"Invalid bounding column name: ({bound_column}) not in schema"
+            )
+        column_type = input_domain.schema[bound_column]
+        if isinstance(column_type, SparkFloatColumnDescriptor):
+            splits = (
+                [float("-inf")]
+                + [-(2**i) * 2**-100 for i in range(200, -1, -1)]
+                + [0]
+                + [2**i * 2**-100 for i in range(201)]
+                + [float("inf")]
+            )
+        elif isinstance(column_type, SparkIntegerColumnDescriptor):
+            splits = (
+                [-(2 ** (column_type.size - 1)) + 1]
+                + [-(2**i) for i in range(column_type.size - 2, -1, -1)]
+                + [0]
+                + [2**i for i in range(column_type.size)]
+            )
+        else:
+            raise ValueError(
+                "Invalid column type, expected [SparkFloatColumnDescriptor,"
+                f" SparkIntegerColumnDescriptor], got {column_type}"
+            )
+        self._splits = splits
+        self._bound_column_type = column_type
+
+        try:
+            validate_exact_number(
+                value=alpha,
+                allow_nonintegral=True,
+                minimum=0,
+                minimum_is_inclusive=True,
+            )
+        except ValueError as e:
+            raise ValueError(f"Invalid noise scale: {e}") from e
+        if not 0 < threshold <= 1:
+            raise ValueError(f"Invalid threshold: {threshold}. Must be in (0, 1]")
+        self._bound_column = bound_column
+        self._alpha = ExactNumber(alpha)
+        self._threshold = threshold
+        super().__init__(
+            input_domain=input_domain,
+            input_metric=SymmetricDifference(),
+            output_measure=PureDP(),
+            is_interactive=False,
+        )
+
+    @property
+    def bound_column(self) -> str:
+        """Returns the column to compute the bounds for."""
+        return self._bound_column
+
+    @property
+    def bound_column_type(self) -> SparkColumnDescriptor:
+        """Returns the type of the bound column."""
+        return self._bound_column_type
+
+    @property
+    def splits(self) -> Union[List[float], List[int]]:
+        """Returns the splits."""
+        return self._splits.copy()
+
+    @property
+    def alpha(self) -> ExactNumber:
+        """Returns the alpha."""
+        return self._alpha
+
+    @property
+    def threshold(self) -> float:
+        """Returns the threshold."""
+        return self._threshold
+
+    @typechecked
+    def privacy_function(self, d_in: ExactNumberInput) -> ExactNumber:
+        """Returns the smallest d_out satisfied by the measurement.
+
+        See the privacy and stability tutorial for more information. # TODO(#1320)
+
+        Args:
+            d_in: Distance between inputs under input_metric.
+        """
+        self.input_metric.validate(d_in)
+        d_in = ExactNumber(d_in)
+        if d_in == 0:
+            return ExactNumber(0)
+        if self._alpha == 0:
+            return ExactNumber(float("inf"))
+        if d_in < 1:
+            raise NotImplementedError()
+        return (4 / self._alpha) * d_in
+
+    def __call__(self, sdf: DataFrame) -> Union[Tuple[float, float], Tuple[int, int]]:
+        """Returns the bounds for the given column."""
+        bin_col = get_nonconflicting_string(sdf.columns)
+        bin_count_col = get_nonconflicting_string(sdf.columns + [bin_col])
+
+        # Split the data into bins
+        bucketizer = Bucketizer(
+            splits=self._splits, inputCol=self._bound_column, outputCol=bin_col
+        )
+        binned: pd.DataFrame = (
+            bucketizer.setHandleInvalid("keep")
+            .transform(sdf)
+            .groupBy(bin_col)
+            .agg(sf.count(bin_col).alias(bin_count_col))
+            .toPandas()
+        )
+
+        non_zero_bins = binned[bin_col].values
+        # Bucketizer returns only non-zero bins, so we need to fill in the rest
+        binned_counts = []
+        for i in range(len(self._splits) - 1):
+            if float(i) not in non_zero_bins:
+                binned_counts.append(0)
+            else:
+                binned_counts.append(
+                    binned.loc[binned[bin_col] == float(i)][bin_count_col].values[0]
+                )
+
+        center = len(binned_counts) // 2
+        negative_bins = binned_counts[:center]
+        negative_bins.reverse()
+        positive_bins = binned_counts[center:]
+        counts_by_bin = [neg + pos for neg, pos in zip(negative_bins, positive_bins)]
+        if isinstance(self._bound_column_type, SparkFloatColumnDescriptor):
+            # Take all except for last value to filter out the infinite bin.
+            counts_by_bin = counts_by_bin[:-1]
+
+        add_threshold_noise = AddGeometricNoise(self._alpha / 2)
+        noisy_threshold = add_threshold_noise(np.int64(0))
+        true_count = self._threshold * sum(counts_by_bin)
+
+        cumulative_counts_by_bin = list(accumulate(counts_by_bin))
+
+        # Finding the bin that contains enough counts above the threshold
+        add_bin_noise = AddGeometricNoise(self._alpha)
+        bounds = self._splits[len(self._splits) // 2 :]
+        if isinstance(self._bound_column_type, SparkFloatColumnDescriptor):
+            # Take all except for last value to filter out the infinite bound.
+            bounds = bounds[:-1]
+
+        for step, bin_count in enumerate(cumulative_counts_by_bin):
+            noisy_count = add_bin_noise(np.int64(bin_count - true_count))
+            upper_bound = bounds[step + 1]
+            if noisy_count >= noisy_threshold:
+                break
+        return -upper_bound, upper_bound
+
+
 def _get_sanitized_df(sdf: DataFrame) -> DataFrame:
     """Returns a randomly repartitioned and materialized DataFrame.
 
     See :ref:`pseudo-side-channel-mitigations` for more details on the specific
     mitigations we apply here.
     """
     # pylint: disable=no-name-in-module
```

### Comparing `tmlt_core-0.9.1/tmlt/core/measures.py` & `tmlt_core-0.9.2/tmlt/core/measures.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/metrics.py` & `tmlt_core-0.9.2/tmlt/core/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright Tumult Labs 2022
 
 # pylint: disable=no-member
 
 from abc import ABC, abstractmethod
 from collections import Counter
 from functools import reduce
-from typing import Any, Dict, Iterable, List, Mapping, Tuple, Union, cast
+from typing import Any, Dict, Iterable, List, Mapping, Sequence, Tuple, Union, cast
 
 import numpy as np  # pylint: disable=unused-import
 import pandas as pd
 import sympy as sp
 from pyspark.sql import functions as sf
 from pyspark.sql.session import SparkSession
 from typeguard import typechecked
@@ -56,18 +56,26 @@
 
     def _validate_distance_arguments(
         self, value1: Any, value2: Any, domain: Domain
     ) -> None:
         """Raise an exception if the arguments to a distance method aren't valid."""
         if not self.supports_domain(domain):
             raise ValueError(f"{repr(self)} does not support domain {repr(domain)}.")
-        if value1 not in domain:
-            raise OutOfDomainError(f"The first argument is not in domain {domain}.")
-        if value2 not in domain:
-            raise OutOfDomainError(f"The second argument is not in domain {domain}.")
+        try:
+            domain.validate(value1)
+        except OutOfDomainError as exception:
+            raise OutOfDomainError(
+                domain, value1, "The first argument is not in the domain"
+            ) from exception
+        try:
+            domain.validate(value2)
+        except OutOfDomainError as exception:
+            raise OutOfDomainError(
+                domain, value2, "The second argument is not in the domain"
+            ) from exception
 
     def __eq__(self, other: Any) -> bool:
         """Return True if both metrics are equal."""
         return repr(self) == repr(other)
 
     def __hash__(self):
         """Returns hash value."""
@@ -890,21 +898,21 @@
         ...     pd.DataFrame({"A": [2, 20], "B": [1, 8]})
         ... )
         >>> metric.distance(value1, value2, domain)
         (4, sqrt(53))
     """
 
     @typechecked
-    def __init__(self, on_columns: List[OnColumn]):
+    def __init__(self, on_columns: Sequence[OnColumn]):
         """Constructor.
 
         Args:
             on_columns: The OnColumn metrics to apply.
         """
-        self._on_columns = on_columns
+        self._on_columns = list(on_columns)
 
     @property
     def on_columns(self) -> List[OnColumn]:
         """Return the OnColumn metrics to apply."""
         return self._on_columns
 
     def validate(self, value: Tuple[ExactNumberInput, ...]):
@@ -1172,15 +1180,15 @@
     @typechecked
     def __init__(self, key_to_metric: Mapping[Any, Metric]):
         """Constructor.
 
         Args:
             key_to_metric: Mapping from dictionary key to metric.
         """
-        self._key_to_metric: Dict[Any, Metric] = dict(key_to_metric.items()).copy()
+        self._key_to_metric: Dict[Any, Metric] = dict(key_to_metric.items())
 
     @property
     def key_to_metric(self) -> Dict[Any, Metric]:
         """Returns mapping from keys to metrics."""
         return self._key_to_metric.copy()
 
     def validate(self, value: Dict[Any, Any]):
@@ -1356,22 +1364,22 @@
         ...     )
         ... }
         >>> metric.distance(value1, value2, domain)
         4
     """
 
     @typechecked
-    def __init__(self, df_to_key_column: Dict[Any, str]):
+    def __init__(self, df_to_key_column: Mapping[Any, str]):
         """Constructor.
 
         Args:
             df_to_key_column: A dictionary mapping dataframe names to the name of the
                 key column in that dataframe.
         """
-        self._df_to_key_column = df_to_key_column.copy()
+        self._df_to_key_column: Dict[Any, str] = dict(df_to_key_column.items())
 
     @property
     def df_to_key_column(self) -> Dict[Any, str]:
         """Returns the key column."""
         return self._df_to_key_column.copy()
 
     @typechecked
```

### Comparing `tmlt_core-0.9.1/tmlt/core/random/continuous_gaussian.py` & `tmlt_core-0.9.2/tmlt/core/random/continuous_gaussian.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,19 +35,19 @@
     arb_sub = lambda x, y: arb.arb_sub(x, y, prec)
     arb_mul = lambda x, y: arb.arb_mul(x, y, prec)
     arb_add = lambda x, y: arb.arb_add(x, y, prec)
     arb_sqrt = lambda x: arb.arb_sqrt(x, prec)
     arb_erfinv = lambda x: arb.arb_erfinv(x, prec)
 
     # The following code corresponds to:
-    #   return u + sigma_squared * sqrt(2) * erfinv(2 * p - 1)
+    #   return u + sigma * sqrt(2) * erfinv(2 * p - 1)
     return arb_add(
         from_float(u),
         arb_mul(
-            from_float(sigma_squared),
+            arb_sqrt(from_float(sigma_squared)),
             arb_mul(
                 arb_sqrt(from_int(2)),
                 arb_erfinv(arb_sub(arb_mul(from_int(2), p), from_int(1))),
             ),
         ),
     )
```

### Comparing `tmlt_core-0.9.1/tmlt/core/random/discrete_gaussian.py` & `tmlt_core-0.9.2/tmlt/core/random/discrete_gaussian.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/random/inverse_cdf.py` & `tmlt_core-0.9.2/tmlt/core/random/inverse_cdf.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/random/laplace.py` & `tmlt_core-0.9.2/tmlt/core/random/laplace.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/random/rng.py` & `tmlt_core-0.9.2/tmlt/core/random/rng.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/random/uniform.py` & `tmlt_core-0.9.2/tmlt/core/random/uniform.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/base.py` & `tmlt_core-0.9.2/tmlt/core/transformations/base.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/chaining.py` & `tmlt_core-0.9.2/tmlt/core/transformations/chaining.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/converters.py` & `tmlt_core-0.9.2/tmlt/core/transformations/converters.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Copyright Tumult Labs 2022
 
 from typing import Any
 
 from pyspark.sql import DataFrame
 from typeguard import typechecked
 
-from tmlt.core.domains.spark_domains import SparkDataFrameDomain
+from tmlt.core.domains.spark_domains import DomainColumnError, SparkDataFrameDomain
 from tmlt.core.metrics import (
     HammingDistance,
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
@@ -28,16 +28,18 @@
         """Constructor.
 
         Args:
             domain: Domain of input DataFrames.
             input_metric: IfGroupedBy metric on input DataFrames.
         """
         if not input_metric.column in domain.schema:
-            raise ValueError(
-                f"Invalid IfGroupedBy metric: {input_metric.column} not in domain"
+            raise DomainColumnError(
+                domain,
+                input_metric.column,
+                f"Invalid IfGroupedBy metric: {input_metric.column} not in domain",
             )
         if not isinstance(input_metric.inner_metric, (SumOf, RootSumOfSquared)):
             raise ValueError(
                 "Inner metric for IfGroupedBy metric must be "
                 "SumOf(SymmetricDifference()), or "
                 "RootSumOfSquared(SymmetricDifference())"
             )
```

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/dictionary.py` & `tmlt_core-0.9.2/tmlt/core/transformations/dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Copyright Tumult Labs 2022
 
 from typing import Any, Callable, Dict, List, Mapping, Tuple, Union, cast
 
 from typeguard import typechecked
 
 from tmlt.core.domains.base import Domain
-from tmlt.core.domains.collections import DictDomain
+from tmlt.core.domains.collections import DictDomain, DomainKeyError
 from tmlt.core.metrics import (
     AddRemoveKeys,
     DictMetric,
     IfGroupedBy,
     Metric,
     SymmetricDifference,
 )
@@ -218,17 +218,22 @@
             input_domain: Domain of input dictionaries.
             input_metric: Distance metric over input dictionaries.
             keys: Keys to be used for extracting subset.
         """
         if not keys:
             raise ValueError("No keys provided.")
         if not set(keys) <= set(input_domain.key_to_domain):
-            raise ValueError(
-                "Can not retrieve subset from dictionary. Invalid keys: "
-                f"{set(keys) - set(input_domain.key_to_domain)}"
+            invalid_keys = set(keys) - set(input_domain.key_to_domain)
+            raise DomainKeyError(
+                input_domain,
+                invalid_keys,
+                (
+                    "Can not retrieve subset from dictionary. Invalid keys: "
+                    f"{invalid_keys}"
+                ),
             )
         output_metric: Union[DictMetric, AddRemoveKeys]
         if isinstance(input_metric, DictMetric):
             if set(input_domain.key_to_domain) != set(input_metric.key_to_metric):
                 raise ValueError(
                     "Input metric invalid for input domain: Expected keys: "
                     f"{set(input_domain.key_to_domain)}, not: "
@@ -285,15 +290,17 @@
 
         Args:
             input_domain: Domain of input dictionaries.
             input_metric: Distance metric for input dictionaries.
             key: Key for retrieval.
         """
         if key not in input_domain.key_to_domain:
-            raise KeyError(f"{repr(key)} is not one of the input domain's keys")
+            raise DomainKeyError(
+                input_domain, key, f"{repr(key)} is not one of the input domain's keys"
+            )
         # Below is the check in base class, but needs to happen before so
         # output_metric = input_metric[key] won't get a KeyError
         if not input_metric.supports_domain(input_domain):
             raise ValueError(
                 f"Input metric {input_metric} and input domain {input_domain} are not"
                 " compatible."
             )
@@ -369,15 +376,15 @@
         hint: A hint for the transformation.
     """
     # High level algorithm:
     # 1. Grab the element to transform from the dictionary
     # 2. Create a one element dictionary from the element
     # 3. Augment around (1 + 2)
     if key not in input_domain.key_to_domain:
-        raise ValueError("key is not in the domain")
+        raise DomainKeyError(input_domain, key, f"key {key} is not in the domain")
     if new_key in input_domain.key_to_domain:
         raise ValueError("new_key is already in the domain")
     copy_and_transform_value = AugmentDictTransformation(
         ChainTT(
             transformation1=ChainTT(
                 transformation1=GetValue(
                     input_domain=input_domain, input_metric=input_metric, key=key
@@ -423,15 +430,15 @@
         key: The original key.
         new_key: The new key.
     """
     # High level algorithm:
     # 1. Copy the element to the new key
     # 2. Use subset to drop the original key
     if key not in input_domain.key_to_domain:
-        raise ValueError("key is not in the domain")
+        raise DomainKeyError(input_domain, key, f"key {key} is not in the domain")
     if new_key in input_domain.key_to_domain:
         raise ValueError("new_key is already in the domain")
     copy_and_transform_value = create_copy_and_transform_value(
         input_domain=input_domain,
         input_metric=input_metric,
         key=key,
         new_key=new_key,
@@ -606,15 +613,15 @@
         hint: A hint for the transformation.
     """
     # High level algorithm:
     # 1. Transform the element and store in at temporary key
     # 2. Remove the original key
     # 3. Rename from the temporary key to the original key
     if key not in input_domain.key_to_domain:
-        raise ValueError("key is not in the domain")
+        raise DomainKeyError(input_domain, key, f"key {key} is not in the domain")
     temporary_key = get_nonconflicting_string(
         [
             other_key
             for other_key in input_domain.key_to_domain
             if isinstance(other_key, str)
         ]
     )
```

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/identity.py` & `tmlt_core-0.9.2/tmlt/core/transformations/identity.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/add_remove_keys.py` & `tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/add_remove_keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 # <placeholder: boilerplate>
 
 from typing import Any, Dict, List, Optional, Tuple, cast
 
 from pyspark.sql import DataFrame
 from typeguard import typechecked
 
-from tmlt.core.domains.collections import DictDomain
+from tmlt.core.domains.collections import DictDomain, DomainKeyError
 from tmlt.core.domains.spark_domains import SparkDataFrameDomain
 from tmlt.core.metrics import AddRemoveKeys, IfGroupedBy, SymmetricDifference
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.transformations.spark_transformations.filter import Filter
 from tmlt.core.transformations.spark_transformations.join import PublicJoin
 from tmlt.core.transformations.spark_transformations.map import (
     FlatMap,
@@ -183,15 +183,17 @@
         """
         if self.__class__ == TransformValue:
             raise ValueError(
                 "Cannot instantiate a TransformValue transformation directly. "
                 "Use one of the subclasses deriving this."
             )
         if key not in input_domain.key_to_domain:
-            raise KeyError(f"{repr(key)} is not one of the input domain's keys")
+            raise DomainKeyError(
+                input_domain, key, f"{repr(key)} is not one of the input domain's keys"
+            )
         if new_key in input_domain.key_to_domain:
             raise ValueError(f"{repr(new_key)} is already a key in the input domain")
         if transformation.input_domain != input_domain.key_to_domain[key]:
             raise ValueError(
                 f"Input domain's value for {repr(key)} does not match transformation's "
                 "input domain"
             )
```

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/agg.py` & `tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/agg.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import numpy as np
 from pyspark.sql import DataFrame
 from pyspark.sql import functions as sf
 from typeguard import typechecked
 
 from tmlt.core.domains.numpy_domains import NumpyFloatDomain, NumpyIntegerDomain
 from tmlt.core.domains.spark_domains import (
+    DomainColumnError,
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
     SparkGroupedDataFrameDomain,
     SparkIntegerColumnDescriptor,
 )
 from tmlt.core.metrics import (
     AbsoluteDifference,
@@ -685,16 +686,18 @@
             input_domain: Domain of input DataFrames.
             input_metric: Metric on input DataFrames.
             measure_column: Name of the column to be summed. This must be a numeric column.
             lower: Lower clipping bound for measure column.
             upper: Upper clipping bound for measure column.
         """
         if measure_column not in input_domain.schema:
-            raise ValueError(
-                f"Invalid measure column: ({measure_column}) does not exist."
+            raise DomainColumnError(
+                input_domain,
+                measure_column,
+                f"Invalid measure column: ({measure_column}) does not exist.",
             )
 
         measure_column_descriptor = input_domain[measure_column]
         if not isinstance(
             measure_column_descriptor,
             (SparkIntegerColumnDescriptor, SparkFloatColumnDescriptor),
         ):
@@ -913,15 +916,19 @@
                 will be named 'sum(<measure_column>)'.
         """
         if sum_column is None:
             sum_column = f"sum({measure_column})"
 
         groupby_columns = input_domain.group_keys.columns
         if measure_column not in set(input_domain.schema) - set(groupby_columns):
-            raise ValueError(f"Invalid measure column: {measure_column}")
+            raise DomainColumnError(
+                input_domain,
+                measure_column,
+                f"Invalid measure column: {measure_column}",
+            )
 
         measure_column_descriptor = input_domain[measure_column]
         if not isinstance(
             measure_column_descriptor,
             (SparkIntegerColumnDescriptor, SparkFloatColumnDescriptor),
         ):
             raise ValueError(
```

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/filter.py` & `tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Copyright Tumult Labs 2022
 
 from typing import Union
 
 from pyspark.sql import DataFrame, SparkSession
 from typeguard import typechecked
 
-from tmlt.core.domains.spark_domains import SparkDataFrameDomain
+from tmlt.core.domains.spark_domains import DomainColumnError, SparkDataFrameDomain
 from tmlt.core.metrics import IfGroupedBy, RootSumOfSquared, SumOf, SymmetricDifference
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.utils.exact_number import ExactNumber, ExactNumberInput
 
 
 class Filter(Transformation):
     """Keeps only selected rows in a Spark DataFrame using an expression.
@@ -112,16 +112,18 @@
             ):
                 raise ValueError(
                     "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
                     "SumOf(SymmetricDifference()), or "
                     "RootSumOfSquared(SymmetricDifference())"
                 )
             if metric.column not in domain.schema:
-                raise ValueError(
-                    f"Invalid IfGroupedBy metric: {metric.column} not in domain."
+                raise DomainColumnError(
+                    domain,
+                    metric.column,
+                    f"Invalid IfGroupedBy metric: {metric.column} not in domain.",
                 )
         try:
             test_df.filter(filter_expr)
         except Exception as e:
             raise ValueError(f"Invalid filter_expr: {filter_expr}.") from e
         super().__init__(
             input_domain=domain,
```

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/groupby.py` & `tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/groupby.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/id.py` & `tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/id.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/join.py` & `tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/join.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pyspark.sql import DataFrame
 from pyspark.sql import functions as sf
 from typeguard import typechecked
 
-from tmlt.core.domains.collections import DictDomain
+from tmlt.core.domains.collections import DictDomain, DomainKeyError
 from tmlt.core.domains.spark_domains import (
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
 )
 from tmlt.core.metrics import (
     AddRemoveKeys,
     DictMetric,
@@ -594,17 +594,25 @@
                 both dataframes will be considered to be equal.
         """
         if input_domain.length != 2:
             raise ValueError("Input domain must be a DictDomain with 2 keys.")
         if left_key == right_key:
             raise ValueError("Left and right keys must be distinct.")
         if left_key not in input_domain.key_to_domain:
-            raise ValueError(f"Invalid key: Key '{left_key}' not in input domain.")
+            raise DomainKeyError(
+                input_domain,
+                left_key,
+                f"Invalid key: Key '{left_key}' not in input domain.",
+            )
         if right_key not in input_domain.key_to_domain:
-            raise ValueError(f"Invalid key: Key '{right_key}' not in input domain.")
+            raise DomainKeyError(
+                input_domain,
+                right_key,
+                f"Invalid key: Key '{right_key}' not in input domain.",
+            )
 
         left_domain, right_domain = input_domain[left_key], input_domain[right_key]
         if not isinstance(left_domain, SparkDataFrameDomain) or not isinstance(
             right_domain, SparkDataFrameDomain
         ):
             raise ValueError("Input domain must be SparkDataFrameDomain for both keys.")
```

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/map.py` & `tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/map.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/nan.py` & `tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/nan.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import Any, Dict, List, Tuple, Union, cast
 
 from pyspark.sql import DataFrame
 from pyspark.sql import functions as sf
 from typeguard import typechecked
 
 from tmlt.core.domains.spark_domains import (
+    DomainColumnError,
     SparkDataFrameDomain,
     SparkFloatColumnDescriptor,
 )
 from tmlt.core.metrics import (
     HammingDistance,
     IfGroupedBy,
     RootSumOfSquared,
@@ -132,17 +133,21 @@
         if len(columns) != len(set(columns)):
             duplicates = set(col for col in columns if columns.count(col) > 1)
             raise ValueError(
                 "`columns` must not contain duplicate names. The column(s)"
                 f" ({duplicates}) appear more than once."
             )
         if not set(columns) <= set(input_domain.schema):
-            raise ValueError(
-                "One or more columns do not exist in the input domain:"
-                f" {set(columns) - set(input_domain.schema)}"
+            raise DomainColumnError(
+                input_domain,
+                set(columns) - set(input_domain.schema),
+                (
+                    "One or more columns do not exist in the input domain:"
+                    f" {set(columns) - set(input_domain.schema)}"
+                ),
             )
         for column in columns:
             if not isinstance(input_domain[column], SparkFloatColumnDescriptor):
                 raise ValueError(
                     f"Cannot drop +inf and -inf from {input_domain[column]}. Only float"
                     " columns can contain +inf or -inf."
                 )
@@ -302,17 +307,21 @@
             duplicates = set(col for col in columns if columns.count(col) > 1)
             raise ValueError(
                 f"`columns` must not contain duplicate names. Columns ({duplicates})"
                 " appear more than once."
             )
 
         if not set(columns) <= set(input_domain.schema):
-            raise ValueError(
-                "One or more columns do not exist in the input domain"
-                f" {set(columns)-set(input_domain.schema)}"
+            raise DomainColumnError(
+                input_domain,
+                set(columns) - set(input_domain.schema),
+                (
+                    "One or more columns do not exist in the input domain"
+                    f" {set(columns)-set(input_domain.schema)}"
+                ),
             )
 
         for column in columns:
             if not isinstance(input_domain[column], SparkFloatColumnDescriptor):
                 raise ValueError(
                     f"Cannot drop NaNs from {input_domain[column]}. Only float columns"
                     " can contain NaNs."
@@ -468,17 +477,21 @@
             duplicates = set(col for col in columns if columns.count(col) > 1)
             raise ValueError(
                 f"`columns` must not contain duplicate names. Columns ({duplicates})"
                 " appear more than once."
             )
 
         if not set(columns) <= set(input_domain.schema):
-            raise ValueError(
-                "One or more columns do not exist in the input domain"
-                f" {set(columns)-set(input_domain.schema)}"
+            raise DomainColumnError(
+                input_domain,
+                set(columns) - set(input_domain.schema),
+                (
+                    "One or more columns do not exist in the input domain"
+                    f" {set(columns)-set(input_domain.schema)}"
+                ),
             )
         output_domain = SparkDataFrameDomain(
             {
                 column: replace(descriptor, allow_null=False)  # type: ignore
                 if column in columns
                 else descriptor
                 for column, descriptor in input_domain.schema.items()
@@ -627,17 +640,21 @@
             )
         if not replace_map:
             raise ValueError(
                 "At least one column must be specified (in `replace_map`)."
             )
 
         if not set(replace_map) <= set(input_domain.schema):
-            raise ValueError(
-                "One or more columns do not exist in the input domain:"
-                f" {set(replace_map) - set(input_domain.schema)}"
+            raise DomainColumnError(
+                input_domain,
+                set(replace_map) - set(input_domain.schema),
+                (
+                    "One or more columns do not exist in the input domain:"
+                    f" {set(replace_map) - set(input_domain.schema)}"
+                ),
             )
         for column in list(replace_map.keys()):
             if not isinstance(input_domain[column], SparkFloatColumnDescriptor):
                 raise ValueError(
                     f"Column of type {input_domain[column]} cannot contain values of"
                     " infinity or -infinity."
                 )
@@ -807,17 +824,21 @@
                 "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
                 "or L1 or L2 over SymmetricDifference."
             )
         if not replace_map:
             raise ValueError("At least one column must be specified.")
 
         if not set(replace_map) <= set(input_domain.schema):
-            raise ValueError(
-                "One or more columns do not exist in the input domain"
-                f" {set(replace_map)-set(input_domain.schema)}"
+            raise DomainColumnError(
+                input_domain,
+                set(replace_map) - set(input_domain.schema),
+                (
+                    "One or more columns do not exist in the input domain"
+                    f" {set(replace_map)-set(input_domain.schema)}"
+                ),
             )
         for column, value in replace_map.items():
             if not isinstance(input_domain[column], SparkFloatColumnDescriptor):
                 raise ValueError(
                     f"Column of type {input_domain[column]} can not contain NaNs."
                 )
             if not cast(SparkFloatColumnDescriptor, input_domain[column]).allow_nan:
@@ -977,17 +998,21 @@
                 "Inner metric for IfGroupedBy metric must be SymmetricDifference, "
                 "or L1 or L2 over SymmetricDifference."
             )
         if not replace_map:
             raise ValueError("At least one column must be specified.")
 
         if not set(replace_map) <= set(input_domain.schema):
-            raise ValueError(
-                "One or more columns do not exist in the input domain"
-                f" {set(replace_map)-set(input_domain.schema)}"
+            raise DomainColumnError(
+                input_domain,
+                set(replace_map) - set(input_domain.schema),
+                (
+                    "One or more columns do not exist in the input domain"
+                    f" {set(replace_map)-set(input_domain.schema)}"
+                ),
             )
         output_domain = SparkDataFrameDomain(
             {
                 column: replace(descriptor, allow_null=False)  # type: ignore
                 if column in replace_map
                 else descriptor
                 for column, descriptor in input_domain.schema.items()
```

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/partition.py` & `tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from pyspark.sql import Column, DataFrame
 from pyspark.sql import functions as sf
 from typeguard import typechecked
 
 from tmlt.core.domains.base import Domain
 from tmlt.core.domains.collections import ListDomain
-from tmlt.core.domains.spark_domains import SparkDataFrameDomain
+from tmlt.core.domains.spark_domains import DomainColumnError, SparkDataFrameDomain
 from tmlt.core.metrics import IfGroupedBy, RootSumOfSquared, SumOf, SymmetricDifference
 from tmlt.core.transformations.base import Transformation
 from tmlt.core.utils.exact_number import ExactNumber, ExactNumberInput
 
 
 class Partition(Transformation):
     """Base class for partition transformations."""
@@ -178,15 +178,19 @@
                 in the output metric.
             keys: List of column names to partition by.
             list_values: Domain for key columns in the DataFrame. This is a list
                 of unique n-tuples, where each value is a tuple corresponds to a key.
         """
         for key in keys:
             if key not in input_domain.schema:
-                raise ValueError(f"Partition key does not exist in input domain: {key}")
+                raise DomainColumnError(
+                    input_domain,
+                    key,
+                    f"Partition key does not exist in input domain: {key}",
+                )
 
         if len(set(list_values)) != len(list_values):
             raise ValueError("Partition key values list contains duplicate.")
 
         for values in list_values:
             if not len(values) == len(keys):
                 raise ValueError(
```

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/persist.py` & `tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/persist.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/rename.py` & `tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/rename.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from typing import Dict, Union
 
 from pyspark.sql import DataFrame
 from pyspark.sql import functions as sf
 from typeguard import typechecked
 
-from tmlt.core.domains.spark_domains import SparkDataFrameDomain
+from tmlt.core.domains.spark_domains import DomainColumnError, SparkDataFrameDomain
 from tmlt.core.metrics import (
     HammingDistance,
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
@@ -112,16 +112,18 @@
             input_domain: Domain of input DataFrame.
             metric: Distance metric for input DataFrames.
             rename_mapping: Dictionary from existing column names to target column
                 names.
         """
         nonexistent_columns = rename_mapping.keys() - set(input_domain.schema)
         if nonexistent_columns:
-            raise ValueError(
-                f"Non existent keys in rename_mapping : {nonexistent_columns}"
+            raise DomainColumnError(
+                input_domain,
+                nonexistent_columns,
+                f"Non existent keys in rename_mapping : {nonexistent_columns}",
             )
         for old, new in rename_mapping.items():
             if new in input_domain.schema and new != old:
                 raise ValueError(f"Cannot rename {old} to {new}. {new} already exists.")
         output_metric = metric
         if isinstance(metric, IfGroupedBy):
             if metric.inner_metric not in (
```

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/select.py` & `tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/select.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Copyright Tumult Labs 2022
 
 from typing import List, Union
 
 from pyspark.sql import DataFrame
 from typeguard import typechecked
 
-from tmlt.core.domains.spark_domains import SparkDataFrameDomain
+from tmlt.core.domains.spark_domains import DomainColumnError, SparkDataFrameDomain
 from tmlt.core.metrics import (
     HammingDistance,
     IfGroupedBy,
     RootSumOfSquared,
     SumOf,
     SymmetricDifference,
 )
@@ -111,16 +111,18 @@
             metric: Distance metric for input and output DataFrames.
             columns: A list of existing column names to keep.
         """
         if len(columns) != len(set(columns)):
             raise ValueError(f"Column name appears more than once in {columns}")
         nonexistent_columns = set(columns) - set(input_domain.schema)
         if nonexistent_columns:
-            raise ValueError(
-                f"Non existent columns in select columns : {nonexistent_columns}"
+            raise DomainColumnError(
+                input_domain,
+                nonexistent_columns,
+                f"Non existent columns in select columns : {nonexistent_columns}",
             )
         output_columns = {col: input_domain[col] for col in columns}
         if isinstance(metric, IfGroupedBy):
             if metric.column not in columns:
                 raise ValueError(
                     "Column used in IfGroupedBy metric must be"
                     f" selected: {metric.column}."
```

### Comparing `tmlt_core-0.9.1/tmlt/core/transformations/spark_transformations/truncation.py` & `tmlt_core-0.9.2/tmlt/core/transformations/spark_transformations/truncation.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/utils/arb.py` & `tmlt_core-0.9.2/tmlt/core/utils/arb.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/utils/cleanup.py` & `tmlt_core-0.9.2/tmlt/core/utils/cleanup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,29 @@
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
 import atexit
 import re
 from typing import List
+from warnings import warn
 
 from pyspark.sql import SparkSession
 
 from tmlt.core.utils.configuration import Config
 
 
 def _cleanup_temp() -> None:
     """Cleanup the temporary table."""
-    spark = SparkSession.builder.getOrCreate()
+    try:
+        spark = SparkSession.builder.getOrCreate()
+    except RuntimeError:
+        warn("Failed to clean up temporary tables, no Spark session available")
+        return
+
     spark.sql(f"DROP DATABASE IF EXISTS `{Config.temp_db_name()}` CASCADE")
 
 
 def cleanup() -> None:
     """Cleanup Core's temporary table.
 
     If you call `spark.stop()`, you should call this function first.
```

### Comparing `tmlt_core-0.9.1/tmlt/core/utils/configuration.py` & `tmlt_core-0.9.2/tmlt/core/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/utils/distributions.py` & `tmlt_core-0.9.2/tmlt/core/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/utils/exact_number.py` & `tmlt_core-0.9.2/tmlt/core/utils/exact_number.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/utils/grouped_dataframe.py` & `tmlt_core-0.9.2/tmlt/core/utils/grouped_dataframe.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/utils/join.py` & `tmlt_core-0.9.2/tmlt/core/utils/join.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/utils/misc.py` & `tmlt_core-0.9.2/tmlt/core/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/utils/parameters.py` & `tmlt_core-0.9.2/tmlt/core/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/utils/testing.py` & `tmlt_core-0.9.2/tmlt/core/utils/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-License-Identifier: Apache-2.0
 # Copyright Tumult Labs 2022
 
 # TODO(#1218): Move dummy aggregate class back to the test.
 
 import logging
+import math
 import shutil
 import sys
 import unittest
 from dataclasses import dataclass
 from typing import (
     Any,
     Callable,
@@ -832,15 +833,17 @@
 
 
 def _create_discrete_gaussian_pmf(loc: int):
     return lambda k, noise_scale: discrete_gaussian_pmf(k - loc, noise_scale)
 
 
 def _create_gaussian_cdf(loc: float):
-    return lambda value, noise_scale: norm.cdf(value, loc=loc, scale=noise_scale)
+    return lambda value, noise_scale: norm.cdf(
+        value, loc=loc, scale=math.sqrt(noise_scale)
+    )
 
 
 def get_prob_functions(
     noise_mechanism: NoiseMechanism, locations: Dict[str, Union[float, int]]
 ) -> Dict[str, Dict[str, Callable]]:
     """Returns probability mass/density functions for different noise mechanisms."""
     if noise_mechanism == NoiseMechanism.LAPLACE:
```

### Comparing `tmlt_core-0.9.1/tmlt/core/utils/truncation.py` & `tmlt_core-0.9.2/tmlt/core/utils/truncation.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,17 @@
         df: DataFrame to truncate.
         grouping_columns: Columns defining the groups.
         key_columns: Column defining the keys.
         threshold: Maximum number of keys to include for each group.
     """
     rank_column = get_nonconflicting_string(df.columns)
     hash_column = get_nonconflicting_string(df.columns + [rank_column])
-    shuffled_partitions = Window.partitionBy(*grouping_columns).orderBy(hash_column)
+    shuffled_partitions = Window.partitionBy(*grouping_columns).orderBy(
+        hash_column, *key_columns
+    )
     return (
         df.withColumn(
             hash_column, sf.hash(*grouping_columns, *key_columns)
         )  # pylint: disable=no-member
         .withColumn(
             rank_column,
             sf.dense_rank().over(shuffled_partitions),  # pylint: disable=no-member
```

### Comparing `tmlt_core-0.9.1/tmlt/core/utils/type_utils.py` & `tmlt_core-0.9.2/tmlt/core/utils/type_utils.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/tmlt/core/utils/validation.py` & `tmlt_core-0.9.2/tmlt/core/utils/validation.py`

 * *Files identical despite different names*

### Comparing `tmlt_core-0.9.1/PKG-INFO` & `tmlt_core-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmlt-core
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tumult's differential privacy primitives
 Home-page: https://gitlab.com/tumult-labs/core
 License: Apache-2.0
 Requires-Python: >=3.7.1,<3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

