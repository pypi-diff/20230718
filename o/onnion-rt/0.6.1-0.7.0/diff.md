# Comparing `tmp/onnion_rt-0.6.1.tar.gz` & `tmp/onnion_rt-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnion_rt-0.6.1.tar", max compression
+gzip compressed data, was "onnion_rt-0.7.0.tar", max compression
```

## Comparing `onnion_rt-0.6.1.tar` & `onnion_rt-0.7.0.tar`

### file list

```diff
@@ -1,116 +1,117 @@
--rw-r--r--   0        0        0      551 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/LICENSE
--rw-r--r--   0        0        0     2983 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/README.md
--rw-r--r--   0        0        0     5187 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/__init__.py
--rw-r--r--   0        0        0      229 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/abs.py
--rw-r--r--   0        0        0      172 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/acos.py
--rw-r--r--   0        0        0      174 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/acosh.py
--rw-r--r--   0        0        0      420 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/add.py
--rw-r--r--   0        0        0      359 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/and_.py
--rw-r--r--   0        0        0     1711 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/argmax.py
--rw-r--r--   0        0        0     1711 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/argmin.py
--rw-r--r--   0        0        0      172 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/asin.py
--rw-r--r--   0        0        0      174 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/asinh.py
--rw-r--r--   0        0        0      172 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/atan.py
--rw-r--r--   0        0        0      174 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/atanh.py
--rw-r--r--   0        0        0      403 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/bitshift.py
--rw-r--r--   0        0        0      668 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/cast.py
--rw-r--r--   0        0        0      231 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/ceil.py
--rw-r--r--   0        0        0      295 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/celu.py
--rw-r--r--   0        0        0      544 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/clip.py
--rw-r--r--   0        0        0      245 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/compress.py
--rw-r--r--   0        0        0      241 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/concat.py
--rw-r--r--   0        0        0      405 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/concatfromsequence.py
--rw-r--r--   0        0        0     1965 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/constant.py
--rw-r--r--   0        0        0      423 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/constantofshape.py
--rw-r--r--   0        0        0      168 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/cos.py
--rw-r--r--   0        0        0      170 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/cosh.py
--rw-r--r--   0        0        0     1034 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/depthtospace.py
--rw-r--r--   0        0        0      731 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/dequantizelinear.py
--rw-r--r--   0        0        0      175 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/det.py
--rw-r--r--   0        0        0      420 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/div.py
--rw-r--r--   0        0        0     1559 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/dropout.py
--rw-r--r--   0        0        0      513 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/dynamicquantizelinear.py
--rw-r--r--   0        0        0      244 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/einsum.py
--rw-r--r--   0        0        0      353 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/elu.py
--rw-r--r--   0        0        0      356 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/equal.py
--rw-r--r--   0        0        0      227 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/erf.py
--rw-r--r--   0        0        0      116 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/error.py
--rw-r--r--   0        0        0      229 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/exp.py
--rw-r--r--   0        0        0      203 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/expand.py
--rw-r--r--   0        0        0      501 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/eyelike.py
--rw-r--r--   0        0        0      360 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/flatten.py
--rw-r--r--   0        0        0      233 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/floor.py
--rw-r--r--   0        0        0      402 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/gather.py
--rw-r--r--   0        0        0      776 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/gatherelements.py
--rw-r--r--   0        0        0     2249 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/gathernd.py
--rw-r--r--   0        0        0     1188 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/gemm.py
--rw-r--r--   0        0        0      232 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/globalaveragepool.py
--rw-r--r--   0        0        0      227 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/globalmaxpool.py
--rw-r--r--   0        0        0      360 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/greater.py
--rw-r--r--   0        0        0      195 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/greaterorequal.py
--rw-r--r--   0        0        0      684 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/hardmax.py
--rw-r--r--   0        0        0      359 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/hardsigmoid.py
--rw-r--r--   0        0        0      566 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/hardswish.py
--rw-r--r--   0        0        0      240 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/identity.py
--rw-r--r--   0        0        0      335 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/if_.py
--rw-r--r--   0        0        0      992 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/instancenormalization.py
--rw-r--r--   0        0        0      450 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/isinf.py
--rw-r--r--   0        0        0      172 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/isnan.py
--rw-r--r--   0        0        0      346 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/leakyrelu.py
--rw-r--r--   0        0        0      393 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/less.py
--rw-r--r--   0        0        0      189 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/lessorequal.py
--rw-r--r--   0        0        0      229 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/log.py
--rw-r--r--   0        0        0     1546 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/logsoftmax.py
--rw-r--r--   0        0        0     1102 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/loop.py
--rw-r--r--   0        0        0      180 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/matmul.py
--rw-r--r--   0        0        0      481 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/matmulinteger.py
--rw-r--r--   0        0        0      438 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/max.py
--rw-r--r--   0        0        0      427 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/mean.py
--rw-r--r--   0        0        0      438 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/min.py
--rw-r--r--   0        0        0      296 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/mod.py
--rw-r--r--   0        0        0      420 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/mul.py
--rw-r--r--   0        0        0      234 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/neg.py
--rw-r--r--   0        0        0     3095 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/negativeloglikelihoodloss.py
--rw-r--r--   0        0        0     4231 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/nonmaxsuppression.py
--rw-r--r--   0        0        0      216 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/nonzero.py
--rw-r--r--   0        0        0      176 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/not_.py
--rw-r--r--   0        0        0     1167 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/onehot.py
--rw-r--r--   0        0        0      395 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/or_.py
--rw-r--r--   0        0        0     1986 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/pad.py
--rw-r--r--   0        0        0      422 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/pow.py
--rw-r--r--   0        0        0      297 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/prelu.py
--rw-r--r--   0        0        0      735 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/randomnormal.py
--rw-r--r--   0        0        0      818 2023-01-18 09:08:59.195416 onnion_rt-0.6.1/onnion_runtime/randomnormallike.py
--rw-r--r--   0        0        0      732 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/randomuniform.py
--rw-r--r--   0        0        0      815 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/randomuniformlike.py
--rw-r--r--   0        0        0      243 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/range.py
--rw-r--r--   0        0        0      243 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/reciprocal.py
--rw-r--r--   0        0        0      390 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/reducel1.py
--rw-r--r--   0        0        0      402 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/reducel2.py
--rw-r--r--   0        0        0      394 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/reducelogsum.py
--rw-r--r--   0        0        0      405 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/reducelogsumexp.py
--rw-r--r--   0        0        0      470 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/reducemax.py
--rw-r--r--   0        0        0      385 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/reducemean.py
--rw-r--r--   0        0        0      470 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/reducemin.py
--rw-r--r--   0        0        0      385 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/reduceprod.py
--rw-r--r--   0        0        0     1329 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/reducesum.py
--rw-r--r--   0        0        0      400 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/reducesumsquare.py
--rw-r--r--   0        0        0      242 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/relu.py
--rw-r--r--   0        0        0     1304 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/reshape.py
--rw-r--r--   0        0        0      173 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/round.py
--rw-r--r--   0        0        0     1266 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/scatternd.py
--rw-r--r--   0        0        0      195 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/shape.py
--rw-r--r--   0        0        0      260 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/sigmoid.py
--rw-r--r--   0        0        0     1075 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/slice.py
--rw-r--r--   0        0        0      925 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/split.py
--rw-r--r--   0        0        0      418 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/squeeze.py
--rw-r--r--   0        0        0      420 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/sub.py
--rw-r--r--   0        0        0      443 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/tile.py
--rw-r--r--   0        0        0     1563 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/topk.py
--rw-r--r--   0        0        0      256 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/transpose.py
--rw-r--r--   0        0        0      517 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/unsqueeze.py
--rw-r--r--   0        0        0      536 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/utils.py
--rw-r--r--   0        0        0      190 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/onnion_runtime/where.py
--rw-r--r--   0        0        0     1038 2023-01-18 09:08:59.199416 onnion_rt-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3881 1970-01-01 00:00:00.000000 onnion_rt-0.6.1/setup.py
--rw-r--r--   0        0        0     3831 1970-01-01 00:00:00.000000 onnion_rt-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      551 2023-07-18 05:39:08.753049 onnion_rt-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3000 2023-07-18 05:39:08.753049 onnion_rt-0.7.0/README.md
+-rw-r--r--   0        0        0     5267 2023-07-18 05:39:08.753049 onnion_rt-0.7.0/onnion_runtime/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-18 05:39:08.753049 onnion_rt-0.7.0/onnion_runtime/abs.py
+-rw-r--r--   0        0        0      172 2023-07-18 05:39:08.753049 onnion_rt-0.7.0/onnion_runtime/acos.py
+-rw-r--r--   0        0        0      174 2023-07-18 05:39:08.753049 onnion_rt-0.7.0/onnion_runtime/acosh.py
+-rw-r--r--   0        0        0      420 2023-07-18 05:39:08.753049 onnion_rt-0.7.0/onnion_runtime/add.py
+-rw-r--r--   0        0        0      359 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/and_.py
+-rw-r--r--   0        0        0     1711 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/argmax.py
+-rw-r--r--   0        0        0     1711 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/argmin.py
+-rw-r--r--   0        0        0      172 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/asin.py
+-rw-r--r--   0        0        0      174 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/asinh.py
+-rw-r--r--   0        0        0      172 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/atan.py
+-rw-r--r--   0        0        0      174 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/atanh.py
+-rw-r--r--   0        0        0      403 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/bitshift.py
+-rw-r--r--   0        0        0      668 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/cast.py
+-rw-r--r--   0        0        0      231 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/ceil.py
+-rw-r--r--   0        0        0      295 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/celu.py
+-rw-r--r--   0        0        0      544 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/clip.py
+-rw-r--r--   0        0        0      245 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/compress.py
+-rw-r--r--   0        0        0      241 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/concat.py
+-rw-r--r--   0        0        0      405 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/concatfromsequence.py
+-rw-r--r--   0        0        0     1965 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/constant.py
+-rw-r--r--   0        0        0      423 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/constantofshape.py
+-rw-r--r--   0        0        0      168 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/cos.py
+-rw-r--r--   0        0        0      170 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/cosh.py
+-rw-r--r--   0        0        0     1034 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/depthtospace.py
+-rw-r--r--   0        0        0      731 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/dequantizelinear.py
+-rw-r--r--   0        0        0      175 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/det.py
+-rw-r--r--   0        0        0      420 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/div.py
+-rw-r--r--   0        0        0     1559 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/dropout.py
+-rw-r--r--   0        0        0      513 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/dynamicquantizelinear.py
+-rw-r--r--   0        0        0      244 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/einsum.py
+-rw-r--r--   0        0        0      353 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/elu.py
+-rw-r--r--   0        0        0      356 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/equal.py
+-rw-r--r--   0        0        0      227 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/erf.py
+-rw-r--r--   0        0        0      116 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/error.py
+-rw-r--r--   0        0        0      229 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/exp.py
+-rw-r--r--   0        0        0      203 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/expand.py
+-rw-r--r--   0        0        0      501 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/eyelike.py
+-rw-r--r--   0        0        0      360 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/flatten.py
+-rw-r--r--   0        0        0      233 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/floor.py
+-rw-r--r--   0        0        0      402 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/gather.py
+-rw-r--r--   0        0        0      776 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/gatherelements.py
+-rw-r--r--   0        0        0     2249 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/gathernd.py
+-rw-r--r--   0        0        0     1188 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/gemm.py
+-rw-r--r--   0        0        0      232 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/globalaveragepool.py
+-rw-r--r--   0        0        0      227 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/globalmaxpool.py
+-rw-r--r--   0        0        0      360 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/greater.py
+-rw-r--r--   0        0        0      195 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/greaterorequal.py
+-rw-r--r--   0        0        0      684 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/hardmax.py
+-rw-r--r--   0        0        0      359 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/hardsigmoid.py
+-rw-r--r--   0        0        0      566 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/hardswish.py
+-rw-r--r--   0        0        0      240 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/identity.py
+-rw-r--r--   0        0        0      335 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/if_.py
+-rw-r--r--   0        0        0      992 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/instancenormalization.py
+-rw-r--r--   0        0        0      450 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/isinf.py
+-rw-r--r--   0        0        0      172 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/isnan.py
+-rw-r--r--   0        0        0      346 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/leakyrelu.py
+-rw-r--r--   0        0        0      393 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/less.py
+-rw-r--r--   0        0        0      189 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/lessorequal.py
+-rw-r--r--   0        0        0      229 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/log.py
+-rw-r--r--   0        0        0     1546 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/logsoftmax.py
+-rw-r--r--   0        0        0     1102 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/loop.py
+-rw-r--r--   0        0        0      180 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/matmul.py
+-rw-r--r--   0        0        0      481 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/matmulinteger.py
+-rw-r--r--   0        0        0      438 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/max.py
+-rw-r--r--   0        0        0      427 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/mean.py
+-rw-r--r--   0        0        0      438 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/min.py
+-rw-r--r--   0        0        0      296 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/mod.py
+-rw-r--r--   0        0        0      420 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/mul.py
+-rw-r--r--   0        0        0      234 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/neg.py
+-rw-r--r--   0        0        0     3095 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/negativeloglikelihoodloss.py
+-rw-r--r--   0        0        0     4231 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/nonmaxsuppression.py
+-rw-r--r--   0        0        0      216 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/nonzero.py
+-rw-r--r--   0        0        0      176 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/not_.py
+-rw-r--r--   0        0        0     1167 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/onehot.py
+-rw-r--r--   0        0        0      395 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/or_.py
+-rw-r--r--   0        0        0     1986 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/pad.py
+-rw-r--r--   0        0        0      422 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/pow.py
+-rw-r--r--   0        0        0      297 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/prelu.py
+-rw-r--r--   0        0        0      735 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/randomnormal.py
+-rw-r--r--   0        0        0      818 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/randomnormallike.py
+-rw-r--r--   0        0        0      732 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/randomuniform.py
+-rw-r--r--   0        0        0      815 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/randomuniformlike.py
+-rw-r--r--   0        0        0      243 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/range.py
+-rw-r--r--   0        0        0      243 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/reciprocal.py
+-rw-r--r--   0        0        0      390 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/reducel1.py
+-rw-r--r--   0        0        0      402 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/reducel2.py
+-rw-r--r--   0        0        0      394 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/reducelogsum.py
+-rw-r--r--   0        0        0      405 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/reducelogsumexp.py
+-rw-r--r--   0        0        0      470 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/reducemax.py
+-rw-r--r--   0        0        0      385 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/reducemean.py
+-rw-r--r--   0        0        0      470 2023-07-18 05:39:08.757049 onnion_rt-0.7.0/onnion_runtime/reducemin.py
+-rw-r--r--   0        0        0      385 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/reduceprod.py
+-rw-r--r--   0        0        0     1329 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/reducesum.py
+-rw-r--r--   0        0        0      400 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/reducesumsquare.py
+-rw-r--r--   0        0        0      242 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/relu.py
+-rw-r--r--   0        0        0     1304 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/reshape.py
+-rw-r--r--   0        0        0      173 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/round.py
+-rw-r--r--   0        0        0     1266 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/scatternd.py
+-rw-r--r--   0        0        0      195 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/shape.py
+-rw-r--r--   0        0        0      260 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/sigmoid.py
+-rw-r--r--   0        0        0     1075 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/slice.py
+-rw-r--r--   0        0        0     1457 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/softmax.py
+-rw-r--r--   0        0        0      925 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/split.py
+-rw-r--r--   0        0        0      231 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/sqrt.py
+-rw-r--r--   0        0        0      418 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/squeeze.py
+-rw-r--r--   0        0        0      420 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/sub.py
+-rw-r--r--   0        0        0      443 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/tile.py
+-rw-r--r--   0        0        0     1563 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/topk.py
+-rw-r--r--   0        0        0      256 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/transpose.py
+-rw-r--r--   0        0        0      517 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/unsqueeze.py
+-rw-r--r--   0        0        0      536 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/utils.py
+-rw-r--r--   0        0        0      190 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/onnion_runtime/where.py
+-rw-r--r--   0        0        0     1035 2023-07-18 05:39:08.761049 onnion_rt-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3844 1970-01-01 00:00:00.000000 onnion_rt-0.7.0/PKG-INFO
```

### Comparing `onnion_rt-0.6.1/LICENSE` & `onnion_rt-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/README.md` & `onnion_rt-0.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -144,16 +144,18 @@
 - Relu
 - Reshape
 - Round
 - ScatterND
 - Shape
 - Sigmoid
 - Slice
+- Softmax
 - Split
   - argument `split` must be specified
+- Sqrt
 - Squeeze
 - Sub
   - must be from opsetversion >= 7
 - Tile
   - must be from opsetversion >= 6
 - TopK
 - Transpose
```

### Comparing `onnion_rt-0.6.1/onnion_runtime/__init__.py` & `onnion_rt-0.7.0/onnion_runtime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,17 @@
 from .relu import Relu  # noqa: F401
 from .reshape import Reshape  # noqa: F401
 from .round import Round  # noqa: F401
 from .scatternd import ScatterND  # noqa: F401
 from .shape import Shape  # noqa: F401
 from .sigmoid import Sigmoid  # noqa: F401
 from .slice import Slice  # noqa: F401
+from .softmax import Softmax  # noqa: F401
 from .split import Split  # noqa: F401
+from .sqrt import Sqrt  # noqa: F401
 from .squeeze import Squeeze  # noqa: F401
 from .sub import Sub  # noqa: F401
 from .tile import Tile  # noqa: F401
 from .topk import TopK  # noqa: F401
 from .transpose import Transpose  # noqa: F401
 from .unsqueeze import Unsqueeze  # noqa: F401
 from .where import Where  # noqa: F401
```

### Comparing `onnion_rt-0.6.1/onnion_runtime/argmax.py` & `onnion_rt-0.7.0/onnion_runtime/argmax.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/argmin.py` & `onnion_rt-0.7.0/onnion_runtime/argmin.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/cast.py` & `onnion_rt-0.7.0/onnion_runtime/cast.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/clip.py` & `onnion_rt-0.7.0/onnion_runtime/clip.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/constant.py` & `onnion_rt-0.7.0/onnion_runtime/constant.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/depthtospace.py` & `onnion_rt-0.7.0/onnion_runtime/depthtospace.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/dequantizelinear.py` & `onnion_rt-0.7.0/onnion_runtime/dequantizelinear.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/dropout.py` & `onnion_rt-0.7.0/onnion_runtime/dropout.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/dynamicquantizelinear.py` & `onnion_rt-0.7.0/onnion_runtime/dynamicquantizelinear.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/gatherelements.py` & `onnion_rt-0.7.0/onnion_runtime/gatherelements.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/gathernd.py` & `onnion_rt-0.7.0/onnion_runtime/gathernd.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/gemm.py` & `onnion_rt-0.7.0/onnion_runtime/gemm.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/hardmax.py` & `onnion_rt-0.7.0/onnion_runtime/hardmax.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/hardswish.py` & `onnion_rt-0.7.0/onnion_runtime/hardswish.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/instancenormalization.py` & `onnion_rt-0.7.0/onnion_runtime/instancenormalization.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/logsoftmax.py` & `onnion_rt-0.7.0/onnion_runtime/logsoftmax.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/loop.py` & `onnion_rt-0.7.0/onnion_runtime/loop.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/negativeloglikelihoodloss.py` & `onnion_rt-0.7.0/onnion_runtime/negativeloglikelihoodloss.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/nonmaxsuppression.py` & `onnion_rt-0.7.0/onnion_runtime/nonmaxsuppression.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/onehot.py` & `onnion_rt-0.7.0/onnion_runtime/onehot.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/pad.py` & `onnion_rt-0.7.0/onnion_runtime/pad.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/randomnormal.py` & `onnion_rt-0.7.0/onnion_runtime/randomnormal.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/randomnormallike.py` & `onnion_rt-0.7.0/onnion_runtime/randomnormallike.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/randomuniform.py` & `onnion_rt-0.7.0/onnion_runtime/randomuniform.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/randomuniformlike.py` & `onnion_rt-0.7.0/onnion_runtime/randomuniformlike.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/reducesum.py` & `onnion_rt-0.7.0/onnion_runtime/reducesum.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/reshape.py` & `onnion_rt-0.7.0/onnion_runtime/reshape.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/scatternd.py` & `onnion_rt-0.7.0/onnion_runtime/scatternd.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/slice.py` & `onnion_rt-0.7.0/onnion_runtime/slice.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/split.py` & `onnion_rt-0.7.0/onnion_runtime/split.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/topk.py` & `onnion_rt-0.7.0/onnion_runtime/topk.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/unsqueeze.py` & `onnion_rt-0.7.0/onnion_runtime/unsqueeze.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/onnion_runtime/utils.py` & `onnion_rt-0.7.0/onnion_runtime/utils.py`

 * *Files identical despite different names*

### Comparing `onnion_rt-0.6.1/pyproject.toml` & `onnion_rt-0.7.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [tool.poetry]
 name = "onnion-rt"
-version = "0.6.1"
+version = "0.7.0"
 description = "run onnx with only numpy"
 authors = ["Idein Inc."]
 license = "Apache-2.0"
 readme = "README.md"
 keywords = ["onnx"]
 repository = "https://github.com/Idein/onnion/tree/master/runtime"
 packages = [
   { include = "onnion_runtime" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.7"
 # use numpy that has whl for 32bit arm.
 numpy = [
     {version = "^1.19.5, < 1.21.5", python = "< 3.8"},
     {version = "^1.19.5", python = ">= 3.8"}
 ]
 
 [tool.poetry.dev-dependencies]
 pysen = {version = "^0.10.1"}
 black = "22.3.0"
 flake8 = "4.0.1"
 flake8-bugbear = "21.9.2"
 isort = "5.9.3"
-mypy = "0.812"
+mypy = "^1.0"
 pytest = "^6.2.4"
 onnx = "^1.9.0"
 onnxruntime = "^1.8.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `onnion_rt-0.6.1/PKG-INFO` & `onnion_rt-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: onnion-rt
-Version: 0.6.1
+Version: 0.7.0
 Summary: run onnx with only numpy
 Home-page: https://github.com/Idein/onnion/tree/master/runtime
 License: Apache-2.0
 Keywords: onnx
 Author: Idein Inc.
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -165,16 +165,18 @@
 - Relu
 - Reshape
 - Round
 - ScatterND
 - Shape
 - Sigmoid
 - Slice
+- Softmax
 - Split
   - argument `split` must be specified
+- Sqrt
 - Squeeze
 - Sub
   - must be from opsetversion >= 7
 - Tile
   - must be from opsetversion >= 6
 - TopK
 - Transpose
```

