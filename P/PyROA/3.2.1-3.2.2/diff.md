# Comparing `tmp/PyROA-3.2.1.tar.gz` & `tmp/PyROA-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyROA-3.2.1.tar", last modified: Mon Jul 17 13:19:39 2023, max compression
+gzip compressed data, was "PyROA-3.2.2.tar", last modified: Tue Jul 18 10:26:08 2023, max compression
```

## Comparing `PyROA-3.2.1.tar` & `PyROA-3.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-17 13:19:39.707255 PyROA-3.2.1/
--rw-r--r--   0 donnanf    (503) staff       (20)      455 2023-07-17 13:19:39.705322 PyROA-3.2.1/PKG-INFO
-drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-17 13:19:39.411310 PyROA-3.2.1/PyROA/
--rw-r--r--   0 donnanf    (503) staff       (20)   111299 2023-07-17 12:31:49.000000 PyROA-3.2.1/PyROA/PyROA.py
--rw-r--r--   0 donnanf    (503) staff       (20)    42132 2023-03-21 15:13:42.000000 PyROA-3.2.1/PyROA/Utils.py
--rw-r--r--   0 donnanf    (503) staff       (20)      228 2023-07-17 13:19:06.000000 PyROA-3.2.1/PyROA/__init__.py
-drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-17 13:19:39.701896 PyROA-3.2.1/PyROA.egg-info/
--rw-r--r--   0 donnanf    (503) staff       (20)      455 2023-07-17 13:19:38.000000 PyROA-3.2.1/PyROA.egg-info/PKG-INFO
--rw-r--r--   0 donnanf    (503) staff       (20)      182 2023-07-17 13:19:38.000000 PyROA-3.2.1/PyROA.egg-info/SOURCES.txt
--rw-r--r--   0 donnanf    (503) staff       (20)        1 2023-07-17 13:19:38.000000 PyROA-3.2.1/PyROA.egg-info/dependency_links.txt
--rw-r--r--   0 donnanf    (503) staff       (20)        6 2023-07-17 13:19:38.000000 PyROA-3.2.1/PyROA.egg-info/top_level.txt
--rw-rw-r--   0 donnanf    (503) staff       (20)    16574 2023-07-17 13:18:50.000000 PyROA-3.2.1/README.md
--rw-r--r--   0 donnanf    (503) staff       (20)       38 2023-07-17 13:19:39.707612 PyROA-3.2.1/setup.cfg
--rw-rw-r--   0 donnanf    (503) staff       (20)      647 2023-07-17 13:18:23.000000 PyROA-3.2.1/setup.py
+drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-18 10:26:08.126862 PyROA-3.2.2/
+-rw-r--r--   0 donnanf    (503) staff       (20)      455 2023-07-18 10:26:08.125650 PyROA-3.2.2/PKG-INFO
+drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-18 10:26:08.086562 PyROA-3.2.2/PyROA/
+-rw-r--r--   0 donnanf    (503) staff       (20)   111603 2023-07-18 10:23:56.000000 PyROA-3.2.2/PyROA/PyROA.py
+-rw-r--r--   0 donnanf    (503) staff       (20)    42132 2023-03-21 15:13:42.000000 PyROA-3.2.2/PyROA/Utils.py
+-rw-r--r--   0 donnanf    (503) staff       (20)      228 2023-07-18 10:25:22.000000 PyROA-3.2.2/PyROA/__init__.py
+drwxr-xr-x   0 donnanf    (503) staff       (20)        0 2023-07-18 10:26:08.123997 PyROA-3.2.2/PyROA.egg-info/
+-rw-r--r--   0 donnanf    (503) staff       (20)      455 2023-07-18 10:26:07.000000 PyROA-3.2.2/PyROA.egg-info/PKG-INFO
+-rw-r--r--   0 donnanf    (503) staff       (20)      182 2023-07-18 10:26:07.000000 PyROA-3.2.2/PyROA.egg-info/SOURCES.txt
+-rw-r--r--   0 donnanf    (503) staff       (20)        1 2023-07-18 10:26:07.000000 PyROA-3.2.2/PyROA.egg-info/dependency_links.txt
+-rw-r--r--   0 donnanf    (503) staff       (20)        6 2023-07-18 10:26:07.000000 PyROA-3.2.2/PyROA.egg-info/top_level.txt
+-rw-rw-r--   0 donnanf    (503) staff       (20)    16574 2023-07-17 13:18:50.000000 PyROA-3.2.2/README.md
+-rw-r--r--   0 donnanf    (503) staff       (20)       38 2023-07-18 10:26:08.127157 PyROA-3.2.2/setup.cfg
+-rw-rw-r--   0 donnanf    (503) staff       (20)      647 2023-07-18 10:25:39.000000 PyROA-3.2.2/setup.py
```

### Comparing `PyROA-3.2.1/PyROA/PyROA.py` & `PyROA-3.2.2/PyROA/PyROA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1296,15 +1296,16 @@
     print(tabulate(table, headers=labels))        
     
 
     
 
     #Define starting position
     
-    pos = 0.2*pos* np.random.randn(int(2.0*Npar), int(Npar - param_delete)) + pos
+    pos = 0.2*np.array(pos)* np.random.randn(int(2.0*Npar), int(Npar - param_delete)) + np.array(pos) + 1e-4* np.random.randn(int(2.0*Npar), int(Npar - param_delete)) 
+
 
     nwalkers, ndim = pos.shape
     print("NWalkers="+str(int(2.0*Npar)))
     # Make sure initial positions aren't outside priors
     # priors_upper=[]
     # priors_lower=[]
     # for i in range(len(priors)):
@@ -2235,19 +2236,19 @@
     init_params_chunks = pos_chunks
 
     pos = list(chain.from_iterable(pos_chunks))#Flatten into single array
     labels = list(chain.from_iterable(labels_chunks))#Flatten into single array     
     
 
     print("Initial Parameter Values")
-    table = [pos]
+    table =[pos]
     print(tabulate(table, headers=labels))
 
     #Define starting position
-    pos = 0.2*pos * np.random.randn(int(2.0*Npar), int(Npar)) + pos
+    pos = 0.2*np.array(pos)* np.random.randn(int(2.0*Npar), int(Npar)) + np.array(pos) + 1e-4* np.random.randn(int(2.0*Npar), int(Npar)) 
     print("NWalkers="+str(int(2.0*Npar)))
     nwalkers, ndim = pos.shape
     with Pool() as pool:
 
         sampler = emcee.EnsembleSampler(nwalkers, ndim, log_probability2, 
                                         args=(data, priors, sig_level, init_params_chunks), pool=pool)
         sampler.run_mcmc(pos, Nsamples, progress=True);
@@ -2895,15 +2896,17 @@
     labels_latex = np.delete(labels_latex, [0,1, 2, 3, 4, 5])       
 
     print("Initial Parameter Values")
     table = [pos]
     print(tabulate(table, headers=labels))
 
     #Define starting position
-    pos = 1e-4 * np.random.randn(int(2.0*Npar), Npar - 6) + pos
+    #pos = 1e-4 * np.random.randn(int(2.0*Npar), Npar - 6) + pos
+    pos = 0.2*np.array(pos)* np.random.randn(int(2.0*Npar), int(Npar - 6)) + np.array(pos) + 1e-4* np.random.randn(int(2.0*Npar), int(Npar - 6)) 
+
     nwalkers, ndim = pos.shape
     
     print("Nwalkers = ", nwalkers)  
     with Pool() as pool:
 
         sampler = emcee.EnsembleSampler(nwalkers, ndim, log_probability3, args=(data, priors, add_var, size, sig_level), pool=pool)
         sampler.run_mcmc(pos, Nsamples, progress=True);
```

### Comparing `PyROA-3.2.1/PyROA/Utils.py` & `PyROA-3.2.2/PyROA/Utils.py`

 * *Files identical despite different names*

### Comparing `PyROA-3.2.1/README.md` & `PyROA-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `PyROA-3.2.1/setup.py` & `PyROA-3.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # upload to pip
 # pip install .
 # python3 setup.py sdist bdist_wheel
 # twine upload dist/pydoppler-0.1.8.tar.gz
 
 setuptools.setup(
      name='PyROA',
-     version='3.2.1',
+     version='3.2.2',
      packages=['PyROA'] ,
      author="Fergus Donnan,",
      author_email="fergus.donnan@physics.ox.ac.uk",
      description="PyROA is a tool for modelling quasar lightcurves",
    long_description_content_type="text/markdown",
      url="https://github.com/FergusDonnan/PyROA",
      classifiers=[
```

