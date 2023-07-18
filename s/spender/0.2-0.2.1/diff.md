# Comparing `tmp/spender-0.2.tar.gz` & `tmp/spender-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spender-0.2.tar", last modified: Tue Jun 20 21:57:41 2023, max compression
+gzip compressed data, was "spender-0.2.1.tar", last modified: Tue Jul 18 02:28:43 2023, max compression
```

## Comparing `spender-0.2.tar` & `spender-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-06-20 21:57:41.661634 spender-0.2/
--rw-r--r--   0 pmelchior   (501) staff       (20)     1082 2022-08-08 22:13:56.000000 spender-0.2/LICENSE
--rw-r--r--   0 pmelchior   (501) staff       (20)     4947 2023-06-20 21:57:41.661492 spender-0.2/PKG-INFO
--rw-r--r--   0 pmelchior   (501) staff       (20)     4259 2023-06-20 21:36:05.000000 spender-0.2/README.md
--rw-r--r--   0 pmelchior   (501) staff       (20)       38 2023-06-20 21:57:41.661673 spender-0.2/setup.cfg
--rw-r--r--   0 pmelchior   (501) staff       (20)     1049 2023-06-20 21:19:50.000000 spender-0.2/setup.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-06-20 21:57:41.659998 spender-0.2/spender/
--rw-r--r--   0 pmelchior   (501) staff       (20)     2791 2023-06-20 20:43:19.000000 spender-0.2/spender/__init__.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-06-20 21:57:41.661080 spender-0.2/spender/data/
--rw-r--r--   0 pmelchior   (501) staff       (20)        0 2022-08-08 22:13:56.000000 spender-0.2/spender/data/__init__.py
--rwxr-xr-x   0 pmelchior   (501) staff       (20)     1082 2023-05-17 22:05:49.000000 spender-0.2/spender/data/emission_lines.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    19391 2023-05-17 22:05:49.000000 spender-0.2/spender/data/sdss.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     3933 2023-05-17 22:05:49.000000 spender-0.2/spender/instrument.py
--rw-r--r--   0 pmelchior   (501) staff       (20)    16440 2023-05-17 22:05:49.000000 spender-0.2/spender/model.py
--rw-r--r--   0 pmelchior   (501) staff       (20)     3569 2023-05-17 22:05:49.000000 spender-0.2/spender/util.py
-drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-06-20 21:57:41.660636 spender-0.2/spender.egg-info/
--rw-r--r--   0 pmelchior   (501) staff       (20)     4947 2023-06-20 21:57:41.000000 spender-0.2/spender.egg-info/PKG-INFO
--rw-r--r--   0 pmelchior   (501) staff       (20)      332 2023-06-20 21:57:41.000000 spender-0.2/spender.egg-info/SOURCES.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)        1 2023-06-20 21:57:41.000000 spender-0.2/spender.egg-info/dependency_links.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)       68 2023-06-20 21:57:41.000000 spender-0.2/spender.egg-info/requires.txt
--rw-r--r--   0 pmelchior   (501) staff       (20)        8 2023-06-20 21:57:41.000000 spender-0.2/spender.egg-info/top_level.txt
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-07-18 02:28:43.585621 spender-0.2.1/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1082 2022-08-08 22:13:56.000000 spender-0.2.1/LICENSE
+-rw-r--r--   0 pmelchior   (501) staff       (20)     5145 2023-07-18 02:28:43.585412 spender-0.2.1/PKG-INFO
+-rw-r--r--   0 pmelchior   (501) staff       (20)     4455 2023-07-18 02:15:37.000000 spender-0.2.1/README.md
+-rw-r--r--   0 pmelchior   (501) staff       (20)       38 2023-07-18 02:28:43.585670 spender-0.2.1/setup.cfg
+-rw-r--r--   0 pmelchior   (501) staff       (20)     1051 2023-07-18 02:21:54.000000 spender-0.2.1/setup.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-07-18 02:28:43.580327 spender-0.2.1/spender/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     2995 2023-07-17 20:35:16.000000 spender-0.2.1/spender/__init__.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-07-18 02:28:43.584739 spender-0.2.1/spender/data/
+-rw-r--r--   0 pmelchior   (501) staff       (20)        0 2022-08-08 22:13:56.000000 spender-0.2.1/spender/data/__init__.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    23672 2023-07-17 17:44:22.000000 spender-0.2.1/spender/data/desi.py
+-rwxr-xr-x   0 pmelchior   (501) staff       (20)     1082 2023-05-17 22:05:49.000000 spender-0.2.1/spender/data/emission_lines.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    19391 2023-05-17 22:05:49.000000 spender-0.2.1/spender/data/sdss.py
+-rwxr-xr-x   0 pmelchior   (501) staff       (20)     7570 2023-07-17 21:35:41.000000 spender-0.2.1/spender/flow.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     3933 2023-05-17 22:05:49.000000 spender-0.2.1/spender/instrument.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)    16440 2023-07-17 20:05:39.000000 spender-0.2.1/spender/model.py
+-rw-r--r--   0 pmelchior   (501) staff       (20)     3569 2023-05-17 22:05:49.000000 spender-0.2.1/spender/util.py
+drwxr-xr-x   0 pmelchior   (501) staff       (20)        0 2023-07-18 02:28:43.581108 spender-0.2.1/spender.egg-info/
+-rw-r--r--   0 pmelchior   (501) staff       (20)     5145 2023-07-18 02:28:43.000000 spender-0.2.1/spender.egg-info/PKG-INFO
+-rw-r--r--   0 pmelchior   (501) staff       (20)      369 2023-07-18 02:28:43.000000 spender-0.2.1/spender.egg-info/SOURCES.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)        1 2023-07-18 02:28:43.000000 spender-0.2.1/spender.egg-info/dependency_links.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)       68 2023-07-18 02:28:43.000000 spender-0.2.1/spender.egg-info/requires.txt
+-rw-r--r--   0 pmelchior   (501) staff       (20)        8 2023-07-18 02:28:43.000000 spender-0.2.1/spender.egg-info/top_level.txt
```

### Comparing `spender-0.2/LICENSE` & `spender-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spender-0.2/PKG-INFO` & `spender-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spender
-Version: 0.2
+Version: 0.2.1
 Summary: Spectrum encoder and decoder
 Home-page: https://github.com/pmelchior/spender
 Author: Peter Melchior
 Author-email: peter.m.melchior@gmail.com
 License: MIT
 Keywords: spectroscopy,autoencoder
 Classifier: Development Status :: 4 - Beta
@@ -18,16 +18,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spender
 
 _Neural spectrum encoder and decoder_
 
-* Paper I: https://arxiv.org/abs/2211.07890
-* Paper II: https://arxiv.org/abs/2302.02496
+* Paper I (SDSS): https://arxiv.org/abs/2211.07890
+* Paper II (SDSS): https://arxiv.org/abs/2302.02496
+* Paper III (DESI EDR): https://arxiv.org/abs/2307.07664
 
 From a data-driven side, galaxy spectra have two fundamental degrees of freedom: their instrinsic spectral properties (or type, if you believe in such a thing) and their redshift. The latter makes them awkward to ingest because it stretches everything, which means spectral features don't appear at the same places. This is why most analyses of the intrinsic properties are done by transforming the observed spectrum to restframe.
 
 We decided to do the opposite. We build a custom architecture, which describes the restframe spectrum by an autoencoder and transforms the restframe model to the observed redshift. While we're at it we also match the spectral resolution and line spread function of the instrument:
 ![sketch](https://github.com/pmelchior/spender/assets/1463403/8e861c0b-358c-4b92-8862-e31325acae1b)
 
 Doing so clearly separates the responsibilities in the architecture. Spender establishes a restframe that has higher resolution and larger wavelength range than the spectra from which it is trained. The model can be trained from spectra at different redshifts or even from different instruments without the need to standardize the observations. Spender also has an explicit, differentiable redshift dependence, which can be coupled with a redshift estimator for a fully data-driven spectrum analysis pipeline.
@@ -57,17 +58,19 @@
 
 # if your machine does not have GPUs, specify the device
 from accelerate import Accelerator
 accelerator = Accelerator(mixed_precision='fp16')
 sdss, model = torch.hub.load(github, 'sdss_II', map_location=accelerator.device)
 ```
  
-## SDSS Outliers Catalog
+## Outliers Catalogs
 
-The [catalog of the latent-space probability](https://hub.pmelchior.net/spender.sdss.paperII.logP.txt.bz2) for the SDSS-I main galaxy sample; see Liang et al. (2023) for details
+catalog of latent-space probabilities for
+* [SDSS-I main galaxy sample](https://hub.pmelchior.net/spender.sdss.paperII.logP.txt.bz2); see Liang et al. (2023a) for details
+* [DESI EDR BGS sample](https://hub.pmelchior.net/spender.desi-edr.full-bgs-objects-logP.txt.bz2); see Liang et al. (2023b) for details
 
 ## Use
 
 Documentation and tutorials are forthcoming. In the meantime, check out `train/diagnostics.ipynb` for a worked through example that generates the figures from the paper.
 
 In short, you can run spender like this:
 ```python
```

### Comparing `spender-0.2/README.md` & `spender-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Spender
 
 _Neural spectrum encoder and decoder_
 
-* Paper I: https://arxiv.org/abs/2211.07890
-* Paper II: https://arxiv.org/abs/2302.02496
+* Paper I (SDSS): https://arxiv.org/abs/2211.07890
+* Paper II (SDSS): https://arxiv.org/abs/2302.02496
+* Paper III (DESI EDR): https://arxiv.org/abs/2307.07664
 
 From a data-driven side, galaxy spectra have two fundamental degrees of freedom: their instrinsic spectral properties (or type, if you believe in such a thing) and their redshift. The latter makes them awkward to ingest because it stretches everything, which means spectral features don't appear at the same places. This is why most analyses of the intrinsic properties are done by transforming the observed spectrum to restframe.
 
 We decided to do the opposite. We build a custom architecture, which describes the restframe spectrum by an autoencoder and transforms the restframe model to the observed redshift. While we're at it we also match the spectral resolution and line spread function of the instrument:
 ![sketch](https://github.com/pmelchior/spender/assets/1463403/8e861c0b-358c-4b92-8862-e31325acae1b)
 
 Doing so clearly separates the responsibilities in the architecture. Spender establishes a restframe that has higher resolution and larger wavelength range than the spectra from which it is trained. The model can be trained from spectra at different redshifts or even from different instruments without the need to standardize the observations. Spender also has an explicit, differentiable redshift dependence, which can be coupled with a redshift estimator for a fully data-driven spectrum analysis pipeline.
@@ -37,17 +38,19 @@
 
 # if your machine does not have GPUs, specify the device
 from accelerate import Accelerator
 accelerator = Accelerator(mixed_precision='fp16')
 sdss, model = torch.hub.load(github, 'sdss_II', map_location=accelerator.device)
 ```
  
-## SDSS Outliers Catalog
+## Outliers Catalogs
 
-The [catalog of the latent-space probability](https://hub.pmelchior.net/spender.sdss.paperII.logP.txt.bz2) for the SDSS-I main galaxy sample; see Liang et al. (2023) for details
+catalog of latent-space probabilities for
+* [SDSS-I main galaxy sample](https://hub.pmelchior.net/spender.sdss.paperII.logP.txt.bz2); see Liang et al. (2023a) for details
+* [DESI EDR BGS sample](https://hub.pmelchior.net/spender.desi-edr.full-bgs-objects-logP.txt.bz2); see Liang et al. (2023b) for details
 
 ## Use
 
 Documentation and tutorials are forthcoming. In the meantime, check out `train/diagnostics.ipynb` for a worked through example that generates the figures from the paper.
 
 In short, you can run spender like this:
 ```python
```

### Comparing `spender-0.2/setup.py` & `spender-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 long_description = open('README.md').read()
 
 setup(
     name="spender",
     description="Spectrum encoder and decoder",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="0.2",
+    version="0.2.1",
     license="MIT",
     author="Peter Melchior",
     author_email="peter.m.melchior@gmail.com",
     url="https://github.com/pmelchior/spender",
     packages=["spender", "spender.data"],
     package_data={"skymapper.data": ['*.txt']},
     classifiers=[
```

### Comparing `spender-0.2/spender/__init__.py` & `spender-0.2.1/spender/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,21 @@
     # load model_struct from hub if url is given
     if filename[:4].lower() == "http":
         kwargs.pop("check_hash", True) # remove check_hash
         model_struct = torch.hub.load_state_dict_from_url(filename, check_hash=True, **kwargs)
     else:
         model_struct = torch.load(filename, **kwargs)
 
+    # check if model_struct['model'] is a single model or list
+    try:
+        model_struct["model"]["decoder.wave_rest"]
+    except TypeError:
+        model_struct["model"] = model_struct["model"][0]
+
+
     # check if LSF is contained in model_struct
     try:
         kernel = model_struct["model"]["encoder.instrument.lsf.weight"].flatten()
         lsf = LSF(kernel)
         instrument.lsf = lsf
     except KeyError:
         pass
```

### Comparing `spender-0.2/spender/data/emission_lines.py` & `spender-0.2.1/spender/data/emission_lines.py`

 * *Files identical despite different names*

### Comparing `spender-0.2/spender/data/sdss.py` & `spender-0.2.1/spender/data/sdss.py`

 * *Files identical despite different names*

### Comparing `spender-0.2/spender/instrument.py` & `spender-0.2.1/spender/instrument.py`

 * *Files identical despite different names*

### Comparing `spender-0.2/spender/model.py` & `spender-0.2.1/spender/model.py`

 * *Files identical despite different names*

### Comparing `spender-0.2/spender/util.py` & `spender-0.2.1/spender/util.py`

 * *Files identical despite different names*

### Comparing `spender-0.2/spender.egg-info/PKG-INFO` & `spender-0.2.1/spender.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spender
-Version: 0.2
+Version: 0.2.1
 Summary: Spectrum encoder and decoder
 Home-page: https://github.com/pmelchior/spender
 Author: Peter Melchior
 Author-email: peter.m.melchior@gmail.com
 License: MIT
 Keywords: spectroscopy,autoencoder
 Classifier: Development Status :: 4 - Beta
@@ -18,16 +18,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spender
 
 _Neural spectrum encoder and decoder_
 
-* Paper I: https://arxiv.org/abs/2211.07890
-* Paper II: https://arxiv.org/abs/2302.02496
+* Paper I (SDSS): https://arxiv.org/abs/2211.07890
+* Paper II (SDSS): https://arxiv.org/abs/2302.02496
+* Paper III (DESI EDR): https://arxiv.org/abs/2307.07664
 
 From a data-driven side, galaxy spectra have two fundamental degrees of freedom: their instrinsic spectral properties (or type, if you believe in such a thing) and their redshift. The latter makes them awkward to ingest because it stretches everything, which means spectral features don't appear at the same places. This is why most analyses of the intrinsic properties are done by transforming the observed spectrum to restframe.
 
 We decided to do the opposite. We build a custom architecture, which describes the restframe spectrum by an autoencoder and transforms the restframe model to the observed redshift. While we're at it we also match the spectral resolution and line spread function of the instrument:
 ![sketch](https://github.com/pmelchior/spender/assets/1463403/8e861c0b-358c-4b92-8862-e31325acae1b)
 
 Doing so clearly separates the responsibilities in the architecture. Spender establishes a restframe that has higher resolution and larger wavelength range than the spectra from which it is trained. The model can be trained from spectra at different redshifts or even from different instruments without the need to standardize the observations. Spender also has an explicit, differentiable redshift dependence, which can be coupled with a redshift estimator for a fully data-driven spectrum analysis pipeline.
@@ -57,17 +58,19 @@
 
 # if your machine does not have GPUs, specify the device
 from accelerate import Accelerator
 accelerator = Accelerator(mixed_precision='fp16')
 sdss, model = torch.hub.load(github, 'sdss_II', map_location=accelerator.device)
 ```
  
-## SDSS Outliers Catalog
+## Outliers Catalogs
 
-The [catalog of the latent-space probability](https://hub.pmelchior.net/spender.sdss.paperII.logP.txt.bz2) for the SDSS-I main galaxy sample; see Liang et al. (2023) for details
+catalog of latent-space probabilities for
+* [SDSS-I main galaxy sample](https://hub.pmelchior.net/spender.sdss.paperII.logP.txt.bz2); see Liang et al. (2023a) for details
+* [DESI EDR BGS sample](https://hub.pmelchior.net/spender.desi-edr.full-bgs-objects-logP.txt.bz2); see Liang et al. (2023b) for details
 
 ## Use
 
 Documentation and tutorials are forthcoming. In the meantime, check out `train/diagnostics.ipynb` for a worked through example that generates the figures from the paper.
 
 In short, you can run spender like this:
 ```python
```

