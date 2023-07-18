# Comparing `tmp/CompactObject_TOV-1.4.1.tar.gz` & `tmp/CompactObject_TOV-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CompactObject_TOV-1.4.1.tar", last modified: Mon Jul 17 01:03:14 2023, max compression
+gzip compressed data, was "CompactObject_TOV-1.5.0.tar", last modified: Tue Jul 18 01:13:28 2023, max compression
```

## Comparing `CompactObject_TOV-1.4.1.tar` & `CompactObject_TOV-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-17 01:03:14.625498 CompactObject_TOV-1.4.1/
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-17 01:03:14.599250 CompactObject_TOV-1.4.1/CompactObject_TOV.egg-info/
--rw-r--r--   0 a9         (501) staff       (20)       83 2023-07-17 01:03:13.000000 CompactObject_TOV-1.4.1/CompactObject_TOV.egg-info/PKG-INFO
--rw-r--r--   0 a9         (501) staff       (20)      355 2023-07-17 01:03:14.000000 CompactObject_TOV-1.4.1/CompactObject_TOV.egg-info/SOURCES.txt
--rw-r--r--   0 a9         (501) staff       (20)        1 2023-07-17 01:03:13.000000 CompactObject_TOV-1.4.1/CompactObject_TOV.egg-info/dependency_links.txt
--rw-r--r--   0 a9         (501) staff       (20)       10 2023-07-17 01:03:13.000000 CompactObject_TOV-1.4.1/CompactObject_TOV.egg-info/top_level.txt
--rw-r--r--   0 a9         (501) staff       (20)     1099 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/LICENSE
--rw-r--r--   0 a9         (501) staff       (20)       83 2023-07-17 01:03:14.621157 CompactObject_TOV-1.4.1/PKG-INFO
--rw-r--r--   0 a9         (501) staff       (20)     3418 2023-07-17 00:57:37.000000 CompactObject_TOV-1.4.1/README.md
-drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-17 01:03:14.618384 CompactObject_TOV-1.4.1/TOVsolver/
--rw-r--r--   0 a9         (501) staff       (20)     2620 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/TOVsolver/EoS_import.py
--rw-r--r--   0 a9         (501) staff       (20)       25 2023-07-17 00:59:11.000000 CompactObject_TOV-1.4.1/TOVsolver/__init__.py
--rw-r--r--   0 a9         (501) staff       (20)      129 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/TOVsolver/constant.py
--rw-r--r--   0 a9         (501) staff       (20)     5622 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/TOVsolver/main.py
--rw-r--r--   0 a9         (501) staff       (20)     8598 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/TOVsolver/solver_code.py
--rw-r--r--   0 a9         (501) staff       (20)      785 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/TOVsolver/speed_of_sound.py
--rw-r--r--   0 a9         (501) staff       (20)     1772 2023-07-16 23:02:27.000000 CompactObject_TOV-1.4.1/TOVsolver/tests_script.py
--rw-r--r--   0 a9         (501) staff       (20)       38 2023-07-17 01:03:14.625687 CompactObject_TOV-1.4.1/setup.cfg
--rw-r--r--   0 a9         (501) staff       (20)      136 2023-07-17 00:59:39.000000 CompactObject_TOV-1.4.1/setup.py
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-18 01:13:28.781543 CompactObject_TOV-1.5.0/
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-18 01:13:28.746019 CompactObject_TOV-1.5.0/CompactObject_TOV.egg-info/
+-rw-r--r--   0 a9         (501) staff       (20)      164 2023-07-18 01:13:28.000000 CompactObject_TOV-1.5.0/CompactObject_TOV.egg-info/PKG-INFO
+-rw-r--r--   0 a9         (501) staff       (20)      462 2023-07-18 01:13:28.000000 CompactObject_TOV-1.5.0/CompactObject_TOV.egg-info/SOURCES.txt
+-rw-r--r--   0 a9         (501) staff       (20)        1 2023-07-18 01:13:28.000000 CompactObject_TOV-1.5.0/CompactObject_TOV.egg-info/dependency_links.txt
+-rw-r--r--   0 a9         (501) staff       (20)       24 2023-07-18 01:13:28.000000 CompactObject_TOV-1.5.0/CompactObject_TOV.egg-info/top_level.txt
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-18 01:13:28.758672 CompactObject_TOV-1.5.0/EOSgenerators/
+-rw-r--r--   0 a9         (501) staff       (20)     6686 2023-07-16 23:02:27.000000 CompactObject_TOV-1.5.0/EOSgenerators/RMF_EOS.py
+-rw-r--r--   0 a9         (501) staff       (20)        0 2023-07-18 01:05:53.000000 CompactObject_TOV-1.5.0/EOSgenerators/__init__.py
+-rw-r--r--   0 a9         (501) staff       (20)      529 2023-07-17 00:24:32.000000 CompactObject_TOV-1.5.0/EOSgenerators/crust_EOS.py
+-rw-r--r--   0 a9         (501) staff       (20)     7140 2023-07-16 23:02:27.000000 CompactObject_TOV-1.5.0/EOSgenerators/fastRMF_EoS.py
+-rw-r--r--   0 a9         (501) staff       (20)     1099 2023-07-16 23:02:27.000000 CompactObject_TOV-1.5.0/LICENSE
+-rw-r--r--   0 a9         (501) staff       (20)      164 2023-07-18 01:13:28.779861 CompactObject_TOV-1.5.0/PKG-INFO
+-rw-r--r--   0 a9         (501) staff       (20)     4854 2023-07-18 01:10:48.000000 CompactObject_TOV-1.5.0/README.md
+drwxr-xr-x   0 a9         (501) staff       (20)        0 2023-07-18 01:13:28.776713 CompactObject_TOV-1.5.0/TOVsolver/
+-rw-r--r--   0 a9         (501) staff       (20)     2620 2023-07-16 23:02:27.000000 CompactObject_TOV-1.5.0/TOVsolver/EoS_import.py
+-rw-r--r--   0 a9         (501) staff       (20)       25 2023-07-18 01:03:26.000000 CompactObject_TOV-1.5.0/TOVsolver/__init__.py
+-rw-r--r--   0 a9         (501) staff       (20)      158 2023-07-17 19:25:29.000000 CompactObject_TOV-1.5.0/TOVsolver/constant.py
+-rw-r--r--   0 a9         (501) staff       (20)     7205 2023-07-17 23:40:59.000000 CompactObject_TOV-1.5.0/TOVsolver/main.py
+-rw-r--r--   0 a9         (501) staff       (20)     8598 2023-07-16 23:02:27.000000 CompactObject_TOV-1.5.0/TOVsolver/solver_code.py
+-rw-r--r--   0 a9         (501) staff       (20)      785 2023-07-16 23:02:27.000000 CompactObject_TOV-1.5.0/TOVsolver/speed_of_sound.py
+-rw-r--r--   0 a9         (501) staff       (20)     1772 2023-07-16 23:02:27.000000 CompactObject_TOV-1.5.0/TOVsolver/tests_script.py
+-rw-r--r--   0 a9         (501) staff       (20)       38 2023-07-18 01:13:28.781724 CompactObject_TOV-1.5.0/setup.cfg
+-rw-r--r--   0 a9         (501) staff       (20)      136 2023-07-18 01:02:17.000000 CompactObject_TOV-1.5.0/setup.py
```

### Comparing `CompactObject_TOV-1.4.1/LICENSE` & `CompactObject_TOV-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.4.1/README.md` & `CompactObject_TOV-1.5.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
-1. Dealing with complex Relativistic Mean field (RMF) theory to generate Equation of State (EOS) of neutron star. ([EOSgenerators](https://github.com/ChunHuangPhy/EoS_inference/blob/main/EOSgenerators) package)
-2. Solves the Tolman-Oppenheimer-Volkoff equation for a spherically symmetric compact object out of given equation of state of neutron star. ([TOVsolver](https://github.com/ChunHuangPhy/EoS_inference/blob/main/TOVsolver) folder)
+1. Dealing with complex Relativistic Mean field (RMF) theory to generate Equation of State (EOS) of neutron star. ([EOSgenerators](https://github.com/ChunHuangPhy/EoS_inference/blob/main/EOSgenerators) Package)
+2. Solves the Tolman-Oppenheimer-Volkoff equation for a spherically symmetric compact object out of given equation of state of neutron star. ([TOVsolver](https://github.com/ChunHuangPhy/EoS_inference/blob/main/TOVsolver) Package)
+3. Implementing Neutron state EOS inference by Nested Sampling, draw constraints from Nuclear experiments, Neutron star mass (and/or) radius observations (from X-ray timing and/or radio timing). That all workflow is inside this folder. ([InferenceWorkflow](https://github.com/ChunHuangPhy/EoS_inference/blob/main/InferenceWorkflow) Package) 
+
+
+Project papers list based these package: (Please consider cite them!)
+
+[1]. [Huang, C., Raaijmakers, G., Watts, A. L., Tolos, L., and Providência, C., “Constraining fundamental nuclear physics parameters using neutron star mass-radius measurements I: Nucleonic models”, <i>arXiv e-prints</i>, 2023. doi:10.48550/arXiv.2303.17518.](https://arxiv.org/abs/2303.17518)
 
 ### Inlcudes
 1. Routine to check a valid equation of state input
 2. Return the mass, radius, and tidal deformability, and compute the corresponding speed of sound.
-3. [Sample TOV solver Notebook](https://github.com/ChunHuangPhy/EoS_inference/blob/main/Test_Case/test_TOVsolver.ipynb) and [Sample RMF Equation of state solver Notebook](https://github.com/ChunHuangPhy/EoS_inference/blob/main/Test_Case/test_EOSgenerators.ipynb) on the github to show off what we can do currently and how to use our code.
-5. Test cases and documentation
+3. [Sample TOV solver Notebook](https://github.com/ChunHuangPhy/EoS_inference/blob/main/Test_Case/test_TOVsolver.ipynb), [Sample RMF Equation of state solver Notebook](https://github.com/ChunHuangPhy/EoS_inference/blob/main/Test_Case/test_EOSgenerators.ipynb) and [Sample Analysis Notebook on Equation of state Inference and tutorial](https://github.com/ChunHuangPhy/EoS_inference/blob/main/Test_Case/test_Inference.ipynb) on the github to show off what we can do currently and how to use our code.
+4. Test cases and documentation
 ### v.1.3 new features:
-6. Added computation function of generating Relativistic mean field theory(RMF) model EOS functionality. Defined two files fastRMF_EOS and RMF_EOS, which the fastRMF_EOS is speed up by numba, which need gcc compiler, could be hard to implement in windows, so we leave the options for users.
+5. Added computation function of generating Relativistic mean field theory(RMF) model EOS functionality. Defined two files fastRMF_EOS and RMF_EOS, which the fastRMF_EOS is speed up by numba, which need gcc compiler, could be hard to implement in windows, so we leave the options for users.
+### v.1.5 new features:
+6. Added Whole workflow of Bayesian inference of neutron star equation of state. Include defining prior by InferenceWorkflow.prior, which included two types: flat distribution and gaussian type. Include defining liklihood generated from nuclear and astrophysical constraint.
+
 
 ## Installation
 
 _Below are commands to install and update the package as well as a link to pypi._
 
 
 ##### [PyPi](https://pypi.org/project/CompactObject-TOV/)
@@ -25,14 +34,28 @@
    ```sh
    pip install CompactObject-TOV
    ```
 2. Update package
    ```sh
    pip install CompactObject-TOV --upgrade
    ```
+
+When you call the package, if you need to do EoS computation just
+   ```sh
+   import EOSgenerators
+   ```
+if you need TOV solver, just
+   ```sh
+   import TOVsolver
+   ```
+if you need to do Bayesian inference, just
+   ```sh
+   import InferenceWorkflow
+   ```
+
 ## Physics notations
 1. CGS units is using here, for input quantity (equation of state): Pressure (P) and Energy density (rho).
 P is in $MeV/fm^{-3}$, same for rho. However, to omit a lot of the repeat of c,G. We set P as rescaled:
 (value in $MeV/fm^{-3}$)*G/c^4, for rho we have (value in $MeV/fm^{-3}$)*G/c^2
 2. Out put M in Mass of sun, radius in km, unit-less for spped of sound and tidal deformability.
 <!-- LICENSE -->
 ## License
@@ -48,14 +71,15 @@
 * Chun Huang - chun.h@wustl.edu
 * Nicole Osborn - n.osborn@wustl.edu
 * Nathan Whitsett - whitsett.n@wustl.edu
 
 Project Link: [[https://github.com/ChunHuangPhy/EoS_inference](https://github.com/ChunHuangPhy/EoS_inference)]
 
 
+
 [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.8145167.svg)](http://dx.doi.org/10.5281/zenodo..8145167)
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- ACKNOWLEDGMENTS -->
 ## Acknowledgments
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,35 +1,53 @@
  ## About The Project 1. Dealing with complex Relativistic Mean field (RMF)
 theory to generate Equation of State (EOS) of neutron star. ([EOSgenerators]
 (https://github.com/ChunHuangPhy/EoS_inference/blob/main/EOSgenerators)
-package) 2. Solves the Tolman-Oppenheimer-Volkoff equation for a spherically
+Package) 2. Solves the Tolman-Oppenheimer-Volkoff equation for a spherically
 symmetric compact object out of given equation of state of neutron star. (
 [TOVsolver](https://github.com/ChunHuangPhy/EoS_inference/blob/main/TOVsolver)
-folder) ### Inlcudes 1. Routine to check a valid equation of state input 2.
-Return the mass, radius, and tidal deformability, and compute the corresponding
-speed of sound. 3. [Sample TOV solver Notebook](https://github.com/
-ChunHuangPhy/EoS_inference/blob/main/Test_Case/test_TOVsolver.ipynb) and
-[Sample RMF Equation of state solver Notebook](https://github.com/ChunHuangPhy/
-EoS_inference/blob/main/Test_Case/test_EOSgenerators.ipynb) on the github to
-show off what we can do currently and how to use our code. 5. Test cases and
-documentation ### v.1.3 new features: 6. Added computation function of
-generating Relativistic mean field theory(RMF) model EOS functionality. Defined
-two files fastRMF_EOS and RMF_EOS, which the fastRMF_EOS is speed up by numba,
-which need gcc compiler, could be hard to implement in windows, so we leave the
-options for users. ## Installation _Below are commands to install and update
-the package as well as a link to pypi._ ##### [PyPi](https://pypi.org/project/
-CompactObject-TOV/) 1. Install package ```sh pip install CompactObject-TOV ```
-2. Update package ```sh pip install CompactObject-TOV --upgrade ``` ## Physics
-notations 1. CGS units is using here, for input quantity (equation of state):
-Pressure (P) and Energy density (rho). P is in $MeV/fm^{-3}$, same for rho.
-However, to omit a lot of the repeat of c,G. We set P as rescaled: (value in
-$MeV/fm^{-3}$)*G/c^4, for rho we have (value in $MeV/fm^{-3}$)*G/c^2 2. Out put
-M in Mass of sun, radius in km, unit-less for spped of sound and tidal
-deformability.  ## License Distributed under the MIT License. See `LICENSE.txt`
-for more information.
+Package) 3. Implementing Neutron state EOS inference by Nested Sampling, draw
+constraints from Nuclear experiments, Neutron star mass (and/or) radius
+observations (from X-ray timing and/or radio timing). That all workflow is
+inside this folder. ([InferenceWorkflow](https://github.com/ChunHuangPhy/
+EoS_inference/blob/main/InferenceWorkflow) Package) Project papers list based
+these package: (Please consider cite them!) [1]. [Huang, C., Raaijmakers, G.,
+Watts, A. L., Tolos, L., and ProvidÃªncia, C., âConstraining fundamental
+nuclear physics parameters using neutron star mass-radius measurements I:
+Nucleonic modelsâ, arXiv e-prints, 2023. doi:10.48550/arXiv.2303.17518.]
+(https://arxiv.org/abs/2303.17518) ### Inlcudes 1. Routine to check a valid
+equation of state input 2. Return the mass, radius, and tidal deformability,
+and compute the corresponding speed of sound. 3. [Sample TOV solver Notebook]
+(https://github.com/ChunHuangPhy/EoS_inference/blob/main/Test_Case/
+test_TOVsolver.ipynb), [Sample RMF Equation of state solver Notebook](https://
+github.com/ChunHuangPhy/EoS_inference/blob/main/Test_Case/
+test_EOSgenerators.ipynb) and [Sample Analysis Notebook on Equation of state
+Inference and tutorial](https://github.com/ChunHuangPhy/EoS_inference/blob/
+main/Test_Case/test_Inference.ipynb) on the github to show off what we can do
+currently and how to use our code. 4. Test cases and documentation ### v.1.3
+new features: 5. Added computation function of generating Relativistic mean
+field theory(RMF) model EOS functionality. Defined two files fastRMF_EOS and
+RMF_EOS, which the fastRMF_EOS is speed up by numba, which need gcc compiler,
+could be hard to implement in windows, so we leave the options for users. ###
+v.1.5 new features: 6. Added Whole workflow of Bayesian inference of neutron
+star equation of state. Include defining prior by InferenceWorkflow.prior,
+which included two types: flat distribution and gaussian type. Include defining
+liklihood generated from nuclear and astrophysical constraint. ## Installation
+_Below are commands to install and update the package as well as a link to
+pypi._ ##### [PyPi](https://pypi.org/project/CompactObject-TOV/) 1. Install
+package ```sh pip install CompactObject-TOV ``` 2. Update package ```sh pip
+install CompactObject-TOV --upgrade ``` When you call the package, if you need
+to do EoS computation just ```sh import EOSgenerators ``` if you need TOV
+solver, just ```sh import TOVsolver ``` if you need to do Bayesian inference,
+just ```sh import InferenceWorkflow ``` ## Physics notations 1. CGS units is
+using here, for input quantity (equation of state): Pressure (P) and Energy
+density (rho). P is in $MeV/fm^{-3}$, same for rho. However, to omit a lot of
+the repeat of c,G. We set P as rescaled: (value in $MeV/fm^{-3}$)*G/c^4, for
+rho we have (value in $MeV/fm^{-3}$)*G/c^2 2. Out put M in Mass of sun, radius
+in km, unit-less for spped of sound and tidal deformability.  ## License
+Distributed under the MIT License. See `LICENSE.txt` for more information.
                                                                   (back_to_top)
  ## Contact * Chun Huang - chun.h@wustl.edu * Nicole Osborn -
 n.osborn@wustl.edu * Nathan Whitsett - whitsett.n@wustl.edu Project Link: [
 [https://github.com/ChunHuangPhy/EoS_inference](https://github.com/
 ChunHuangPhy/EoS_inference)] [![DOI](https://zenodo.org/badge/doi/10.5281/
 zenodo.8145167.svg)](http://dx.doi.org/10.5281/zenodo..8145167)
                                                                   (back_to_top)
```

### Comparing `CompactObject_TOV-1.4.1/TOVsolver/EoS_import.py` & `CompactObject_TOV-1.5.0/TOVsolver/EoS_import.py`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.4.1/TOVsolver/main.py` & `CompactObject_TOV-1.5.0/TOVsolver/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,17 +50,18 @@
 #if   all(x<y for x, y in zip(eps_total_poly[:], eps_total_poly[[1:])) and all(x<y for x, y in zip(pres_total_poly[j][:], pres_total_poly[j][1:])):
     for i in range(len(density)):
         try:
             Radius.append(TOV_solver.solveTOV(density[i], energy_density, pressure)[1])
             Mass.append(TOV_solver.solveTOV(density[i], energy_density, pressure)[0])
     #This is sentense is for avoiding the outflow of the result, like when solveTOV blow up because of ill EOS, we need to stop
         except OverflowError as e:
-            print("This EOS is ill-defined to reach an infinity result, that is not phyiscal, No Mass radius will be generated.")
+            #print("This EOS is ill-defined to reach an infinity result, that is not phyiscal, No Mass radius will be generated.")
+            break
     MR = np.vstack((Radius, Mass)).T
-    print("Mass Radius file will be generated and stored as  2-d array. The first column is Radius, second one is mass")
+    #print("Mass Radius file will be generated and stored as  2-d array. The first column is Radius, second one is mass")
     
     return MR
 
 def OutputMRT(input_file='',density=[],pressure=[]):
 
     """Outputs the mass, radius, and tidal deformability
     Args:
@@ -95,22 +96,21 @@
     for i in range(len(density)):
         try:
             Radius.append(TOV_solver.solveTOV_tidal(density[i], energy_density, pressure)[1])
             Mass.append(TOV_solver.solveTOV_tidal(density[i], energy_density, pressure)[0])
             tidal.append(TOV_solver.solveTOV_tidal(density[i], energy_density, pressure)[2])
     #This is sentense is for avoiding the outflow of the result, like when solveTOV blow up because of ill EOS, we need to stop
         except OverflowError as e:
-            print("This EOS is ill-defined to reach an infinity result, that is not phyiscal, No Mass radius will be generated.")
-
+            #print("This EOS is ill-defined to reach an infinity result, that is not phyiscal, No Mass radius will be generated.")
+            break
     MRT = np.vstack((Radius, Mass,tidal)).T
-    print("Mass Radius and tidal will be generated as the 3-d array. The first column is Radius, second one is mass,last is tidal")
+    #print("Mass Radius and tidal will be generated as the 3-d array. The first column is Radius, second one is mass,last is tidal")
 
     return MRT
 
-
 def OutputC_s(input_file='',density=[],pressure=[]):
 
     """Calls function to open csv (if needed) and check equation of state validity.
         Then calls function to calculate speed of sound.
 
     Args:
         file_name (string, optional): string. CSV file to be opened.
@@ -120,7 +120,44 @@
     Returns:
         C_s (array): numpy 1D array. List of speeds of sound.
     """
 
     energy_density, pressure = EoS_import.EOS_import(input_file,density,pressure)
     C_s = speed_of_sound.speed_of_sound_calc(energy_density, pressure)
     return C_s
+
+def OutputMRpoint(central_density,energy_density,pressure):
+
+    """Outputs the mass, radius, and tidal deformability
+    Args:
+        file_name (string, optional): string. CSV file to be opened.
+        density (array, optional): numpy 1Darray. Passed into a check function and returned if valid.
+        pressure (array, optional): numpy 1Darray. Passed into a check function and returned if valid.
+
+    Returns:
+        MR (tuple): tuple with mass, radius.
+    """
+
+    c = 3e10
+    G = 6.67428e-8
+    Msun = 1.989e33
+
+    dyncm2_to_MeVfm3 = 1./(1.6022e33)
+    gcm3_to_MeVfm3 = 1./(1.7827e12)
+    oneoverfm_MeV = 197.33
+    
+    Radius = []
+    Mass = []
+    
+#This following step is to make a dicision whether the EOS ingredients is always increase. We can do that outsie of this main to the 
+#EOS import.
+#if   all(x<y for x, y in zip(eps_total_poly[:], eps_total_poly[[1:])) and all(x<y for x, y in zip(pres_total_poly[j][:], pres_total_poly[j][1:])):
+    try:
+        Radius.append(TOV_solver.solveTOV(central_density, energy_density, pressure)[1])
+        Mass.append(TOV_solver.solveTOV(central_density, energy_density, pressure)[0])
+    #This is sentense is for avoiding the outflow of the result, like when solveTOV blow up because of ill EOS, we need to stop
+    except OverflowError as e:
+        print("This EOS is ill-defined to reach an infinity result, that is not phyiscal, No Mass radius will be generated.")
+    MR = np.vstack((Radius, Mass)).T
+    if len(MR[0]) != 0:
+        print("should have some in mr")
+    return MR
```

### Comparing `CompactObject_TOV-1.4.1/TOVsolver/solver_code.py` & `CompactObject_TOV-1.5.0/TOVsolver/solver_code.py`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.4.1/TOVsolver/speed_of_sound.py` & `CompactObject_TOV-1.5.0/TOVsolver/speed_of_sound.py`

 * *Files identical despite different names*

### Comparing `CompactObject_TOV-1.4.1/TOVsolver/tests_script.py` & `CompactObject_TOV-1.5.0/TOVsolver/tests_script.py`

 * *Files identical despite different names*

