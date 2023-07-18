# Comparing `tmp/TDCRPy-0.0.6.tar.gz` & `tmp/TDCRPy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TDCRPy-0.0.6.tar", last modified: Fri Jul 14 13:54:23 2023, max compression
+gzip compressed data, was "dist\TDCRPy-0.0.7.tar", last modified: Tue Jul 18 10:02:38 2023, max compression
```

## Comparing `TDCRPy-0.0.6.tar` & `TDCRPy-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 13:54:23.000000 TDCRPy-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-07-14 13:54:23.000000 TDCRPy-0.0.6/Code/
--rw-rw-rw-   0        0        0    11530 2023-07-05 06:46:32.000000 TDCRPy-0.0.6/Code/Activity_TDCR.py
--rw-rw-rw-   0        0        0     4829 2023-07-05 09:18:15.000000 TDCRPy-0.0.6/Code/EfficiencyProfils.py
--rw-rw-rw-   0        0        0    23202 2023-07-13 12:37:29.000000 TDCRPy-0.0.6/Code/TDCRPy.py
--rw-rw-rw-   0        0        0    79115 2023-07-13 12:37:29.000000 TDCRPy-0.0.6/Code/TDCR_model_lib.py
--rw-rw-rw-   0        0        0     3171 2023-07-13 14:12:55.000000 TDCRPy-0.0.6/Code/TDCRoptimize.py
--rw-rw-rw-   0        0        0       93 2023-07-14 12:49:39.000000 TDCRPy-0.0.6/Code/__init__.py
--rw-rw-rw-   0        0        0      817 2023-05-23 08:42:51.000000 TDCRPy-0.0.6/Code/decay.py
--rw-rw-rw-   0        0        0      212 2023-07-14 13:41:00.000000 TDCRPy-0.0.6/Code/test.py
--rw-rw-rw-   0        0        0     3250 2023-05-23 08:42:51.000000 TDCRPy-0.0.6/Code/test1.py
--rw-rw-rw-   0        0        0     1086 2023-07-14 13:43:17.000000 TDCRPy-0.0.6/LICENCE.md
--rw-rw-rw-   0        0        0      799 2023-07-14 13:54:23.000000 TDCRPy-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4737 2023-05-23 08:42:51.000000 TDCRPy-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 13:54:23.000000 TDCRPy-0.0.6/TDCRPy.egg-info/
--rw-rw-rw-   0        0        0      799 2023-07-14 13:54:23.000000 TDCRPy-0.0.6/TDCRPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-14 13:54:23.000000 TDCRPy-0.0.6/TDCRPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 13:54:23.000000 TDCRPy-0.0.6/TDCRPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-14 13:54:23.000000 TDCRPy-0.0.6/TDCRPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-14 13:54:23.000000 TDCRPy-0.0.6/TDCRPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 13:54:23.000000 TDCRPy-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-07-14 13:49:13.000000 TDCRPy-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:02:39.000000 TDCRPy-0.0.7/
+-rw-rw-rw-   0        0        0     1086 2023-07-14 13:43:17.000000 TDCRPy-0.0.7/LICENCE.md
+-rw-rw-rw-   0        0        0     5610 2023-07-18 10:02:38.000000 TDCRPy-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4737 2023-05-23 08:42:51.000000 TDCRPy-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 10:02:38.000000 TDCRPy-0.0.7/TDCRPy/
+-rw-rw-rw-   0        0        0    11530 2023-07-05 06:46:32.000000 TDCRPy-0.0.7/TDCRPy/Activity_TDCR.py
+-rw-rw-rw-   0        0        0     4829 2023-07-05 09:18:15.000000 TDCRPy-0.0.7/TDCRPy/EfficiencyProfils.py
+-rw-rw-rw-   0        0        0    23207 2023-07-18 09:23:02.000000 TDCRPy-0.0.7/TDCRPy/TDCRPy.py
+-rw-rw-rw-   0        0        0    79829 2023-07-18 09:23:02.000000 TDCRPy-0.0.7/TDCRPy/TDCR_model_lib.py
+-rw-rw-rw-   0        0        0     3171 2023-07-13 14:12:55.000000 TDCRPy-0.0.7/TDCRPy/TDCRoptimize.py
+-rw-rw-rw-   0        0        0       93 2023-07-14 12:49:39.000000 TDCRPy-0.0.7/TDCRPy/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-05-23 08:42:51.000000 TDCRPy-0.0.7/TDCRPy/decay.py
+-rw-rw-rw-   0        0        0      292 2023-07-18 09:45:23.000000 TDCRPy-0.0.7/TDCRPy/test.py
+-rw-rw-rw-   0        0        0     3250 2023-05-23 08:42:51.000000 TDCRPy-0.0.7/TDCRPy/test1.py
+drwxrwxrwx   0        0        0        0 2023-07-18 10:02:38.000000 TDCRPy-0.0.7/TDCRPy.egg-info/
+-rw-rw-rw-   0        0        0     5610 2023-07-18 10:02:38.000000 TDCRPy-0.0.7/TDCRPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-07-18 10:02:38.000000 TDCRPy-0.0.7/TDCRPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 10:02:38.000000 TDCRPy-0.0.7/TDCRPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-18 10:02:38.000000 TDCRPy-0.0.7/TDCRPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 10:02:38.000000 TDCRPy-0.0.7/TDCRPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 10:02:39.000000 TDCRPy-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1188 2023-07-18 09:57:04.000000 TDCRPy-0.0.7/setup.py
```

### Comparing `TDCRPy-0.0.6/Code/Activity_TDCR.py` & `TDCRPy-0.0.7/TDCRPy/Activity_TDCR.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.6/Code/EfficiencyProfils.py` & `TDCRPy-0.0.7/TDCRPy/EfficiencyProfils.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.6/Code/TDCRPy.py` & `TDCRPy-0.0.7/TDCRPy/TDCRPy.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
                 energy_vec[i] = tl.energie_dep_beta(energy_vec[i])
                 particle_vec.append("gamma")
                 particle_vec.append("gamma")
                 energy_vec.append(511)
                 energy_vec.append(511)
 
             if p == "gamma" or p == "XKA" or p == "XKB" or p == "XL":
-                energy_vec[i] = tl.energie_dep_gamma(energy_vec[i])          # sampling energy free from photon
+                energy_vec[i] = tl.energie_dep_gamma(energy_vec[i],v=10)          # sampling energy free from photon
                 particle_vec[i] = "electron"
             if p == "Auger K" or p == "Auger L":
                 particle_vec[i] = "electron"
                 energy_vec[i] = tl.energie_dep_beta(energy_vec[i])
         if Display: print("\t Summary of the final charged particles")
         if Display: print("\t\t particles : ", particle_vec)
         if Display: print("\t\t energy    : ", energy_vec, "keV")
```

### Comparing `TDCRPy-0.0.6/Code/TDCR_model_lib.py` & `TDCRPy-0.0.7/TDCRPy/TDCR_model_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1262,22 +1262,26 @@
 #============================================================================================
 
 #============================================================================================
 
 #========================= énergie gamma ===================================================
 #'''
 if absolutePath: 
-    fp1 = 'G:\Python_modules\Jialin\Code\\MCNP-MATRIX/matrice/fichier/matrice_p_1_200k.txt'       #gamma-10ml-1-200keV-niveau 0
-    fp2 = 'G:\Python_modules\Jialin\Code\\MCNP-MATRIX/matrice/fichier/matrice_p_200_2000k.txt'    #gamma-10ml-200-2000keV-niveau 0
-    fp3 = 'G:\Python_modules\Jialin\Code\\MCNP-MATRIX/matrice/fichier/matrice_p_2000_10000k.txt'  #gamma-10ml-2000-10000keV-niveau 0
+    fp1 = 'G:\Python_modules\Jialin\Code\\MCNP-MATRIX/matrice/fichier/matrice_10ml-photon_1_200k.txt'       #gamma-10ml-1-200keV-niveau 0
+    fp2 = 'G:\Python_modules\Jialin\Code\\MCNP-MATRIX/matrice/fichier/matrice_10ml-photon_200_2000k.txt'    #gamma-10ml-200-2000keV-niveau 0
+    fp3 = 'G:\Python_modules\Jialin\Code\\MCNP-MATRIX/matrice/fichier/matrice_10ml-photon_2000_10000k.txt'  #gamma-10ml-2000-10000keV-niveau 0
+    fp4 = 'G:\Python_modules\Jialin\Code\\MCNP-MATRIX/matrice/fichier/matrice_16ml-photon_1_200k.txt'       #gamma-10ml-1-200keV-niveau 0
+    fp5 = 'G:\Python_modules\Jialin\Code\\MCNP-MATRIX/matrice/fichier/matrice_16ml-photon_200_2000k.txt'       #gamma-10ml-1-200keV-niveau 0
     fe = "G:\Python_modules\Jialin\Code\\MCNP-MATRIX/matrice/fichier/E_depose.txt"  
 else:
-    fp1 = 'MCNP-MATRIX/matrice/fichier/matrice_p_1_200k.txt'      #gamma-10ml-1-200keV-niveau 0
-    fp2 = 'MCNP-MATRIX/matrice/fichier/matrice_p_200_2000k.txt'   #gamma-10ml-200-2000keV-niveau 0
-    fp3 = 'MCNP-MATRIX/matrice/fichier/matrice_p_2000_10000k.txt' #gamma-10ml-2000-10000keV-niveau 0
+    fp1 = 'MCNP-MATRIX/matrice/fichier/matrice_10ml-photon_1_200k.txt'      #gamma-10ml-1-200keV-niveau 0
+    fp2 = 'MCNP-MATRIX/matrice/fichier/matrice_10ml-photon_200_2000k.txt'   #gamma-10ml-200-2000keV-niveau 0
+    fp3 = 'MCNP-MATRIX/matrice/fichier/matrice_10ml-photon_2000_10000k.txt' #gamma-10ml-2000-10000keV-niveau 0
+    fp4 = 'MCNP-MATRIX/matrice/fichier/matrice_16ml-photon_1_200k.txt'      #gamma-10ml-1-200keV-niveau 0
+    fp5 = 'MCNP-MATRIX/matrice/fichier/matrice_16ml-photon_200_2000k.txt'      #gamma-10ml-1-200keV-niveau 0
     fe = "MCNP-MATRIX/matrice/fichier/E_depose.txt"
 '''
 data1 = f1.readlines()
 data2 = f2.readlines()
 data3 = f3.readlines()
 data_e = fe.readlines()
 
@@ -1325,17 +1329,19 @@
             matrice[i][j] = float(data[i][j])
     return matrice
 
 
 Matrice10_p_1 = read_matrice(fp1,0)
 Matrice10_p_2 = read_matrice(fp2,1)
 Matrice10_p_3 = read_matrice(fp3,2)
+Matrice16_p_1 = read_matrice(fp4,0)
+Matrice16_p_2 = read_matrice(fp5,1)
 Matrice_e = read_matrice(fe,'e')
 
-def energie_dep_gamma(e_inci,*,matrice10_1=Matrice10_p_1,matrice10_2=Matrice10_p_2,matrice10_3=Matrice10_p_3,ed=Matrice_e):
+def energie_dep_gamma(e_inci,v,matrice10_1=Matrice10_p_1,matrice10_2=Matrice10_p_2,matrice10_3=Matrice10_p_3,matrice16_1=Matrice16_p_1,matrice16_2=Matrice16_p_2,ed=Matrice_e):
     """ 
     ----------
     Parameters
     ----------
     e_inci : float
         l'énergie incidente de particule.
     * : TYPE
@@ -1353,24 +1359,27 @@
     -------
     result : float
         l'énergie déposée.
 
     """
     ## sort keV / entrée : keV
     if e_inci <= 200:
-        index = int(e_inci)            # index de colonne de la matrice de l'énergie incidente la plus proche 
-        #doc = 'MCNP-MATRIX/matrice/matrice_p_1_200k.txt'
-        matrice = matrice1
-        #taille_x = 200
+        index = int(e_inci)            # index de colonne de la matrice de l'énergie incidente la plus proche
+        if v == 10: 
+            matrice = matrice10_1
+        elif v == 16:
+            matrice = matrice16_1
         e = ed[:,0]
     
     elif e_inci <= 2000:
         index = int((e_inci-200)/2)
-        #doc = 'MCNP-MATRIX/matrice/matrice_p_200_2000k.txt'
-        matrice = matrice2
+        if v == 10: 
+            matrice = matrice10_2
+        elif v == 16:
+            matrice = matrice16_2
         #taille_x = 901
         e = ed[:,1]
 
     else:
         index = (int(e_inci)-2000)//10
         #doc = 'MCNP-MATRIX/matrice/matrice_p_2000_10000k.txt'
         matrice = matrice3
@@ -1391,16 +1400,16 @@
     inde = sampling(matrice[1:,index])
     if inde == 1 : result = 0
         #elif e_inci<25: result = e[inde-1]*1e3*e_inci/matrice[0][index]
     else: result = e[inde]*1e3*e_inci/matrice[0][index]
     if result  > e_inci: result = e_inci
     return result
 
-#for i in range(50):
-    #print(energie_dep_gamma(511))
+#for i in range(10):
+ #   print(energie_dep_gamma(511,16))
 
 
 if absolutePath: 
     fe1 = 'G:\Python_modules\Jialin\Code\\MCNP-MATRIX/matrice/fichier/matrice_beta-_1_200k.txt' # electron-10ml-1-200keV-niveau 0
     fe2 = 'G:\Python_modules\Jialin\Code\\MCNP-MATRIX/matrice/fichier/matrice_beta-_200_2000k.txt' # electron-10ml-200-2000keV-niveau 1
     fe3 = 'G:\Python_modules\Jialin\Code\\MCNP-MATRIX/matrice/fichier/matrice_beta-_2000_10000k.txt' # electron-10ml-2000-10000keV-niveau 2
     fe = "G:\Python_modules\Jialin\Code\\MCNP-MATRIX/matrice/fichier/E_depose.txt"   # electron-10ml-énergie-niveau 'e'
```

### Comparing `TDCRPy-0.0.6/Code/TDCRoptimize.py` & `TDCRPy-0.0.7/TDCRPy/TDCRoptimize.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.6/Code/decay.py` & `TDCRPy-0.0.7/TDCRPy/decay.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.6/Code/test1.py` & `TDCRPy-0.0.7/TDCRPy/test1.py`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.6/LICENCE.md` & `TDCRPy-0.0.7/LICENCE.md`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.6/README.md` & `TDCRPy-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `TDCRPy-0.0.6/setup.py` & `TDCRPy-0.0.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 DESCRIPTION = "TDCR model"
 
+with open("README.md", "r") as f:
+    long_description = f.read()
+
 setup(
     name = "TDCRPy",
     version = VERSION,
     author = "RomainCoulon (Romain Coulon)",
     author_email = "<romain.coulon@bipm.org>",
     description = DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/RomainCoulon/TDCRPy",
     packages = find_packages(),
     install_requires = ["numpy","scipy","sys","time","urllib","zipfile","re"],
     keywords = ["python","TDCR","Monte-Carlo","radionuclide","scintillation","counting"],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Science/Research",
-		"License :: OSI Approved :: MIT License",
-		"Natural Language :: English",
-		"Natural Language :: French",
+	"License :: OSI Approved :: MIT License",
+	"Natural Language :: English",
+	"Natural Language :: French",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
-		"Topic :: Scientific/Engineering :: Physics",
+	"Topic :: Scientific/Engineering :: Physics",
     ]
 )
```

