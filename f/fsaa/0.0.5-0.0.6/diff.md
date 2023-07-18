# Comparing `tmp/fsaa-0.0.5.tar.gz` & `tmp/fsaa-0.0.6.tar.gz`

## Comparing `fsaa-0.0.5.tar` & `fsaa-0.0.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fsaa-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fsaa-0.0.5/CITATION.cff
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 fsaa-0.0.5/CODEOWNERS
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.5/CONTRIBUTING.md
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.5/environment.yml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fsaa-0.0.5/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fsaa-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.5/.vscode/launch.json
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.5/.vscode/settings.json
--rw-r--r--   0        0        0    22260 2020-02-02 00:00:00.000000 fsaa-0.0.5/assets/logo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/__init__.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/attack.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/core.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/utils.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/examples/tutorial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/initializers/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/initializers/random.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/initializers/random_sign.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/losses/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/losses/cossim_loss.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/losses/lpips_loss.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/losses/mse_loss.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/masks/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/masks/custom.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/masks/jnd.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/masks/nomask.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/models/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/models/dinov2/dinov2.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/models/hf_models/hf_models.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/models/ibot/ibot.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/models/ibot/utils.py
--rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/models/ibot/vits.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/transforms/__init__.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/transforms/compose.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/transforms/normalize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/updaters/__init__.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/updaters/fgsm.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/updaters/langevin.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/updaters/pgd.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fsaa-0.0.5/fsaa/updaters/random.py
--rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.5/imgs/adv.png
--rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.5/imgs/mask.png
--rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.5/imgs/orig.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/test_attack.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/test_initializers.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/test_masks.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/test_models.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/test_transforms.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fsaa-0.0.5/tests/test_updaters.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 fsaa-0.0.5/.gitignore
--rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.5/LICENSE
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fsaa-0.0.5/README.md
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 fsaa-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 fsaa-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 fsaa-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fsaa-0.0.6/CITATION.cff
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 fsaa-0.0.6/CODEOWNERS
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fsaa-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 fsaa-0.0.6/environment.yml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fsaa-0.0.6/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 fsaa-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fsaa-0.0.6/.vscode/launch.json
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fsaa-0.0.6/.vscode/settings.json
+-rw-r--r--   0        0        0    22260 2020-02-02 00:00:00.000000 fsaa-0.0.6/assets/logo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/__init__.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/attack.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/core.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/utils.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/examples/tutorial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/initializers/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/initializers/random.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/initializers/random_sign.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/losses/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/losses/cossim_loss.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/losses/lpips_loss.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/losses/mse_loss.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/masks/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/masks/custom.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/masks/jnd.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/masks/nomask.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/models/__init__.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/models/hf_models/hf_models.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/models/hub_models/hub_models.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/models/ibot/ibot.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/models/ibot/utils.py
+-rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/models/ibot/vits.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/transforms/__init__.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/transforms/compose.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/transforms/normalize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/updaters/__init__.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/updaters/fgsm.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/updaters/langevin.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/updaters/pgd.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fsaa-0.0.6/fsaa/updaters/random.py
+-rw-r--r--   0        0        0   730255 2020-02-02 00:00:00.000000 fsaa-0.0.6/imgs/adv.png
+-rw-r--r--   0        0        0   450674 2020-02-02 00:00:00.000000 fsaa-0.0.6/imgs/mask.png
+-rw-r--r--   0        0        0   694498 2020-02-02 00:00:00.000000 fsaa-0.0.6/imgs/orig.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/test_attack.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/test_initializers.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/test_masks.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/test_models.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/test_transforms.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fsaa-0.0.6/tests/test_updaters.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 fsaa-0.0.6/.gitignore
+-rw-r--r--   0        0        0    19333 2020-02-02 00:00:00.000000 fsaa-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fsaa-0.0.6/README.md
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 fsaa-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4464 2020-02-02 00:00:00.000000 fsaa-0.0.6/PKG-INFO
```

### Comparing `fsaa-0.0.5/.pre-commit-config.yaml` & `fsaa-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/environment.yml` & `fsaa-0.0.6/environment.yml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/.github/workflows/python-publish.yml` & `fsaa-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/.vscode/launch.json` & `fsaa-0.0.6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/assets/logo.png` & `fsaa-0.0.6/assets/logo.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/fsaa/attack.py` & `fsaa-0.0.6/fsaa/attack.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/fsaa/core.py` & `fsaa-0.0.6/fsaa/core.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/fsaa/utils.py` & `fsaa-0.0.6/fsaa/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from fsaa.initializers.random_sign import RandomSignInitializer
 from fsaa.losses.cossim_loss import CosSimLoss
 from fsaa.losses.lpips_loss import LPIPSAlexLoss, LPIPSVGGLoss
 from fsaa.losses.mse_loss import MeanSquaredErrorLoss
 from fsaa.masks.custom import CustomMask
 from fsaa.masks.jnd import JNDMask
 from fsaa.masks.nomask import NoMask
-from fsaa.models.dinov2.dinov2 import SUPPORTED_DINOV2_MODELS, DinoV2Model
 from fsaa.models.hf_models.hf_models import SUPPORTED_HF_MODELS, HFModel
+from fsaa.models.hub_models.hub_models import SUPPORTED_HUB_MODELS, HubModel
 from fsaa.models.ibot.ibot import SUPPORTED_IBOT_MODELS, iBOTModel
 from fsaa.updaters.fgsm import FGSMUpdater
 from fsaa.updaters.langevin import LangevinUpdater
 from fsaa.updaters.pgd import PGDUpdater
 from fsaa.updaters.random import RandomUpdater
 
 INITIALIZERS = {
@@ -39,16 +39,19 @@
 
 MASKS = {
     "JND": JNDMask,
     "Custom": CustomMask,
     "NoMask": NoMask
 }
 
-SUPPORTED_MODELS = SUPPORTED_DINOV2_MODELS + \
-    SUPPORTED_HF_MODELS + SUPPORTED_IBOT_MODELS
+SUPPORTED_MODELS = (
+    SUPPORTED_HUB_MODELS +
+    SUPPORTED_HF_MODELS +
+    SUPPORTED_IBOT_MODELS
+)
 
 
 def get_initializer(name: str, lr: float, **kwargs) -> PerturbationInitializer:
     """Returns the initializer used for the attack."""
     return INITIALIZERS[name](lr, **kwargs)
 
 
@@ -71,15 +74,15 @@
     """Returns the model used for the attack."""
     if model_name not in SUPPORTED_MODELS:
         raise ValueError(
             f"Model '{model_name}' is not supported. \
                 Pick one of {SUPPORTED_MODELS}"
         )
 
-    if model_name in SUPPORTED_DINOV2_MODELS:
-        return DinoV2Model(model_name)
+    if model_name in SUPPORTED_HUB_MODELS:
+        return HubModel(model_name)
 
     if model_name in SUPPORTED_HF_MODELS:
         return HFModel(model_name)
 
     if model_name in SUPPORTED_IBOT_MODELS:
         return iBOTModel(model_name)
```

### Comparing `fsaa-0.0.5/fsaa/examples/tutorial.py` & `fsaa-0.0.6/fsaa/examples/tutorial.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/fsaa/losses/lpips_loss.py` & `fsaa-0.0.6/fsaa/losses/lpips_loss.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/fsaa/masks/jnd.py` & `fsaa-0.0.6/fsaa/masks/jnd.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/fsaa/models/hf_models/hf_models.py` & `fsaa-0.0.6/fsaa/models/hf_models/hf_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "facebook/deit-small-patch16-224",
     "facebook/deit-tiny-distilled-patch16-224",
     "facebook/deit-tiny-patch16-224",
 ]
 
 SUPPORTED_DINO_MODELS = [
     "facebook/dino-vits8",
-    "facebook/dino-vitb16",
+    "facebook/dino-vits16",
     "facebook/dino-vitb8",
     "facebook/dino-vitb16",
 ]
 
 SUPPORTED_MAE_MODELS = [
     "facebook/vit-mae-base",
     "facebook/vit-mae-large",
```

### Comparing `fsaa-0.0.5/fsaa/models/ibot/ibot.py` & `fsaa-0.0.6/fsaa/models/ibot/ibot.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/fsaa/models/ibot/utils.py` & `fsaa-0.0.6/fsaa/models/ibot/utils.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/fsaa/models/ibot/vits.py` & `fsaa-0.0.6/fsaa/models/ibot/vits.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/fsaa/transforms/normalize.py` & `fsaa-0.0.6/fsaa/transforms/normalize.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/fsaa/updaters/langevin.py` & `fsaa-0.0.6/fsaa/updaters/langevin.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/fsaa/updaters/pgd.py` & `fsaa-0.0.6/fsaa/updaters/pgd.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/fsaa/updaters/random.py` & `fsaa-0.0.6/fsaa/updaters/random.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/imgs/adv.png` & `fsaa-0.0.6/imgs/adv.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/imgs/mask.png` & `fsaa-0.0.6/imgs/mask.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/imgs/orig.png` & `fsaa-0.0.6/imgs/orig.png`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/tests/test_attack.py` & `fsaa-0.0.6/tests/test_attack.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/tests/test_initializers.py` & `fsaa-0.0.6/tests/test_initializers.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/tests/test_masks.py` & `fsaa-0.0.6/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/tests/test_models.py` & `fsaa-0.0.6/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/tests/test_updaters.py` & `fsaa-0.0.6/tests/test_updaters.py`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/.gitignore` & `fsaa-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/LICENSE` & `fsaa-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/README.md` & `fsaa-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fsaa-0.0.5/pyproject.toml` & `fsaa-0.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 # Project metadata
 [project]
 name = "fsaa"
-version = "0.0.5"
+version = "0.0.6"
 authors = [{ name="Brian Pulfer", email="brianpulfer95@gmail.com" }]
 description = "A simple library for adversarial attacks in feature space."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: Other/Proprietary License",
```

### Comparing `fsaa-0.0.5/PKG-INFO` & `fsaa-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsaa
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple library for adversarial attacks in feature space.
 Project-URL: Homepage, https://github.com/BrianPulfer/fsaa
 Project-URL: Bug Tracker, https://github.com/BrianPulfer/fsaa/issues
 Author-email: Brian Pulfer <brianpulfer95@gmail.com>
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

