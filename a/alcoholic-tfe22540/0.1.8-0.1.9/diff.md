# Comparing `tmp/alcoholic_tfe22540-0.1.8.tar.gz` & `tmp/alcoholic_tfe22540-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alcoholic_tfe22540-0.1.8.tar", last modified: Mon Jul 10 08:16:05 2023, max compression
+gzip compressed data, was "alcoholic_tfe22540-0.1.9.tar", last modified: Tue Jul 18 08:51:57 2023, max compression
```

## Comparing `alcoholic_tfe22540-0.1.8.tar` & `alcoholic_tfe22540-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 08:16:05.882727 alcoholic_tfe22540-0.1.8/
--rw-rw-rw-   0        0        0     8446 2023-07-10 08:16:05.882727 alcoholic_tfe22540-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     7946 2022-12-13 15:38:44.000000 alcoholic_tfe22540-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 08:16:05.637513 alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/
--rw-rw-rw-   0        0        0     8446 2023-07-10 08:16:05.000000 alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      995 2023-07-10 08:16:05.000000 alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 08:16:05.000000 alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-07-10 08:16:05.000000 alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 08:16:05.000000 alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 08:16:05.882727 alcoholic_tfe22540-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1320 2023-07-10 08:14:00.000000 alcoholic_tfe22540-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 08:16:05.882727 alcoholic_tfe22540-0.1.8/tfe22540/
--rw-rw-rw-   0        0        0     4578 2022-12-16 10:35:08.000000 alcoholic_tfe22540-0.1.8/tfe22540/CN2.py
--rw-rw-rw-   0        0        0     5893 2022-12-19 15:24:24.000000 alcoholic_tfe22540-0.1.8/tfe22540/Corpus_callosum_division.py
--rw-rw-rw-   0        0        0     3875 2022-12-19 15:26:00.000000 alcoholic_tfe22540-0.1.8/tfe22540/Corpus_callosum_reg.py
--rw-rw-rw-   0        0        0     4821 2022-12-19 15:26:12.000000 alcoholic_tfe22540-0.1.8/tfe22540/DMD_before_reg.py
--rw-rw-rw-   0        0        0     6185 2022-12-19 15:27:02.000000 alcoholic_tfe22540-0.1.8/tfe22540/DTI_kmeans_clustering.py
--rw-rw-rw-   0        0        0    15376 2022-12-19 15:27:10.000000 alcoholic_tfe22540-0.1.8/tfe22540/DTI_tissue_classification.py
--rw-rw-rw-   0        0        0     6009 2023-07-10 08:10:19.000000 alcoholic_tfe22540-0.1.8/tfe22540/FA_DMD.py
--rw-rw-rw-   0        0        0     1854 2022-11-17 08:44:54.000000 alcoholic_tfe22540-0.1.8/tfe22540/Stat_test.py
--rw-rw-rw-   0        0        0        0 2022-12-19 15:20:54.000000 alcoholic_tfe22540-0.1.8/tfe22540/__init__.py
--rw-rw-rw-   0        0        0    53993 2022-12-19 15:22:58.000000 alcoholic_tfe22540-0.1.8/tfe22540/analyse_ttest.py
--rw-rw-rw-   0        0        0     7194 2022-12-19 15:23:04.000000 alcoholic_tfe22540-0.1.8/tfe22540/atlas_modif_name.py
--rw-rw-rw-   0        0        0     2784 2022-12-19 15:23:12.000000 alcoholic_tfe22540-0.1.8/tfe22540/atlas_registration.py
--rw-rw-rw-   0        0        0    34689 2022-12-19 15:23:22.000000 alcoholic_tfe22540-0.1.8/tfe22540/clustering.py
--rw-rw-rw-   0        0        0    37380 2022-12-19 15:23:32.000000 alcoholic_tfe22540-0.1.8/tfe22540/clustering_v2.py
--rw-rw-rw-   0        0        0    10073 2022-12-19 15:24:18.000000 alcoholic_tfe22540-0.1.8/tfe22540/comportement.py
--rw-rw-rw-   0        0        0     9779 2022-12-19 15:26:16.000000 alcoholic_tfe22540-0.1.8/tfe22540/dMRI_metric_reg.py
--rw-rw-rw-   0        0        0     1925 2022-12-19 15:26:06.000000 alcoholic_tfe22540-0.1.8/tfe22540/diamond_fractions.py
--rw-rw-rw-   0        0        0     2510 2022-12-19 15:27:16.000000 alcoholic_tfe22540-0.1.8/tfe22540/f0_f1_to_ftot.py
--rw-rw-rw-   0        0        0     5939 2022-12-19 15:27:36.000000 alcoholic_tfe22540-0.1.8/tfe22540/job_submission.py
--rw-rw-rw-   0        0        0    10455 2022-12-19 15:28:02.000000 alcoholic_tfe22540-0.1.8/tfe22540/moyenne_ROI_v2.py
--rw-rw-rw-   0        0        0    25142 2022-12-19 15:01:40.000000 alcoholic_tfe22540-0.1.8/tfe22540/moyenne_par_ROI.py
--rw-rw-rw-   0        0        0     1494 2022-12-19 15:28:12.000000 alcoholic_tfe22540-0.1.8/tfe22540/opening_closing.py
--rw-rw-rw-   0        0        0     2165 2022-11-17 07:33:18.000000 alcoholic_tfe22540-0.1.8/tfe22540/perso_path.py
--rw-rw-rw-   0        0        0     8477 2022-12-19 15:28:24.000000 alcoholic_tfe22540-0.1.8/tfe22540/plot_functions.py
--rw-rw-rw-   0        0        0     2861 2022-12-13 13:03:24.000000 alcoholic_tfe22540-0.1.8/tfe22540/preprocessing.py
--rw-rw-rw-   0        0        0     6130 2022-11-16 21:19:56.000000 alcoholic_tfe22540-0.1.8/tfe22540/registration.py
--rw-rw-rw-   0        0        0    55481 2022-12-19 15:29:18.000000 alcoholic_tfe22540-0.1.8/tfe22540/ttest.py
--rw-rw-rw-   0        0        0     2684 2022-12-19 15:29:24.000000 alcoholic_tfe22540-0.1.8/tfe22540/useful_fct.py
--rw-rw-rw-   0        0        0     6060 2022-12-19 15:29:40.000000 alcoholic_tfe22540-0.1.8/tfe22540/volumes_zones.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:51:57.102690 alcoholic_tfe22540-0.1.9/
+-rw-rw-rw-   0        0        0     8446 2023-07-18 08:51:57.102690 alcoholic_tfe22540-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7946 2022-12-13 15:38:44.000000 alcoholic_tfe22540-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 08:51:57.079736 alcoholic_tfe22540-0.1.9/alcoholic_tfe22540.egg-info/
+-rw-rw-rw-   0        0        0     8446 2023-07-18 08:51:56.000000 alcoholic_tfe22540-0.1.9/alcoholic_tfe22540.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2023-07-18 08:51:56.000000 alcoholic_tfe22540-0.1.9/alcoholic_tfe22540.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 08:51:56.000000 alcoholic_tfe22540-0.1.9/alcoholic_tfe22540.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-07-18 08:51:56.000000 alcoholic_tfe22540-0.1.9/alcoholic_tfe22540.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 08:51:56.000000 alcoholic_tfe22540-0.1.9/alcoholic_tfe22540.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 08:51:57.102690 alcoholic_tfe22540-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1320 2023-07-18 08:37:07.000000 alcoholic_tfe22540-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:51:57.101688 alcoholic_tfe22540-0.1.9/tfe22540/
+-rw-rw-rw-   0        0        0     4578 2022-12-16 10:35:08.000000 alcoholic_tfe22540-0.1.9/tfe22540/CN2.py
+-rw-rw-rw-   0        0        0     5893 2022-12-19 15:24:24.000000 alcoholic_tfe22540-0.1.9/tfe22540/Corpus_callosum_division.py
+-rw-rw-rw-   0        0        0     3875 2022-12-19 15:26:00.000000 alcoholic_tfe22540-0.1.9/tfe22540/Corpus_callosum_reg.py
+-rw-rw-rw-   0        0        0     4821 2022-12-19 15:26:12.000000 alcoholic_tfe22540-0.1.9/tfe22540/DMD_before_reg.py
+-rw-rw-rw-   0        0        0     6185 2022-12-19 15:27:02.000000 alcoholic_tfe22540-0.1.9/tfe22540/DTI_kmeans_clustering.py
+-rw-rw-rw-   0        0        0    15376 2022-12-19 15:27:10.000000 alcoholic_tfe22540-0.1.9/tfe22540/DTI_tissue_classification.py
+-rw-rw-rw-   0        0        0     5850 2023-07-18 08:34:12.000000 alcoholic_tfe22540-0.1.9/tfe22540/FA_DMD.py
+-rw-rw-rw-   0        0        0     1854 2022-11-17 08:44:54.000000 alcoholic_tfe22540-0.1.9/tfe22540/Stat_test.py
+-rw-rw-rw-   0        0        0        0 2022-12-19 15:20:54.000000 alcoholic_tfe22540-0.1.9/tfe22540/__init__.py
+-rw-rw-rw-   0        0        0    53993 2022-12-19 15:22:58.000000 alcoholic_tfe22540-0.1.9/tfe22540/analyse_ttest.py
+-rw-rw-rw-   0        0        0     7194 2022-12-19 15:23:04.000000 alcoholic_tfe22540-0.1.9/tfe22540/atlas_modif_name.py
+-rw-rw-rw-   0        0        0     2784 2022-12-19 15:23:12.000000 alcoholic_tfe22540-0.1.9/tfe22540/atlas_registration.py
+-rw-rw-rw-   0        0        0    34689 2022-12-19 15:23:22.000000 alcoholic_tfe22540-0.1.9/tfe22540/clustering.py
+-rw-rw-rw-   0        0        0    37380 2022-12-19 15:23:32.000000 alcoholic_tfe22540-0.1.9/tfe22540/clustering_v2.py
+-rw-rw-rw-   0        0        0    10073 2022-12-19 15:24:18.000000 alcoholic_tfe22540-0.1.9/tfe22540/comportement.py
+-rw-rw-rw-   0        0        0     9779 2022-12-19 15:26:16.000000 alcoholic_tfe22540-0.1.9/tfe22540/dMRI_metric_reg.py
+-rw-rw-rw-   0        0        0     1925 2022-12-19 15:26:06.000000 alcoholic_tfe22540-0.1.9/tfe22540/diamond_fractions.py
+-rw-rw-rw-   0        0        0     2510 2022-12-19 15:27:16.000000 alcoholic_tfe22540-0.1.9/tfe22540/f0_f1_to_ftot.py
+-rw-rw-rw-   0        0        0     5939 2022-12-19 15:27:36.000000 alcoholic_tfe22540-0.1.9/tfe22540/job_submission.py
+-rw-rw-rw-   0        0        0    10455 2022-12-19 15:28:02.000000 alcoholic_tfe22540-0.1.9/tfe22540/moyenne_ROI_v2.py
+-rw-rw-rw-   0        0        0    25142 2022-12-19 15:01:40.000000 alcoholic_tfe22540-0.1.9/tfe22540/moyenne_par_ROI.py
+-rw-rw-rw-   0        0        0     1494 2022-12-19 15:28:12.000000 alcoholic_tfe22540-0.1.9/tfe22540/opening_closing.py
+-rw-rw-rw-   0        0        0     2165 2022-11-17 07:33:18.000000 alcoholic_tfe22540-0.1.9/tfe22540/perso_path.py
+-rw-rw-rw-   0        0        0     8477 2022-12-19 15:28:24.000000 alcoholic_tfe22540-0.1.9/tfe22540/plot_functions.py
+-rw-rw-rw-   0        0        0     2861 2022-12-13 13:03:24.000000 alcoholic_tfe22540-0.1.9/tfe22540/preprocessing.py
+-rw-rw-rw-   0        0        0     6130 2022-11-16 21:19:56.000000 alcoholic_tfe22540-0.1.9/tfe22540/registration.py
+-rw-rw-rw-   0        0        0    55481 2022-12-19 15:29:18.000000 alcoholic_tfe22540-0.1.9/tfe22540/ttest.py
+-rw-rw-rw-   0        0        0     2684 2022-12-19 15:29:24.000000 alcoholic_tfe22540-0.1.9/tfe22540/useful_fct.py
+-rw-rw-rw-   0        0        0     6060 2022-12-19 15:29:40.000000 alcoholic_tfe22540-0.1.9/tfe22540/volumes_zones.py
```

### Comparing `alcoholic_tfe22540-0.1.8/PKG-INFO` & `alcoholic_tfe22540-0.1.9/alcoholic_tfe22540.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alcoholic_tfe22540
-Version: 0.1.8
+Name: alcoholic-tfe22540
+Version: 0.1.9
 Summary: Framework of my master thesis on the effect of withdrawal on the white matter of alcoholic patients using dMRI data.
 Home-page: https://github.com/mdausort/TFE22-540
 Author: Manon Dausort
 Author-email: manon.dausort@uclouvain.be
 License: BSD 2-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `alcoholic_tfe22540-0.1.8/README.md` & `alcoholic_tfe22540-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/PKG-INFO` & `alcoholic_tfe22540-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alcoholic-tfe22540
-Version: 0.1.8
+Name: alcoholic_tfe22540
+Version: 0.1.9
 Summary: Framework of my master thesis on the effect of withdrawal on the white matter of alcoholic patients using dMRI data.
 Home-page: https://github.com/mdausort/TFE22-540
 Author: Manon Dausort
 Author-email: manon.dausort@uclouvain.be
 License: BSD 2-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `alcoholic_tfe22540-0.1.8/alcoholic_tfe22540.egg-info/SOURCES.txt` & `alcoholic_tfe22540-0.1.9/alcoholic_tfe22540.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/setup.py` & `alcoholic_tfe22540-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='alcoholic_tfe22540',
-    version='0.1.8',
+    version='0.1.9',
     description='Framework of my master thesis on the effect of withdrawal on the white matter of alcoholic patients using dMRI data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mdausort/TFE22-540',
     author='Manon Dausort',
     author_email='manon.dausort@uclouvain.be',
     license='BSD 2-clause',
```

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/CN2.py` & `alcoholic_tfe22540-0.1.9/tfe22540/CN2.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/Corpus_callosum_division.py` & `alcoholic_tfe22540-0.1.9/tfe22540/Corpus_callosum_division.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/Corpus_callosum_reg.py` & `alcoholic_tfe22540-0.1.9/tfe22540/Corpus_callosum_reg.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/DMD_before_reg.py` & `alcoholic_tfe22540-0.1.9/tfe22540/DMD_before_reg.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/DTI_kmeans_clustering.py` & `alcoholic_tfe22540-0.1.9/tfe22540/DTI_kmeans_clustering.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/DTI_tissue_classification.py` & `alcoholic_tfe22540-0.1.9/tfe22540/DTI_tissue_classification.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/FA_DMD.py` & `alcoholic_tfe22540-0.1.9/tfe22540/FA_DMD.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,111 +10,106 @@
 from tfe22540.perso_path import perso_path_string
 
 
 perso_path, excel_path, subjects_path, patients_path, plot_path, atlas_path = perso_path_string()
 
 
 def get_FA_DIAMOND(folder_path, patient_path):
-
     """
         Parameters
         ----------
         folder_path : String 
             Link of the file in which we are. 
         patient_path : List of strings
             Number of all patients in string ["sub#_E1"] for example.
-    
+
         Returns
         -------
         None. But creation of files containing the cFA, cMD, cAD and cRD for each patient. "c" stands for compartment.
     """
-    
-    tenseur_list = ["t0", "t1"]       
-    
+
+    tenseur_list = ["t0", "t1"]
+
     for tenseur in tenseur_list:
-        
+
         path = folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/dti/" + patient_path + "_FA.nii.gz"
-        
+
         comp = folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_diamond_" + tenseur + ".nii.gz"
         comp = nib.load(comp).get_fdata()
-       
-        MD = np.zeros((comp.shape[0],comp.shape[1],comp.shape[2]))
-        AD = np.zeros((comp.shape[0],comp.shape[1],comp.shape[2]))
-        RD = np.zeros((comp.shape[0],comp.shape[1],comp.shape[2]))
-        FA = np.zeros((comp.shape[0],comp.shape[1],comp.shape[2]))
-        
-        
-        D = np.array([[np.squeeze(comp[:,:,:,:,0]), np.squeeze(comp[:,:,:,:,1]), np.squeeze(comp[:,:,:,:,3])],
-                      [np.squeeze(comp[:,:,:,:,1]), np.squeeze(comp[:,:,:,:,2]), np.squeeze(comp[:,:,:,:,4])],
-                      [np.squeeze(comp[:,:,:,:,3]), np.squeeze(comp[:,:,:,:,4]), np.squeeze(comp[:,:,:,:,5])]])
-        
+
+        MD = np.zeros((comp.shape[0], comp.shape[1], comp.shape[2]))
+        AD = np.zeros((comp.shape[0], comp.shape[1], comp.shape[2]))
+        RD = np.zeros((comp.shape[0], comp.shape[1], comp.shape[2]))
+        FA = np.zeros((comp.shape[0], comp.shape[1], comp.shape[2]))
+
+        D = np.array([[np.squeeze(comp[:, :, :, :, 0]), np.squeeze(comp[:, :, :, :, 1]), np.squeeze(comp[:, :, :, :, 3])],
+                      [np.squeeze(comp[:, :, :, :, 1]), np.squeeze(comp[:, :, :, :, 2]), np.squeeze(comp[:, :, :, :, 4])],
+                      [np.squeeze(comp[:, :, :, :, 3]), np.squeeze(comp[:, :, :, :, 4]), np.squeeze(comp[:, :, :, :, 5])]])
 
         for i in range(comp.shape[0]):
             for j in range(comp.shape[1]):
                 for k in range(comp.shape[2]):
-                    
-                    valeurs_propres = np.array(np.linalg.eigvals(D[:,:,i,j,k]))
+
+                    valeurs_propres = np.array(np.linalg.eigvals(D[:, :, i, j, k]))
                     max_valeur = max(np.abs(valeurs_propres))
-                    index_lambda = [l for l in range(len(valeurs_propres)) if abs(valeurs_propres[l])==max_valeur]
-        
+                    index_lambda = [l for l in range(len(valeurs_propres)) if abs(valeurs_propres[l]) == max_valeur]
+
                     copy_valeurs_propres = np.copy(valeurs_propres)
                     copy_valeurs_propres = np.delete(copy_valeurs_propres, index_lambda[0])
                     copy_valeurs_propres = np.array(copy_valeurs_propres)
-                    
-                    MD[i,j,k] = (valeurs_propres[0] + valeurs_propres[1] + valeurs_propres[2])/3
-                    AD[i,j,k] = valeurs_propres[index_lambda[0]]
-                    RD[i,j,k] = (copy_valeurs_propres[0]+copy_valeurs_propres[1])/2
-                    
+
+                    MD[i, j, k] = (valeurs_propres[0] + valeurs_propres[1] + valeurs_propres[2]) / 3
+                    AD[i, j, k] = valeurs_propres[index_lambda[0]]
+                    RD[i, j, k] = (copy_valeurs_propres[0] + copy_valeurs_propres[1]) / 2
+
                     if((valeurs_propres[0]**2 + valeurs_propres[1]**2 + valeurs_propres[2]**2) == 0):
-                        FA[i,j,k] = 0
+                        FA[i, j, k] = 0
                     else:
-                        FA[i,j,k] = np.sqrt(3/2)*np.sqrt(((valeurs_propres[0] - MD[i,j,k])**2 + (valeurs_propres[1] - MD[i,j,k])**2 + (valeurs_propres[2] - MD[i,j,k])**2)/(valeurs_propres[0]**2 + valeurs_propres[1]**2 + valeurs_propres[2]**2))
-                    
+                        FA[i, j, k] = np.sqrt(3 / 2) * np.sqrt(((valeurs_propres[0] - MD[i, j, k])**2 + (valeurs_propres[1] - MD[i, j, k])**2 + (valeurs_propres[2] - MD[i, j, k])**2) / (valeurs_propres[0]**2 + valeurs_propres[1]**2 + valeurs_propres[2]**2))
+
         MD[np.isnan(MD)] = 0
-        out = nib.Nifti1Image(MD, affine = nib.load(path).affine, header = nib.load(path).header)
+        print(MD.shape)
+        out = nib.Nifti1Image(MD, affine=nib.load(path).affine, header=nib.load(path).header)
         out.to_filename(folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_MD_DMD_" + tenseur + ".nii.gz")
 
         AD[np.isnan(AD)] = 0
-        out1 = nib.Nifti1Image(AD, affine = nib.load(path).affine, header = nib.load(path).header)
+        out1 = nib.Nifti1Image(AD, affine=nib.load(path).affine, header=nib.load(path).header)
         out1.to_filename(folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_AD_DMD_" + tenseur + ".nii.gz")
 
         RD[np.isnan(RD)] = 0
-        out2 = nib.Nifti1Image(RD, affine = nib.load(path).affine, header = nib.load(path).header)
+        out2 = nib.Nifti1Image(RD, affine=nib.load(path).affine, header=nib.load(path).header)
         out2.to_filename(folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_RD_DMD_" + tenseur + ".nii.gz")
 
         FA[np.isnan(FA)] = 0
-        out3 = nib.Nifti1Image(FA, affine = nib.load(path).affine, header = nib.load(path).header)
+        out3 = nib.Nifti1Image(FA, affine=nib.load(path).affine, header=nib.load(path).header)
         out3.to_filename(folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_FA_DMD_" + tenseur + ".nii.gz")
-        
-       
 
-def get_cMetrics(folder_path, patient_path):
 
+def get_cMetrics(folder_path, patient_path):
     """
         Parameters
         ----------
         folder_path : String 
             Link of the file in which we are. 
         patient_path : List of strings
             Number of all patients in string ["sub#_E1"] for example.
-    
+
         Returns
         -------
         None. But creation of files containing the wFA, wMD, wAD and wRD for each patient. "w" stands for weigthed.
     """
 
-    metrics = ["FA","MD","AD","RD"]
-    
-    for metric in metrics :    
-        metric_t0   = folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_" + metric + "_DMD_t0.nii.gz"
-        
-        metric_t1   = folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_" + metric + "_DMD_t1.nii.gz"
-         
+    metrics = ["FA", "MD", "AD", "RD"]
+
+    for metric in metrics:
+        metric_t0 = folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_" + metric + "_DMD_t0.nii.gz"
+
+        metric_t1 = folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_" + metric + "_DMD_t1.nii.gz"
+
         fraction_t0 = folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_diamond_fractions_f0.nii.gz"
-        
+
         fraction_t1 = folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_diamond_fractions_f1.nii.gz"
-        
-        
-        cMetric = (nib.load(metric_t0).get_fdata() * nib.load(fraction_t0).get_fdata() + nib.load(metric_t1).get_fdata() * nib.load(fraction_t1).get_fdata())/(nib.load(fraction_t1).get_fdata() + nib.load(fraction_t0).get_fdata())
-        
-        out = nib.Nifti1Image(cMetric, affine = nib.load(metric_t0).affine, header = nib.load(metric_t0).header)
+
+        cMetric = (nib.load(metric_t0).get_fdata() * nib.load(fraction_t0).get_fdata() + nib.load(metric_t1).get_fdata() * nib.load(fraction_t1).get_fdata()) / (nib.load(fraction_t1).get_fdata() + nib.load(fraction_t0).get_fdata())
+
+        out = nib.Nifti1Image(cMetric, affine=nib.load(metric_t0).affine, header=nib.load(metric_t0).header)
         out.to_filename(folder_path + "/subjects/" + patient_path + "/dMRI/microstructure/diamond/" + patient_path + "_w" + metric + ".nii.gz")
```

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/Stat_test.py` & `alcoholic_tfe22540-0.1.9/tfe22540/Stat_test.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/analyse_ttest.py` & `alcoholic_tfe22540-0.1.9/tfe22540/analyse_ttest.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/atlas_modif_name.py` & `alcoholic_tfe22540-0.1.9/tfe22540/atlas_modif_name.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/atlas_registration.py` & `alcoholic_tfe22540-0.1.9/tfe22540/atlas_registration.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/clustering.py` & `alcoholic_tfe22540-0.1.9/tfe22540/clustering.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/clustering_v2.py` & `alcoholic_tfe22540-0.1.9/tfe22540/clustering_v2.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/comportement.py` & `alcoholic_tfe22540-0.1.9/tfe22540/comportement.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/dMRI_metric_reg.py` & `alcoholic_tfe22540-0.1.9/tfe22540/dMRI_metric_reg.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/diamond_fractions.py` & `alcoholic_tfe22540-0.1.9/tfe22540/diamond_fractions.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/f0_f1_to_ftot.py` & `alcoholic_tfe22540-0.1.9/tfe22540/f0_f1_to_ftot.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/job_submission.py` & `alcoholic_tfe22540-0.1.9/tfe22540/job_submission.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/moyenne_ROI_v2.py` & `alcoholic_tfe22540-0.1.9/tfe22540/moyenne_ROI_v2.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/moyenne_par_ROI.py` & `alcoholic_tfe22540-0.1.9/tfe22540/moyenne_par_ROI.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/opening_closing.py` & `alcoholic_tfe22540-0.1.9/tfe22540/opening_closing.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/perso_path.py` & `alcoholic_tfe22540-0.1.9/tfe22540/perso_path.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/plot_functions.py` & `alcoholic_tfe22540-0.1.9/tfe22540/plot_functions.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/preprocessing.py` & `alcoholic_tfe22540-0.1.9/tfe22540/preprocessing.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/registration.py` & `alcoholic_tfe22540-0.1.9/tfe22540/registration.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/ttest.py` & `alcoholic_tfe22540-0.1.9/tfe22540/ttest.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/useful_fct.py` & `alcoholic_tfe22540-0.1.9/tfe22540/useful_fct.py`

 * *Files identical despite different names*

### Comparing `alcoholic_tfe22540-0.1.8/tfe22540/volumes_zones.py` & `alcoholic_tfe22540-0.1.9/tfe22540/volumes_zones.py`

 * *Files identical despite different names*

