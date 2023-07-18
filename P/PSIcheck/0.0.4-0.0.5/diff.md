# Comparing `tmp/PSIcheck-0.0.4.tar.gz` & `tmp/PSIcheck-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PSIcheck-0.0.4.tar", last modified: Sun Sep 25 10:42:59 2022, max compression
+gzip compressed data, was "PSIcheck-0.0.5.tar", last modified: Tue Jul 18 06:29:13 2023, max compression
```

## Comparing `PSIcheck-0.0.4.tar` & `PSIcheck-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2022-09-25 10:42:59.501882 PSIcheck-0.0.4/
--rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2022-09-25 10:42:59.498884 PSIcheck-0.0.4/PKG-INFO
-drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2022-09-25 10:42:59.375671 PSIcheck-0.0.4/PSIcheck/
--rwxrwxrwx   0 edith     (1000) edith     (1000)      477 2022-09-23 05:47:23.000000 PSIcheck-0.0.4/PSIcheck/__init__.py
--rwxrwxrwx   0 edith     (1000) edith     (1000)      517 2022-09-25 10:42:19.000000 PSIcheck-0.0.4/PSIcheck/get_parser.py
--rwxrwxrwx   0 edith     (1000) edith     (1000)     8264 2022-09-25 10:41:04.000000 PSIcheck-0.0.4/PSIcheck/screen_for_magPro.py
-drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2022-09-25 10:42:59.479884 PSIcheck-0.0.4/PSIcheck.egg-info/
--rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2022-09-25 10:42:59.000000 PSIcheck-0.0.4/PSIcheck.egg-info/PKG-INFO
--rwxrwxrwx   0 edith     (1000) edith     (1000)      276 2022-09-25 10:42:59.000000 PSIcheck-0.0.4/PSIcheck.egg-info/SOURCES.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)        1 2022-09-25 10:42:59.000000 PSIcheck-0.0.4/PSIcheck.egg-info/dependency_links.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)       43 2022-09-25 10:42:59.000000 PSIcheck-0.0.4/PSIcheck.egg-info/entry_points.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)       21 2022-09-25 10:42:59.000000 PSIcheck-0.0.4/PSIcheck.egg-info/requires.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)        9 2022-09-25 10:42:59.000000 PSIcheck-0.0.4/PSIcheck.egg-info/top_level.txt
--rwxrwxrwx   0 edith     (1000) edith     (1000)       38 2022-09-25 10:42:59.501882 PSIcheck-0.0.4/setup.cfg
--rwxrwxrwx   0 edith     (1000) edith     (1000)     1028 2022-09-25 10:42:12.000000 PSIcheck-0.0.4/setup.py
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 06:29:13.202091 PSIcheck-0.0.5/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-18 06:29:13.194135 PSIcheck-0.0.5/PKG-INFO
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 06:29:12.845990 PSIcheck-0.0.5/PSIcheck/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      477 2022-09-23 05:47:24.000000 PSIcheck-0.0.5/PSIcheck/__init__.py
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      517 2023-07-18 06:28:21.000000 PSIcheck-0.0.5/PSIcheck/get_parser.py
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     9040 2022-11-29 13:40:30.000000 PSIcheck-0.0.5/PSIcheck/screen_for_magPro.py
+drwxrwxrwx   0 edith     (1000) edith     (1000)        0 2023-07-18 06:29:13.143126 PSIcheck-0.0.5/PSIcheck.egg-info/
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      419 2023-07-18 06:29:12.000000 PSIcheck-0.0.5/PSIcheck.egg-info/PKG-INFO
+-rwxrwxrwx   0 edith     (1000) edith     (1000)      276 2023-07-18 06:29:12.000000 PSIcheck-0.0.5/PSIcheck.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)        1 2023-07-18 06:29:12.000000 PSIcheck-0.0.5/PSIcheck.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       43 2023-07-18 06:29:12.000000 PSIcheck-0.0.5/PSIcheck.egg-info/entry_points.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       21 2023-07-18 06:29:12.000000 PSIcheck-0.0.5/PSIcheck.egg-info/requires.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)        9 2023-07-18 06:29:12.000000 PSIcheck-0.0.5/PSIcheck.egg-info/top_level.txt
+-rwxrwxrwx   0 edith     (1000) edith     (1000)       38 2023-07-18 06:29:13.203132 PSIcheck-0.0.5/setup.cfg
+-rwxrwxrwx   0 edith     (1000) edith     (1000)     1028 2023-07-18 06:28:09.000000 PSIcheck-0.0.5/setup.py
```

### Comparing `PSIcheck-0.0.4/PSIcheck/get_parser.py` & `PSIcheck-0.0.5/PSIcheck/get_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 def get_parser():
     import argparse
     
     parser = argparse.ArgumentParser(
              prog="PSIcheck", 
             )
-    parser.add_argument('-v', '--version', action='version', version='%(prog)s 0.0.4', help='show PSIcheck version number and exit')
+    parser.add_argument('-v', '--version', action='version', version='%(prog)s 0.0.5', help='show PSIcheck version number and exit')
     parser.add_argument('PsiResultPath', type=str, help='directory stores PSI-Blast results')
     parser.add_argument('-gbk','--GenbankFilesPath', type=str, help='directory stores Genbank files')
 
     args = parser.parse_args()
     return args
```

### Comparing `PSIcheck-0.0.4/PSIcheck/screen_for_magPro.py` & `PSIcheck-0.0.5/PSIcheck/screen_for_magPro.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,68 +26,90 @@
                     list_.append(line)
 
     list_.append('blank line')
 
     genome_name = os.path.basename(psiblasted_txt).replace('.txt','')
     mgc_dict = {}
     idlist=[]
+    gnamelist=[]
     namelist=[]
+    fullname=[]
     acclist=[]
     evallist=[]
     namelist_tmp = []
+    fullname_tmp = []
     acclist_tmp = []
     evallist_tmp = []
     for i in range(len(list_)-1):
         if 'Query=' in list_[i]:
             if ('Query=' not in list_[i+1]) & ('blank' not in list_[i+1]):
                 id = re.search('LOCUSTAG_[0-9]+', list_[i]).group()
                 idlist.append(id)
+                gname = list_[i].replace('Query=','').split('_LOCUSTAG')[0]
+                gnamelist.append(gname)
                 if namelist_tmp:
                     namelist.append(namelist_tmp)
                 if acclist_tmp:
                     acclist.append(acclist_tmp)
                 if evallist_tmp:
                     evallist.append(evallist_tmp)
+                if fullname_tmp:
+                    fullname.append(fullname_tmp)
                 namelist_tmp = []
                 acclist_tmp = []
-                evallist_tmp = [] 
+                evallist_tmp = []
+                fullname_tmp = [] 
         elif pattern4.match(list_[i]) and pattern5.search(list_[i]):
             list_tmp = [i for i in list_[i].split(' ') if i.strip()]
             name_tmp = ' '.join(list_tmp[1:-2])
             p1 = pattern1.search(name_tmp)
             p3 = pattern3.search(name_tmp)
             p2 = pattern2.search(name_tmp)
             if p1:
                 name = p1.group()
             elif p3:
                 name = p3.group()
             elif p2:
                 name = name_tmp
             namelist_tmp.append(name)
+            fullname_tmp.append(name_tmp)
             acclist_tmp.append(list_tmp[0])
             evallist_tmp.append(pattern5.search(list_[i]).group().strip())
+        else:
+            namelist_tmp.append('NaN')
+            fullname_tmp.append('NaN')
+            acclist_tmp.append('NaN')
+            evallist_tmp.append('NaN')
     if namelist_tmp:
         namelist.append(namelist_tmp)
+    if fullname_tmp:
+        fullname.append(fullname_tmp)     
     if acclist_tmp:
         acclist.append(acclist_tmp)
     if evallist_tmp:
         evallist.append(evallist_tmp)     
     mgc_dict = {'genomes': genome_name,
                 'locustag' : idlist,
+                'gname' : gnamelist,
                'pro_name': namelist,
+               'fullname': fullname,
                'accession': acclist,
                'e-value': evallist} 
+
     return mgc_dict
 
+
 def get_all_putative_mgc_csv(list_psiblasted_txts):
     df_list = []
     for txt in list_psiblasted_txts:
-        df_tmp = pd.DataFrame.from_dict(check_putative_mgc_id_acc(txt)).explode(['pro_name','accession', 'e-value'])
+        mgc_dict = check_putative_mgc_id_acc(txt)
+        df_tmp = pd.DataFrame.from_dict(mgc_dict).explode(['pro_name','fullname','accession', 'e-value'])
         df_list.append(df_tmp)
     df_all = pd.concat(df_list)
+    # df_all.to_csv('dfall.csv')
     return df_all
 
 def get_identity_value(df_all, list_psiblasted_txts):
     identities = {
         'genomes':[],
         'locustag':[],
         'accession':[],
@@ -127,18 +149,19 @@
 
     df_iden = pd.DataFrame(identities)
     return df_iden
 
 def concat_df_all_iden(df_all, df_iden):
     df_all.set_index(['genomes','locustag','accession'],inplace = True)
     df_iden.set_index(['genomes','locustag','accession'], inplace=True)
-    if not (df_all.index == df_iden.index).all():
-        raise ValueError('The identitiy dataframe seems to have a different index with all_dataframe')
+    # if not (df_all.index == df_iden.index).all():
+    #     raise ValueError('The identitiy dataframe seems to have a different index with all_dataframe')
     df_all['identity'] = df_iden.identity
     df_all.reset_index(inplace=True)
+    df_all.to_csv('df_all.csv')
     return df_all
 
 def use_eval_iden_criteria(df_all):
     # first screen by iden>=0.3 and eval <0.001
     df_all['eval_float'] = df_all['e-value'].apply(float)
     def p2f(x):
         if type(x) == str:
@@ -153,14 +176,15 @@
     df_meet_criteria.sort_values(['genomes', 'locustag', 'iden_float','eval_float'], ascending=[True, True, False, True], inplace=True)
     df_meet_criteria.drop_duplicates(subset=['genomes', 'locustag'], inplace=True)
     return df_meet_criteria
            
 def get_file_path(psi_res_path):
     list_psiblasted_txts = glob.glob(f'{psi_res_path}/*.txt')
     return list_psiblasted_txts
+    
 
 def check_and_reform(psi_res_path):
     list_psiblasted_txts = get_file_path(psi_res_path)
     num_of_files = len(list_psiblasted_txts)
     df_all_tmp = get_all_putative_mgc_csv(list_psiblasted_txts)
     df_iden = get_identity_value(df_all_tmp, list_psiblasted_txts)
     df_all = concat_df_all_iden(df_all_tmp, df_iden)
```

### Comparing `PSIcheck-0.0.4/setup.py` & `PSIcheck-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PSIcheck',
-    version='0.0.4',
+    version='0.0.5',
     description="check PSI-Blast result",
     author='Runjia Ji',
     author_email='jirunjia@gmail.com',
     # py_modules=["magcluster", 'args', 'capture_args', 'maga', 'magm', 'magsc', 'main'],
     # package_dir={'': 'src'},
     packages=find_packages(),
     classifiers=[
```

