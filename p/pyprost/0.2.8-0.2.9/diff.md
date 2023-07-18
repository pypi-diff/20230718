# Comparing `tmp/pyprost-0.2.8.tar.gz` & `tmp/pyprost-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprost-0.2.8.tar", last modified: Fri Apr 21 01:00:50 2023, max compression
+gzip compressed data, was "pyprost-0.2.9.tar", last modified: Sat Apr 22 19:16:57 2023, max compression
```

## Comparing `pyprost-0.2.8.tar` & `pyprost-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:00:50.828802 pyprost-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-21 00:58:38.000000 pyprost-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-21 01:00:50.828802 pyprost-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-21 00:58:38.000000 pyprost-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:00:50.828802 pyprost-0.2.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15023 2023-04-21 00:58:38.000000 pyprost-0.2.8/bin/prost
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-21 00:58:38.000000 pyprost-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-21 01:00:50.832803 pyprost-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:00:50.828802 pyprost-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:00:50.828802 pyprost-0.2.8/src/pyprost/
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-21 00:58:38.000000 pyprost-0.2.8/src/pyprost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-21 00:58:38.000000 pyprost-0.2.8/src/pyprost/esmts25_13.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-21 00:58:38.000000 pyprost-0.2.8/src/pyprost/prosttools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 01:00:50.828802 pyprost-0.2.8/src/pyprost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-21 01:00:50.000000 pyprost-0.2.8/src/pyprost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-21 01:00:50.000000 pyprost-0.2.8/src/pyprost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 01:00:50.000000 pyprost-0.2.8/src/pyprost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 01:00:50.000000 pyprost-0.2.8/src/pyprost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 01:00:50.000000 pyprost-0.2.8/src/pyprost.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:16:57.332708 pyprost-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-22 19:14:26.000000 pyprost-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-22 19:16:57.332708 pyprost-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-22 19:14:26.000000 pyprost-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:16:57.328709 pyprost-0.2.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22563 2023-04-22 19:14:26.000000 pyprost-0.2.9/bin/prost
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-22 19:14:26.000000 pyprost-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-22 19:16:57.332708 pyprost-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:16:57.324708 pyprost-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:16:57.328709 pyprost-0.2.9/src/pyprost/
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-04-22 19:14:26.000000 pyprost-0.2.9/src/pyprost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-22 19:14:26.000000 pyprost-0.2.9/src/pyprost/esmts25_13.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-22 19:14:26.000000 pyprost-0.2.9/src/pyprost/prosttools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:16:57.332708 pyprost-0.2.9/src/pyprost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-22 19:16:57.000000 pyprost-0.2.9/src/pyprost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-22 19:16:57.000000 pyprost-0.2.9/src/pyprost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:16:57.000000 pyprost-0.2.9/src/pyprost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-22 19:16:57.000000 pyprost-0.2.9/src/pyprost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 19:16:57.000000 pyprost-0.2.9/src/pyprost.egg-info/top_level.txt
```

### Comparing `pyprost-0.2.8/LICENSE` & `pyprost-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprost-0.2.8/PKG-INFO` & `pyprost-0.2.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pyprost
-Version: 0.2.8
-Summary: PRotein Ortholog Search Tool
-Home-page: https://github.com/mesihk/prost
-Author: Mesih Kilinc
-Author-email: mesih@iastate.edu
-Project-URL: Bug Tracker, https://github.com/mesihk/prost/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## PROST python package v0.2.8
 
 PRotein Ortholog Search Tool is a new homolog detection tool that utilizes ESM-1b language model and iDCT quantization method.
 PROST is fast and accurate compared to traditional tools. 
 
 ### Installation
 
@@ -26,25 +11,34 @@
 ```
 On the initial run, PROST will download required files to `~/.config/prost` or an user defined directory via `PROSTDIR` environment variable.
 
 ### How to use
 
 Following commands can be used to create databases and perform homology search.
 
-* makedb: creates a PROST database from given fasta file. The fasta file usually contains more than one entry.
-* search: searches a query database agains a target database. Query database can contain one or more sequences embedded using makedb command. `--thr` can be used to specify an e-value threshold. The default threshold is 0.05.
-* searchsp: searches a query database agains a SwissProt February 2023 database. Performs GO enrichment analysis on found homologs. Query database can contain one or more sequences embedded using makedb command. Again `--thr` can be used to specify an e-value threshold.  `--gothr` can be used to specifiy different e-value threshold for GO enrichment analysis.
-
 ```
 prost makedb db/sp.fa db/sp.prdb
 prost makedb db/covid.fa db/covid.prdb
-prost search --thr 0.05 db/covid.prdb db/sp.prdb results.tsv
-prost searchsp --thr 0.05 db/covid.prdb results.tsv
+prost search --thr 0.05 db/covid.prdb db/sp.prdb results
+prost searchsp --thr 0.05 db/covid.prdb results
 ```
 
+* `makedb`: creates a PROST database from given fasta file. The fasta file usually contains more than one entry.
+* `search`: searches a query database agains a target database. Query database can contain one or more sequences embedded using makedb command. `--thr` can be used to specify an e-value threshold. The default threshold is 0.05.
+* `searchsp`: searches a query database agains a SwissProt February 2023 database. Performs GO enrichment analysis on found homologs. Query database can contain one or more sequences embedded using makedb command. Again `--thr` can be used to specify an e-value threshold.  `--gothr` can be used to specifiy different e-value threshold for GO enrichment analysis. 
+`searchsp` produces a tab seprataed file `.tsv` and a JSON file `.json` that can be used with the tool [JSONWP](https://jsonwp.onrender.com/). 
+Here is an example result:
+![jsonwp1](asset/jsonwp1.png)
+![jsonwp2](asset/jsonwp2.png)
+Sequence alignment done automatically using the [PROTSUB](https://onlinelibrary.wiley.com/doi/full/10.1002/prot.26050) matrix which is better for aligning remote proteins then BLOSUM62 matrix. 
+Protein structures are fetched from the Alphafold 2 database. No alignment produced this time.
+![jsonwp3](asset/jsonwp3.png)
+
+
+
 ### Scripting
 
 ```
 import pyprost
 
 hpo30 = '''MPLIMYKFLLVTSIFLIVSGLILTAFSLFSPLWEVVDFPRSHLSHHHGLWWDCIVHHET
 LIPLHEDQAELRGDRCDSKMDSSVQASLRVALEKGDEEARELLLHRFLPHHKGVIFFAVF
@@ -70,7 +64,8 @@
 ### Resources
 
 * Yeast analysis: https://mesihk.github.io/prostyeast
 * Unannotated Human Proteins Analysis: https://mesihk.github.io/prosthuman
 * Webserver: https://mesihk.github.io/prost 
 * PROST Python package: https://github.com/MesihK/prost
 * PROST Research Data: https://github.com/MesihK/prost-data 
+* JSONWP: https://jsonwp.onrender.com/
```

### Comparing `pyprost-0.2.8/bin/prost` & `pyprost-0.2.9/bin/prost`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import numpy as np
 import scipy.stats as st
 from pickle import load,loads,dump,dumps
 import click
 import blosc
 from statsmodels.stats.multitest import multipletests 
 import re
+from datetime import datetime
+import json
 
 import os
 from pathlib import Path
 if 'PROSTDIR' in os.environ: prostdir = os.environ['PROSTDIR']
 else: prostdir = str(Path.home())+'/.config/prost'
 
 from itertools import groupby
@@ -321,28 +323,30 @@
         f.write(blosc.compress(dumps([np.array(names),np.array(quant)])))
 
     if not no_cache:
         if cacheDirty:
             with open(prostdir+'/cache.pkl','wb') as f:
                 dump(cache,f)
 
-def _search(thr, gothr, querydb, targetdb, godb, out):
+def _search(thr, gothr, querydb, targetdb, godb):
     if godb != None:
         with open(godb,'rb') as f:
             go,goFrq,goDesc = load(f)
     with open(querydb,'rb') as f:
         qnames,qdb = loads(blosc.decompress(f.read()))
     with open(targetdb,'rb') as f:
         tnames,tdb = loads(blosc.decompress(f.read()))
     ldb = len(tdb)
-    output = []
+    homologList, goList = {},{}
 
     mem = np.zeros((ldb,475),dtype='int8')
     for i,q in enumerate(qdb):
         qname = parseName(qnames[i])[0]
+        goList[qname] = []
+        homologList[qname] = []
         print(f'Searching for {qname}')
         np.subtract(tdb,q,out=mem)
         np.absolute(mem,out=mem)
         dbdiff = mem.sum(axis=1)
         m=np.median(dbdiff)
         s=st.median_abs_deviation(dbdiff)*1.4826
         zscore = (dbdiff-m)/s
@@ -350,60 +354,146 @@
         res = np.where(e < thr)[0]
         sort = np.argsort(e[res])
         res = res[sort]
         dbdiff = dbdiff[res]/2
         evals = e[res]
         names = tnames[res]
         
-        
         if godb != None:
             res2 = np.where(e < gothr)[0]
             sort2 = np.argsort(e[res2])
             res2 = res2[sort2]
             for a in annotate(res2,e[res2],go,goFrq,goDesc):
-                output.append(f'{qname}\t{a[0]}\t{a[1]}\t{a[2]:.3f}\t{parseName(tnames[a[3]])[0]}\t{a[5]}\t{a[4]:.2e}')
+                goList[qname].append([a[0], a[1], f'{a[2]:.3f}', parseName(tnames[a[3]])[0], a[5], f'{a[4]:.2e}'])
                 
         for n,diff,ev in zip(names,dbdiff,evals):
             n = parseName(n)
-            output.append(f'{qname}\t{n[0]}\t{n[1]}\t{n[2]}\t{n[3]}\t{diff}\t{ev:.2e}')
+            homologList[qname].append([n[0], n[1], n[2], n[3], diff, f'{ev:.2e}'])
 
-    with open(out,'w') as f:
-        for o in output:
-            f.write(o+'\n')
+    return goList,homologList
+    
+def toTSV(goList,homologList,out):
+    with open(out+'.tsv','w') as f:
+        for queryP in homologList:
+            for go in goList[queryP]:
+                f.write(f'{queryP}\t'+'\t'.join([str(i) for i in go])+'\n')
+            for hom in homologList[queryP]:
+                f.write(f'{queryP}\t'+'\t'.join([str(i) for i in hom])+'\n')
+
+def createAlignmentPage(p1,p2):
+    return {
+        "h2:caption":f"{p1} & {p2} Alignment",
+        "md:info":f"Alignment of [{p1}](https://www.uniprot.org/uniprotkb/{p1}) and it's homolog [{p2}](https://www.uniprot.org/uniprotkb/{p2}) found by PROST",
+        "alnpdb:test":{
+            "pdb1":f"https://alphafold.ebi.ac.uk/files/AF-{p1}-F1-model_v4.pdb",
+            "pdb2":f"https://alphafold.ebi.ac.uk/files/AF-{p2}-F1-model_v4.pdb",
+            "alnpdb":"",
+            "lineLen":120
+        }
+    }
+
+def toJSONWP(queryDB,targetDB,thr,gothr,goList,homologList,out):
+    # Retrieve user name
+    username = os.getlogin()
+    # Retrieve time of day and date
+    now = datetime.now()
+    time_of_day = now.strftime("%H:%M:%S")  # Format time as hours:minutes:seconds
+    date = now.strftime("%Y-%m-%d")  # Format date as year-month-day
+
+    jsonwp = {
+        'md:caption':'## [PROST](https://www.pnas.org/doi/10.1073/pnas.2211823120) v0.2.9 Search Results',
+        'md:info1':f'The query database is **{queryDB}** and the target database is **{targetDB}**.', 
+        'md:info2':f'This search was conducted by **{username}** at {time_of_day} on {date}.',        
+        'md:info3':f'The e-value threshold for homology detection is **{thr}** and the threshold for GO annotation enrichment is **{gothr}**',
+        'h3:tablecap':'Query Database Proteins',
+        'md:info4':'Please click the link under the "Query Protein" column to access results for each query protein listed',
+        'table:proteinList':{'columns':['l:Query Protein','# Homologs','# GO','Best Homolog','Best H. e-val'],'rows':[]},
+        'navpage:about':{'md:info5':'''### PROST Method
+The Protein Language Search Tool (**PROST**) is a highly accurate and efficient homology search tool designed for remote homology prediction tasks. In comparison to the current state-of-the-art tools, such as CS-BLAST or PHMMER, PROST outperforms them in terms of accuracy and speed. PROST utilizes a protein language model and quantization technique to represent proteins in a numerical format that retains their biophysical, biochemical, and evolutionary information. PROST calculates the distances of all proteins in the database to the user's query protein and performs a statistical test based on the Z-Score of the distance distribution over the entire database. The results are presented with an expected value (e-value) that estimates the likelihood of a match occurring by chance. This value is calculated from the CDF of the z-score and is corrected for multiple testing using the Bonferroni method.
+
+### Automatic GO Enrichment Analysis
+The GO annotation enrichment pipeline in PROST allows for the selection of a different e-value cutoff. This threshold determines the level of significance for the enrichment analysis. To assess the significance of the enriched GO terms, contingency tables are constructed by comparing the frequency of individual GO terms in homologs and the Swissprot database. A term-specific p-value is then calculated by subjecting the contingency table to the Chi-square test. Subsequently, Bonferroni multiple p-test corrections are applied to correct the p-values for each term. Any GO term with a p-value greater than 0.001 is removed from the analysis. The remaining GO terms are evaluated based on their source proteins' e-values, which are combined using Stouffer’s method. The resulting GO terms are subjected to another round of multiple test correction, and the enriched terms are reported..
+
+### Manuscript
+PROST manuscript can be accessed form this [link](https://www.pnas.org/doi/10.1073/pnas.2211823120). Please cite if you used PROST for finding homologs.
+
+### Python Package
+PROST [python package](https://github.com/MesihK/prost) can be used to generate this result webpage with the help of JSONWP visualizer. Please cite both of the work (PROST and JSONWP)
+
+### Citations
+
+``` 
+@article{kilinc2023improved,
+  title={Improved global protein homolog detection with major gains in function identification},
+  author={Kilinc, Mesih and Jia, Kejue and Jernigan, Robert L},
+  journal={Proceedings of the National Academy of Sciences},
+  volume={120},
+  number={9},
+  pages={e2211823120},
+  year={2023},
+  publisher={National Acad Sciences}
+}
+```
+'''},
+        'navpage:disclaimer':{'p:disc':'For documents and software available from this server, we do not warrant or assume any legal liability or responsibility for the accuracy, completeness, or usefulness of any information, product, or process disclosed. We do not endorse or recommend any commercial products, processes, or services. Some pages may provide links to other Internet sites for the convenience of users. We are not responsible for the availability or content of these external sites, nor do we endorse, warrant, or guarantee the products, services, or information described or offered at these other Internet sites. Information that is created by this site is within the public domain. It is not the intention to provide specific medically related advice but rather to provide users with information for better understanding. However, it is requested that in any subsequent use of this work, PROST be given appropriate acknowledgment. We do not collect any personally identifiable information (PII) about visitors to our Web sites.'}
+             }
+    for queryP in homologList:
+        jsonwp[f'page:{queryP}'] = {
+            'h2:caption':f'PROST Results for {queryP}',
+            'h3:goCaption':'GO Annotations',
+            'md:info1':'Link under "GO Term" column directs user to amigo geneontology website for a detailed inspection of the GO term',
+            'table:goList':{'columns':['l:GO Term','Description','Confidence','Source','# Proteins','e-val'],'rows':[]},
+            'h3:homCaption':'Putative Homologs',
+            'md:info2':'Links under "Uniprot" column directs user to Uniprot website for a detailed inspection. Links under "e-value" column opens sequence alignment and protein structure visualization page',
+            'table:homList':{'columns':['l:Uniprot','Name','Type','Organim','Distance','l:e-value'],'rows':[]}
+        }
+        for go in goList[queryP]:
+            jsonwp[f'page:{queryP}']['table:goList']['rows'].append([f'http://amigo.geneontology.org/amigo/term/{go[0]}@{go[0]}']+go[1:])
+        for hom in homologList[queryP]:
+            jsonwp[f'page:{queryP}']['table:homList']['rows'].append([f'https://www.uniprot.org/uniprot/{hom[0]}@{hom[0]}']+hom[1:5]+
+                                                                    [f'{queryP}-{hom[0]}@{hom[5]}'])
+            jsonwp[f'page:{queryP}-{hom[0]}'] = createAlignmentPage(queryP,hom[0])
+        jsonwp['table:proteinList']['rows'].append([f'{queryP}@{queryP}',len(homologList[queryP]),len(goList[queryP]),homologList[queryP][0][0],homologList[queryP][0][5]])
+    # Write the dictionary to a JSON file
+    with open(out+'.json', "w") as f:
+        json.dump(jsonwp, f)
 
 @click.command()
 @click.option('--thr', default=0.05, help='E-value threshold for homolog detection')
 @click.argument('querydb', type=click.Path(exists=True,file_okay=True,dir_okay=False))
 @click.argument('targetdb', type=click.Path(exists=True,file_okay=True,dir_okay=False))
 @click.argument('out', type=click.Path(exists=False,file_okay=True,dir_okay=False))
 def search(thr, querydb, targetdb, out):
     '''Search a query database in target database.
 This command searches a query database against a target database.
 Both databases should be created using makedb command.
 Databases can contain one or more sequences.
 An e-value threshold can be specified with --thr flag. The default e-value threshold is 0.05'''
-    _search(thr,None,querydb,targetdb,None,out)
+    goList,homologList = _search(thr,None,querydb,targetdb,None)
+    toTSV(goList,homologList,out)
 
 @click.command()
 @click.option('--thr', default=0.05, help='E-value threshold for homolog detection')
 @click.option('--gothr', default=0.05, help='E-value threshold for GO annotation')
 @click.argument('querydb', type=click.Path(exists=True,file_okay=True,dir_okay=False))
-@click.argument('out', type=click.Path(exists=False,file_okay=True,dir_okay=False))
+@click.argument('out', default='PROST.res', type=click.Path(exists=False,file_okay=True,dir_okay=False))
 def searchsp(thr,gothr, querydb, out):
     '''Search query database in SwissProt February 2023 database.
 This command searches a query database against a SwissProt February 2023 database.
 Query database should be created using makedb command.
 It can contain one or more sequences.
 An e-value threshold can be specified with --thr flag. The default e-value threshold is 0.05.
 An seperate GO annotation threshold can be specified with --gothr flag. The default is 0.05.'''
-    _search(thr,gothr,querydb,prostdir+'/sp.02.23.parsed.prdb',prostdir+'/sp.02.23.go.pkl',out)
+    goList,homologList = _search(thr,gothr,querydb,prostdir+'/sp.02.23.parsed.prdb',prostdir+'/sp.02.23.go.pkl')
+    toTSV(goList,homologList,out)
+    toJSONWP(querydb,"SwissProt February 2023",thr,gothr,goList,homologList,out)
 
 @click.group()
 def cli():
-    '''PROST python package v0.2.7
+    '''PROST python package v0.2.9
 Please specify a command.
 makedb: creates a PROST database from given fasta file. The fasta file usually contains more than one entry.
 search: searches a query database against a target database. Query database can contain one or more sequences embedded using makedb command.
 searchsp: searches a query database against SwissProt February 2023 database. Query database can contain one or more sequences embedded using makedb command.'''
     pass
 
 cli.add_command(makedb)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyprost-0.2.8/setup.cfg` & `pyprost-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyprost
-version = 0.2.8
+version = 0.2.9
 author = Mesih Kilinc
 author_email = mesih@iastate.edu
 description = PRotein Ortholog Search Tool
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mesihk/prost
 project_urls =
```

### Comparing `pyprost-0.2.8/src/pyprost/__init__.py` & `pyprost-0.2.9/src/pyprost/__init__.py`

 * *Files identical despite different names*

### Comparing `pyprost-0.2.8/src/pyprost/esmts25_13.py` & `pyprost-0.2.9/src/pyprost/esmts25_13.py`

 * *Files identical despite different names*

### Comparing `pyprost-0.2.8/src/pyprost/prosttools.py` & `pyprost-0.2.9/src/pyprost/prosttools.py`

 * *Files identical despite different names*

### Comparing `pyprost-0.2.8/src/pyprost.egg-info/PKG-INFO` & `pyprost-0.2.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprost
-Version: 0.2.8
+Version: 0.2.9
 Summary: PRotein Ortholog Search Tool
 Home-page: https://github.com/mesihk/prost
 Author: Mesih Kilinc
 Author-email: mesih@iastate.edu
 Project-URL: Bug Tracker, https://github.com/mesihk/prost/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,25 +26,34 @@
 ```
 On the initial run, PROST will download required files to `~/.config/prost` or an user defined directory via `PROSTDIR` environment variable.
 
 ### How to use
 
 Following commands can be used to create databases and perform homology search.
 
-* makedb: creates a PROST database from given fasta file. The fasta file usually contains more than one entry.
-* search: searches a query database agains a target database. Query database can contain one or more sequences embedded using makedb command. `--thr` can be used to specify an e-value threshold. The default threshold is 0.05.
-* searchsp: searches a query database agains a SwissProt February 2023 database. Performs GO enrichment analysis on found homologs. Query database can contain one or more sequences embedded using makedb command. Again `--thr` can be used to specify an e-value threshold.  `--gothr` can be used to specifiy different e-value threshold for GO enrichment analysis.
-
 ```
 prost makedb db/sp.fa db/sp.prdb
 prost makedb db/covid.fa db/covid.prdb
-prost search --thr 0.05 db/covid.prdb db/sp.prdb results.tsv
-prost searchsp --thr 0.05 db/covid.prdb results.tsv
+prost search --thr 0.05 db/covid.prdb db/sp.prdb results
+prost searchsp --thr 0.05 db/covid.prdb results
 ```
 
+* `makedb`: creates a PROST database from given fasta file. The fasta file usually contains more than one entry.
+* `search`: searches a query database agains a target database. Query database can contain one or more sequences embedded using makedb command. `--thr` can be used to specify an e-value threshold. The default threshold is 0.05.
+* `searchsp`: searches a query database agains a SwissProt February 2023 database. Performs GO enrichment analysis on found homologs. Query database can contain one or more sequences embedded using makedb command. Again `--thr` can be used to specify an e-value threshold.  `--gothr` can be used to specifiy different e-value threshold for GO enrichment analysis. 
+`searchsp` produces a tab seprataed file `.tsv` and a JSON file `.json` that can be used with the tool [JSONWP](https://jsonwp.onrender.com/). 
+Here is an example result:
+![jsonwp1](asset/jsonwp1.png)
+![jsonwp2](asset/jsonwp2.png)
+Sequence alignment done automatically using the [PROTSUB](https://onlinelibrary.wiley.com/doi/full/10.1002/prot.26050) matrix which is better for aligning remote proteins then BLOSUM62 matrix. 
+Protein structures are fetched from the Alphafold 2 database. No alignment produced this time.
+![jsonwp3](asset/jsonwp3.png)
+
+
+
 ### Scripting
 
 ```
 import pyprost
 
 hpo30 = '''MPLIMYKFLLVTSIFLIVSGLILTAFSLFSPLWEVVDFPRSHLSHHHGLWWDCIVHHET
 LIPLHEDQAELRGDRCDSKMDSSVQASLRVALEKGDEEARELLLHRFLPHHKGVIFFAVF
@@ -70,7 +79,8 @@
 ### Resources
 
 * Yeast analysis: https://mesihk.github.io/prostyeast
 * Unannotated Human Proteins Analysis: https://mesihk.github.io/prosthuman
 * Webserver: https://mesihk.github.io/prost 
 * PROST Python package: https://github.com/MesihK/prost
 * PROST Research Data: https://github.com/MesihK/prost-data 
+* JSONWP: https://jsonwp.onrender.com/
```

