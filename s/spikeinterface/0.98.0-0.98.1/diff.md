# Comparing `tmp/spikeinterface-0.98.0.tar.gz` & `tmp/spikeinterface-0.98.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spikeinterface-0.98.0.tar", last modified: Fri Jul  7 12:50:21 2023, max compression
+gzip compressed data, was "spikeinterface-0.98.1.tar", last modified: Tue Jul 18 09:06:10 2023, max compression
```

## Comparing `spikeinterface-0.98.0.tar` & `spikeinterface-0.98.1.tar`

### file list

```diff
@@ -1,383 +1,383 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.396705 spikeinterface-0.98.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-07 12:50:21.396705 spikeinterface-0.98.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 12:50:21.396705 spikeinterface-0.98.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.340702 spikeinterface-0.98.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.344702 spikeinterface-0.98.0/src/spikeinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.348703 spikeinterface-0.98.0/src/spikeinterface/comparison/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/comparison/basecomparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/comparison/collisioncomparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/comparison/collisionstudy.py
--rw-r--r--   0 runner    (1001) docker     (123)    24739 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/comparison/comparisontools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/comparison/correlogramcomparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/comparison/correlogramstudy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/comparison/groundtruthstudy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/comparison/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/comparison/multicomparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)    25783 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/comparison/paircomparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/comparison/studytools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.352703 spikeinterface-0.98.0/src/spikeinterface/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40071 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/baseevent.py
--rw-r--r--   0 runner    (1001) docker     (123)    29103 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/baserecording.py
--rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/baserecordingsnippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/basesnippets.py
--rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/basesorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/binaryfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/binaryrecordingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/channelsaggregationrecording.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/channelslice.py
--rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/core_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/frameslicerecording.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/frameslicesorting.py
--rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/injecttemplates.py
--rw-r--r--   0 runner    (1001) docker     (123)    15527 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/job_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/npyfoldersnippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/npysnippetsextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/npzfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/npzsortingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/numpyextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/old_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13093 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/recording_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    25339 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/segmentutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/snippets_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/sparsity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/template_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/testing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/unitsaggregationsorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/unitsselectionsorting.py
--rw-r--r--   0 runner    (1001) docker     (123)    77877 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/waveform_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/waveform_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/core/zarrrecordingextractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.356703 spikeinterface-0.98.0/src/spikeinterface/curation/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/curation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19016 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/curation/auto_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/curation/curation_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/curation/curationsorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/curation/mergeunitssorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/curation/remove_duplicated_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/curation/remove_excess_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/curation/remove_redundant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/curation/sortingview_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/curation/splitunitsorting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.356703 spikeinterface-0.98.0/src/spikeinterface/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/exporters/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/exporters/to_phy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.356703 spikeinterface-0.98.0/src/spikeinterface/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/alfsortingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/bids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/cbin_ibl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/cellexplorersortingextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/combinatoextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/extractorlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10107 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/hdsortextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/herdingspikesextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/iblstreamingrecording.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/klustaextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/matlabhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/mclustextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/mcsh5extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25261 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/mdaextractors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.360703 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/alphaomega.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/axona.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/biocam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/blackrock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/ced.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/edf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/intan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/maxwell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/mcsraw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/mearec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/neo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/neobaseextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/neuralynx.py
--rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/neuroscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/nix.py
--rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/plexon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/spike2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/spikegadgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/spikeglx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/tdt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/neuropixels_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25073 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/nwbextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/phykilosortextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/shybridextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/spykingcircusextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/toy_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/tridesclousextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/waveclussnippetstextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/waveclustextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/extractors/yassextractors.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/full.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.364703 spikeinterface-0.98.0/src/spikeinterface/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/postprocessing/alignsorting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/postprocessing/amplitude_scalings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/postprocessing/correlograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/postprocessing/isi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/postprocessing/noise_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/postprocessing/principal_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/postprocessing/spike_amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/postprocessing/spike_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/postprocessing/template_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/postprocessing/template_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/postprocessing/template_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    22736 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/postprocessing/unit_localization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.368703 spikeinterface-0.98.0/src/spikeinterface/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/align_snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/astype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/average_across_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/basepreprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/common_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/correct_lsb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.368703 spikeinterface-0.98.0/src/spikeinterface/preprocessing/deepinterpolation/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/deepinterpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/deepinterpolation/deepinterpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/depth_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/detect_bad_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/directional_derivative.py
--rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/filter_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/filter_opencl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/highpass_spatial_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/interpolate_bad_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/normalize_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/phase_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/preprocessing_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/preprocessinglist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/rectify.py
--rw-r--r--   0 runner    (1001) docker     (123)    20814 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/remove_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/silence_periods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/unsigned_to_signed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/whiten.py
--rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/preprocessing/zero_channel_pad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.368703 spikeinterface-0.98.0/src/spikeinterface/qualitymetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/qualitymetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41381 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/qualitymetrics/misc_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    38030 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/qualitymetrics/pca_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/qualitymetrics/quality_metric_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/qualitymetrics/quality_metric_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/qualitymetrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.368703 spikeinterface-0.98.0/src/spikeinterface/sorters/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/basesorter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.372703 spikeinterface-0.98.0/src/spikeinterface/sorters/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/combinato.py
--rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/hdsort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/hdsort_master.m
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/herdingspikes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/ironclust.py
--rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort2_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort2_5_master.m
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort2_master.m
--rw-r--r--   0 runner    (1001) docker     (123)     9942 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort3_master.m
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort_master.m
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosortbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/klusta.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/klusta_config_default.prm
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/mountainsort4.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/mountainsort5.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/pykilosort.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/sc_config_default.params
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/spyking_circus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/tridesclous.py
--rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/waveclus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/waveclus_master.m
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/waveclus_snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/waveclus_snippets_master.m
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/yass.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/external/yass_config_default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.372703 spikeinterface-0.98.0/src/spikeinterface/sorters/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/internal/si_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/internal/spyking_circus2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/internal/tridesclous2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    29273 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/runsorter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/sorterlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.372703 spikeinterface-0.98.0/src/spikeinterface/sorters/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/utils/constructNPYheader.m
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/utils/shellscript.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sorters/utils/writeNPY.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.376704 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.376704 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21585 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    29179 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)    21903 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25550 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_localization.py
--rw-r--r--   0 runner    (1001) docker     (123)    25089 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.380704 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/circus.py
--rw-r--r--   0 runner    (1001) docker     (123)    27271 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/clustering_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/isocut5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/method_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/position_and_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/position_and_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/position_ptp_scaled.py
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/random_projections.py
--rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/sliding_hdbscan.py
--rw-r--r--   0 runner    (1001) docker     (123)    27670 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/sliding_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/triage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/features_from_peaks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.380704 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/matching/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33854 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/matching/circus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/matching/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/matching/method_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/matching/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/matching/tdc.py
--rw-r--r--   0 runner    (1001) docker     (123)    44820 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/matching/wobble.py
--rw-r--r--   0 runner    (1001) docker     (123)    59332 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/motion_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/motion_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/peak_localization.py
--rw-r--r--   0 runner    (1001) docker     (123)    21800 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/peak_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/peak_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.380704 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/waveforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/waveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/waveforms/neural_network_denoiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/waveforms/savgol_denoiser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11587 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/waveforms/temporal_pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/waveforms/waveform_thresholder.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/waveforms/waveform_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.384704 spikeinterface-0.98.0/src/spikeinterface/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.388704 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/agreementmatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/basewidget.py
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/collisioncomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/confusionmatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/correlogramcomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/correlograms_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/depthamplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/gtcomparison.py
--rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/gtstudy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/isidistribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/multicompgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/presence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/principalcomponent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/probemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/rasters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/sortingperformance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/timeseries_.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/unitlocalization_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/unitprobemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/unitsummary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveformdensitymap_.py
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveforms_.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/all_amplitudes_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/autocorrelograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/crosscorrelograms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.388704 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/base_ipywidgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/spike_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/spikes_on_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/template_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/unit_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/unit_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/unit_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.392704 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/all_amplitudes_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/autocorrelograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/base_mpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/crosscorrelograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/spike_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/spikes_on_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/template_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/template_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/unit_depths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/unit_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/unit_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/unit_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/unit_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/unit_waveforms_density_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sorting_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.396705 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/autocorrelograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/base_sortingview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/crosscorrelograms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/sorting_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/spike_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/template_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/template_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/unit_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/unit_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/spike_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/spikes_on_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/template_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/template_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/unit_depths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/unit_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/unit_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/unit_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/unit_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/unit_waveforms_density_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-07 12:48:26.000000 spikeinterface-0.98.0/src/spikeinterface/widgets/widget_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 12:50:21.344702 spikeinterface-0.98.0/src/spikeinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-07 12:50:21.000000 spikeinterface-0.98.0/src/spikeinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18324 2023-07-07 12:50:21.000000 spikeinterface-0.98.0/src/spikeinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 12:50:21.000000 spikeinterface-0.98.0/src/spikeinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-07 12:50:21.000000 spikeinterface-0.98.0/src/spikeinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 12:50:21.000000 spikeinterface-0.98.0/src/spikeinterface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.055112 spikeinterface-0.98.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-18 09:06:10.055112 spikeinterface-0.98.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:06:10.055112 spikeinterface-0.98.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.951110 spikeinterface-0.98.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.959110 spikeinterface-0.98.1/src/spikeinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.963110 spikeinterface-0.98.1/src/spikeinterface/comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/basecomparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/collisioncomparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/collisionstudy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24739 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/comparisontools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/correlogramcomparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/correlogramstudy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/groundtruthstudy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/multicomparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25783 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/paircomparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/comparison/studytools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.967110 spikeinterface-0.98.1/src/spikeinterface/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41463 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/baseevent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29103 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/baserecording.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/baserecordingsnippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/basesnippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/basesorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/binaryfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/binaryrecordingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/channelsaggregationrecording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/channelslice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/core_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/frameslicerecording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/frameslicesorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/injecttemplates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15527 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/job_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/npyfoldersnippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/npysnippetsextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/npzfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/npzsortingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/numpyextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/old_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13093 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/recording_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25339 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/segmentutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/snippets_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/sparsity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/template_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/testing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/unitsaggregationsorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/unitsselectionsorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77909 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/waveform_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/waveform_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/core/zarrrecordingextractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.971110 spikeinterface-0.98.1/src/spikeinterface/curation/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19016 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/auto_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/curation_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/curationsorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/mergeunitssorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/remove_duplicated_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/remove_excess_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/remove_redundant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/sortingview_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/curation/splitunitsorting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.971110 spikeinterface-0.98.1/src/spikeinterface/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/exporters/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/exporters/to_phy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.975110 spikeinterface-0.98.1/src/spikeinterface/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/alfsortingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/bids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/cbin_ibl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/cellexplorersortingextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/combinatoextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/extractorlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/hdsortextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/herdingspikesextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/iblstreamingrecording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/klustaextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/matlabhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/mclustextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/mcsh5extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25313 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/mdaextractors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.983111 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/alphaomega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/axona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/biocam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/blackrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/ced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/edf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/intan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/maxwell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/mcsraw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/mearec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27769 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neobaseextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neuralynx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neuroscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/nix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/plexon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/spike2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/spikegadgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/spikeglx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/tdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/neuropixels_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25141 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/nwbextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/phykilosortextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/shybridextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/spykingcircusextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/toy_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/tridesclousextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/waveclussnippetstextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/waveclustextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/extractors/yassextractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/full.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.987110 spikeinterface-0.98.1/src/spikeinterface/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/alignsorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/amplitude_scalings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/correlograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8996 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/isi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/noise_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/principal_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/spike_amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/spike_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/template_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/template_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/template_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22736 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/postprocessing/unit_localization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.995111 spikeinterface-0.98.1/src/spikeinterface/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/align_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/astype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/average_across_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/basepreprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/common_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/correct_lsb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.995111 spikeinterface-0.98.1/src/spikeinterface/preprocessing/deepinterpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/deepinterpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16137 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/deepinterpolation/deepinterpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/depth_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/detect_bad_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/directional_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/filter_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/filter_opencl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/highpass_spatial_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/interpolate_bad_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/normalize_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/phase_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/preprocessing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/preprocessinglist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/rectify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20814 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/remove_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/silence_periods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/unsigned_to_signed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/whiten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/preprocessing/zero_channel_pad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.999111 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41381 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/misc_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38030 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/pca_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/quality_metric_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/quality_metric_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.999111 spikeinterface-0.98.1/src/spikeinterface/sorters/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/basesorter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.007111 spikeinterface-0.98.1/src/spikeinterface/sorters/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/combinato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/hdsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/hdsort_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/herdingspikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/ironclust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2_5_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort3_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosortbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/klusta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/klusta_config_default.prm
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/mountainsort4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/mountainsort5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/pykilosort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/sc_config_default.params
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/spyking_circus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/tridesclous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus_snippets_master.m
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/yass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/external/yass_config_default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.011111 spikeinterface-0.98.1/src/spikeinterface/sorters/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/internal/si_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/internal/spyking_circus2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/internal/tridesclous2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16497 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29273 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/runsorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/sorterlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.011111 spikeinterface-0.98.1/src/spikeinterface/sorters/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/utils/constructNPYheader.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/utils/shellscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sorters/utils/writeNPY.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.015111 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.015111 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21585 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29179 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21887 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25550 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25089 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.019111 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/circus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27271 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/clustering_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/isocut5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/method_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position_and_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position_and_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position_ptp_scaled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/random_projections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21202 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/sliding_hdbscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/sliding_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/triage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14589 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/features_from_peaks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.023111 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33854 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/circus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/method_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/tdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44820 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/wobble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59332 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/motion_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15683 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/motion_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40384 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21800 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.023111 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/neural_network_denoiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/savgol_denoiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11587 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/temporal_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/waveform_thresholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/waveform_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.031112 spikeinterface-0.98.1/src/spikeinterface/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.039112 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/agreementmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/basewidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/collisioncomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/confusionmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/correlogramcomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/correlograms_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/depthamplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/gtcomparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/gtstudy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/isidistribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/multicompgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/principalcomponent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/probemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/rasters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/sortingperformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/timeseries_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitlocalization_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitprobemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitsummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveformdensitymap_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveforms_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/all_amplitudes_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/autocorrelograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/crosscorrelograms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.043112 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/base_ipywidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/spike_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/spikes_on_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/template_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/unit_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/unit_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/unit_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.051112 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/all_amplitudes_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/autocorrelograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/base_mpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/crosscorrelograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/spike_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/spikes_on_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/template_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/template_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_depths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_waveforms_density_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sorting_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:10.055112 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/autocorrelograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/base_sortingview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/crosscorrelograms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/sorting_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/spike_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/template_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/template_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/unit_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/unit_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/spike_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/spikes_on_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/template_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/template_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/unit_depths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/unit_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/unit_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/unit_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/unit_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/unit_waveforms_density_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-18 09:04:40.000000 spikeinterface-0.98.1/src/spikeinterface/widgets/widget_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:06:09.959110 spikeinterface-0.98.1/src/spikeinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-07-18 09:06:09.000000 spikeinterface-0.98.1/src/spikeinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18324 2023-07-18 09:06:09.000000 spikeinterface-0.98.1/src/spikeinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:06:09.000000 spikeinterface-0.98.1/src/spikeinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-18 09:06:09.000000 spikeinterface-0.98.1/src/spikeinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 09:06:09.000000 spikeinterface-0.98.1/src/spikeinterface.egg-info/top_level.txt
```

### Comparing `spikeinterface-0.98.0/LICENSE` & `spikeinterface-0.98.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/PKG-INFO` & `spikeinterface-0.98.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spikeinterface
-Version: 0.98.0
+Version: 0.98.1
 Summary: Python toolkit for analysis, visualization, and comparison of spike sorting output
 Author-email: Alessio Buccino <alessiop.buccino@gmail.com>, Samuel Garcia <sam.garcia.die@gmail.com>
 Project-URL: homepage, https://github.com/SpikeInterface/spikeinterface
 Project-URL: repository, https://github.com/SpikeInterface/spikeinterface
 Project-URL: documentation, https://spikeinterface.readthedocs.io/
 Project-URL: changelog, https://spikeinterface.readthedocs.io/en/latest/whatisnew.html
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -18,14 +18,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: extractors
 Provides-Extra: streaming_extractors
 Provides-Extra: full
 Provides-Extra: widgets
 Provides-Extra: test_core
 Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 # SpikeInterface: a unified framework for spike sorting
 
 <table>
 <tr>
   <td>Latest Release</td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spikeinterface Version: 0.98.0 Summary: Python
+Metadata-Version: 2.1 Name: spikeinterface Version: 0.98.1 Summary: Python
 toolkit for analysis, visualization, and comparison of spike sorting output
 Author-email: Alessio Buccino
 buccino@gmail.com>, Samuel Garcia
 garcia.die@gmail.com> Project-URL: homepage, https://github.com/SpikeInterface/
 spikeinterface Project-URL: repository, https://github.com/SpikeInterface/
 spikeinterface Project-URL: documentation, https://
 spikeinterface.readthedocs.io/ Project-URL: changelog, https://
@@ -10,15 +10,16 @@
 Language :: Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT
 License Classifier: Intended Audience :: Science/Research Classifier: Operating
 System :: POSIX :: Linux Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS Classifier: Operating System :: OS
 Independent Requires-Python: <4.0,>=3.8 Description-Content-Type: text/markdown
 Provides-Extra: extractors Provides-Extra: streaming_extractors Provides-Extra:
 full Provides-Extra: widgets Provides-Extra: test_core Provides-Extra: test
-License-File: LICENSE # SpikeInterface: a unified framework for spike sorting
+Provides-Extra: docs License-File: LICENSE # SpikeInterface: a unified
+framework for spike sorting
 Latest Release [latest_release]
 Documentation  [latest_documentation]
 License        [license]
 Build Status   [CI_build_status]
 Codecov        [codecov]
 [![Twitter](https://img.shields.io/badge/@spikeinterface-
 %231DA1F2.svg?style=for-the-badge&logo=Twitter&logoColor=white)](https://
```

### Comparing `spikeinterface-0.98.0/README.md` & `spikeinterface-0.98.1/README.md`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/pyproject.toml` & `spikeinterface-0.98.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spikeinterface"
-version = "0.98.0"
+version = "0.98.1"
 authors = [
   { name="Alessio Buccino", email="alessiop.buccino@gmail.com" },
   { name="Samuel Garcia", email="sam.garcia.die@gmail.com" },
 ]
 description = "Python toolkit for analysis, visualization, and comparison of spike sorting output"
 readme = "README.md"
 requires-python = ">=3.8,<4.0"
@@ -16,19 +16,19 @@
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
     "Operating System :: OS Independent"
 ]
 
 dependencies = [
     "numpy",
-    "neo>=0.11.1",
+    "neo>=0.12.0",
     "joblib",
     "threadpoolctl",
     "tqdm",
-    "probeinterface>=0.2.16",
+    "probeinterface>=0.2.17",
 ]
 
 [build-system]
 requires = ["setuptools>=62.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
@@ -135,18 +135,35 @@
     ## sliding_nn
     "pymde",
     "torch",
     "pynndescent",
 
     # for github test : probeinterface and neo from master
     # for release we need pypi, so this need to be commented
-    # "probeinterface @ git+https://github.com/SpikeInterface/probeinterface.git",
-    # "neo @ git+https://github.com/NeuralEnsemble/python-neo.git",
+    # "probeinterface @ git+https://github.com/SpikeInterface/probeinterface.git",
+    # "neo @ git+https://github.com/NeuralEnsemble/python-neo.git",
 ]
 
+docs = [
+    "Sphinx==5.1.1",
+    "sphinx_rtd_theme==1.0.0",
+    "sphinx-gallery",
+    "numpydoc",
+
+    # for notebooks in the gallery
+    "MEArec",   # Use as an example
+    "datalad==0.16.2",  # Download mearec data, not sure if needed as is installed with conda as well because of git-annex
+    "pandas", # Don't know where this is needed
+    "hdbscan",   # For sorters, probably spikingcircus
+    "numba", # For sorters, probably spikingcircus
+    # for release we need pypi, so this needs to be commented
+    # "probeinterface @ git+https://github.com/SpikeInterface/probeinterface.git",  # We always build from the latest version
+    # "neo @ git+https://github.com/NeuralEnsemble/python-neo.git",  # We always build from the latest version
+
+]
 
 [tool.pytest.ini_options]
 markers = [
     "core",
     "extractors",
     "preprocessing",
     "postprocessing",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/__init__.py` & `spikeinterface-0.98.1/src/spikeinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/comparison/__init__.py` & `spikeinterface-0.98.1/src/spikeinterface/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/comparison/basecomparison.py` & `spikeinterface-0.98.1/src/spikeinterface/comparison/basecomparison.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/comparison/collisioncomparison.py` & `spikeinterface-0.98.1/src/spikeinterface/comparison/collisioncomparison.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/comparison/collisionstudy.py` & `spikeinterface-0.98.1/src/spikeinterface/comparison/collisionstudy.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/comparison/comparisontools.py` & `spikeinterface-0.98.1/src/spikeinterface/comparison/comparisontools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/comparison/correlogramcomparison.py` & `spikeinterface-0.98.1/src/spikeinterface/comparison/correlogramcomparison.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/comparison/correlogramstudy.py` & `spikeinterface-0.98.1/src/spikeinterface/comparison/correlogramstudy.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/comparison/groundtruthstudy.py` & `spikeinterface-0.98.1/src/spikeinterface/comparison/groundtruthstudy.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/comparison/hybrid.py` & `spikeinterface-0.98.1/src/spikeinterface/comparison/hybrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
         InjectTemplatesRecording.__init__(
             self, self.injected_sorting, templates, wvf_extractor.nbefore, parent_recording=target_recording
         )
 
         self._kwargs = dict(
             wvf_extractor=str(wvf_extractor.folder.absolute()),
-            injected_sorting=self.injected_sorting.to_dict(),
+            injected_sorting=self.injected_sorting,
             unit_ids=unit_ids,
             max_injected_per_unit=max_injected_per_unit,
             injected_rate=injected_rate,
             refractory_period_ms=refractory_period_ms,
             injected_sorting_folder=None,
         )
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/comparison/multicomparisons.py` & `spikeinterface-0.98.1/src/spikeinterface/comparison/multicomparisons.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,27 +195,27 @@
             "match_score": float(self.match_score),
             "chance_score": float(self.chance_score),
         }
         with (save_folder / "kwargs.json").open("w") as f:
             json.dump(kwargs, f)
         sortings = {}
         for name, sorting in zip(self.name_list, self.object_list):
-            sortings[name] = sorting.to_dict()
+            sortings[name] = sorting.to_dict(recursive=True, relative_to=save_folder)
         with (save_folder / "sortings.json").open("w") as f:
             json.dump(sortings, f)
 
     @staticmethod
     def load_from_folder(folder_path):
         folder_path = Path(folder_path)
         with (folder_path / "kwargs.json").open() as f:
             kwargs = json.load(f)
         with (folder_path / "sortings.json").open() as f:
             dict_sortings = json.load(f)
         name_list = list(dict_sortings.keys())
-        sorting_list = [load_extractor(v) for v in dict_sortings.values()]
+        sorting_list = [load_extractor(v, base_folder=folder_path) for v in dict_sortings.values()]
         mcmp = MultiSortingComparison(sorting_list=sorting_list, name_list=list(name_list), do_matching=False, **kwargs)
         filename = str(folder_path / "multicomparison.gpickle")
         with open(filename, "rb") as f:
             mcmp.graph = pickle.load(f)
         # do step 3 and 4
         mcmp._clean_graph()
         mcmp._do_agreement()
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/comparison/paircomparisons.py` & `spikeinterface-0.98.1/src/spikeinterface/comparison/paircomparisons.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/comparison/studytools.py` & `spikeinterface-0.98.1/src/spikeinterface/comparison/studytools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/__init__.py` & `spikeinterface-0.98.1/src/spikeinterface/core/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/base.py` & `spikeinterface-0.98.1/src/spikeinterface/core/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,15 +318,15 @@
         Parameters
         ----------
         include_annotations: bool
             If True, all annotations are added to the dict, by default False
         include_properties: bool
             If True, all properties are added to the dict, by default False
         relative_to: str, Path, or None
-            If not None, file_paths are serialized relative to this path, by default None
+            If not None, files and folders are serialized relative to this path, by default None
             Used in waveform extractor to maintain relative paths to binary files even if the
             containing folder / diretory is moved
         folder_metadata: str, Path, or None
             Folder with numpy `npy` files containing additional information (e.g. probe in BaseRecording) and properties.
         recursive: bool
             If True, all dicitionaries in the kwargs are expanded with `to_dict` as well, by default False.
 
@@ -334,14 +334,17 @@
         -------
         dump_dict: dict
             A dictionary representation of the extractor.
         """
 
         kwargs = self._kwargs
 
+        if relative_to and not recursive:
+            raise ValueError("`relative_to` is only posible when `recursive=True`")
+
         if recursive:
             to_dict_kwargs = dict(
                 include_annotations=include_annotations,
                 include_properties=include_properties,
                 relative_to=None,  # '_make_paths_relative' is already recursive!
                 folder_metadata=folder_metadata,
                 recursive=recursive,
@@ -390,21 +393,21 @@
         if include_properties:
             dump_dict["properties"] = self._properties
         else:
             # include only main properties
             dump_dict["properties"] = {k: self._properties.get(k, None) for k in self._main_properties}
 
         if relative_to is not None:
-            relative_to = Path(relative_to).absolute()
+            relative_to = Path(relative_to).resolve().absolute()
             assert relative_to.is_dir(), "'relative_to' must be an existing directory"
             dump_dict = _make_paths_relative(dump_dict, relative_to)
 
         if folder_metadata is not None:
             if relative_to is not None:
-                folder_metadata = Path(folder_metadata).absolute().relative_to(relative_to)
+                folder_metadata = Path(folder_metadata).resolve().absolute().relative_to(relative_to)
             dump_dict["folder_metadata"] = str(folder_metadata)
 
         return dump_dict
 
     @staticmethod
     def from_dict(dictionary: dict, base_folder: Optional[Union[Path, str]] = None) -> "BaseExtractor":
         """
@@ -543,100 +546,114 @@
         """
         Dumps extractor to json or pickle
 
         Parameters
         ----------
         file_path: str or Path
             The output file (either .json or .pkl/.pickle)
-        relative_to: str, Path, or None
-            If not None, file_paths are serialized relative to this path
+        relative_to: str, Path, True or None
+            If not None, files and folders are serialized relative to this path. If True, the relative folder is the parent folder.
+            This means that file and folder paths in extractor objects kwargs are changed to be relative rather than absolute.
         """
         if str(file_path).endswith(".json"):
             self.dump_to_json(file_path, relative_to=relative_to, folder_metadata=folder_metadata)
         elif str(file_path).endswith(".pkl") or str(file_path).endswith(".pickle"):
             self.dump_to_pickle(file_path, relative_to=relative_to, folder_metadata=folder_metadata)
         else:
             raise ValueError("Dump: file must .json or .pkl")
 
     def dump_to_json(self, file_path: Union[str, Path, None] = None, relative_to=None, folder_metadata=None) -> None:
         """
         Dump recording extractor to json file.
-        The extractor can be re-loaded with load_extractor_from_json(json_file)
+        The extractor can be re-loaded with load_extractor(json_file)
 
         Parameters
         ----------
         file_path: str
             Path of the json file
-        relative_to: str, Path, or None
-            If not None, file_paths are serialized relative to this path
+        relative_to: str, Path, True or None
+            If not None, files and folders are serialized relative to this path. If True, the relative folder is the parent folder.
+            This means that file and folder paths in extractor objects kwargs are changed to be relative rather than absolute.
+        folder_metadata: str, Path, or None
+            Folder with files containing additional information (e.g. probe in BaseRecording) and properties.
         """
-        assert self.check_if_dumpable()
+        assert self.check_if_json_serializable(), "The extractor is not json serializable"
+
+        # Writing paths as relative_to requires recursively expanding the dict
+        if relative_to:
+            relative_to = Path(file_path).parent if relative_to is True else Path(relative_to)
+            relative_to = relative_to.resolve().absolute()
+
         dump_dict = self.to_dict(
-            include_annotations=True, include_properties=False, relative_to=relative_to, folder_metadata=folder_metadata
+            include_annotations=True,
+            include_properties=False,
+            relative_to=relative_to,
+            folder_metadata=folder_metadata,
+            recursive=True,
         )
         file_path = self._get_file_path(file_path, [".json"])
 
         file_path.write_text(
             json.dumps(dump_dict, indent=4, cls=SIJsonEncoder),
             encoding="utf8",
         )
 
     def dump_to_pickle(
         self,
         file_path: Union[str, Path, None] = None,
         include_properties: bool = True,
-        relative_to=None,
         folder_metadata=None,
-        recursive: bool = False,
     ):
         """
         Dump recording extractor to a pickle file.
-        The extractor can be re-loaded with load_extractor_from_json(json_file)
+        The extractor can be re-loaded with load_extractor(pickle_file)
 
         Parameters
         ----------
         file_path: str
             Path of the json file
         include_properties: bool
             If True, all properties are dumped
-        relative_to: str, Path, or None
-            If not None, file_paths are serialized relative to this path
-        recursive: bool
-            If True, all dicitionaries in the kwargs are expanded with `to_dict` as well, by default False.
+        folder_metadata: str, Path, or None
+            Folder with files containing additional information (e.g. probe in BaseRecording) and properties.
         """
-        assert self.check_if_dumpable()
+        assert self.check_if_dumpable(), "The extractor is not dumpable"
+
         dump_dict = self.to_dict(
             include_annotations=True,
             include_properties=include_properties,
-            relative_to=relative_to,
             folder_metadata=folder_metadata,
-            recursive=recursive,
+            recursive=False,
         )
         file_path = self._get_file_path(file_path, [".pkl", ".pickle"])
 
         file_path.write_bytes(pickle.dumps(dump_dict))
 
     @staticmethod
-    def load(file_path: Union[str, Path], base_folder=None) -> "BaseExtractor":
+    def load(file_path: Union[str, Path], base_folder: Optional[Union[Path, str, bool]] = None) -> "BaseExtractor":
         """
         Load extractor from file path (.json or .pkl)
 
         Used both after:
           * dump(...) json or pickle file
           * save (...)  a folder which contain data  + json (or pickle) + metadata.
+
         """
 
         file_path = Path(file_path)
+        if base_folder is True:
+            base_folder = file_path.parent
+
         if file_path.is_file():
             # standard case based on a file (json or pickle)
             if str(file_path).endswith(".json"):
-                with open(str(file_path), "r") as f:
+                with open(file_path, "r") as f:
                     d = json.load(f)
             elif str(file_path).endswith(".pkl") or str(file_path).endswith(".pickle"):
-                with open(str(file_path), "rb") as f:
+                with open(file_path, "rb") as f:
                     d = pickle.load(f)
             else:
                 raise ValueError(f"Impossible to load {file_path}")
             if "warning" in d and "not dumpable" in d["warning"]:
                 print("The extractor was not dumpable")
                 return None
             extractor = BaseExtractor.from_dict(d, base_folder=base_folder)
@@ -917,15 +934,15 @@
 
         cached = read_zarr(zarr_path)
 
         return cached
 
 
 def _make_paths_relative(d, relative) -> dict:
-    relative = str(Path(relative).absolute())
+    relative = str(Path(relative).resolve().absolute())
     func = lambda p: os.path.relpath(str(p), start=relative)
     return recursive_path_modifier(d, func, target="path", copy=True)
 
 
 def _make_paths_absolute(d, base):
     base = Path(base)
     func = lambda p: str((base / p).resolve().absolute())
@@ -1026,22 +1043,27 @@
       * a json file
       * a pickle file
       * folder (after save)
       * a zarr folder (after save)
 
     Parameters
     ----------
-    file_or_folder_or_dict: dictionary or folder or file (json, pickle)
+    file_or_folder_or_dict : dictionary or folder or file (json, pickle)
+        The file path, folder path, or dictionary to load the extractor from
+    base_folder : str | Path | bool (optional)
+        The base folder to make relative paths absolute.
+        If True and file_or_folder_or_dict is a file, the parent folder of the file is used.
 
     Returns
     -------
     extractor: Recording or Sorting
         The loaded extractor object
     """
     if isinstance(file_or_folder_or_dict, dict):
+        assert not isinstance(base_folder, bool), "`base_folder` must be a string or Path when loading from dict"
         return BaseExtractor.from_dict(file_or_folder_or_dict, base_folder=base_folder)
     else:
         return BaseExtractor.load(file_or_folder_or_dict, base_folder=base_folder)
 
 
 def load_extractor_from_dict(d, base_folder=None) -> BaseExtractor:
     warnings.warn("Use load_extractor(..) instead")
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/baseevent.py` & `spikeinterface-0.98.1/src/spikeinterface/core/baseevent.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/baserecording.py` & `spikeinterface-0.98.1/src/spikeinterface/core/baserecording.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/baserecordingsnippets.py` & `spikeinterface-0.98.1/src/spikeinterface/core/baserecordingsnippets.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         else:
             return True
 
     def has_probe(self):
         return "contact_vector" in self.get_property_keys()
 
     def has_channel_location(self):
-        return self.has_probe() or "channel_location" in self.get_property_keys()
+        return self.has_probe() or "location" in self.get_property_keys()
 
     def is_filtered(self):
         # the is_filtered is handle with annotation
         return self._annotations.get("is_filtered", False)
 
     def _channel_slice(self, channel_ids, renamed_channel_ids=None):
         raise NotImplementedError
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/basesnippets.py` & `spikeinterface-0.98.1/src/spikeinterface/core/basesnippets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/basesorting.py` & `spikeinterface-0.98.1/src/spikeinterface/core/basesorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/binaryfolder.py` & `spikeinterface-0.98.1/src/spikeinterface/core/binaryfolder.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         d = _make_paths_absolute(d, folder_path)
 
         BinaryRecordingExtractor.__init__(self, **d["kwargs"])
 
         folder_metadata = folder_path
         self.load_metadata_from_folder(folder_metadata)
 
-        self._kwargs = dict(folder_path=str(folder_path.absolute()))
+        self._kwargs = dict(folder_path=str(Path(folder_path).absolute()))
         self._bin_kwargs = d["kwargs"]
         if "num_channels" not in self._bin_kwargs:
             assert "num_chan" in self._bin_kwargs, "Cannot find num_channels or num_chan in binary.json"
             self._bin_kwargs["num_channels"] = self._bin_kwargs["num_chan"]
 
     def is_binary_compatible(self):
         return True
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/binaryrecordingextractor.py` & `spikeinterface-0.98.1/src/spikeinterface/core/binaryrecordingextractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         if gain_to_uV is not None:
             self.set_channel_gains(gain_to_uV)
 
         if offset_to_uV is not None:
             self.set_channel_offsets(offset_to_uV)
 
         self._kwargs = {
-            "file_paths": [str(e.absolute()) for e in file_path_list],
+            "file_paths": [str(Path(e).absolute()) for e in file_path_list],
             "sampling_frequency": sampling_frequency,
             "t_starts": t_starts,
             "num_channels": num_channels,
             "dtype": dtype.str,
             "channel_ids": channel_ids,
             "time_axis": time_axis,
             "file_offset": file_offset,
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/channelsaggregationrecording.py` & `spikeinterface-0.98.1/src/spikeinterface/core/channelsaggregationrecording.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/channelslice.py` & `spikeinterface-0.98.1/src/spikeinterface/core/channelslice.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/core_tools.py` & `spikeinterface-0.98.1/src/spikeinterface/core/core_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/datasets.py` & `spikeinterface-0.98.1/src/spikeinterface/core/datasets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/frameslicerecording.py` & `spikeinterface-0.98.1/src/spikeinterface/core/frameslicerecording.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/frameslicesorting.py` & `spikeinterface-0.98.1/src/spikeinterface/core/frameslicesorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/generate.py` & `spikeinterface-0.98.1/src/spikeinterface/core/generate.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/globals.py` & `spikeinterface-0.98.1/src/spikeinterface/core/globals.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/injecttemplates.py` & `spikeinterface-0.98.1/src/spikeinterface/core/injecttemplates.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/job_tools.py` & `spikeinterface-0.98.1/src/spikeinterface/core/job_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/npyfoldersnippets.py` & `spikeinterface-0.98.1/src/spikeinterface/core/npyfoldersnippets.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,12 +44,12 @@
         d = _make_paths_absolute(d, folder_path)
 
         NpySnippetsExtractor.__init__(self, **d["kwargs"])
 
         folder_metadata = folder_path
         self.load_metadata_from_folder(folder_metadata)
 
-        self._kwargs = dict(folder_path=str(folder_path.absolute()))
+        self._kwargs = dict(folder_path=str(Path(folder_path).absolute()))
         self._bin_kwargs = d["kwargs"]
 
 
 read_npy_snippets_folder = define_function_from_class(source_class=NpyFolderSnippets, name="read_npy_snippets_folder")
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/npysnippetsextractor.py` & `spikeinterface-0.98.1/src/spikeinterface/core/npysnippetsextractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         if gain_to_uV is not None:
             self.set_channel_gains(gain_to_uV)
 
         if offset_to_uV is not None:
             self.set_channel_offsets(offset_to_uV)
 
         self._kwargs = {
-            "file_paths": [str(f) for f in file_paths],
+            "file_paths": [str(Path(f).absolute()) for f in file_paths],
             "sampling_frequency": sampling_frequency,
             "channel_ids": channel_ids,
             "nbefore": nbefore,
             "gain_to_uV": gain_to_uV,
             "offset_to_uV": offset_to_uV,
         }
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/npzfolder.py` & `spikeinterface-0.98.1/src/spikeinterface/core/npzfolder.py`

 * *Files 24% similar despite different names*

```diff
@@ -43,12 +43,12 @@
         d = _make_paths_absolute(d, folder_path)
 
         NpzSortingExtractor.__init__(self, **d["kwargs"])
 
         folder_metadata = folder_path
         self.load_metadata_from_folder(folder_metadata)
 
-        self._kwargs = dict(folder_path=str(folder_path.absolute()))
+        self._kwargs = dict(folder_path=str(Path(folder_path).absolute()))
         self._npz_kwargs = d["kwargs"]
 
 
 read_npz_folder = define_function_from_class(source_class=NpzFolderSorting, name="read_npz_folder")
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/npzsortingextractor.py` & `spikeinterface-0.98.1/src/spikeinterface/core/npzsortingextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/numpyextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/core/numpyextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/old_api_utils.py` & `spikeinterface-0.98.1/src/spikeinterface/core/old_api_utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/recording_tools.py` & `spikeinterface-0.98.1/src/spikeinterface/core/recording_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/segmentutils.py` & `spikeinterface-0.98.1/src/spikeinterface/core/segmentutils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/snippets_tools.py` & `spikeinterface-0.98.1/src/spikeinterface/core/snippets_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/sparsity.py` & `spikeinterface-0.98.1/src/spikeinterface/core/sparsity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/template_tools.py` & `spikeinterface-0.98.1/src/spikeinterface/core/template_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/testing.py` & `spikeinterface-0.98.1/src/spikeinterface/core/testing.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/unitsaggregationsorting.py` & `spikeinterface-0.98.1/src/spikeinterface/core/unitsaggregationsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/unitsselectionsorting.py` & `spikeinterface-0.98.1/src/spikeinterface/core/unitsselectionsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/waveform_extractor.py` & `spikeinterface-0.98.1/src/spikeinterface/core/waveform_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -917,18 +917,18 @@
                 shutil.rmtree(folder)
             assert not folder.is_dir(), "Folder already exists. Use 'overwrite=True'"
             zarr_root = zarr.open(str(folder), mode="w")
             # write metadata
             zarr_root.attrs["params"] = check_json(self._params)
             if self.has_recording():
                 if self.recording.check_if_json_serializable():
-                    rec_dict = self.recording.to_dict(relative_to=relative_to)
+                    rec_dict = self.recording.to_dict(relative_to=relative_to, recursive=True)
                     zarr_root.attrs["recording"] = check_json(rec_dict)
             if self.sorting.check_if_json_serializable():
-                sort_dict = self.sorting.to_dict(relative_to=relative_to)
+                sort_dict = self.sorting.to_dict(relative_to=relative_to, recursive=True)
                 zarr_root.attrs["sorting"] = check_json(sort_dict)
             else:
                 warn(
                     "Sorting object is not dumpable, which might result in downstream errors for "
                     "parallel processing. To make the sorting dumpable, use the `sorting.save()` function."
                 )
             recording_info = zarr_root.create_group("recording_info")
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/waveform_tools.py` & `spikeinterface-0.98.1/src/spikeinterface/core/waveform_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/core/zarrrecordingextractor.py` & `spikeinterface-0.98.1/src/spikeinterface/core/zarrrecordingextractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
         if storage_options is None:
             if isinstance(root_path, str):
                 root_path_init = root_path
                 root_path = Path(root_path)
             else:
                 root_path_init = str(root_path)
-            root_path_kwarg = str(root_path.absolute())
+            root_path_kwarg = str(Path(root_path).absolute())
         else:
             root_path_init = root_path
             root_path_kwarg = root_path_init
 
         self._root = zarr.open(root_path_init, mode="r", storage_options=storage_options)
 
         sampling_frequency = self._root.attrs.get("sampling_frequency", None)
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/curation/__init__.py` & `spikeinterface-0.98.1/src/spikeinterface/curation/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/curation/auto_merge.py` & `spikeinterface-0.98.1/src/spikeinterface/curation/auto_merge.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/curation/curation_tools.py` & `spikeinterface-0.98.1/src/spikeinterface/curation/curation_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/curation/curationsorting.py` & `spikeinterface-0.98.1/src/spikeinterface/curation/curationsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/curation/mergeunitssorting.py` & `spikeinterface-0.98.1/src/spikeinterface/curation/mergeunitssorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/curation/remove_duplicated_spikes.py` & `spikeinterface-0.98.1/src/spikeinterface/curation/remove_duplicated_spikes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/curation/remove_excess_spikes.py` & `spikeinterface-0.98.1/src/spikeinterface/curation/remove_excess_spikes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/curation/remove_redundant.py` & `spikeinterface-0.98.1/src/spikeinterface/curation/remove_redundant.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/curation/sortingview_curation.py` & `spikeinterface-0.98.1/src/spikeinterface/curation/sortingview_curation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/curation/splitunitsorting.py` & `spikeinterface-0.98.1/src/spikeinterface/curation/splitunitsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/exporters/report.py` & `spikeinterface-0.98.1/src/spikeinterface/exporters/report.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/exporters/to_phy.py` & `spikeinterface-0.98.1/src/spikeinterface/exporters/to_phy.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     np.save(str(output_folder / "spike_templates.npy"), spike_labels[:, np.newaxis])
     np.save(str(output_folder / "spike_clusters.npy"), spike_labels[:, np.newaxis])
 
     # export templates/templates_ind/similar_templates
     # shape (num_units, num_samples, max_num_channels)
     max_num_channels = max(len(chan_inds) for chan_inds in sparse_dict.values())
     num_samples = waveform_extractor.nbefore + waveform_extractor.nafter
-    templates = np.zeros((len(unit_ids), num_samples, max_num_channels), dtype=waveform_extractor.dtype)
+    templates = np.zeros((len(unit_ids), num_samples, max_num_channels), dtype="float64")
     # here we pad template inds with -1 if len of sparse channels is unequal
     templates_ind = -np.ones((len(unit_ids), max_num_channels), dtype="int64")
     for unit_ind, unit_id in enumerate(unit_ids):
         chan_inds = sparse_dict[unit_id]
         template = waveform_extractor.get_template(unit_id, mode=template_mode, sparsity=sparsity)
         templates[unit_ind, :, :][:, : len(chan_inds)] = template
         templates_ind[unit_ind, : len(chan_inds)] = chan_inds
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/alfsortingextractor.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/alfsortingextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/bids.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/bids.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/cbin_ibl.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/cbin_ibl.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,18 @@
                 num_channels_per_adc = 16
             else:  # NP1.0
                 num_channels_per_adc = 12
 
             sample_shifts = get_neuropixels_sample_shifts(self.get_num_channels(), num_channels_per_adc)
             self.set_property("inter_sample_shift", sample_shifts)
 
-        self._kwargs = {"folder_path": str(folder_path.absolute()), "load_sync_channel": load_sync_channel}
+        self._kwargs = {
+            "folder_path": str(Path(folder_path).absolute()),
+            "load_sync_channel": load_sync_channel,
+        }
 
 
 class CBinIblRecordingSegment(BaseRecordingSegment):
     def __init__(self, cbuffer, sampling_frequency, load_sync_channel):
         BaseRecordingSegment.__init__(self, sampling_frequency=sampling_frequency)
         self._cbuffer = cbuffer
         self._load_sync_channel = load_sync_channel
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/cellexplorersortingextractor.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/cellexplorersortingextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/combinatoextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/combinatoextractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     installation_mesg = "To use the CombinatoSortingExtractor install h5py: \n\n pip install h5py\n\n"
     name = "combinato"
 
     def __init__(self, folder_path, sampling_frequency=None, user="simple", det_sign="both", keep_good_only=True):
         folder_path = Path(folder_path)
         assert folder_path.is_dir(), "Folder {} doesn't exist".format(folder_path)
         if sampling_frequency is None:
-            h5_path = str(folder_path) + ".h5"
+            h5_path = str(Path(folder_path).absolute()) + ".h5"
             if Path(h5_path).exists():
                 with h5py.File(h5_path, mode="r") as f:
                     sampling_frequency = f["sr"][0]
 
         # ~ self.set_sampling_frequency(sampling_frequency)
         det_file = str(folder_path / Path("data_" + folder_path.stem + ".h5"))
         sort_cat_files = []
@@ -81,15 +81,15 @@
                     metadata[unit_counter] = {"group_type": group_type[gr]}
                     unit_counter = unit_counter + 1
         unit_ids = np.arange(unit_counter, dtype="int64")
         BaseSorting.__init__(self, sampling_frequency, unit_ids)
         self.add_sorting_segment(CombinatoSortingSegment(spiketrains))
         self.set_property("unsorted", np.array([metadata[u]["group_type"] == 0 for u in range(unit_counter)]))
         self.set_property("artifact", np.array([metadata[u]["group_type"] == -1 for u in range(unit_counter)]))
-        self._kwargs = {"folder_path": str(folder_path), "user": user, "det_sign": det_sign}
+        self._kwargs = {"folder_path": str(Path(folder_path).absolute()), "user": user, "det_sign": det_sign}
 
         self.extra_requirements.append("h5py")
 
 
 class CombinatoSortingSegment(BaseSortingSegment):
     def __init__(self, spiketrains):
         BaseSortingSegment.__init__(self)
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/extractorlist.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/extractorlist.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/hdsortextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/hdsortextractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             else:
                 template = unit["footprint"]
             templates.append(template)
             templates_frames_cut_before.append(unit["cutLeft"].flatten())
         self.set_property("template", np.array(templates))
         self.set_property("template_frames_cut_before", np.array(templates_frames_cut_before))
 
-        self._kwargs = {"file_path": str(file_path), "keep_good_only": keep_good_only}
+        self._kwargs = {"file_path": str(Path(file_path).absolute()), "keep_good_only": keep_good_only}
 
         # TODO features
         # ~ for uc, unit in enumerate(units):
         # ~ unit_id = int(_squeeze_ds(unit["ID"]))
         # ~ self.set_unit_spike_features(unit_id, "amplitudes", _squeeze(unit["spikeAmplitudes"]))
         # ~ self.set_unit_spike_features(unit_id, "detection_channel", _squeeze(unit["detectionChannel"]).astype(np.int))
         # ~ idx = unit["detectionChannel"].astype(int) - 1
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/herdingspikesextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/herdingspikesextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/iblstreamingrecording.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/iblstreamingrecording.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/klustaextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/klustaextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/matlabhelpers.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/matlabhelpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if not isinstance(file_path, Path):
             raise TypeError(f"Expected a str or Path file_path but got '{type(file_path).__name__}'")
 
         file_path = file_path.resolve()  # get absolute path to this file
         if not file_path.is_file():
             raise ValueError(f"Specified file path '{file_path}' is not a file.")
 
-        self._kwargs = {"file_path": str(file_path.absolute())}
+        self._kwargs = {"file_path": str(Path(file_path).absolute())}
 
         try:  # load old-style (up to 7.2) .mat file
             self._data = loadmat(file_path, matlab_compatible=True)
             self._old_style_mat = True
         except NameError:  # loadmat not defined
             raise ImportError("Old-style .mat file given, but `loadmat` is not defined.")
         except NotImplementedError:  # new style .mat file
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/mclustextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/mclustextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/mcsh5extractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/mcsh5extractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/mdaextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/mdaextractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,23 +192,26 @@
     """
 
     extractor_name = "MdaSorting"
     mode = "file"
     name = "mda"
 
     def __init__(self, file_path, sampling_frequency):
-        firings = readmda(str(file_path))
+        firings = readmda(str(Path(file_path).absolute()))
         labels = firings[2, :]
         unit_ids = np.unique(labels).astype(int)
         BaseSorting.__init__(self, unit_ids=unit_ids, sampling_frequency=sampling_frequency)
 
         sorting_segment = MdaSortingSegment(firings)
         self.add_sorting_segment(sorting_segment)
 
-        self._kwargs = {"file_path": str(Path(file_path).absolute()), "sampling_frequency": sampling_frequency}
+        self._kwargs = {
+            "file_path": str(Path(file_path).absolute()),
+            "sampling_frequency": sampling_frequency,
+        }
 
     @staticmethod
     def write_sorting(sorting, save_path, write_primary_channels=False):
         assert sorting.get_num_segments() == 1, "MdaSorting.write_sorting() can only write a single segment " "sorting"
         unit_ids = sorting.get_unit_ids()
         times_list = []
         labels_list = []
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/__init__.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/alphaomega.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/alphaomega.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor, NeoBaseEventExtractor
 
 
 class AlphaOmegaRecordingExtractor(NeoBaseRecordingExtractor):
     """
@@ -28,15 +30,15 @@
     name = "alphaomega"
 
     def __init__(self, folder_path, lsx_files=None, stream_id="RAW", stream_name=None, all_annotations=False):
         neo_kwargs = self.map_to_neo_kwargs(folder_path, lsx_files)
         NeoBaseRecordingExtractor.__init__(
             self, stream_id=stream_id, stream_name=stream_name, all_annotations=all_annotations, **neo_kwargs
         )
-        self._kwargs.update(dict(folder_path=str(folder_path), lsx_files=lsx_files))
+        self._kwargs.update(dict(folder_path=str(Path(folder_path).absolute()), lsx_files=lsx_files))
 
     @classmethod
     def map_to_neo_kwargs(cls, folder_path, lsx_files=None):
         neo_kwargs = {
             "dirname": str(folder_path),
             "lsx_files": lsx_files,
         }
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/axona.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/axona.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor
 
 
 class AxonaRecordingExtractor(NeoBaseRecordingExtractor):
     """
@@ -20,15 +22,15 @@
     mode = "folder"
     NeoRawIOClass = "AxonaRawIO"
     name = "axona"
 
     def __init__(self, file_path, all_annotations=False):
         neo_kwargs = self.map_to_neo_kwargs(file_path)
         NeoBaseRecordingExtractor.__init__(self, all_annotations=all_annotations, **neo_kwargs)
-        self._kwargs.update({"file_path": file_path})
+        self._kwargs.update({"file_path": str(Path(file_path).absolute())})
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path):
         neo_kwargs = {"filename": str(file_path)}
         return neo_kwargs
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/biocam.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/biocam.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 import probeinterface as pi
 
 from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor
 
 
@@ -53,15 +55,21 @@
         if electrode_width is not None:
             probe_kwargs["electrode_width"] = electrode_width
         probe = pi.read_3brain(file_path, **probe_kwargs)
         self.set_probe(probe, in_place=True)
         self.set_property("row", self.get_property("contact_vector")["row"])
         self.set_property("col", self.get_property("contact_vector")["col"])
 
-        self._kwargs.update({"file_path": str(file_path), "mea_pitch": mea_pitch, "electrode_width": electrode_width})
+        self._kwargs.update(
+            {
+                "file_path": str(Path(file_path).absolute()),
+                "mea_pitch": mea_pitch,
+                "electrode_width": electrode_width,
+            }
+        )
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path):
         neo_kwargs = {"filename": str(file_path)}
         return neo_kwargs
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/blackrock.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/blackrock.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             self,
             stream_id=stream_id,
             stream_name=stream_name,
             all_annotations=all_annotations,
             use_names_as_ids=use_names_as_ids,
             **neo_kwargs,
         )
-        self._kwargs.update({"file_path": str(file_path)})
+        self._kwargs.update({"file_path": str(Path(file_path).absolute())})
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path):
         neo_kwargs = {"filename": str(file_path)}
         return neo_kwargs
 
 
@@ -103,15 +103,15 @@
             sampling_frequency=sampling_frequency,
             stream_id=stream_id,
             stream_name=stream_name,
             **neo_kwargs,
         )
 
         self._kwargs = {
-            "file_path": file_path,
+            "file_path": str(Path(file_path).absolute()),
             "sampling_frequency": sampling_frequency,
             "stream_id": stream_id,
             "stream_name": stream_name,
         }
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path):
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/ced.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/ced.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor
 
 
 class CedRecordingExtractor(NeoBaseRecordingExtractor):
     """
@@ -30,15 +32,15 @@
     name = "ced"
 
     def __init__(self, file_path, stream_id=None, stream_name=None, all_annotations=False):
         neo_kwargs = self.map_to_neo_kwargs(file_path)
         NeoBaseRecordingExtractor.__init__(
             self, stream_id=stream_id, stream_name=stream_name, all_annotations=all_annotations, **neo_kwargs
         )
-        self._kwargs.update(dict(file_path=str(file_path)))
+        self._kwargs.update(dict(file_path=str(Path(file_path).absolute())))
         self.extra_requirements.append("neo[ced]")
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path):
         neo_kwargs = {"filename": str(file_path)}
         return neo_kwargs
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/edf.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/edf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor
 
 
 class EDFRecordingExtractor(NeoBaseRecordingExtractor):
     """
@@ -27,15 +29,15 @@
     name = "edf"
 
     def __init__(self, file_path, stream_id=None, stream_name=None, all_annotations=False):
         neo_kwargs = {"filename": str(file_path)}
         NeoBaseRecordingExtractor.__init__(
             self, stream_id=stream_id, stream_name=stream_name, all_annotations=all_annotations, **neo_kwargs
         )
-        self._kwargs.update({"file_path": str(file_path)})
+        self._kwargs.update({"file_path": str(Path(file_path).absolute())})
         self.extra_requirements.append("neo[edf]")
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path):
         neo_kwargs = {"filename": str(file_path)}
         return neo_kwargs
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/intan.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/intan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor, NeoBaseSortingExtractor
 
 
 class IntanRecordingExtractor(NeoBaseRecordingExtractor):
     """
@@ -32,15 +34,15 @@
             stream_id=stream_id,
             stream_name=stream_name,
             all_annotations=all_annotations,
             use_names_as_ids=use_names_as_ids,
             **neo_kwargs,
         )
 
-        self._kwargs.update(dict(file_path=str(file_path)))
+        self._kwargs.update(dict(file_path=str(Path(file_path).absolute())))
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path):
         neo_kwargs = {"filename": str(file_path)}
         return neo_kwargs
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/maxwell.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/maxwell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from pathlib import Path
 
 import probeinterface as pi
 
 from spikeinterface import BaseEvent, BaseEventSegment
 from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor
@@ -66,15 +67,15 @@
         # well_name is stream_id
         well_name = self.stream_id
         # rec_name auto set by neo
         rec_name = self.neo_reader.rec_name
         probe = pi.read_maxwell(file_path, well_name=well_name, rec_name=rec_name)
         self.set_probe(probe, in_place=True)
         self.set_property("electrode", self.get_property("contact_vector")["electrode"])
-        self._kwargs.update(dict(file_path=str(file_path), rec_name=rec_name))
+        self._kwargs.update(dict(file_path=str(Path(file_path).absolute()), rec_name=rec_name))
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path, rec_name=None):
         neo_kwargs = {"filename": str(file_path), "rec_name": rec_name}
         return neo_kwargs
 
     def install_maxwell_plugin(self, force_download=False):
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/mcsraw.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/mcsraw.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor
 
 
 class MCSRawRecordingExtractor(NeoBaseRecordingExtractor):
     """
@@ -36,15 +38,15 @@
             self,
             stream_id=stream_id,
             stream_name=stream_name,
             block_index=block_index,
             all_annotations=all_annotations,
             **neo_kwargs,
         )
-        self._kwargs.update(dict(file_path=str(file_path)))
+        self._kwargs.update(dict(file_path=str(Path(file_path).absolute())))
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path):
         neo_kwargs = {"filename": str(file_path)}
         return neo_kwargs
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/mearec.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/plexon.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,75 @@
 from pathlib import Path
-from typing import Union
 
-import numpy as np
-
-import probeinterface as pi
+from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor, NeoBaseSortingExtractor
 
 
-class MEArecRecordingExtractor(NeoBaseRecordingExtractor):
+class PlexonRecordingExtractor(NeoBaseRecordingExtractor):
     """
-    Class for reading data from a MEArec simulated data.
+    Class for reading plexon plx files.
 
-    Based on :py:class:`neo.rawio.MEArecRawIO`
+    Based on :py:class:`neo.rawio.PlexonRawIO`
 
     Parameters
     ----------
     file_path: str
         The file path to load the recordings from.
+    stream_id: str, optional
+        If there are several streams, specify the stream id you want to load.
+    stream_name: str, optional
+        If there are several streams, specify the stream name you want to load.
     all_annotations: bool, default: False
         Load exhaustively all annotations from neo.
     """
 
     mode = "file"
-    NeoRawIOClass = "MEArecRawIO"
-    name = "mearec"
+    NeoRawIOClass = "PlexonRawIO"
+    name = "plexon"
 
-    def __init__(self, file_path: Union[str, Path], all_annotations: bool = False):
+    def __init__(self, file_path, stream_id=None, stream_name=None, all_annotations=False):
         neo_kwargs = self.map_to_neo_kwargs(file_path)
-        NeoBaseRecordingExtractor.__init__(self, all_annotations=all_annotations, **neo_kwargs)
-
-        self.extra_requirements.append("mearec")
+        NeoBaseRecordingExtractor.__init__(
+            self, stream_id=stream_id, stream_name=stream_name, all_annotations=all_annotations, **neo_kwargs
+        )
+        self._kwargs.update({"file_path": str(Path(file_path).absolute())})
 
-        probe = pi.read_mearec(file_path)
-        probe.annotations["mearec_name"] = str(probe.annotations["mearec_name"])
-        self.set_probe(probe, in_place=True)
-        self.annotate(is_filtered=True)
+    @classmethod
+    def map_to_neo_kwargs(cls, file_path):
+        neo_kwargs = {"filename": str(file_path)}
+        return neo_kwargs
 
-        if hasattr(self.neo_reader._recgen, "gain_to_uV"):
-            self.set_channel_gains(self.neo_reader._recgen.gain_to_uV)
 
-        self._kwargs.update({"file_path": str(file_path)})
+class PlexonSortingExtractor(NeoBaseSortingExtractor):
+    """
+    Class for reading plexon spiking data (.plx files).
 
-    @classmethod
-    def map_to_neo_kwargs(
-        cls,
-        file_path,
-    ):
-        neo_kwargs = {"filename": str(file_path), "load_spiketrains": False, "load_analogsignal": True}
-        return neo_kwargs
+    Based on :py:class:`neo.rawio.PlexonRawIO`
 
+    Parameters
+    ----------
+    file_path: str
+        The file path to load the recordings from.
+    """
 
-class MEArecSortingExtractor(NeoBaseSortingExtractor):
     mode = "file"
-    NeoRawIOClass = "MEArecRawIO"
-    neo_returns_frames = False
-    name = "mearec"
+    NeoRawIOClass = "PlexonRawIO"
+    name = "plexon"
+    neo_returns_frames = True
 
-    def __init__(self, file_path: Union[str, Path]):
+    def __init__(self, file_path):
         neo_kwargs = self.map_to_neo_kwargs(file_path)
-
-        sampling_frequency = self.read_sampling_frequency(file_path=file_path)
-        NeoBaseSortingExtractor.__init__(self, sampling_frequency=sampling_frequency, use_format_ids=True, **neo_kwargs)
-
-        self._kwargs = {"file_path": str(file_path)}
+        self.neo_reader = NeoBaseSortingExtractor.get_neo_io_reader(self.NeoRawIOClass, **neo_kwargs)
+        self.neo_reader.parse_header()
+        sampling_frequency = self.neo_reader._global_ssampling_rate
+        NeoBaseSortingExtractor.__init__(self, sampling_frequency=sampling_frequency, **neo_kwargs)
+        self._kwargs = {"file_path": str(Path(file_path).absolute())}
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path):
-        neo_kwargs = {"filename": str(file_path), "load_spiketrains": True, "load_analogsignal": False}
+        neo_kwargs = {"filename": str(file_path)}
         return neo_kwargs
 
-    def read_sampling_frequency(self, file_path: Union[str, Path]) -> float:
-        from h5py import File
-
-        with File(file_path, "r") as f:
-            info = f["info"]
-            recordings = info["recordings"]
-            sampling_frequency = recordings["fs"][()]
-
-            if isinstance(sampling_frequency, bytes):
-                sampling_frequency = sampling_frequency.decode("utf-8")
-            elif isinstance(sampling_frequency, np.generic):
-                sampling_frequency = sampling_frequency.item()
-
-        return float(sampling_frequency)
 
-
-def read_mearec(file_path):
-    """Read a MEArec file.
-
-    Parameters
-    ----------
-    file_path: str or Path
-        Path to MEArec h5 file
-
-    Returns
-    -------
-    recording: MEArecRecordingExtractor
-        The recording extractor object
-    sorting: MEArecSortingExtractor
-        The sorting extractor object
-    """
-    recording = MEArecRecordingExtractor(file_path)
-    sorting = MEArecSortingExtractor(file_path)
-    return recording, sorting
+read_plexon = define_function_from_class(source_class=PlexonRecordingExtractor, name="read_plexon")
+read_plexon_sorting = define_function_from_class(source_class=PlexonSortingExtractor, name="read_plexon_sorting")
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/neo_utils.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neo_utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/neobaseextractor.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neobaseextractor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/neuralynx.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neuralynx.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Optional
+from pathlib import Path
 
 from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor, NeoBaseSortingExtractor
 
 
 class NeuralynxRecordingExtractor(NeoBaseRecordingExtractor):
@@ -28,15 +29,15 @@
     name = "neuralynx"
 
     def __init__(self, folder_path, stream_id=None, stream_name=None, all_annotations=False):
         neo_kwargs = self.map_to_neo_kwargs(folder_path)
         NeoBaseRecordingExtractor.__init__(
             self, stream_id=stream_id, stream_name=stream_name, all_annotations=all_annotations, **neo_kwargs
         )
-        self._kwargs.update(dict(folder_path=str(folder_path)))
+        self._kwargs.update(dict(folder_path=str(Path(folder_path).absolute())))
 
     @classmethod
     def map_to_neo_kwargs(cls, folder_path):
         neo_kwargs = {"dirname": str(folder_path)}
         return neo_kwargs
 
 
@@ -57,15 +58,15 @@
         Used to extract information about the sampling frequency and t_start from the analog signal if provided.
     stream_name: str, optional
         Used to extract information about the sampling frequency and t_start from the analog signal if provided.
     """
 
     mode = "folder"
     NeoRawIOClass = "NeuralynxRawIO"
-    neo_returns_timestamps = False
+    neo_returns_frames = True
     need_t_start_from_signal_stream = True
     name = "neuralynx"
 
     def __init__(
         self,
         folder_path: str,
         sampling_frequency: Optional[float] = None,
@@ -78,15 +79,15 @@
             sampling_frequency=sampling_frequency,
             stream_id=stream_id,
             stream_name=stream_name,
             **neo_kwargs,
         )
 
         self._kwargs = {
-            "folder_path": folder_path,
+            "folder_path": str(Path(folder_path).absolute()),
             "sampling_frequency": sampling_frequency,
             "stream_id": stream_id,
             "stream_name": stream_name,
         }
 
     @classmethod
     def map_to_neo_kwargs(cls, folder_path):
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/neuroscope.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/neuroscope.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,26 +47,28 @@
 
     def __init__(self, file_path, xml_file_path=None, stream_id=None, stream_name=None, all_annotations=False):
         neo_kwargs = self.map_to_neo_kwargs(file_path, xml_file_path)
 
         NeoBaseRecordingExtractor.__init__(
             self, stream_id=stream_id, stream_name=stream_name, all_annotations=all_annotations, **neo_kwargs
         )
-        self._kwargs.update(dict(file_path=str(file_path), xml_file_path=xml_file_path))
+        if xml_file_path is not None:
+            xml_file_path = str(Path(xml_file_path).absolute())
+        self._kwargs.update(dict(file_path=str(Path(file_path).absolute()), xml_file_path=xml_file_path))
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path, xml_file_path=None):
         # For this because of backwards compatibility we have a strange convention
         # filename is the xml file
         # binary_file is the binary file in .dat, .lfp, .eeg
 
         if xml_file_path is not None:
-            neo_kwargs = {"binary_file": file_path, "filename": xml_file_path}
+            neo_kwargs = {"binary_file": str(file_path), "filename": str(xml_file_path)}
         else:
-            neo_kwargs = {"filename": file_path}
+            neo_kwargs = {"filename": str(file_path)}
 
         return neo_kwargs
 
 
 class NeuroScopeSortingExtractor(BaseSorting):
     """
     Extracts spiking information from an arbitrary number of .res.%i and .clu.%i files in the general folder path.
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/nix.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/nix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor
 
 
 class NixRecordingExtractor(NeoBaseRecordingExtractor):
     """
@@ -33,15 +35,15 @@
             self,
             stream_id=stream_id,
             stream_name=stream_name,
             block_index=block_index,
             all_annotations=all_annotations,
             **neo_kwargs,
         )
-        self._kwargs.update(dict(file_path=str(file_path), stream_id=stream_id))
+        self._kwargs.update(dict(file_path=str(Path(file_path).absolute()), stream_id=stream_id))
         self.extra_requirements.append("neo[nixio]")
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path):
         neo_kwargs = {"filename": str(file_path)}
         return neo_kwargs
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/openephys.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/openephys.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             self,
             stream_id=stream_id,
             stream_name=stream_name,
             block_index=block_index,
             all_annotations=all_annotations,
             **neo_kwargs,
         )
-        self._kwargs.update(dict(folder_path=str(folder_path)))
+        self._kwargs.update(dict(folder_path=str(Path(folder_path).absolute())))
 
     @classmethod
     def map_to_neo_kwargs(cls, folder_path):
         neo_kwargs = {"dirname": str(folder_path)}
         return neo_kwargs
 
 
@@ -145,16 +145,16 @@
             oe_stream = stream_name
         exp_ids = sorted(list(self.neo_reader.folder_structure[record_node]["experiments"].keys()))
         if block_index is None:
             exp_id = exp_ids[0]
         else:
             exp_id = exp_ids[block_index]
 
-        # do not load probe for NIDQ stream
-        if "NI-DAQmx" not in stream_name:
+        # do not load probe for NIDQ stream or if load_sync_channel is True
+        if "NI-DAQmx" not in stream_name and not load_sync_channel:
             settings_file = self.neo_reader.folder_structure[record_node]["experiments"][exp_id]["settings_file"]
 
             if Path(settings_file).is_file():
                 probe = pi.read_openephys(settings_file=settings_file, stream_name=stream_name, raise_error=False)
             else:
                 probe = None
 
@@ -200,15 +200,15 @@
                 try:
                     self.set_times(times=sync_times, segment_index=segment_index, with_warning=False)
                 except AssertionError:
                     warnings.warn(f"Could not load synchronized timestamps for {stream_name}")
 
         self._kwargs.update(
             dict(
-                folder_path=str(folder_path),
+                folder_path=str(Path(folder_path).absolute()),
                 load_sync_channel=load_sync_channel,
                 load_sync_timestamps=load_sync_timestamps,
                 experiment_names=experiment_names,
             )
         )
 
     @classmethod
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/spike2.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/spike2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor, NeoBaseSortingExtractor
 
 
 class Spike2RecordingExtractor(NeoBaseRecordingExtractor):
     """
@@ -27,15 +29,15 @@
     name = "spike2"
 
     def __init__(self, file_path, stream_id=None, stream_name=None, all_annotations=False):
         neo_kwargs = self.map_to_neo_kwargs(file_path)
         NeoBaseRecordingExtractor.__init__(
             self, stream_id=stream_id, stream_name=stream_name, all_annotations=all_annotations, **neo_kwargs
         )
-        self._kwargs.update({"file_path": str(file_path)})
+        self._kwargs.update({"file_path": str(Path(file_path).absolute())})
         self.extra_requirements.append("sonpy")
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path):
         neo_kwargs = {"filename": str(file_path)}
         return neo_kwargs
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/spikegadgets.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/spikegadgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor
 
 
 class SpikeGadgetsRecordingExtractor(NeoBaseRecordingExtractor):
     """
@@ -26,15 +28,15 @@
     name = "spikegadgets"
 
     def __init__(self, file_path, stream_id=None, stream_name=None, block_index=None, all_annotations=False):
         neo_kwargs = self.map_to_neo_kwargs(file_path)
         NeoBaseRecordingExtractor.__init__(
             self, stream_id=stream_id, stream_name=stream_name, all_annotations=all_annotations, **neo_kwargs
         )
-        self._kwargs.update(dict(file_path=str(file_path), stream_id=stream_id))
+        self._kwargs.update(dict(file_path=str(Path(file_path).absolute()), stream_id=stream_id))
 
     @classmethod
     def map_to_neo_kwargs(cls, file_path):
         neo_kwargs = {"filename": str(file_path)}
         return neo_kwargs
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/spikeglx.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/spikeglx.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from packaging import version
 
 import numpy as np
+from pathlib import Path
 
 import neo
 import probeinterface as pi
 
 from spikeinterface.extractors.neuropixels_utils import get_neuropixels_sample_shifts
 
 
@@ -86,15 +87,15 @@
                 chans = pi.get_saved_channel_indices_from_spikeglx_meta(meta_filename)
                 # lets clip to 384 because this contains also the synchro channel
                 chans = chans[chans < total_channels]
                 sample_shifts = sample_shifts[chans]
 
             self.set_property("inter_sample_shift", sample_shifts)
 
-        self._kwargs.update(dict(folder_path=str(folder_path), load_sync_channel=load_sync_channel))
+        self._kwargs.update(dict(folder_path=str(Path(folder_path).absolute()), load_sync_channel=load_sync_channel))
 
     @classmethod
     def map_to_neo_kwargs(cls, folder_path, load_sync_channel=False):
         neo_kwargs = {"dirname": str(folder_path), "load_sync_channel": load_sync_channel}
         return neo_kwargs
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neoextractors/tdt.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neoextractors/tdt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 from spikeinterface.core.core_tools import define_function_from_class
 
 from .neobaseextractor import NeoBaseRecordingExtractor
 
 
 class TdtRecordingExtractor(NeoBaseRecordingExtractor):
     """
@@ -31,15 +33,15 @@
             self,
             stream_id=stream_id,
             stream_name=stream_name,
             block_index=block_index,
             all_annotations=all_annotations,
             **neo_kwargs,
         )
-        self._kwargs.update(dict(folder_path=str(folder_path)))
+        self._kwargs.update(dict(folder_path=str(Path(folder_path).absolute())))
 
     @classmethod
     def map_to_neo_kwargs(cls, folder_path):
         neo_kwargs = {"dirname": str(folder_path)}
         return neo_kwargs
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/neuropixels_utils.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/neuropixels_utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/nwbextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/nwbextractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     This function can stream data from either the "fsspec" or "ros3" protocols.
 
 
     Examples
     --------
     >>> nwbfile = read_nwbfile("data.nwb", stream_mode="ros3")
     """
-    file_path = str(file_path)
+    file_path = str(Path(file_path).absolute())
     from pynwb import NWBHDF5IO, NWBFile
 
     if stream_mode == "fsspec":
         import fsspec
         import h5py
 
         from fsspec.implementations.cached import CachingFileSystem
@@ -473,24 +473,24 @@
             import h5py
 
             self.stream_cache_path = stream_cache_path if stream_cache_path is not None else "cache"
             self.cfs = CachingFileSystem(
                 fs=fsspec.filesystem("http"),
                 cache_storage=self.stream_cache_path,
             )
-            self._file_path = self.cfs.open(str(file_path), "rb")
+            self._file_path = self.cfs.open(str(Path(file_path).absolute()), "rb")
             file = h5py.File(self._file_path)
             self.io = NWBHDF5IO(file=file, mode="r", load_namespaces=True)
 
         elif stream_mode == "ros3":
-            self._file_path = str(file_path)
+            self._file_path = str(Path(file_path).absolute())
             self.io = NWBHDF5IO(self._file_path, mode="r", load_namespaces=True, driver="ros3")
 
         else:
-            self._file_path = str(file_path)
+            self._file_path = str(Path(file_path).absolute())
             self.io = NWBHDF5IO(self._file_path, mode="r", load_namespaces=True)
 
         self._nwbfile = self.io.read()
         units_ids = list(self._nwbfile.units.id[:])
 
         timestamps = None
         if sampling_frequency is None:
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/phykilosortextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/phykilosortextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/shybridextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/shybridextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/spykingcircusextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/spykingcircusextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/toy_example.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/toy_example.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/tridesclousextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/tridesclousextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/waveclussnippetstextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/waveclussnippetstextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/waveclustextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/waveclustextractors.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/extractors/yassextractors.py` & `spikeinterface-0.98.1/src/spikeinterface/extractors/yassextractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         unit_ids = np.unique(spiketrains[:, 1])
 
         # initialize
         sampling_frequency = self.config["recordings"]["sampling_rate"]
         BaseSorting.__init__(self, sampling_frequency, unit_ids)
         self.add_sorting_segment(YassSortingSegment(spiketrains))
 
-        self._kwargs = {"folder_path": str(folder_path)}
+        self._kwargs = {"folder_path": str(Path(folder_path).absolute())}
         self.extra_requirements.append("pyyaml")
 
 
 class YassSortingSegment(BaseSortingSegment):
     def __init__(self, spiketrains):
         BaseSortingSegment.__init__(self)
         # spiketrains is a 2 columns
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/full.py` & `spikeinterface-0.98.1/src/spikeinterface/full.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/postprocessing/__init__.py` & `spikeinterface-0.98.1/src/spikeinterface/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/postprocessing/alignsorting.py` & `spikeinterface-0.98.1/src/spikeinterface/postprocessing/alignsorting.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/postprocessing/amplitude_scalings.py` & `spikeinterface-0.98.1/src/spikeinterface/postprocessing/amplitude_scalings.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/postprocessing/correlograms.py` & `spikeinterface-0.98.1/src/spikeinterface/postprocessing/correlograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/postprocessing/isi.py` & `spikeinterface-0.98.1/src/spikeinterface/postprocessing/isi.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/postprocessing/noise_level.py` & `spikeinterface-0.98.1/src/spikeinterface/postprocessing/noise_level.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/postprocessing/principal_component.py` & `spikeinterface-0.98.1/src/spikeinterface/postprocessing/principal_component.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/postprocessing/spike_amplitudes.py` & `spikeinterface-0.98.1/src/spikeinterface/postprocessing/spike_amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/postprocessing/spike_locations.py` & `spikeinterface-0.98.1/src/spikeinterface/postprocessing/spike_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/postprocessing/template_metrics.py` & `spikeinterface-0.98.1/src/spikeinterface/postprocessing/template_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/postprocessing/template_similarity.py` & `spikeinterface-0.98.1/src/spikeinterface/postprocessing/template_similarity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/postprocessing/template_tools.py` & `spikeinterface-0.98.1/src/spikeinterface/postprocessing/template_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/postprocessing/unit_localization.py` & `spikeinterface-0.98.1/src/spikeinterface/postprocessing/unit_localization.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/align_snippets.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/align_snippets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/astype.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/astype.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/average_across_direction.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/average_across_direction.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/basepreprocessor.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/basepreprocessor.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/clip.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/clip.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/common_reference.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/common_reference.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/correct_lsb.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/correct_lsb.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/deepinterpolation/deepinterpolation.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/deepinterpolation/deepinterpolation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/depth_order.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/depth_order.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,10 +27,15 @@
         order_f, order_r = order_channels_by_depth(parent_recording, channel_ids=channel_ids, dimensions=dimensions)
         reordered_channel_ids = parent_recording.channel_ids[order_f]
         ChannelSliceRecording.__init__(
             self,
             parent_recording,
             channel_ids=reordered_channel_ids,
         )
+        self._kwargs = dict(
+            parent_recording=parent_recording,
+            channel_ids=channel_ids,
+            dimensions=dimensions,
+        )
 
 
 depth_order = define_function_from_class(source_class=DepthOrderRecording, name="depth_order")
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/detect_bad_channels.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/detect_bad_channels.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/directional_derivative.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/directional_derivative.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/filter.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/filter.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/filter_gaussian.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/filter_gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         sf = recording.sampling_frequency
         BasePreprocessor.__init__(self, recording)
         self.annotate(is_filtered=True)
 
         for parent_segment in recording._recording_segments:
             self.add_recording_segment(GaussianFilterRecordingSegment(parent_segment, freq_min, freq_max))
 
-        self._kwargs = {"recording": recording.to_dict(), "freq_min": freq_min, "freq_max": freq_max}
+        self._kwargs = {"recording": recording, "freq_min": freq_min, "freq_max": freq_max}
 
 
 class GaussianFilterRecordingSegment(BasePreprocessorSegment):
     def __init__(self, parent_recording_segment: BaseRecordingSegment, freq_min: float, freq_max: float):
         BasePreprocessorSegment.__init__(self, parent_recording_segment)
 
         self.freq_min = freq_min
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/filter_opencl.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/filter_opencl.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/highpass_spatial_filter.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/highpass_spatial_filter.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/interpolate_bad_channels.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/interpolate_bad_channels.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/motion.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/motion.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,15 +254,15 @@
         motion_info = None
 
     job_kwargs = fix_job_kwargs(job_kwargs)
 
     noise_levels = get_noise_levels(recording, return_scaled=False)
 
     if select_kwargs is None:
-        # maybe do this directly in the folderwhen not None
+        # maybe do this directly in the folder when not None
         gather_mode = "memory"
 
         # node detect
         method = detect_kwargs.pop("method", "locally_exclusive")
         method_class = detect_peak_methods[method]
         node0 = method_class(recording, **detect_kwargs)
 
@@ -324,18 +324,20 @@
         parameters = dict(
             detect_kwargs=detect_kwargs,
             select_kwargs=select_kwargs,
             localize_peaks_kwargs=localize_peaks_kwargs,
             estimate_motion_kwargs=estimate_motion_kwargs,
             interpolate_motion_kwargs=interpolate_motion_kwargs,
             job_kwargs=job_kwargs,
+            sampling_frequency=recording.sampling_frequency,
         )
         (folder / "parameters.json").write_text(json.dumps(parameters, indent=4, cls=SIJsonEncoder), encoding="utf8")
         (folder / "run_times.json").write_text(json.dumps(run_times, indent=4), encoding="utf8")
-        recording.dump_to_json(folder / "recording.json")
+        if recording.check_if_json_serializable():
+            recording.dump_to_json(folder / "recording.json")
 
         np.save(folder / "peaks.npy", peaks)
         np.save(folder / "peak_locations.npy", peak_locations)
         np.save(folder / "temporal_bins.npy", temporal_bins)
         np.save(folder / "motion.npy", motion)
         np.save(folder / "peak_locations.npy", peak_locations)
         if spatial_bins is not None:
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/normalize_scale.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/normalize_scale.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/phase_shift.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/phase_shift.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/preprocessing_tools.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/preprocessing_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/preprocessinglist.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/preprocessinglist.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/rectify.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/rectify.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/remove_artifacts.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/remove_artifacts.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/resample.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/resample.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/silence_periods.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/silence_periods.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/unsigned_to_signed.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/unsigned_to_signed.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/whiten.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/whiten.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/preprocessing/zero_channel_pad.py` & `spikeinterface-0.98.1/src/spikeinterface/preprocessing/zero_channel_pad.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/qualitymetrics/misc_metrics.py` & `spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/misc_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/qualitymetrics/pca_metrics.py` & `spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/pca_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/qualitymetrics/quality_metric_calculator.py` & `spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/quality_metric_calculator.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/qualitymetrics/quality_metric_list.py` & `spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/quality_metric_list.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/qualitymetrics/utils.py` & `spikeinterface-0.98.1/src/spikeinterface/qualitymetrics/utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/basesorter.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/basesorter.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,16 +116,16 @@
                     "Locations can be added to the RecordingExtractor by loading a probe file "
                     "(.prb or .csv) or by setting them manually."
                 )
 
         if output_folder is None:
             output_folder = cls.sorter_name + "_output"
 
-        #  .absolute() not anymore
-        output_folder = Path(output_folder)
+        # Resolve path
+        output_folder = Path(output_folder).absolute()
         sorter_output_folder = output_folder / "sorter_output"
 
         if output_folder.is_dir():
             if remove_existing_folder:
                 shutil.rmtree(str(output_folder))
             else:
                 raise ValueError(f"Folder {output_folder} already exists")
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/combinato.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/combinato.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/hdsort.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/hdsort.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/hdsort_master.m` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/hdsort_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/herdingspikes.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/herdingspikes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/ironclust.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/ironclust.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort2.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         "minfr_goodchannels": 0.1,
         "freq_min": 150,
         "sigmaMask": 30,
         "nPCs": 3,
         "ntbuff": 64,
         "nfilt_factor": 4,
         "NT": None,
+        "AUCsplit": 0.9,
         "wave_length": 61,
         "keep_good_only": False,
         "skip_kilosort_preprocessing": False,
         "scaleproc": None,
         "save_rez_to_mat": False,
         "delete_tmp_files": True,
         "delete_recording_dat": False,
@@ -62,14 +63,15 @@
         "minfr_goodchannels": "Minimum firing rate on a 'good' channel",
         "freq_min": "High-pass filter cutoff frequency",
         "sigmaMask": "Spatial constant in um for computing residual variance of spike",
         "nPCs": "Number of PCA dimensions",
         "ntbuff": "Samples of symmetrical buffer for whitening and spike detection",
         "nfilt_factor": "Max number of clusters per good channel (even temporary ones) 4",
         "NT": "Batch size (if None it is automatically computed)",
+        "AUCsplit": "Threshold on the area under the curve (AUC) criterion for performing a split in the final step",
         "wave_length": "size of the waveform extracted around each detected peak, (Default 61, maximum 81)",
         "keep_good_only": "If True only 'good' units are returned",
         "skip_kilosort_preprocessing": "Can optionaly skip the internal kilosort preprocessing",
         "scaleproc": "int16 scaling of whitened data, if None set to 200.",
         "save_rez_to_mat": "Save the full rez internal struc to mat file",
         "delete_tmp_files": "Whether to delete all temporary files after a successful run",
         "delete_recording_dat": "Whether to delete the 'recording.dat' file after a successful run",
@@ -157,15 +159,15 @@
         # threshold on projections (like in Kilosort1, can be different for last pass like [10 4])
         ops["Th"] = projection_threshold
 
         # how important is the amplitude penalty (like in Kilosort1, 0 means not used, 10 is average, 50 is a lot)
         ops["lam"] = 10.0
 
         # splitting a cluster at the end requires at least this much isolation for each sub-cluster (max = 1)
-        ops["AUCsplit"] = 0.9
+        ops["AUCsplit"] = params["AUCsplit"]
 
         # minimum spike rate (Hz), if a cluster falls below this for too long it gets removed
         ops["minFR"] = params["minFR"]
 
         # number of samples to average over (annealed from first to second value)
         ops["momentum"] = [20.0, 400.0]
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort2_5.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2_5.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         "sig": 20,
         "freq_min": 150,
         "sigmaMask": 30,
         "nPCs": 3,
         "ntbuff": 64,
         "nfilt_factor": 4,
         "NT": None,
+        "AUCsplit": 0.9,
         "do_correction": True,
         "wave_length": 61,
         "keep_good_only": False,
         "skip_kilosort_preprocessing": False,
         "scaleproc": None,
         "save_rez_to_mat": False,
         "delete_tmp_files": True,
@@ -72,14 +73,15 @@
         "freq_min": "High-pass filter cutoff frequency",
         "sigmaMask": "Spatial constant in um for computing residual variance of spike",
         "nPCs": "Number of PCA dimensions",
         "ntbuff": "Samples of symmetrical buffer for whitening and spike detection",
         "nfilt_factor": "Max number of clusters per good channel (even temporary ones) 4",
         "do_correction": "If True drift registration is applied",
         "NT": "Batch size (if None it is automatically computed)",
+        "AUCsplit": "Threshold on the area under the curve (AUC) criterion for performing a split in the final step",
         "keep_good_only": "If True only 'good' units are returned",
         "wave_length": "size of the waveform extracted around each detected peak, (Default 61, maximum 81)",
         "skip_kilosort_preprocessing": "Can optionaly skip the internal kilosort preprocessing",
         "scaleproc": "int16 scaling of whitened data, if None set to 200.",
         "save_rez_to_mat": "Save the full rez internal struc to mat file",
         "delete_tmp_files": "Whether to delete all temporary files after a successful run",
         "delete_recording_dat": "Whether to delete the 'recording.dat' file after a successful run",
@@ -178,15 +180,15 @@
         # threshold on projections (like in Kilosort1, can be different for last pass like [10 4])
         ops["Th"] = projection_threshold
 
         # how important is the amplitude penalty (like in Kilosort1, 0 means not used, 10 is average, 50 is a lot)
         ops["lam"] = 10.0
 
         # splitting a cluster at the end requires at least this much isolation for each sub-cluster (max = 1)
-        ops["AUCsplit"] = 0.9
+        ops["AUCsplit"] = params["AUCsplit"]
 
         # minimum spike rate (Hz), if a cluster falls below this for too long it gets removed
         ops["minFR"] = params["minFR"]
 
         # number of samples to average over (annealed from first to second value)
         ops["momentum"] = [20.0, 400.0]
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort2_5_master.m` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2_5_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort2_master.m` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort2_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort3.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort3.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         "freq_min": 300,
         "sigmaMask": 30,
         "nPCs": 3,
         "ntbuff": 64,
         "nfilt_factor": 4,
         "do_correction": True,
         "NT": None,
+        "AUCsplit": 0.8,
         "wave_length": 61,
         "keep_good_only": False,
         "skip_kilosort_preprocessing": False,
         "scaleproc": None,
         "save_rez_to_mat": False,
         "delete_tmp_files": True,
         "delete_recording_dat": False,
@@ -69,14 +70,15 @@
         "freq_min": "High-pass filter cutoff frequency",
         "sigmaMask": "Spatial constant in um for computing residual variance of spike",
         "nPCs": "Number of PCA dimensions",
         "ntbuff": "Samples of symmetrical buffer for whitening and spike detection",
         "nfilt_factor": "Max number of clusters per good channel (even temporary ones) 4",
         "do_correction": "If True drift registration is applied",
         "NT": "Batch size (if None it is automatically computed)",
+        "AUCsplit": "Threshold on the area under the curve (AUC) criterion for performing a split in the final step",
         "wave_length": "size of the waveform extracted around each detected peak, (Default 61, maximum 81)",
         "keep_good_only": "If True only 'good' units are returned",
         "skip_kilosort_preprocessing": "Can optionaly skip the internal kilosort preprocessing",
         "scaleproc": "int16 scaling of whitened data, if None set to 200.",
         "save_rez_to_mat": "Save the full rez internal struc to mat file",
         "delete_tmp_files": "Whether to delete all temporary files after a successful run",
         "delete_recording_dat": "Whether to delete the 'recording.dat' file after a successful run",
@@ -167,15 +169,15 @@
         # threshold on projections (like in Kilosort1, can be different for last pass like [10 4])
         ops["Th"] = projection_threshold
 
         # how important is the amplitude penalty (like in Kilosort1, 0 means not used, 10 is average, 50 is a lot)
         ops["lam"] = 20.0
 
         # splitting a cluster at the end requires at least this much isolation for each sub-cluster (max = 1)
-        ops["AUCsplit"] = 0.8
+        ops["AUCsplit"] = params["AUCsplit"]
 
         # minimum firing rate on a "good" channel (0 to skip)
         ops["minfr_goodchannels"] = params["minfr_goodchannels"]
 
         # minimum spike rate (Hz), if a cluster falls below this for too long it gets removed
         ops["minFR"] = params["minFR"]
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort3_master.m` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort3_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosort_master.m` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosort_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/kilosortbase.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/kilosortbase.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/klusta.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/klusta.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/klusta_config_default.prm` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/klusta_config_default.prm`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/mountainsort4.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/mountainsort4.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/mountainsort5.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/mountainsort5.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/pykilosort.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/pykilosort.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/sc_config_default.params` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/sc_config_default.params`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/spyking_circus.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/spyking_circus.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/tridesclous.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/tridesclous.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/waveclus.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/waveclus_master.m` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/waveclus_snippets.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus_snippets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/waveclus_snippets_master.m` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/waveclus_snippets_master.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/yass.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/yass.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/external/yass_config_default.yaml` & `spikeinterface-0.98.1/src/spikeinterface/sorters/external/yass_config_default.yaml`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/internal/si_based.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/internal/si_based.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/internal/spyking_circus2.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/internal/spyking_circus2.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/internal/tridesclous2.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/internal/tridesclous2.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/launcher.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
             docker_image = docker_images.get(sorter_name, None)
             singularity_image = singularity_images.get(sorter_name, None)
             _check_container_images(docker_image, singularity_image, sorter_name)
 
             if need_dump:
                 if not recording.check_if_dumpable():
                     raise Exception("recording not dumpable call recording.save() before")
-                recording_arg = recording.to_dict()
+                recording_arg = recording.to_dict(recursive=True)
             else:
                 recording_arg = recording
 
             task_args = (
                 sorter_name,
                 recording_arg,
                 output_folder,
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/runsorter.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/runsorter.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/sorterlist.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/sorterlist.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/utils/constructNPYheader.m` & `spikeinterface-0.98.1/src/spikeinterface/sorters/utils/constructNPYheader.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/utils/misc.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/utils/shellscript.py` & `spikeinterface-0.98.1/src/spikeinterface/sorters/utils/shellscript.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sorters/utils/writeNPY.m` & `spikeinterface-0.98.1/src/spikeinterface/sorters/utils/writeNPY.m`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_clustering.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_clustering.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_matching.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_matching.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_estimation.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_estimation.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,20 +333,18 @@
             ymin, ymax = ax.get_ylim()
             ax.set_ylabel("depth (um)")
             ax.set_xlabel(None)
 
         channel_positions = self.recording.get_channel_locations()
         probe_y_min, probe_y_max = channel_positions[:, 1].min(), channel_positions[:, 1].max()
 
-        times = self.recording.get_times()
-
         peak_locations_corrected = correct_motion_on_peaks(
             self.selected_peaks,
             self.peak_locations,
-            times,
+            self.recording.sampling_frequency,
             self.motion,
             self.temporal_bins,
             self.spatial_bins,
             direction="y",
         )
         if axes is None:
             if show_probe:
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_interpolation.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_motion_interpolation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_localization.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_localization.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_selection.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_peak_selection.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/benchmark/benchmark_tools.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/benchmark/benchmark_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/circus.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/circus.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/clustering_tools.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/clustering_tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/isocut5.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/isocut5.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/main.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/main.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/method_list.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/method_list.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/position.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/position_and_features.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position_and_features.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/position_and_pca.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position_and_pca.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/position_ptp_scaled.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/position_ptp_scaled.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/random_projections.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/random_projections.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/sliding_hdbscan.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/sliding_hdbscan.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/sliding_nn.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/sliding_nn.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
         # )
 
         return labels, peak_labels
 
 
 if HAVE_NUMBA:
 
-    @numba.jit(fastmath=True, cache=True)
+    @numba.jit(nopython=True, fastmath=True, cache=True)
     def sparse_euclidean(x, y, n_samples, n_dense):
         """Euclidean distance metric over sparse vectors, where first n_dense
         elements are indices, and n_samples is the length of the second dimension
         """
         # break out sparse into columns and data
         x_best = x[:n_dense]  # dense indices
         x = x[n_dense:]
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/clustering/triage.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/clustering/triage.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/features_from_peaks.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/features_from_peaks.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/matching/circus.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/circus.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/matching/main.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/main.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/matching/naive.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/naive.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/matching/tdc.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/tdc.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/matching/wobble.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/matching/wobble.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/motion_estimation.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/motion_estimation.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/motion_interpolation.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/motion_interpolation.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 # except ImportError:
 #     HAVE_NUMBA = False
 
 
 def correct_motion_on_peaks(
     peaks,
     peak_locations,
-    times,
+    sampling_frequency,
     motion,
     temporal_bins,
     spatial_bins,
     direction="y",
 ):
     """
     Given the output of estimate_motion(), apply inverse motion on peak locations.
 
     Parameters
     ----------
     peaks: np.array
         peaks vector
     peak_locations: np.array
         peaks location vector
-    times: np.array
-        times vector of recording
+    sampling_frequency: np.array
+        sampling_frequency of the recording
     motion: np.array 2D
         motion.shape[0] equal temporal_bins.shape[0]
         motion.shape[1] equal 1 when "rigid" motion equal temporal_bins.shape[0] when "non-rigid"
     temporal_bins: np.array
         Temporal bins in second.
     spatial_bins: np.array
         Bins for non-rigid motion. If spatial_bins.sahpe[0] == 1 then rigid motion is used.
@@ -47,26 +47,25 @@
     Returns
     -------
     corrected_peak_locations: np.array
         Motion-corrected peak locations
     """
     corrected_peak_locations = peak_locations.copy()
 
+    spike_times = peaks["sample_index"] / sampling_frequency
     if spatial_bins.shape[0] == 1:
         # rigid motion interpolation 1D
-        sample_bins = np.searchsorted(times, temporal_bins)
-        f = scipy.interpolate.interp1d(sample_bins, motion[:, 0], bounds_error=False, fill_value="extrapolate")
-        shift = f(peaks["sample_index"])
+        f = scipy.interpolate.interp1d(temporal_bins, motion[:, 0], bounds_error=False, fill_value="extrapolate")
+        shift = f(spike_times)
         corrected_peak_locations[direction] -= shift
     else:
         # non rigid motion = interpolation 2D
         f = scipy.interpolate.RegularGridInterpolator(
             (temporal_bins, spatial_bins), motion, method="linear", bounds_error=False, fill_value=None
         )
-        spike_times = times[peaks["sample_index"]]
         shift = f(np.c_[spike_times, peak_locations[direction]])
         corrected_peak_locations[direction] -= shift
 
     return corrected_peak_locations
 
 
 def interpolate_motion_on_traces(
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/peak_detection.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,15 +636,15 @@
             sample_inds = np.array(sample_inds.cpu())
             chan_inds = np.array(chan_inds.cpu())
         return sample_inds, chan_inds
 
 
 if HAVE_NUMBA:
 
-    @numba.jit(parallel=False)
+    @numba.jit(nopython=True, parallel=False)
     def _numba_detect_peak_pos(
         traces, traces_center, peak_mask, exclude_sweep_size, abs_threholds, peak_sign, neighbours_mask
     ):
         num_chans = traces_center.shape[1]
         for chan_ind in range(num_chans):
             for s in range(peak_mask.shape[0]):
                 if not peak_mask[s, chan_ind]:
@@ -661,15 +661,15 @@
                         )
                         if not peak_mask[s, chan_ind]:
                             break
                     if not peak_mask[s, chan_ind]:
                         break
         return peak_mask
 
-    @numba.jit(parallel=False)
+    @numba.jit(nopython=True, parallel=False)
     def _numba_detect_peak_neg(
         traces, traces_center, peak_mask, exclude_sweep_size, abs_threholds, peak_sign, neighbours_mask
     ):
         num_chans = traces_center.shape[1]
         for chan_ind in range(num_chans):
             for s in range(peak_mask.shape[0]):
                 if not peak_mask[s, chan_ind]:
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/peak_localization.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_localization.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/peak_pipeline.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_pipeline.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/peak_selection.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/peak_selection.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/tools.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/tools.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/waveforms/neural_network_denoiser.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/neural_network_denoiser.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/waveforms/savgol_denoiser.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/savgol_denoiser.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/waveforms/temporal_pca.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/temporal_pca.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/waveforms/waveform_thresholder.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/waveform_thresholder.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/sortingcomponents/waveforms/waveform_utils.py` & `spikeinterface-0.98.1/src/spikeinterface/sortingcomponents/waveforms/waveform_utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/__init__.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/__init__.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/activity.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/activity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/agreementmatrix.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/agreementmatrix.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/amplitudes.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/basewidget.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/basewidget.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/collisioncomp.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/collisioncomp.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/confusionmatrix.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/confusionmatrix.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/correlogramcomp.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/correlogramcomp.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/correlograms_.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/correlograms_.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/depthamplitude.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/depthamplitude.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/gtcomparison.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/gtcomparison.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/gtstudy.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/gtstudy.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/isidistribution.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/isidistribution.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/multicompgraph.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/multicompgraph.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/presence.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/presence.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/principalcomponent.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/principalcomponent.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/probemap.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/probemap.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/rasters.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/rasters.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/sortingperformance.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/sortingperformance.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/timeseries_.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/timeseries_.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/unitlocalization_.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitlocalization_.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/unitprobemap.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitprobemap.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/unitsummary.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitsummary.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveformdensitymap_.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveformdensitymap_.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveforms_.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/unitwaveforms_.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/_legacy_mpl_widgets/utils.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/_legacy_mpl_widgets/utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/all_amplitudes_distributions.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/all_amplitudes_distributions.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/amplitudes.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/base.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/base.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/crosscorrelograms.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/crosscorrelograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/amplitudes.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/base_ipywidgets.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/base_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/metrics.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/spike_locations.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/spike_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/spikes_on_traces.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/spikes_on_traces.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/timeseries.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/timeseries.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/unit_locations.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/unit_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/unit_waveforms.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/unit_waveforms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/ipywidgets/utils.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/ipywidgets/utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/__init__.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/all_amplitudes_distributions.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/all_amplitudes_distributions.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/amplitudes.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/autocorrelograms.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/autocorrelograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/base_mpl.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/base_mpl.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/crosscorrelograms.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/crosscorrelograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/metrics.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/spike_locations.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/spike_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/spikes_on_traces.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/spikes_on_traces.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/template_similarity.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/template_similarity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/timeseries.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/timeseries.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/unit_depths.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_depths.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/unit_locations.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/unit_summary.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_summary.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/unit_waveforms.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_waveforms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/matplotlib/unit_waveforms_density_map.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/matplotlib/unit_waveforms_density_map.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/metrics.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/motion.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/motion.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,48 +10,61 @@
 
 class MotionWidget(BaseWidget):
     """
     Plot unit depths
 
     Parameters
     ----------
-    recording : RecordingExtractor
-        The recording extractor object
     motion_info: dict
         The motion info return by correct_motion() or load back with load_motion_info()
-    depth_lim: tuple
+    recording : RecordingExtractor, optional
+        The recording extractor object (only used to get "real" times), default None
+    sampling_frequency : float, optional
+        The sampling frequency (needed if recording is None), default None
+    depth_lim : tuple
         The min and max depth to display, default None (min and max of the recording)
-    motion_lim: tuple
+    motion_lim : tuple
         The min and max motion to display, default None (min and max of the motion)
-    color_amplitude: bool
+    color_amplitude : bool
         If True, the color of the scatter points is the amplitude of the peaks, default False
-    scatter_decimate: int
+    scatter_decimate : int
         If > 1, the scatter points are decimated, default None
-    amplitude_cmap: str
+    amplitude_cmap : str
         The colormap to use for the amplitude, default 'inferno'
+    amplitude_clim : tuple
+        The min and max amplitude to display, default None (min and max of the amplitudes)
+    amplitude_alpha : float
+        The alpha of the scatter points, default 0.5
     """
 
     possible_backends = {}
 
     def __init__(
         self,
-        recording,
         motion_info,
+        recording=None,
         depth_lim=None,
         motion_lim=None,
         color_amplitude=False,
         scatter_decimate=None,
         amplitude_cmap="inferno",
+        amplitude_clim=None,
+        amplitude_alpha=1,
         backend=None,
         **backend_kwargs,
     ):
+        times = recording.get_times() if recording is not None else None
+
         plot_data = dict(
-            rec=recording,
+            sampling_frequency=motion_info["parameters"]["sampling_frequency"],
+            times=times,
             depth_lim=depth_lim,
             motion_lim=motion_lim,
             color_amplitude=color_amplitude,
             scatter_decimate=scatter_decimate,
             amplitude_cmap=amplitude_cmap,
+            amplitude_clim=amplitude_clim,
+            amplitude_alpha=amplitude_alpha,
             **motion_info,
         )
 
         BaseWidget.__init__(self, plot_data, backend=backend, **backend_kwargs)
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/quality_metrics.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/sorting_summary.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/sorting_summary.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/__init__.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/__init__.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/amplitudes.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/amplitudes.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/autocorrelograms.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/autocorrelograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/base_sortingview.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/base_sortingview.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/crosscorrelograms.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/crosscorrelograms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/metrics.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/sorting_summary.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/sorting_summary.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/spike_locations.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/spike_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/template_similarity.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/template_similarity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/timeseries.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/timeseries.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/unit_locations.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/unit_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/sortingview/unit_templates.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/sortingview/unit_templates.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/spike_locations.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/spike_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/spikes_on_traces.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/spikes_on_traces.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/template_metrics.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/template_metrics.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/template_similarity.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/template_similarity.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/timeseries.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/timeseries.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/unit_depths.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/unit_depths.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/unit_locations.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/unit_locations.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/unit_summary.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/unit_summary.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/unit_waveforms.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/unit_waveforms.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/unit_waveforms_density_map.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/unit_waveforms_density_map.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/utils.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface/widgets/widget_list.py` & `spikeinterface-0.98.1/src/spikeinterface/widgets/widget_list.py`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface.egg-info/PKG-INFO` & `spikeinterface-0.98.1/src/spikeinterface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spikeinterface
-Version: 0.98.0
+Version: 0.98.1
 Summary: Python toolkit for analysis, visualization, and comparison of spike sorting output
 Author-email: Alessio Buccino <alessiop.buccino@gmail.com>, Samuel Garcia <sam.garcia.die@gmail.com>
 Project-URL: homepage, https://github.com/SpikeInterface/spikeinterface
 Project-URL: repository, https://github.com/SpikeInterface/spikeinterface
 Project-URL: documentation, https://spikeinterface.readthedocs.io/
 Project-URL: changelog, https://spikeinterface.readthedocs.io/en/latest/whatisnew.html
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -18,14 +18,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: extractors
 Provides-Extra: streaming_extractors
 Provides-Extra: full
 Provides-Extra: widgets
 Provides-Extra: test_core
 Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 # SpikeInterface: a unified framework for spike sorting
 
 <table>
 <tr>
   <td>Latest Release</td>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spikeinterface Version: 0.98.0 Summary: Python
+Metadata-Version: 2.1 Name: spikeinterface Version: 0.98.1 Summary: Python
 toolkit for analysis, visualization, and comparison of spike sorting output
 Author-email: Alessio Buccino
 buccino@gmail.com>, Samuel Garcia
 garcia.die@gmail.com> Project-URL: homepage, https://github.com/SpikeInterface/
 spikeinterface Project-URL: repository, https://github.com/SpikeInterface/
 spikeinterface Project-URL: documentation, https://
 spikeinterface.readthedocs.io/ Project-URL: changelog, https://
@@ -10,15 +10,16 @@
 Language :: Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT
 License Classifier: Intended Audience :: Science/Research Classifier: Operating
 System :: POSIX :: Linux Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS Classifier: Operating System :: OS
 Independent Requires-Python: <4.0,>=3.8 Description-Content-Type: text/markdown
 Provides-Extra: extractors Provides-Extra: streaming_extractors Provides-Extra:
 full Provides-Extra: widgets Provides-Extra: test_core Provides-Extra: test
-License-File: LICENSE # SpikeInterface: a unified framework for spike sorting
+Provides-Extra: docs License-File: LICENSE # SpikeInterface: a unified
+framework for spike sorting
 Latest Release [latest_release]
 Documentation  [latest_documentation]
 License        [license]
 Build Status   [CI_build_status]
 Codecov        [codecov]
 [![Twitter](https://img.shields.io/badge/@spikeinterface-
 %231DA1F2.svg?style=for-the-badge&logo=Twitter&logoColor=white)](https://
```

### Comparing `spikeinterface-0.98.0/src/spikeinterface.egg-info/SOURCES.txt` & `spikeinterface-0.98.1/src/spikeinterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spikeinterface-0.98.0/src/spikeinterface.egg-info/requires.txt` & `spikeinterface-0.98.1/src/spikeinterface.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 numpy
-neo>=0.11.1
+neo>=0.12.0
 joblib
 threadpoolctl
 tqdm
-probeinterface>=0.2.16
+probeinterface>=0.2.17
+
+[docs]
+Sphinx==5.1.1
+sphinx_rtd_theme==1.0.0
+sphinx-gallery
+numpydoc
+MEArec
+datalad==0.16.2
+pandas
+hdbscan
+numba
 
 [extractors]
 MEArec>=1.8
 pynwb>=2.3.0
 pyedflib>=0.1.30
 lxml
 scipy
```

