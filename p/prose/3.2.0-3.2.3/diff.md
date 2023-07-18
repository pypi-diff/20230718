# Comparing `tmp/prose-3.2.0.tar.gz` & `tmp/prose-3.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prose-3.2.0.tar", max compression
+gzip compressed data, was "prose-3.2.3.tar", max compression
```

## Comparing `prose-3.2.0.tar` & `prose-3.2.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1097 2023-06-15 15:57:18.286445 prose-3.2.0/LICENSE
--rw-r--r--   0        0        0     3752 2023-06-15 15:57:18.286445 prose-3.2.0/README.md
--rw-r--r--   0        0        0      652 2023-06-15 15:57:18.378447 prose-3.2.0/prose/__init__.py
--rw-r--r--   0        0        0       84 2023-06-15 15:57:18.378447 prose-3.2.0/prose/archive/__init__.py
--rw-r--r--   0        0        0     2397 2023-06-15 15:57:18.378447 prose-3.2.0/prose/archive/pos1.py
--rw-r--r--   0        0        0     2071 2023-06-15 15:57:18.378447 prose-3.2.0/prose/archive/sdss.py
--rw-r--r--   0        0        0      254 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/__init__.py
--rw-r--r--   0        0        0     4760 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/alignment.py
--rw-r--r--   0        0        0     3680 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/background.py
--rw-r--r--   0        0        0    10501 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/catalogs.py
--rw-r--r--   0        0        0     8768 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/centroids.py
--rw-r--r--   0        0        0    13480 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/detection.py
--rw-r--r--   0        0        0    10037 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/geometry.py
--rw-r--r--   0        0        0     4135 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/photometry.py
--rw-r--r--   0        0        0    13998 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/psf.py
--rw-r--r--   0        0        0     3703 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/shepard.py
--rw-r--r--   0        0        0    20516 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/utils.py
--rw-r--r--   0        0        0     4034 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/visualization.py
--rw-r--r--   0        0        0     4069 2023-06-15 15:57:18.378447 prose-3.2.0/prose/builtins.py
--rw-r--r--   0        0        0    10673 2023-06-15 15:57:18.378447 prose-3.2.0/prose/citations.py
--rw-r--r--   0        0        0     5933 2023-06-15 15:57:18.378447 prose-3.2.0/prose/config.py
--rw-r--r--   0        0        0     3733 2023-06-15 15:57:18.378447 prose-3.2.0/prose/console_utils.py
--rw-r--r--   0        0        0      120 2023-06-15 15:57:18.382447 prose-3.2.0/prose/core/__init__.py
--rw-r--r--   0        0        0     3651 2023-06-15 15:57:18.382447 prose-3.2.0/prose/core/block.py
--rw-r--r--   0        0        0    24834 2023-06-15 15:57:18.382447 prose-3.2.0/prose/core/image.py
--rw-r--r--   0        0        0     9842 2023-06-15 15:57:18.382447 prose-3.2.0/prose/core/sequence.py
--rw-r--r--   0        0        0    16797 2023-06-15 15:57:18.382447 prose-3.2.0/prose/core/source.py
--rw-r--r--   0        0        0    17451 2023-06-15 15:57:18.382447 prose-3.2.0/prose/fluxes.py
--rw-r--r--   0        0        0      137 2023-06-15 15:57:18.382447 prose-3.2.0/prose/io/__init__.py
--rw-r--r--   0        0        0      686 2023-06-15 15:57:18.382447 prose-3.2.0/prose/io/create_fm_db.sql
--rw-r--r--   0        0        0    25095 2023-06-15 15:57:18.382447 prose-3.2.0/prose/io/fitsmanager.py
--rw-r--r--   0        0        0     6374 2023-06-15 15:57:18.382447 prose-3.2.0/prose/io/io.py
--rw-r--r--   0        0        0    15043 2023-06-15 15:57:18.382447 prose-3.2.0/prose/simulations.py
--rw-r--r--   0        0        0     7901 2023-06-15 15:57:18.382447 prose-3.2.0/prose/telescope.py
--rw-r--r--   0        0        0    14009 2023-06-15 15:57:18.382447 prose-3.2.0/prose/utils.py
--rw-r--r--   0        0        0    29851 2023-06-15 15:57:18.382447 prose-3.2.0/prose/visualization.py
--rw-r--r--   0        0        0     1030 2023-06-15 15:57:18.382447 prose-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     4840 1970-01-01 00:00:00.000000 prose-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-07-18 11:24:22.371726 prose-3.2.3/LICENSE
+-rw-r--r--   0        0        0     3752 2023-07-18 11:24:22.371726 prose-3.2.3/README.md
+-rw-r--r--   0        0        0      652 2023-07-18 11:24:22.471727 prose-3.2.3/prose/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-18 11:24:22.471727 prose-3.2.3/prose/archive/__init__.py
+-rw-r--r--   0        0        0     2397 2023-07-18 11:24:22.471727 prose-3.2.3/prose/archive/pos1.py
+-rw-r--r--   0        0        0     2071 2023-07-18 11:24:22.471727 prose-3.2.3/prose/archive/sdss.py
+-rw-r--r--   0        0        0      254 2023-07-18 11:24:22.471727 prose-3.2.3/prose/blocks/__init__.py
+-rw-r--r--   0        0        0     4837 2023-07-18 11:24:22.471727 prose-3.2.3/prose/blocks/alignment.py
+-rw-r--r--   0        0        0     3695 2023-07-18 11:24:22.471727 prose-3.2.3/prose/blocks/background.py
+-rw-r--r--   0        0        0    11056 2023-07-18 11:24:22.471727 prose-3.2.3/prose/blocks/catalogs.py
+-rw-r--r--   0        0        0     8794 2023-07-18 11:24:22.471727 prose-3.2.3/prose/blocks/centroids.py
+-rw-r--r--   0        0        0    13530 2023-07-18 11:24:22.471727 prose-3.2.3/prose/blocks/detection.py
+-rw-r--r--   0        0        0    10421 2023-07-18 11:24:22.471727 prose-3.2.3/prose/blocks/geometry.py
+-rw-r--r--   0        0        0     4187 2023-07-18 11:24:22.471727 prose-3.2.3/prose/blocks/photometry.py
+-rw-r--r--   0        0        0    14031 2023-07-18 11:24:22.471727 prose-3.2.3/prose/blocks/psf.py
+-rw-r--r--   0        0        0     3703 2023-07-18 11:24:22.471727 prose-3.2.3/prose/blocks/shepard.py
+-rw-r--r--   0        0        0    20552 2023-07-18 11:24:22.471727 prose-3.2.3/prose/blocks/utils.py
+-rw-r--r--   0        0        0     4034 2023-07-18 11:24:22.471727 prose-3.2.3/prose/blocks/visualization.py
+-rw-r--r--   0        0        0     4069 2023-07-18 11:24:22.471727 prose-3.2.3/prose/builtins.py
+-rw-r--r--   0        0        0    10673 2023-07-18 11:24:22.471727 prose-3.2.3/prose/citations.py
+-rw-r--r--   0        0        0     5933 2023-07-18 11:24:22.471727 prose-3.2.3/prose/config.py
+-rw-r--r--   0        0        0     3733 2023-07-18 11:24:22.471727 prose-3.2.3/prose/console_utils.py
+-rw-r--r--   0        0        0      120 2023-07-18 11:24:22.471727 prose-3.2.3/prose/core/__init__.py
+-rw-r--r--   0        0        0     4416 2023-07-18 11:24:22.471727 prose-3.2.3/prose/core/block.py
+-rw-r--r--   0        0        0    24919 2023-07-18 11:24:22.471727 prose-3.2.3/prose/core/image.py
+-rw-r--r--   0        0        0     9842 2023-07-18 11:24:22.471727 prose-3.2.3/prose/core/sequence.py
+-rw-r--r--   0        0        0    16797 2023-07-18 11:24:22.471727 prose-3.2.3/prose/core/source.py
+-rw-r--r--   0        0        0    17556 2023-07-18 11:24:22.471727 prose-3.2.3/prose/fluxes.py
+-rw-r--r--   0        0        0      137 2023-07-18 11:24:22.471727 prose-3.2.3/prose/io/__init__.py
+-rw-r--r--   0        0        0      686 2023-07-18 11:24:22.471727 prose-3.2.3/prose/io/create_fm_db.sql
+-rw-r--r--   0        0        0    25095 2023-07-18 11:24:22.471727 prose-3.2.3/prose/io/fitsmanager.py
+-rw-r--r--   0        0        0     6374 2023-07-18 11:24:22.471727 prose-3.2.3/prose/io/io.py
+-rw-r--r--   0        0        0    15043 2023-07-18 11:24:22.471727 prose-3.2.3/prose/simulations.py
+-rw-r--r--   0        0        0     7901 2023-07-18 11:24:22.471727 prose-3.2.3/prose/telescope.py
+-rw-r--r--   0        0        0    14691 2023-07-18 11:24:22.471727 prose-3.2.3/prose/utils.py
+-rw-r--r--   0        0        0    29851 2023-07-18 11:24:22.471727 prose-3.2.3/prose/visualization.py
+-rw-r--r--   0        0        0     1030 2023-07-18 11:24:22.471727 prose-3.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4840 1970-01-01 00:00:00.000000 prose-3.2.3/PKG-INFO
```

### Comparing `prose-3.2.0/LICENSE` & `prose-3.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/README.md` & `prose-3.2.3/README.md`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/__init__.py` & `prose-3.2.3/prose/__init__.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/archive/pos1.py` & `prose-3.2.3/prose/archive/pos1.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/archive/sdss.py` & `prose-3.2.3/prose/archive/sdss.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/blocks/alignment.py` & `prose-3.2.3/prose/blocks/alignment.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,22 @@
         Parameters
         ----------
         inverse: bool, optional
             whether to apply the inverse of the image transform by default False
         name : str, optional
             name of the block, by default None
         """
-        super().__init__(name)
+        super().__init__(name, read=["transform"])
         self.inverse = inverse
 
     def run(self, image: Image):
         try:
             image.data = warp(
                 image.data,
-                image.transform if self.inverse else image.transform,
+                image.transform.inverse if self.inverse else image.transform,
                 cval=np.nanmedian(image.data),
                 output_shape=image.shape,
             )
         except np.linalg.LinAlgError:
             image.discard = True
 
     @property
@@ -69,15 +69,15 @@
         verbose : bool, optional
             _description_, by default False
         discard_tolerance: float, optional
             fraction of sources that needs to be matched before discarding image
         match_tolerance: float, optional
             maximum distance between matched sources in pixels, default 5
         """
-        super().__init__(name, verbose)
+        super().__init__(name, verbose, read=["transform", "sources"])
         self.reference_sources = reference.sources
         self._parallel_friendly = True
         self.discard_tolerance = discard_tolerance
         self.match_tolerance = match_tolerance
         self._transform_block = ComputeTransformTwirl(reference)
 
     def run(self, image: Image):
@@ -127,15 +127,15 @@
         Parameters
         ----------
         reference : Image
             reference image containing a valid WCS
         n : int, optional
             number of stars used to match WCS, by default 6
         """
-        super().__init__(name, verbose)
+        super().__init__(name, verbose, read=["sources"])
         self.reference = reference
         assert reference.plate_solved, "reference must have valid WCS"
         self.n = n
 
     def run(self, image: Image):
         ref_skycoords = self.reference.wcs.pixel_to_world(
             *self.reference.sources.coords[0 : self.n].T
```

### Comparing `prose-3.2.0/prose/blocks/background.py` & `prose-3.2.3/prose/blocks/background.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         subtract : bool, optional
             Whether to subtract the estimated background from the image. Default is True.
         box_size : tuple of int, optional
             The size of the box used to compute the background. Default is (50, 50).
         filter_size : tuple of int, optional
             The size of the filter used to smooth the background. Default is (3, 3).
         """
-        super().__init__(name=name)
+        super().__init__(name=name, read=["data"])
         self.sigma_clip = SigmaClip(sigma=3.0)
         self.bkg_estimator = MedianBackground()
         self.subtract = subtract
         self.box_size = box_size
         self.filter_size = filter_size
 
     def run(self, image):
```

### Comparing `prose-3.2.0/prose/blocks/catalogs.py` & `prose-3.2.3/prose/blocks/catalogs.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,24 +46,29 @@
         table["ra"] = skycoord.ra
         table["dec"] = skycoord.dec
 
     return table
 
 
 class _CatalogBlock(Block):
-    def __init__(self, name, mode=None, limit=10000, **kwargs):
+    def __init__(self, name, mode: str = None, limit=10000, **kwargs):
         super().__init__(**kwargs)
         self.mode = mode
         self.catalog_name = name
         self.limit = limit
 
+        if self.mode == "replace":
+            self.require = ["sources"]
+
     def get_catalog(self, image):
         raise NotImplementedError()
 
     def run(self, image):
+        if not image.plate_solved:
+            raise ValueError("Image is not plate solved.")
         catalog = self.get_catalog(image)
         radecs = np.array(
             [catalog["ra"].quantity.to(u.deg), catalog["dec"].quantity.to(u.deg)]
         )
         stars_coords = np.array(SkyCoord(*radecs, unit="deg").to_pixel(image.wcs))
         catalog["x"], catalog["y"] = stars_coords
         catalog = catalog.to_pandas()
@@ -115,14 +120,18 @@
         image.catalogs[self.catalog_name] = catalog.iloc[0 : self.limit]
 
 
 class PlateSolve(Block):
     """
     A block that performs plate solving on an astronomical image using a Gaia catalog.
 
+    |read| :code:`Image.sources`, :code:`Image.pixel_scale`
+
+    |write| :code:`Image.wcs`
+
     Parameters
     ----------
     reference : `None` or `~prose.Image`
         A reference image containing a Gaia catalog to use for plate solving.
         If `None`, a new catalog will be queried using `image_gaia_query`.
         Default is `None`.
     n : int
@@ -174,15 +183,15 @@
         self.tolerance = tolerance
         self.quads_tolerance = quads_tolerance
         self.debug = debug
         self.field = field
         self.min_match = min_match
 
     def run(self, image):
-        radius = image.fov.max() / 12 if self.radius is None else self.radius
+        radius = image.fov.min() / 12 if self.radius is None else self.radius
         stars = image.sources.coords * image.pixel_scale.to("arcmin").value
         stars = (
             sparsify(stars, radius.to("arcmin").value)
             / image.pixel_scale.to("arcmin").value
         )
 
         if self.reference is None:
@@ -190,62 +199,72 @@
                 image, wcs=False, circular=True, fov=image.fov.max() * self.field
             ).to_pandas()
             gaias = np.array([table.ra, table.dec]).T
             gaias = gaias[~np.any(np.isnan(gaias), 1)]
         else:
             gaias = self.reference.catalogs["gaia"][["ra", "dec"]].values
 
-        gaias = sparsify(gaias, radius.to("deg").value)
+        sparse_gaias = sparsify(gaias, radius.to("deg").value)
 
         new_wcs = twirl.compute_wcs(
             stars,
-            gaias[0 : self.n],
+            sparse_gaias[0 : self.n],
             tolerance=self.tolerance,
             quads_tolerance=self.quads_tolerance,
             min_match=self.min_match,
         )
         image.wcs = new_wcs
-        coords = np.array(image.wcs.world_to_pixel(SkyCoord(gaias, unit="deg"))).T
+        coords = np.array(
+            image.wcs.world_to_pixel(SkyCoord(sparse_gaias, unit="deg"))
+        ).T
         idxs = cross_match(image.sources.coords, coords, return_idxs=True)
         image.computed["plat_solve_success"] = np.count_nonzero(
             ~np.isnan(idxs[:, 1])
-        ) / len(gaias)
+        ) / len(sparse_gaias)
 
         if self.debug:
             image.show()
-            coords = np.array(image.wcs.world_to_pixel(SkyCoord(gaias, unit="deg"))).T
-            _gaias = Sources([PointSource(coords=c) for c in coords])
-            _gaias.plot(c="y")
+            coords = np.array(
+                image.wcs.world_to_pixel(SkyCoord(sparse_gaias, unit="deg"))
+            ).T
+            Sources(coords[: self.n]).plot(c="y", label=False)
+            Sources(coords[self.n :]).plot(c="y", alpha=0.5, label=False)
 
     @property
     def citations(self):
         return super().citations + ["twirl"]
 
 
 class GaiaCatalog(_CatalogBlock):
-    def __init__(self, correct_pm=True, limit=10000, mode=None):
+    def __init__(
+        self,
+        correct_pm=True,
+        limit=10000,
+        mode: str = None,
+    ):
         """Query gaia catalog
 
         Catalog is written in Image.catalogs as a pandas DataFrame. If mode is ""crossmatch" the index of catalog sources in the DataFrame matches with the index of sources in Image.sources
 
-        |read| :code:`Image.sources` if mode is "crossmatch"
+        |read| :code:`Image.sources` if mode is "crossmatch" and valid :code:`Image.wcs`
 
         |write| :code:`Image.catalogs`
 
         - :code:`Image.sources` if mode is "crossmatch"
         - :code:`Image.catalogs`
 
         Parameters
         ----------
         correct_pm : bool, optional
             whether to correct proper motion, by default True
         limit : int, optional
             limit number of stars queried, by default 10000
-        mode: str, optional
-            "crossmatch" to match existing Image.sources or "replace" to use queried stars as Image.sources
+        mode: ["replace", "crossmatch", None], optional
+            "crossmatch" to match existing Image.sources or "replace" to use queried
+            stars as Image.sources. Default is None and only write to Image.catalogs
         """
         _CatalogBlock.__init__(self, "gaia", limit=limit, mode=mode)
         self.correct_pm = correct_pm
 
     def get_catalog(self, image):
         max_fov = image.fov.max() * np.sqrt(2)
         table = image_gaia_query(
```

### Comparing `prose-3.2.0/prose/blocks/centroids.py` & `prose-3.2.3/prose/blocks/centroids.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         centroid_func : function
             photutils.centroids function
         limit : int, optional
             maximum deviation from initial coordinate, by default `cutout/2`
         cutout : int, optional
             size of the cutout to be used for centroiding, by default 21
         """
-        super().__init__(name=name)
+        super().__init__(name=name, read=["sources", "data"])
         self.cutout = cutout
         self.centroid_func = centroid_func
         if limit is None:
             limit = cutout / 2
         self.limit = limit
 
     def run(self, image):
```

### Comparing `prose-3.2.0/prose/blocks/detection.py` & `prose-3.2.3/prose/blocks/detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         min_separation: float = None,
         min_area: float = 0,
         minor_length: float = 0,
         name: str = None,
     ):
         """Base class for sources detection.
 
+        |read| :code:`Image.data`
+
         Parameters
         ----------
         threshold : float, optional
             detection threshold for sources, by default 4
         n : int, optional
             number of sources to detect, by default None
         sort : bool, optional
@@ -37,15 +39,15 @@
         min_area : float, optional
             minimum area in pixels of the sources to detect, by default 0
         minor_length : float, optional
             minimum length of semi-major axis of sources to detect, by default 0
         name : str, optional
             name of the block, by default None
         """
-        super().__init__(name=name)
+        super().__init__(name=name, read=["data"])
         self.n = n
         self.sort = sort
         self.min_separation = min_separation
         self.threshold = threshold
         self.min_area = min_area
         self.minor_length = minor_length
```

### Comparing `prose-3.2.0/prose/blocks/geometry.py` & `prose-3.2.3/prose/blocks/geometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from scipy.spatial import cKDTree
 from skimage.transform import AffineTransform
 from twirl import find_transform, quads
 from twirl.geometry import get_transform_matrix, pad
 from twirl.match import count_cross_match
 
 from prose.core import Block, Image
+from prose.utils import cross_match
 
 __all__ = [
     "Trim",
     "Cutouts",
     "Drizzle",
     "ComputeTransformXYShift",
     "ComputeTransformTwirl",
@@ -84,15 +85,15 @@
         wcs : bool, optional
             whether to compute cutouts WCS, by default False
         name : str, optional
             name of the blocks, by default None
         sources: bool, optional
             whether to keep sources in cutouts, by default False
         """
-        super().__init__(name=name)
+        super().__init__(name=name, read=["sources"])
         if isinstance(shape, int):
             shape = (shape, shape)
         self.shape = shape
         self.wcs = wcs
         self.sources = sources
         self._parallel_friendly = True
 
@@ -212,15 +213,24 @@
 
             if min_match is not None:
                 if isinstance(min_match, float):
                     if match >= min_match * len(coords):
                         break
 
         i, j = pairs[np.argmax(matches)]
-        return get_transform_matrix(self.asterisms_ref[j], asterisms_image[i])
+
+        if True:
+            M = get_transform_matrix(self.asterisms_ref[j], asterisms_image[i])
+            test = (M @ pad(self.ref).T)[0:2].T
+            s1, s2 = cross_match(coords, test, tolerance=tolerance, return_idxs=True).T
+            M = get_transform_matrix(self.ref[s2], coords[s1])
+        else:
+            M = get_transform_matrix(self.asterisms_ref[j], asterisms_image[i])
+
+        return M
 
 
 # backward compatibility
 ComputeTransform = ComputeTransformTwirl
 
 
 class ComputeTransformXYShift(Block):
```

### Comparing `prose-3.2.0/prose/blocks/photometry.py` & `prose-3.2.3/prose/blocks/photometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         radii : np.ndarray, optional
             apertures radii (definition varies depending on sources), by default None
         scale : bool, optional
             whether to scale radii with :code:`Image.fwhm` usually present in :code:`Image.epsf`, by default True
         name : str, optional
             name of the block, by default None
         """
-        super().__init__(name=name)
+        super().__init__(name=name, read=["sources", "data"])
         if radii is None:
             # log-uniform
             self._radii = np.exp(np.linspace(np.log(0.1), np.log(12), 30))
         else:
             self._radii = radii
         self.scale = scale
 
@@ -48,15 +48,15 @@
     @property
     def citations(self) -> list:
         return super().citations + ["photutils"]
 
 
 class _AnnulusPhotometry(Block):
     def __init__(self, name=None, rin=5, rout=8, scale=True):
-        super().__init__(name=name)
+        super().__init__(name=name, read=["sources", "data"])
         self.rin = rin
         self.rout = rout
         self.scale = scale
 
     @property
     def citations(self) -> list:
         return super().citations + ["photutils"]
```

### Comparing `prose-3.2.0/prose/blocks/psf.py` & `prose-3.2.3/prose/blocks/psf.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         Parameters
         ----------
         max_sources : int, optional
             maximum number of sources in a cutout for the cutout to be used, by default 1
         normalize : bool, optional
             whether to normalize cutouts to form a normalized EPSF, by default True
         """
-        super().__init__(name=name)
+        super().__init__(name=name, read=["cutouts"])
         self.max_sources = max_sources
         self.normalize = normalize
         self._parallel_friendly = True
 
     def run(self, image):
         good_cutouts = np.array(
             [c.data for c in image.cutouts if len(c.sources) <= self.max_sources]
@@ -94,15 +94,15 @@
         reference_image : _type_, optional
             _description_, by default None
         name : _type_, optional
             _description_, by default None
         verbose : bool, optional
             _description_, by default False
         """
-        super().__init__(name, verbose)
+        super().__init__(name, verbose, read=["epsf"])
         self._init = reference_image.epsf.params if reference_image else None
         self.shape = (0, 0)  # reference_image.epsf.shape if reference_image else None
         self.x, self.y = None, None
         self._last_init = None
         self._parallel_friendly = True
 
     def run(self, image: Image):
```

### Comparing `prose-3.2.0/prose/blocks/shepard.py` & `prose-3.2.3/prose/blocks/shepard.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/blocks/utils.py` & `prose-3.2.3/prose/blocks/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         name : _type_, optional
             _description_, by default None
         Returns
         -------
         _type_
             _description_
         """
-        super().__init__(name, verbose)
+        super().__init__(name, verbose, read=["sources"])
         if isinstance(key, str):
             if key == "cutout_sum":
 
                 def key(cutout):
                     return np.nansum(cutout.data)
 
         assert callable(key)
@@ -166,14 +166,16 @@
         easy_ram: bool = True,
         verbose: bool = True,
         shared: bool = False,
         **kwargs,
     ):
         """Flat, Bias and Dark calibration.
 
+        |modify|
+
         The provided calibration images can be either:
 
         - a list of paths to FITS files
         - a list of :py:class:`~prose.Image` objects
         - an array of np.ndarray images
         - a single :py:class:`~prose.Image` object
         - a single np.ndarray image
```

### Comparing `prose-3.2.0/prose/blocks/visualization.py` & `prose-3.2.3/prose/blocks/visualization.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/builtins.py` & `prose-3.2.3/prose/builtins.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/citations.py` & `prose-3.2.3/prose/citations.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/config.py` & `prose-3.2.3/prose/config.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/console_utils.py` & `prose-3.2.3/prose/console_utils.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/core/block.py` & `prose-3.2.3/prose/core/block.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         name of the block, by default None
     size: int, optional
         number of images processed by the block, by default 1
 
     All prose blocks must be child of this parent class
     """
 
-    def __init__(self, name=None, verbose=False, size=1):
+    def __init__(self, name=None, verbose=False, size=1, read=None):
         assert size % 2 == 1, "block size must be odd"
         _name = self.__class__.__name__
         _issue = f"https://github.com/lgrcia/prose/issues/new?title=Missing+doc+for+{_name}&body=Documentation+is+missing+for+block+{_name}"
 
         self.__doc__ = f"[**click to ask for documentation**]({_issue})"
 
         self.name = name
@@ -36,27 +36,44 @@
         self.processing_time = 0
         self.runs = 0
         self.in_sequence = False
         self.verbose = verbose
 
         self._data_block = False
         self.size = size
+        if read is not None:
+            assert isinstance(read, list), "require must be a list"
+            self.read = read
+        else:
+            self.read = []
 
     @property
     def args(self):
         return self._args
 
+    def _check_require(self, image):
+        for _require in self.read:
+            if _require == "sources":
+                if len(image.sources) == 0:
+                    raise AttributeError(f"Image must have sources (0 found)")
+            elif _require == "wcs":
+                if not image.plate_solved:
+                    raise AttributeError(f"Image must have valid WCS")
+            if not hasattr(image, _require) and not hasattr(image.computed, _require):
+                raise AttributeError(f"Image must have attribute '{_require}'")
+
     def _run(self, buffer):
         t0 = time()
         if isinstance(buffer, Buffer):
             image = buffer[0] if self.size == 1 else buffer
         elif isinstance(buffer, Image):
             image = buffer
         else:
             raise ValueError("block must be run on a Buffer or an Image")
+        self._check_require(image)
         self.run(image)
         self.processing_time += time() - t0
         self.runs += 1
 
     def run(self, image: Image):
         """Running on a image (must be overwritten when subclassed)
 
@@ -85,15 +102,15 @@
 
     @staticmethod
     def _doc():
         return ""
 
     def __call__(self, image):
         image_copy = image.copy()
-        self.run(image_copy)
+        self._run(image_copy)
         if image_copy.discard:
             warning(f"{self.__class__.__name__} discarded Image")
         return image_copy
 
 
 # rewrite the tested function to accept Block instances as well as strings
 # requires pytest and is not used in the docs for now
```

### Comparing `prose-3.2.0/prose/core/image.py` & `prose-3.2.3/prose/core/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     def __getattr__(self, name):
         if "computed" not in self.__dict__:
             super.__getattr__(self, name)
         else:
             if name in self.computed:
                 return self.computed[name]
             else:
-                raise AttributeError(f"{name} cannot be interpreted as Image attribute")
+                raise AttributeError(f"Image has no '{name}'")
 
     def copy(self, data=True):
         """Copy of image object
 
         Parameters
         ----------
         data : bool, optional
@@ -307,19 +307,21 @@
     def sources(self) -> Sources:
         """Image sources.
 
         Returns
         -------
         prose.core.source.Sources
         """
-        return self._sources
+        return self._sources if self._sources is not None else Sources()
 
     @sources.setter
     def sources(self, new_sources):
-        if isinstance(new_sources, Sources):
+        if new_sources is None:
+            self._sources = None
+        elif isinstance(new_sources, Sources):
             self._sources = new_sources
         else:
             self._sources = Sources(np.array(new_sources))
 
     def cutout(
         self,
         coords: Union[list, tuple, np.ndarray],
```

### Comparing `prose-3.2.0/prose/core/sequence.py` & `prose-3.2.3/prose/core/sequence.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/core/source.py` & `prose-3.2.3/prose/core/source.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/fluxes.py` & `prose-3.2.3/prose/fluxes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,22 @@
 import pickle
 import warnings
 from copy import deepcopy
 from dataclasses import asdict, dataclass
+from functools import partial
 from pathlib import Path
 from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 from prose import utils
 
 
-def binned_white_function(x, bins: int = 12):
-    # set binning idxs for white noise evaluation
-    bins = np.min([x.shape[-1], bins])
-    n = x.shape[-1] // bins
-    idxs = np.arange(n * bins)
-
-    def compute(f):
-        return np.nanmean(
-            np.nanstd(np.array(np.split(f.take(idxs, axis=-1), n, axis=-1)), axis=-1),
-            axis=0,
-        )
-
-    return compute
-
-
 def weights(
     fluxes: np.ndarray, tolerance: float = 1e-3, max_iteration: int = 200, bins: int = 5
 ):
     """Returns the weights computed using Broeg 2005
 
     Parameters
     ----------
@@ -47,44 +33,48 @@
     -------
     np.ndarray
         Broeg weights
     """
 
     # normalize
     dfluxes = fluxes / np.expand_dims(np.nanmean(fluxes, -1), -1)
-    binned_white = binned_white_function(fluxes, bins=bins)
+
+    def weight_function(fluxes):
+        return 1 / np.std(fluxes, axis=-1)
 
     i = 0
     evolution = 1e25
     lcs = None
     weights = None
     last_weights = np.zeros(dfluxes.shape[0 : len(dfluxes.shape) - 1])
 
     # Broeg 2004 algorithm to find weights of comp stars
     # --------------------------------------------------
     while evolution > tolerance and i < max_iteration:
         if i == 0:
-            weights = 1 / binned_white(dfluxes)
+            weights = weight_function(dfluxes)
+            mask = np.where(~np.isfinite(weights))
         else:
             # This metric is preferred from std to optimize over white noise and not red noise
-            std = binned_white(lcs)
-            weights = 1 / std
+            weights = weight_function(lcs)
 
         weights[~np.isfinite(weights)] = 0
 
-        # Keep track of weights
-        evolution = np.nanstd(
-            np.abs(np.nanmean(weights, axis=-1) - np.nanmean(last_weights, axis=-1))
+        evolution = np.abs(
+            np.nanmean(weights, axis=-1) - np.nanmean(last_weights, axis=-1)
         )
 
         last_weights = weights
         lcs = diff(dfluxes, weights=weights)
+
         i += 1
 
-    return weights
+    weights[0, mask] = 0
+
+    return weights[0]
 
 
 def diff(fluxes: np.ndarray, weights: np.ndarray = None):
     """Returns differential fluxes.
 
     If weights are specified, they are used to produce an artificial light curve by which all flux are differentiated (see Broeg 2005)
 
@@ -114,15 +104,15 @@
 
 
 def auto_diff_1d(fluxes, i=None):
     dfluxes = fluxes / np.expand_dims(np.nanmean(fluxes, -1), -1)
     w = weights(dfluxes)
     if i is not None:
         idxs = np.argsort(w)[::-1]
-        white_noise = binned_white_function(dfluxes)
+        white_noise = utils.binned_nanstd(dfluxes)
         last_white_noise = 1e10
 
         def best_weights(j):
             _w = w.copy()
             _w[idxs[j::]] = 0.0
             _w[i] = 0.0
             return _w
@@ -162,15 +152,15 @@
         np.all(
             (fluxes - np.median(fluxes, 1)[..., None])
             < sigma * np.std(fluxes, 1)[..., None],
             0,
         ),
     ]
     if method == "binned":
-        white_noise = binned_white_function(fluxes)
+        white_noise = utils.binned_nanstd(fluxes)
         criterion = white_noise(fluxes)
     elif method == "stddiff":
         criterion = utils.std_diff_metric(fluxes)
     elif method == "stability":
         criterion = utils.stability_aperture(fluxes)
     else:
         raise ValueError("{} is not a valid method".format(method))
@@ -274,14 +264,26 @@
         return self.fluxes.shape
 
     @property
     def ndim(self):
         """Number of dimensions of fluxes"""
         return self.fluxes.ndim
 
+    @property
+    def comparisons(self):
+        """Comparison stars indices ordered from most to less weighted"""
+        if self.weights is None:
+            return None
+        else:
+            if self.aperture is None:
+                raise ValueError("aperture must be set")
+
+            idxs = np.argsort(self.weights[self.aperture])[::-1]
+            return idxs[np.flatnonzero(self.weights[self.aperture][idxs] > 0.0)]
+
     def vander(consant=True, **kwargs):
         pass
 
     def diff(self, comps: np.ndarray = None):
         """Differential photometry
 
         Parameters
```

### Comparing `prose-3.2.0/prose/io/create_fm_db.sql` & `prose-3.2.3/prose/io/create_fm_db.sql`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/io/fitsmanager.py` & `prose-3.2.3/prose/io/fitsmanager.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/io/io.py` & `prose-3.2.3/prose/io/io.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/simulations.py` & `prose-3.2.3/prose/simulations.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/telescope.py` & `prose-3.2.3/prose/telescope.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/prose/utils.py` & `prose-3.2.3/prose/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,14 +373,20 @@
     """
 
     from astroquery.gaia import Gaia
 
     if isinstance(center, SkyCoord):
         ra = center.ra.to(u.deg).value
         dec = center.dec.to(u.deg).value
+    elif isinstance(center, (tuple, list)):
+        ra, dec = center
+        if isinstance(ra, u.Quantity):
+            ra = ra.to(u.deg).value
+        if isinstance(dec, u.Quantity):
+            dec = dec.to(u.deg).value
 
     if not isinstance(fov, u.Quantity):
         fov = fov * u.deg
 
     if fov.ndim == 1:
         ra_fov, dec_fov = fov.to(u.deg).value
     else:
@@ -452,14 +458,16 @@
         if distances[closest] < tolerance:
             matches.append([i, closest])
         else:
             if none:
                 matches.append([i, np.nan])
 
     matches = np.array(matches)
+    matches = matches[np.all(~np.isnan(matches), 1)]
+    matches = matches.astype(int)
 
     if return_idxs:
         return matches
     else:
         if len(matches) > 0:
             return s1[matches[:, 0]], s2[matches[:, 1]]
         else:
@@ -508,7 +516,22 @@
         getattr(blocks, b)
         for b in dir(blocks)
         if isinstance(getattr(blocks, b), type)
         and issubclass(getattr(blocks, b), blocks.Block)
     ]
 
     return blocks
+
+
+def binned_nanstd(x, bins: int = 12):
+    # set binning idxs for white noise evaluation
+    bins = np.min([x.shape[-1], bins])
+    n = x.shape[-1] // bins
+    idxs = np.arange(n * bins)
+
+    def compute(f):
+        return np.nanmean(
+            np.nanstd(np.array(np.split(f.take(idxs, axis=-1), n, axis=-1)), axis=-1),
+            axis=0,
+        )
+
+    return compute
```

### Comparing `prose-3.2.0/prose/visualization.py` & `prose-3.2.3/prose/visualization.py`

 * *Files identical despite different names*

### Comparing `prose-3.2.0/pyproject.toml` & `prose-3.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prose"
-version = "3.2.0"
+version = "3.2.3"
 description = "Modular image processing pipelines for Astronomy"
 authors = ["Lionel Garcia"]
 license = "MIT"
 readme = "README.md"
 include = ["prose/io/*.sql"]
 
 [tool.poetry.dependencies]
```

### Comparing `prose-3.2.0/PKG-INFO` & `prose-3.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prose
-Version: 3.2.0
+Version: 3.2.3
 Summary: Modular image processing pipelines for Astronomy
 License: MIT
 Author: Lionel Garcia
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prose Version: 3.2.0 Summary: Modular image
+Metadata-Version: 2.1 Name: prose Version: 3.2.3 Summary: Modular image
 processing pipelines for Astronomy License: MIT Author: Lionel Garcia Requires-
 Python: >=3.8,<3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: astropy (>=5.1.1,<6.0.0) Requires-
 Dist: astroquery (>=0.4.6,<0.5.0) Requires-Dist: celerite2 Requires-Dist:
```

