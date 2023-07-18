# Comparing `tmp/graphmb-0.2.4.tar.gz` & `tmp/graphmb-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\graphmb-0.2.4.tar", last modified: Fri Mar 31 15:14:14 2023, max compression
+gzip compressed data, was "graphmb-0.2.5.tar", last modified: Tue Jul 18 11:57:14 2023, max compression
```

## Comparing `graphmb-0.2.4.tar` & `graphmb-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 15:14:14.000000 graphmb-0.2.4/
--rw-rw-rw-   0        0        0     1091 2023-03-31 12:50:25.000000 graphmb-0.2.4/LICENSE
--rw-rw-rw-   0        0        0       73 2023-03-31 12:50:25.000000 graphmb-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0      189 2023-03-31 15:14:14.000000 graphmb-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      130 2023-03-31 12:50:25.000000 graphmb-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0    16902 2023-03-31 12:50:25.000000 graphmb-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-03-31 15:14:14.000000 graphmb-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      898 2023-03-31 12:52:53.000000 graphmb-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 15:14:13.000000 graphmb-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-03-31 15:14:14.000000 graphmb-0.2.4/src/graphmb/
--rw-rw-rw-   0        0        0    12675 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/amber_eval.py
--rw-rw-rw-   0        0        0     8911 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/arg_options.py
--rw-rw-rw-   0        0        0    41252 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/contigsdataset.py
--rw-rw-rw-   0        0        0     9079 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/dgl_dataset.py
--rw-rw-rw-   0        0        0    26317 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/evaluate.py
--rw-rw-rw-   0        0        0    16151 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/gnn_models.py
--rw-rw-rw-   0        0        0    18223 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/graphmb1.py
--rw-rw-rw-   0        0        0    14586 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/graphsage_unsupervised.py
--rw-rw-rw-   0        0        0    13135 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/layers.py
--rw-rw-rw-   0        0        0    25971 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/main.py
--rw-rw-rw-   0        0        0    29439 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/models.py
--rw-rw-rw-   0        0        0    22040 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/train_ccvae.py
--rw-rw-rw-   0        0        0    11091 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/train_gnn.py
--rw-rw-rw-   0        0        0    10610 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/utils.py
--rw-rw-rw-   0        0        0    19350 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/vamb_clustering.py
--rw-rw-rw-   0        0        0       25 2023-03-31 12:53:57.000000 graphmb-0.2.4/src/graphmb/version.py
--rw-rw-rw-   0        0        0    11367 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/visualize.py
--rw-rw-rw-   0        0        0      109 2023-03-31 12:50:25.000000 graphmb-0.2.4/src/graphmb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 15:14:14.000000 graphmb-0.2.4/src/graphmb.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-31 15:14:12.000000 graphmb-0.2.4/src/graphmb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-03-31 15:14:12.000000 graphmb-0.2.4/src/graphmb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      189 2023-03-31 15:14:12.000000 graphmb-0.2.4/src/graphmb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-03-31 15:14:12.000000 graphmb-0.2.4/src/graphmb.egg-info/requires.txt
--rw-rw-rw-   0        0        0      727 2023-03-31 15:14:12.000000 graphmb-0.2.4/src/graphmb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-03-31 15:14:12.000000 graphmb-0.2.4/src/graphmb.egg-info/top_level.txt
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2023-07-18 11:57:14.743369 graphmb-0.2.5/
+-rw-r--r--   0 andre     (1000) andre     (1000)     1073 2023-07-12 09:57:57.000000 graphmb-0.2.5/LICENSE
+-rw-r--r--   0 andre     (1000) andre     (1000)       72 2023-07-17 15:19:22.000000 graphmb-0.2.5/MANIFEST.in
+-rw-r--r--   0 andre     (1000) andre     (1000)      177 2023-07-18 11:57:14.743369 graphmb-0.2.5/PKG-INFO
+-rw-r--r--   0 andre     (1000) andre     (1000)    16550 2023-07-12 09:57:57.000000 graphmb-0.2.5/README.md
+-rw-r--r--   0 andre     (1000) andre     (1000)      127 2023-07-12 09:57:57.000000 graphmb-0.2.5/pyproject.toml
+-rw-r--r--   0 andre     (1000) andre     (1000)       38 2023-07-18 11:57:14.743369 graphmb-0.2.5/setup.cfg
+-rw-r--r--   0 andre     (1000) andre     (1000)      864 2023-07-18 10:20:47.000000 graphmb-0.2.5/setup.py
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2023-07-18 11:57:14.732536 graphmb-0.2.5/src/
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2023-07-18 11:57:14.743369 graphmb-0.2.5/src/graphmb/
+-rw-r--r--   0 andre     (1000) andre     (1000)      104 2023-07-12 09:57:57.000000 graphmb-0.2.5/src/graphmb/__init__.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    12455 2023-07-12 09:57:57.000000 graphmb-0.2.5/src/graphmb/amber_eval.py
+-rw-r--r--   0 andre     (1000) andre     (1000)     8994 2023-07-18 09:00:26.000000 graphmb-0.2.5/src/graphmb/arg_options.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    40439 2023-07-12 09:57:57.000000 graphmb-0.2.5/src/graphmb/contigsdataset.py
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2023-07-18 11:57:14.743369 graphmb-0.2.5/src/graphmb/data/
+-rw-r--r--   0 andre     (1000) andre     (1000)     1587 2023-07-17 15:19:46.000000 graphmb-0.2.5/src/graphmb/data/Bacteria.ms
+-rw-r--r--   0 andre     (1000) andre     (1000)    77187 2023-07-17 15:19:40.000000 graphmb-0.2.5/src/graphmb/data/kernel.npz
+-rw-r--r--   0 andre     (1000) andre     (1000)     8869 2023-07-12 09:57:57.000000 graphmb-0.2.5/src/graphmb/dgl_dataset.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    25724 2023-07-12 09:57:57.000000 graphmb-0.2.5/src/graphmb/evaluate.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    15718 2023-07-12 09:57:57.000000 graphmb-0.2.5/src/graphmb/gnn_models.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    17817 2023-07-12 09:57:57.000000 graphmb-0.2.5/src/graphmb/graphmb1.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    14210 2023-07-12 09:57:57.000000 graphmb-0.2.5/src/graphmb/graphsage_unsupervised.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    12860 2023-07-12 09:57:57.000000 graphmb-0.2.5/src/graphmb/layers.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    25924 2023-07-18 11:13:01.000000 graphmb-0.2.5/src/graphmb/main.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    28797 2023-07-12 09:57:57.000000 graphmb-0.2.5/src/graphmb/models.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    21626 2023-07-18 09:07:21.000000 graphmb-0.2.5/src/graphmb/train_ccvae.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    10901 2023-07-18 09:07:44.000000 graphmb-0.2.5/src/graphmb/train_gnn.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    10361 2023-07-12 09:57:57.000000 graphmb-0.2.5/src/graphmb/utils.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    18874 2023-07-12 09:57:57.000000 graphmb-0.2.5/src/graphmb/vamb_clustering.py
+-rw-r--r--   0 andre     (1000) andre     (1000)       23 2023-07-18 11:18:53.000000 graphmb-0.2.5/src/graphmb/version.py
+-rw-r--r--   0 andre     (1000) andre     (1000)    11057 2023-07-12 09:57:57.000000 graphmb-0.2.5/src/graphmb/visualize.py
+drwxr-xr-x   0 andre     (1000) andre     (1000)        0 2023-07-18 11:57:14.743369 graphmb-0.2.5/src/graphmb.egg-info/
+-rw-r--r--   0 andre     (1000) andre     (1000)      177 2023-07-18 11:57:14.000000 graphmb-0.2.5/src/graphmb.egg-info/PKG-INFO
+-rw-r--r--   0 andre     (1000) andre     (1000)      784 2023-07-18 11:57:14.000000 graphmb-0.2.5/src/graphmb.egg-info/SOURCES.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)        1 2023-07-18 11:57:14.000000 graphmb-0.2.5/src/graphmb.egg-info/dependency_links.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)       47 2023-07-18 11:57:14.000000 graphmb-0.2.5/src/graphmb.egg-info/entry_points.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)      111 2023-07-18 11:57:14.000000 graphmb-0.2.5/src/graphmb.egg-info/requires.txt
+-rw-r--r--   0 andre     (1000) andre     (1000)        8 2023-07-18 11:57:14.000000 graphmb-0.2.5/src/graphmb.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `graphmb-0.2.4/LICENSE` & `graphmb-0.2.5/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `graphmb-0.2.4/README.md` & `graphmb-0.2.5/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,352 +1,352 @@
-# GraphMB: Assembly Graph Metagenomic Binner
-
-# Introduction
-
-GraphMB is a Metagenomic Binner developed for long-read assemblies, that takes advantage of graph machine learning 
-algorithms and the assembly graph generated during assembly. It has been tested on (meta)flye assemblies.
-
-Our peer-reviewed paper: 
-> Andre Lamurias, Mantas Sereika, Mads Albertsen, Katja Hose, Thomas Dyhre Nielsen, Metagenomic binning with assembly graph embeddings, Bioinformatics, 2022;, btac557, https://doi.org/10.1093/bioinformatics/btac557
-
-## Dependencies
-
-GraphMB was developed with Python 3.7.
-All of its dependencies are automatically installed.
-For pre-processing and post-processing, check this README.
-
-## Documentation
-
-Can be found here: https://graphmb.readthedocs.io/en/latest/
-
-## Installation
-
-### NEW - Option 1 - From pypi
-```bash
-pip install graphmb
-```
-
-### Option 2 - From wheel
-```bash
-pip install https://github.com/AndreLamurias/GraphMB/releases/download/v0.1.5/graphmb-0.2.2-py3-none-any.whl
-```
-
-### Option 3 - From source
-Clone this repository, and then:
-```bash
-cd GraphMB
-python -m venv venv; source venv/bin/activate # optional
-pip install .
-```
-
-### Option 4 - Docker
-Either build the docker image with the Dockerfile or pull from dockerhub:
-```bash
-docker pull andrelamurias/graphmb
-```
-
-Then you can run GraphMB on a container. The image includes the Strong100 dataset. 
-If you want to use other datasets, use the -v option to mount the path to your data.
-
-```bash
-docker run -it andrelamurias/graphmb bash
-```
-
-### Option 5 - From conda
-```bash
-conda create -n graphmb -c conda-forge make cmake libgcc python=3.7 pip tensorflow
-conda activate graphmb
-pip install graphmb
-```
-
-## Input files
-
-The only files required are the contigs in fasta format, and the assembly graph in GFA format. For optimal performance,
-the assembly graph should be generated with Flye 2.9, since it includes the number of reads mapping to each pair of
-contigs. Also, for better results, CheckM is run on each contig using the general Bacteria marker sets. This is optional
-though, you can just run the model for a number of epochs and pick the last model. The marker genes are also used to
-improve model training through a constrained loss function.
-By default, it runs with with early stopping.
-
-In summary, you need to have a directory with these files (names can be changed with arguments):
-- assembly.fasta: assembly graph edge sequences or contigs
-- assembly_graph.gfa: assembly graph. it should have the sequences of assembly.fasta as nodes.
-- assembly_depth.txt: output of `jgi_summarize_bam_contig_depths`
-- marker_gene_stats.csv (optional): output of CheckM for each contig
-
-If you do not specify this directory the `--assembly`, you have to use the full path of all files.
-Otherwise, it will assume that the files are inside the directory.
-
-You can get an example of these files [here](https://drive.google.com/drive/folders/1m6uTgTPUghk_q9GxfX1UNEOfn8jnIdt5?usp=sharing).
-Download from this link and extract to data/strong100.
-The datasets used in our experiments are available [here](https://zenodo.org/record/6122610)
-These datasets include the VAE embeddings obtained with Vamb, which are automatically used by GraphMB.
-If you want to re-run Vamb, use the `--vamb` option.
-## How to run
-If you have your assembly in some directory, with the files mentioned above:
-
-```bash
-graphmb --assembly data/strong100/ --outdir results/strong100/ --markers marker_gene_stats.tsv
-```
-
-The outdir will be created if it does not exist. The marker file is optional. 
-You can specify the filenames:
-
-```bash
-graphmb --assembly data/strong100/ --outdir results/strong100/ --assembly_name edges.fasta --graph_file assembly_graph.gfa --depth edges_depth.txt --markers marker_gene_stats.tsv
-```
-
-By default GraphMB saves a TSV file mapping each contig to a bin to the assembly directory, as well as the weights and output embeddings of the best model.
-The output directory can be changed with the `--outdir` argument.
-
-To prevent GraphMB from run clustering after each epoch, do not provide the markers param or set the `--evalepochs` option to a higher number (default is 10)
-This will make it run faster but the results might not be optimal.
-
-```bash
-graphmb --assembly data/strong100/ --outdir results/strong100/
-```
-
-To use GPU both for training and clustering, use the --cuda param:
-
-```bash
-graphmb --assembly data/strong100/ --outdir results/strong100/ --cuda
-```
-
-
-You can also run on CPU and limit the number of threads to use:
-```bash
-graphmb --assembly data/strong100/ --outdir results/strong100/ --numcores 4
-```
-
-GraphMB was tested on graphs where the nodes are contig paths and not full contigs.
-This gives more granularity to the algorithm and the edges are directly obtained from the assembly graph.
-However in some cases this might be inconvenient, for example if 
-We implemented an option to use a graph where the nodes are contigs.
-```bash
-graphmb --assembly data/strong100/ --outdir results/strong100/ --assembly_name contigs.fasta --depth contig_depth.txt --contignodes
-```
-
-## Typical workflow
-Our workflows are available [here](https://github.com/AndreLamurias/binning_workflows).
-On this section we present an overview of how to get your data ready for GraphMB.
-
-### Pre-processing
-
-1. Assembly your reads with metaflye: ```flye -nano-raw <reads_file> -o <output> --meta```
-2. Filter and polish assembly if necessary (or extract edge sequences and polish edge sequences instead)
-```bash
-mv assembly.fasta contigs.fasta
-awk '/^S/{print ">"$2"\n"$3}' assembly_graph.gfa | fold > assembly.fasta
-```
-3. Convert assembly graph to contig-based graph if you want to use full contig instead of edges
-4. Run CheckM on sequences with Bacteria markers: 
-```bash
-mkdir edges
-cd edges; cat ../assembly.fasta | awk '{ if (substr($0, 1, 1)==">") {filename=(substr($0,2) ".fa")} print $0 > filename }'; cd ..
-find edges/ -name "* *" -type f | rename 's/ /_/g'
-# evaluate edges
-checkm taxonomy_wf -x fa domain Bacteria edges/ checkm_edges/
-checkm qa checkm_edges/Bacteria.ms checkm_edges/ -f checkm_edges_polished_results.txt --tab_table -o 2
-```
-5. Get abundances with `jgi_summarize_bam_contig_depths`:
-```bash
-minimap2 -I 64GB -d assembly.mmi assembly.fasta # make index
-minimap2 -I 64GB -ax map-ont assembly.mmi <reads_file> > assembly.sam
-samtools sort assembly.sam > assembly.bam
-jgi_summarize_bam_contig_depths --outputDepth assembly_depth.txt assembly.bam
-```
-6. Now you should have all the files to run GraphMB: assembly.fasta, assembly_graph.gfa and assembly_depth.txt. The marker_gene_stats.csv file will be saved to checkm_edges/storage/.
-
-We have only tested GraphMB on flye assemblies. Flye generates a repeat graph where the nodes do not correspond to full contigs. 
-Depending on your setup, you need to either use the edges as contigs.
-
-### Post-processing
-To evaluate the binning output, we run checkM with the `--reduced-tree` option and count HQ bins (>90 completeness 
-and <5 contamination).
-The bins will be written to fasta files if `writebins` is included in the `--post` argument.
-Alternatively, the `--post contig2bin` option can be used (on by default) and the bins from that file can be written 
-to fasta with `src/write_fasta_bins.py`.
-Then you can run checkM on the bins directory:
-```bash
-checkm lineage_wf -x fa --reduced_tree -t 4 --tab_table bins_dir/ outputdir/ -f outputdir/checkm.tsv
-```
-We also provide a script to filter the checkM output and get the number of HQ bins:
-```bash
-python src/process_checkm_results_expanded.py outputdir/checkm.tsv 90 5
-```
-
-
-## Parameters
-
-GraphMB contains many parameters to run various experiments, from changing the data inputs, to architecture of the 
-model, training loss, data preprocessing, and output type.
-The defaults were chosen to obtain the published results on the WWTP datasets, but may require some tuning for different
-datasets and scenarios.
-The full list of parameters is below but this section focused on the most relevant ones.
-
-### assembly, assembly_name, graph_file, features, labels, markers, depth
-If --assembly is given, that is used as the base data directory. 
-Every other path is in relation to that directory.
-Otherwise, every data file path must be given in relation to the current directory
-
-Note about markers: this file is not mandatory but assumed to exist by default.
-This is because we have run all of our experiments with it.
-Without this, the number of HQ bins will be probably worse.
-
-### outdir, outname
-Where to write the output files, including caches, and what prefix to use.
-If not given, GraphMB writes to the data directory given by --assembly.
-
-### reload
-
-Ignore cache and reprocess data files.
-
-### nruns, seed
-Repeat experiment nrun times. Use --seed to specify the initial seed, which is changed
-with every run to get different results.
-
-### cuda
-
-Run model training and clustering on GPU.
-
-### contignodes
-
-If the contigs given by the --assembly_name parameter are actual contigs and not assembly graph edges,
-use this parameter, which will transform the assembly graph to use full contigs as nodes.
-
-### model
-
-Model to be used by GraphMB. By default it uses a Graph Convolution Network, and trains a Variational Autoencoder first
-to generate node features. The VAE embeddings are saved to make it faster to rerun the GCN.
-
-Other models: 
-- sage_lstm: original GraphMB GraphSAGE model, requires DGL installation
-- gat and sage: alternative GNN model to GCN (VAEGBin)
-- gcn_ccvae, gat_ccvae, sage_ccvae: combined VAE and GNN models, trained end-to-end, or without GNN if layers_gnn=0
-
-## Full list of parameters
-```
-usage: graphmb [-h] [--assembly ASSEMBLY] [--assembly_name ASSEMBLY_NAME] [--graph_file GRAPH_FILE] [--edge_threshold EDGE_THRESHOLD] [--depth DEPTH] [--features FEATURES] [--labels LABELS] [--embs EMBS] [--model_name MODEL_NAME]
-               [--activation ACTIVATION] [--layers_vae LAYERS_VAE] [--layers_gnn LAYERS_GNN] [--hidden_gnn HIDDEN_GNN] [--hidden_vae HIDDEN_VAE] [--embsize_gnn EMBSIZE_GNN] [--embsize_vae EMBSIZE_VAE] [--batchsize BATCHSIZE]
-               [--batchtype BATCHTYPE] [--dropout_gnn DROPOUT_GNN] [--dropout_vae DROPOUT_VAE] [--lr_gnn LR_GNN] [--lr_vae LR_VAE] [--graph_alpha GRAPH_ALPHA] [--kld_alpha KLD_ALPHA] [--ae_alpha AE_ALPHA] [--scg_alpha SCG_ALPHA]
-               [--clusteringalgo CLUSTERINGALGO] [--kclusters KCLUSTERS] [--aggtype AGGTYPE] [--decoder_input DECODER_INPUT] [--vaepretrain VAEPRETRAIN] [--ae_only] [--negatives NEGATIVES] [--quick] [--classify] [--fanout FANOUT]
-               [--epoch EPOCH] [--print PRINT] [--evalepochs EVALEPOCHS] [--evalskip EVALSKIP] [--eval_split EVAL_SPLIT] [--kmer KMER] [--rawfeatures] [--clusteringloss] [--targetmetric TARGETMETRIC] [--concatfeatures]
-               [--no_loss_weights] [--no_sample_weights] [--early_stopping EARLY_STOPPING] [--nruns NRUNS] [--mincontig MINCONTIG] [--minbin MINBIN] [--mincomp MINCOMP] [--randomize] [--labelgraph] [--binarize] [--noedges]
-               [--read_embs] [--reload] [--markers MARKERS] [--post POST] [--skip_preclustering] [--outname OUTNAME] [--cuda] [--noise] [--savemodel] [--tsne] [--numcores NUMCORES] [--outdir OUTDIR]
-               [--assembly_type ASSEMBLY_TYPE] [--contignodes] [--seed SEED] [--quiet] [--read_cache] [--version] [--loglevel LOGLEVEL] [--configfile CONFIGFILE]
-
-Train graph embedding model
-
-
-
-options:
-  -h, --help            show this help message and exit
-  --assembly ASSEMBLY   Assembly base path
-  --assembly_name ASSEMBLY_NAME
-                        File name with contigs
-  --graph_file GRAPH_FILE
-                        File name with graph
-  --edge_threshold EDGE_THRESHOLD
-                        Remove edges with weight lower than this (keep only >=)
-  --depth DEPTH         Depth file from jgi
-  --features FEATURES   Features file mapping contig name to features
-  --labels LABELS       File mapping contig to label
-  --embs EMBS           No train, load embs
-  --model_name MODEL_NAME
-                        One of the implemented models
-  --activation ACTIVATION
-                        Activation function to use(relu, prelu, sigmoid, tanh)
-  --layers_vae LAYERS_VAE
-                        Number of layers of the VAE
-  --layers_gnn LAYERS_GNN
-                        Number of layers of the GNN
-  --hidden_gnn HIDDEN_GNN
-                        Dimension of hidden layers of GNN
-  --hidden_vae HIDDEN_VAE
-                        Dimension of hidden layers of VAE
-  --embsize_gnn EMBSIZE_GNN, --zg EMBSIZE_GNN
-                        Output embedding dimension of GNN
-  --embsize_vae EMBSIZE_VAE, --zl EMBSIZE_VAE
-                        Output embedding dimension of VAE
-  --batchsize BATCHSIZE
-                        batchsize to train the VAE
-  --batchtype BATCHTYPE
-                        Batch type, nodes or edges
-  --dropout_gnn DROPOUT_GNN
-                        dropout of the GNN
-  --dropout_vae DROPOUT_VAE
-                        dropout of the VAE
-  --lr_gnn LR_GNN       learning rate
-  --lr_vae LR_VAE       learning rate
-  --graph_alpha GRAPH_ALPHA
-                        Coeficient for graph loss
-  --kld_alpha KLD_ALPHA
-                        Coeficient for KLD loss
-  --ae_alpha AE_ALPHA   Coeficient for AE loss
-  --scg_alpha SCG_ALPHA
-                        Coeficient for SCG loss
-  --clusteringalgo CLUSTERINGALGO
-                        clustering algorithm
-  --kclusters KCLUSTERS
-                        Number of clusters (only for some clustering methods)
-  --aggtype AGGTYPE     Aggregation type for GraphSAGE (mean, pool, lstm, gcn)
-  --decoder_input DECODER_INPUT
-                        What to use for input to the decoder
-  --vaepretrain VAEPRETRAIN
-                        How many epochs to pretrain VAE
-  --ae_only             Do not use GNN (ae model must be used and decoder input must be ae
-  --negatives NEGATIVES
-                        Number of negatives to train GraphSAGE
-  --quick               Reduce number of nodes to run quicker
-  --classify            Run classification instead of clustering
-  --fanout FANOUT       Fan out, number of positive neighbors sampled at each level
-  --epoch EPOCH         Number of epochs to train model
-  --print PRINT         Print interval during training
-  --evalepochs EVALEPOCHS
-                        Epoch interval to run eval
-  --evalskip EVALSKIP   Skip eval of these epochs
-  --eval_split EVAL_SPLIT
-                        Percentage of dataset to use for eval
-  --kmer KMER
-  --rawfeatures         Use raw features
-  --clusteringloss      Train with clustering loss
-  --targetmetric TARGETMETRIC
-                        Metric to pick best epoch
-  --concatfeatures      Concat learned and original features before clustering
-  --no_loss_weights     Using edge weights for loss (positive only)
-  --no_sample_weights   Using edge weights to sample negatives
-  --early_stopping EARLY_STOPPING
-                        Stop training if delta between last two losses is less than this
-  --nruns NRUNS         Number of runs
-  --mincontig MINCONTIG
-                        Minimum size of input contigs
-  --minbin MINBIN       Minimum size of clusters in bp
-  --mincomp MINCOMP     Minimum size of connected components
-  --randomize           Randomize graph
-  --labelgraph          Create graph based on labels (ignore assembly graph)
-  --binarize            Binarize adj matrix
-  --noedges             Remove all but self edges from adj matrix
-  --read_embs           Read embeddings from file
-  --reload              Reload data
-  --markers MARKERS     File with precomputed checkm results to eval
-  --post POST           Output options
-  --skip_preclustering  Use precomputed checkm results to eval
-  --outname OUTNAME, --outputname OUTNAME
-                        Output (experiment) name
-  --cuda                Use gpu
-  --noise               Use noise generator
-  --savemodel           Save best model to disk
-  --tsne                Plot tsne at checkpoints
-  --numcores NUMCORES   Number of cores to use
-  --outdir OUTDIR, --outputdir OUTDIR
-                        Output dir (same as input assembly dir if not defined
-  --assembly_type ASSEMBLY_TYPE
-                        flye or spades
-  --contignodes         Use contigs as nodes instead of edges
-  --seed SEED           Set seed
-  --quiet, -q           Do not output epoch progress
-  --read_cache          Do not check assembly files, read cached files only
-  --version, -v         Print version and exit
-  --loglevel LOGLEVEL, -l LOGLEVEL
-                        Log level
-
-```
+# GraphMB: Assembly Graph Metagenomic Binner
+
+# Introduction
+
+GraphMB is a Metagenomic Binner developed for long-read assemblies, that takes advantage of graph machine learning 
+algorithms and the assembly graph generated during assembly. It has been tested on (meta)flye assemblies.
+
+Our peer-reviewed paper: 
+> Andre Lamurias, Mantas Sereika, Mads Albertsen, Katja Hose, Thomas Dyhre Nielsen, Metagenomic binning with assembly graph embeddings, Bioinformatics, 2022;, btac557, https://doi.org/10.1093/bioinformatics/btac557
+
+## Dependencies
+
+GraphMB was developed with Python 3.7.
+All of its dependencies are automatically installed.
+For pre-processing and post-processing, check this README.
+
+## Documentation
+
+Can be found here: https://graphmb.readthedocs.io/en/latest/
+
+## Installation
+
+### NEW - Option 1 - From pypi
+```bash
+pip install graphmb
+```
+
+### Option 2 - From wheel
+```bash
+pip install https://github.com/AndreLamurias/GraphMB/releases/download/v0.1.5/graphmb-0.2.2-py3-none-any.whl
+```
+
+### Option 3 - From source
+Clone this repository, and then:
+```bash
+cd GraphMB
+python -m venv venv; source venv/bin/activate # optional
+pip install .
+```
+
+### Option 4 - Docker
+Either build the docker image with the Dockerfile or pull from dockerhub:
+```bash
+docker pull andrelamurias/graphmb
+```
+
+Then you can run GraphMB on a container. The image includes the Strong100 dataset. 
+If you want to use other datasets, use the -v option to mount the path to your data.
+
+```bash
+docker run -it andrelamurias/graphmb bash
+```
+
+### Option 5 - From conda
+```bash
+conda create -n graphmb -c conda-forge make cmake libgcc python=3.7 pip tensorflow
+conda activate graphmb
+pip install graphmb
+```
+
+## Input files
+
+The only files required are the contigs in fasta format, and the assembly graph in GFA format. For optimal performance,
+the assembly graph should be generated with Flye 2.9, since it includes the number of reads mapping to each pair of
+contigs. Also, for better results, CheckM is run on each contig using the general Bacteria marker sets. This is optional
+though, you can just run the model for a number of epochs and pick the last model. The marker genes are also used to
+improve model training through a constrained loss function.
+By default, it runs with with early stopping.
+
+In summary, you need to have a directory with these files (names can be changed with arguments):
+- assembly.fasta: assembly graph edge sequences or contigs
+- assembly_graph.gfa: assembly graph. it should have the sequences of assembly.fasta as nodes.
+- assembly_depth.txt: output of `jgi_summarize_bam_contig_depths`
+- marker_gene_stats.csv (optional): output of CheckM for each contig
+
+If you do not specify this directory the `--assembly`, you have to use the full path of all files.
+Otherwise, it will assume that the files are inside the directory.
+
+You can get an example of these files [here](https://drive.google.com/drive/folders/1m6uTgTPUghk_q9GxfX1UNEOfn8jnIdt5?usp=sharing).
+Download from this link and extract to data/strong100.
+The datasets used in our experiments are available [here](https://zenodo.org/record/6122610)
+These datasets include the VAE embeddings obtained with Vamb, which are automatically used by GraphMB.
+If you want to re-run Vamb, use the `--vamb` option.
+## How to run
+If you have your assembly in some directory, with the files mentioned above:
+
+```bash
+graphmb --assembly data/strong100/ --outdir results/strong100/ --markers marker_gene_stats.tsv
+```
+
+The outdir will be created if it does not exist. The marker file is optional. 
+You can specify the filenames:
+
+```bash
+graphmb --assembly data/strong100/ --outdir results/strong100/ --assembly_name edges.fasta --graph_file assembly_graph.gfa --depth edges_depth.txt --markers marker_gene_stats.tsv
+```
+
+By default GraphMB saves a TSV file mapping each contig to a bin to the assembly directory, as well as the weights and output embeddings of the best model.
+The output directory can be changed with the `--outdir` argument.
+
+To prevent GraphMB from run clustering after each epoch, do not provide the markers param or set the `--evalepochs` option to a higher number (default is 10)
+This will make it run faster but the results might not be optimal.
+
+```bash
+graphmb --assembly data/strong100/ --outdir results/strong100/
+```
+
+To use GPU both for training and clustering, use the --cuda param:
+
+```bash
+graphmb --assembly data/strong100/ --outdir results/strong100/ --cuda
+```
+
+
+You can also run on CPU and limit the number of threads to use:
+```bash
+graphmb --assembly data/strong100/ --outdir results/strong100/ --numcores 4
+```
+
+GraphMB was tested on graphs where the nodes are contig paths and not full contigs.
+This gives more granularity to the algorithm and the edges are directly obtained from the assembly graph.
+However in some cases this might be inconvenient, for example if 
+We implemented an option to use a graph where the nodes are contigs.
+```bash
+graphmb --assembly data/strong100/ --outdir results/strong100/ --assembly_name contigs.fasta --depth contig_depth.txt --contignodes
+```
+
+## Typical workflow
+Our workflows are available [here](https://github.com/AndreLamurias/binning_workflows).
+On this section we present an overview of how to get your data ready for GraphMB.
+
+### Pre-processing
+
+1. Assembly your reads with metaflye: ```flye -nano-raw <reads_file> -o <output> --meta```
+2. Filter and polish assembly if necessary (or extract edge sequences and polish edge sequences instead)
+```bash
+mv assembly.fasta contigs.fasta
+awk '/^S/{print ">"$2"\n"$3}' assembly_graph.gfa | fold > assembly.fasta
+```
+3. Convert assembly graph to contig-based graph if you want to use full contig instead of edges
+4. Run CheckM on sequences with Bacteria markers: 
+```bash
+mkdir edges
+cd edges; cat ../assembly.fasta | awk '{ if (substr($0, 1, 1)==">") {filename=(substr($0,2) ".fa")} print $0 > filename }'; cd ..
+find edges/ -name "* *" -type f | rename 's/ /_/g'
+# evaluate edges
+checkm taxonomy_wf -x fa domain Bacteria edges/ checkm_edges/
+checkm qa checkm_edges/Bacteria.ms checkm_edges/ -f checkm_edges_polished_results.txt --tab_table -o 2
+```
+5. Get abundances with `jgi_summarize_bam_contig_depths`:
+```bash
+minimap2 -I 64GB -d assembly.mmi assembly.fasta # make index
+minimap2 -I 64GB -ax map-ont assembly.mmi <reads_file> > assembly.sam
+samtools sort assembly.sam > assembly.bam
+jgi_summarize_bam_contig_depths --outputDepth assembly_depth.txt assembly.bam
+```
+6. Now you should have all the files to run GraphMB: assembly.fasta, assembly_graph.gfa and assembly_depth.txt. The marker_gene_stats.csv file will be saved to checkm_edges/storage/.
+
+We have only tested GraphMB on flye assemblies. Flye generates a repeat graph where the nodes do not correspond to full contigs. 
+Depending on your setup, you need to either use the edges as contigs.
+
+### Post-processing
+To evaluate the binning output, we run checkM with the `--reduced-tree` option and count HQ bins (>90 completeness 
+and <5 contamination).
+The bins will be written to fasta files if `writebins` is included in the `--post` argument.
+Alternatively, the `--post contig2bin` option can be used (on by default) and the bins from that file can be written 
+to fasta with `src/write_fasta_bins.py`.
+Then you can run checkM on the bins directory:
+```bash
+checkm lineage_wf -x fa --reduced_tree -t 4 --tab_table bins_dir/ outputdir/ -f outputdir/checkm.tsv
+```
+We also provide a script to filter the checkM output and get the number of HQ bins:
+```bash
+python src/process_checkm_results_expanded.py outputdir/checkm.tsv 90 5
+```
+
+
+## Parameters
+
+GraphMB contains many parameters to run various experiments, from changing the data inputs, to architecture of the 
+model, training loss, data preprocessing, and output type.
+The defaults were chosen to obtain the published results on the WWTP datasets, but may require some tuning for different
+datasets and scenarios.
+The full list of parameters is below but this section focused on the most relevant ones.
+
+### assembly, assembly_name, graph_file, features, labels, markers, depth
+If --assembly is given, that is used as the base data directory. 
+Every other path is in relation to that directory.
+Otherwise, every data file path must be given in relation to the current directory
+
+Note about markers: this file is not mandatory but assumed to exist by default.
+This is because we have run all of our experiments with it.
+Without this, the number of HQ bins will be probably worse.
+
+### outdir, outname
+Where to write the output files, including caches, and what prefix to use.
+If not given, GraphMB writes to the data directory given by --assembly.
+
+### reload
+
+Ignore cache and reprocess data files.
+
+### nruns, seed
+Repeat experiment nrun times. Use --seed to specify the initial seed, which is changed
+with every run to get different results.
+
+### cuda
+
+Run model training and clustering on GPU.
+
+### contignodes
+
+If the contigs given by the --assembly_name parameter are actual contigs and not assembly graph edges,
+use this parameter, which will transform the assembly graph to use full contigs as nodes.
+
+### model
+
+Model to be used by GraphMB. By default it uses a Graph Convolution Network, and trains a Variational Autoencoder first
+to generate node features. The VAE embeddings are saved to make it faster to rerun the GCN.
+
+Other models: 
+- sage_lstm: original GraphMB GraphSAGE model, requires DGL installation
+- gat and sage: alternative GNN model to GCN (VAEGBin)
+- gcn_ccvae, gat_ccvae, sage_ccvae: combined VAE and GNN models, trained end-to-end, or without GNN if layers_gnn=0
+
+## Full list of parameters
+```
+usage: graphmb [-h] [--assembly ASSEMBLY] [--assembly_name ASSEMBLY_NAME] [--graph_file GRAPH_FILE] [--edge_threshold EDGE_THRESHOLD] [--depth DEPTH] [--features FEATURES] [--labels LABELS] [--embs EMBS] [--model_name MODEL_NAME]
+               [--activation ACTIVATION] [--layers_vae LAYERS_VAE] [--layers_gnn LAYERS_GNN] [--hidden_gnn HIDDEN_GNN] [--hidden_vae HIDDEN_VAE] [--embsize_gnn EMBSIZE_GNN] [--embsize_vae EMBSIZE_VAE] [--batchsize BATCHSIZE]
+               [--batchtype BATCHTYPE] [--dropout_gnn DROPOUT_GNN] [--dropout_vae DROPOUT_VAE] [--lr_gnn LR_GNN] [--lr_vae LR_VAE] [--graph_alpha GRAPH_ALPHA] [--kld_alpha KLD_ALPHA] [--ae_alpha AE_ALPHA] [--scg_alpha SCG_ALPHA]
+               [--clusteringalgo CLUSTERINGALGO] [--kclusters KCLUSTERS] [--aggtype AGGTYPE] [--decoder_input DECODER_INPUT] [--vaepretrain VAEPRETRAIN] [--ae_only] [--negatives NEGATIVES] [--quick] [--classify] [--fanout FANOUT]
+               [--epoch EPOCH] [--print PRINT] [--evalepochs EVALEPOCHS] [--evalskip EVALSKIP] [--eval_split EVAL_SPLIT] [--kmer KMER] [--rawfeatures] [--clusteringloss] [--targetmetric TARGETMETRIC] [--concatfeatures]
+               [--no_loss_weights] [--no_sample_weights] [--early_stopping EARLY_STOPPING] [--nruns NRUNS] [--mincontig MINCONTIG] [--minbin MINBIN] [--mincomp MINCOMP] [--randomize] [--labelgraph] [--binarize] [--noedges]
+               [--read_embs] [--reload] [--markers MARKERS] [--post POST] [--skip_preclustering] [--outname OUTNAME] [--cuda] [--noise] [--savemodel] [--tsne] [--numcores NUMCORES] [--outdir OUTDIR]
+               [--assembly_type ASSEMBLY_TYPE] [--contignodes] [--seed SEED] [--quiet] [--read_cache] [--version] [--loglevel LOGLEVEL] [--configfile CONFIGFILE]
+
+Train graph embedding model
+
+
+
+options:
+  -h, --help            show this help message and exit
+  --assembly ASSEMBLY   Assembly base path
+  --assembly_name ASSEMBLY_NAME
+                        File name with contigs
+  --graph_file GRAPH_FILE
+                        File name with graph
+  --edge_threshold EDGE_THRESHOLD
+                        Remove edges with weight lower than this (keep only >=)
+  --depth DEPTH         Depth file from jgi
+  --features FEATURES   Features file mapping contig name to features
+  --labels LABELS       File mapping contig to label
+  --embs EMBS           No train, load embs
+  --model_name MODEL_NAME
+                        One of the implemented models
+  --activation ACTIVATION
+                        Activation function to use(relu, prelu, sigmoid, tanh)
+  --layers_vae LAYERS_VAE
+                        Number of layers of the VAE
+  --layers_gnn LAYERS_GNN
+                        Number of layers of the GNN
+  --hidden_gnn HIDDEN_GNN
+                        Dimension of hidden layers of GNN
+  --hidden_vae HIDDEN_VAE
+                        Dimension of hidden layers of VAE
+  --embsize_gnn EMBSIZE_GNN, --zg EMBSIZE_GNN
+                        Output embedding dimension of GNN
+  --embsize_vae EMBSIZE_VAE, --zl EMBSIZE_VAE
+                        Output embedding dimension of VAE
+  --batchsize BATCHSIZE
+                        batchsize to train the VAE
+  --batchtype BATCHTYPE
+                        Batch type, nodes or edges
+  --dropout_gnn DROPOUT_GNN
+                        dropout of the GNN
+  --dropout_vae DROPOUT_VAE
+                        dropout of the VAE
+  --lr_gnn LR_GNN       learning rate
+  --lr_vae LR_VAE       learning rate
+  --graph_alpha GRAPH_ALPHA
+                        Coeficient for graph loss
+  --kld_alpha KLD_ALPHA
+                        Coeficient for KLD loss
+  --ae_alpha AE_ALPHA   Coeficient for AE loss
+  --scg_alpha SCG_ALPHA
+                        Coeficient for SCG loss
+  --clusteringalgo CLUSTERINGALGO
+                        clustering algorithm
+  --kclusters KCLUSTERS
+                        Number of clusters (only for some clustering methods)
+  --aggtype AGGTYPE     Aggregation type for GraphSAGE (mean, pool, lstm, gcn)
+  --decoder_input DECODER_INPUT
+                        What to use for input to the decoder
+  --vaepretrain VAEPRETRAIN
+                        How many epochs to pretrain VAE
+  --ae_only             Do not use GNN (ae model must be used and decoder input must be ae
+  --negatives NEGATIVES
+                        Number of negatives to train GraphSAGE
+  --quick               Reduce number of nodes to run quicker
+  --classify            Run classification instead of clustering
+  --fanout FANOUT       Fan out, number of positive neighbors sampled at each level
+  --epoch EPOCH         Number of epochs to train model
+  --print PRINT         Print interval during training
+  --evalepochs EVALEPOCHS
+                        Epoch interval to run eval
+  --evalskip EVALSKIP   Skip eval of these epochs
+  --eval_split EVAL_SPLIT
+                        Percentage of dataset to use for eval
+  --kmer KMER
+  --rawfeatures         Use raw features
+  --clusteringloss      Train with clustering loss
+  --targetmetric TARGETMETRIC
+                        Metric to pick best epoch
+  --concatfeatures      Concat learned and original features before clustering
+  --no_loss_weights     Using edge weights for loss (positive only)
+  --no_sample_weights   Using edge weights to sample negatives
+  --early_stopping EARLY_STOPPING
+                        Stop training if delta between last two losses is less than this
+  --nruns NRUNS         Number of runs
+  --mincontig MINCONTIG
+                        Minimum size of input contigs
+  --minbin MINBIN       Minimum size of clusters in bp
+  --mincomp MINCOMP     Minimum size of connected components
+  --randomize           Randomize graph
+  --labelgraph          Create graph based on labels (ignore assembly graph)
+  --binarize            Binarize adj matrix
+  --noedges             Remove all but self edges from adj matrix
+  --read_embs           Read embeddings from file
+  --reload              Reload data
+  --markers MARKERS     File with precomputed checkm results to eval
+  --post POST           Output options
+  --skip_preclustering  Use precomputed checkm results to eval
+  --outname OUTNAME, --outputname OUTNAME
+                        Output (experiment) name
+  --cuda                Use gpu
+  --noise               Use noise generator
+  --savemodel           Save best model to disk
+  --tsne                Plot tsne at checkpoints
+  --numcores NUMCORES   Number of cores to use
+  --outdir OUTDIR, --outputdir OUTDIR
+                        Output dir (same as input assembly dir if not defined
+  --assembly_type ASSEMBLY_TYPE
+                        flye or spades
+  --contignodes         Use contigs as nodes instead of edges
+  --seed SEED           Set seed
+  --quiet, -q           Do not output epoch progress
+  --read_cache          Do not check assembly files, read cached files only
+  --version, -v         Print version and exit
+  --loglevel LOGLEVEL, -l LOGLEVEL
+                        Log level
+
+```
```

### Comparing `graphmb-0.2.4/src/graphmb/amber_eval.py` & `graphmb-0.2.5/src/graphmb/amber_eval.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,220 +1,220 @@
-from collections import OrderedDict
-from collections import defaultdict
-import itertools
-import pandas as pd
-from graphmb.contigsdataset import process_node_name
-
-
-def write_amber_bins(contig_to_bin, outputfile):
-    with open(outputfile, "w") as f:
-        f.write("#\n@Version:0.9.0\n@SampleID:SAMPLEID\n@@SEQUENCEID\tBINID\n")
-        for c in contig_to_bin:
-            f.write(f"{str(c)}\t{str(contig_to_bin[c])}\n")
-
-# adapt eval scripts from amber but simplified
-
-
-def load_binnings(file_path_query, assemblytype, columns=["SEQUENCEID", "BINID"]):
-    # columns = ["SEQUENCEID", "BINID", "TAXID", "LENGTH", "_LENGTH"]
-    # sample_id_to_query_df = OrderedDict()
-    #for metadata in columns:
-        # logging.getLogger('amber').info('Loading ' + metadata[2]['SAMPLEID'])
-        # nrows = metadata[1] - metadata[0] + 1
-        # col_indices = [k for k, v in metadata[3].items() if v in columns]
-        # amber files start with 4 header lines
-    df = pd.read_csv(file_path_query, sep="\t", comment="#", skiprows=3, header=0)  # , usecols=col_indices)
-    df = df.rename(columns={df.columns[i]: c for i, c in enumerate(columns)}, inplace=False)
-    df = df.astype({'SEQUENCEID':'string'})
-    df["SEQUENCEID"]= df["SEQUENCEID"].apply(process_node_name, assembly_type=assemblytype)
-    if "_LENGTH" in columns:
-        df.rename(columns={"_LENGTH": "LENGTH"}, inplace=True)
-        df["LENGTH"] = pd.to_numeric(df["LENGTH"])
-    return df
-
-
-def amber_eval(gs_path, bin_path, labels=["graphmb"], assemblytype="flye"):
-    gs_df = load_binnings(gs_path, columns=["SEQUENCEID", "BINID", "_LENGTH"], assemblytype=assemblytype)
-    bin_df = load_binnings(bin_path, assemblytype=assemblytype)
-    # load_queries(gs_df, bin_df, labels=labels, options, options_gs)
-    gs_df = gs_df[["SEQUENCEID", "BINID", "LENGTH"]].rename(columns={"LENGTH": "seq_length",
-                                                                       "BINID": "genome_id",
-                                                                       "SEQUENCEID": "SEQUENCEID"})
-    bin_df = bin_df[["SEQUENCEID", "BINID"]].rename(columns={"SEQUENCEID": "SEQUENCEID"})
-    gs_df["seq_length"] = pd.to_numeric(gs_df["seq_length"])
-    query_df = bin_df[["SEQUENCEID", "BINID"]]
-    query_w_length = pd.merge(query_df, gs_df.drop_duplicates("SEQUENCEID"), on="SEQUENCEID", sort=False)
-    query_w_length_no_dups = query_w_length.drop_duplicates("SEQUENCEID")
-    gs_df_no_dups = gs_df.drop_duplicates("SEQUENCEID")
-    percentage_of_assigned_bps = query_w_length_no_dups["seq_length"].sum() / gs_df_no_dups["seq_length"].sum()
-    percentage_of_assigned_seqs = query_w_length_no_dups.shape[0] / gs_df_no_dups["SEQUENCEID"].shape[0]
-    query_w_length_mult_seqs = query_df.reset_index().merge(gs_df, on="SEQUENCEID", sort=False)
-    """if query_w_length.shape[0] < query_w_length_mult_seqs.shape[0]:
-        query_w_length_mult_seqs.drop_duplicates(['index', 'genome_id'], inplace=True)
-        confusion_df = query_w_length_mult_seqs.groupby(['BINID', 'genome_id'], sort=False).agg({'seq_length': 'sum', 'SEQUENCEID': 'count'}).rename(columns={'seq_length': 'genome_length', 'SEQUENCEID': 'genome_seq_counts'})
-
-        most_abundant_genome_df = confusion_df.loc[confusion_df.groupby('BINID', sort=False)['genome_length'].idxmax()]
-        most_abundant_genome_df = most_abundant_genome_df.reset_index()[['BINID', 'genome_id']]
-
-        matching_genomes_df = pd.merge(query_w_length_mult_seqs, most_abundant_genome_df, on=['BINID', 'genome_id']).set_index('index')
-        query_w_length_mult_seqs.set_index('index', inplace=True)
-        difference_df = query_w_length_mult_seqs.drop(matching_genomes_df.index).groupby(['index'], sort=False).first()
-        query_w_length = pd.concat([matching_genomes_df, difference_df])
-
-        # Modify gs such that multiple binnings of the same sequence are not required
-        matching_genomes_df = pd.merge(gs_df, query_w_length[['SEQUENCEID', 'genome_id']], on=['SEQUENCEID', 'genome_id'])
-        matching_genomes_df = matching_genomes_df[['SEQUENCEID', 'genome_id', 'seq_length']].drop_duplicates(['SEQUENCEID', 'genome_id'])
-        condition = gs_df_no_dups['SEQUENCEID'].isin(matching_genomes_df['SEQUENCEID'])
-        difference_df = gs_df_no_dups[~condition]
-        gs_df = pd.concat([difference_df, matching_genomes_df])"""
-
-    # query_w_length_mult_seqs.reset_index(inplace=True)
-    # query_w_length_mult_seqs = pd.merge(query_w_length_mult_seqs, most_abundant_genome_df, on=['BINID'])
-    # grouped = query_w_length_mult_seqs.groupby(['index'], sort=False, as_index=False)
-    # query_w_length = grouped.apply(lambda x: x[x['genome_id_x'] == x['genome_id_y'] if any(x['genome_id_x'] == x['genome_id_y']) else len(x) * [True]])
-    # query_w_length = query_w_length.groupby(['index'], sort=False).first().drop(columns='genome_id_y').rename(columns={'genome_id_x': 'genome_id'})
-
-    df = query_w_length
-
-    confusion_df = (
-        query_w_length.groupby(["BINID", "genome_id"], sort=False)
-        .agg({"seq_length": "sum", "SEQUENCEID": "count"})
-        .rename(columns={"seq_length": "genome_length", "SEQUENCEID": "genome_seq_counts"})
-    )
-    # self.confusion_df = confusion_df
-
-    # rand_index_bp, adjusted_rand_index_bp = Metrics.compute_rand_index(
-    #    confusion_df, "BINID", "genome_id", "genome_length"
-    # )
-    # rand_index_seq, adjusted_rand_index_seq = Metrics.compute_rand_index(
-    #    confusion_df, "BINID", "genome_id", "genome_seq_counts"
-    # )
-
-    most_abundant_genome_df = (
-        confusion_df.loc[confusion_df.groupby("BINID", sort=False)["genome_length"].idxmax()]
-        .reset_index()
-        .set_index("BINID")
-    )
-
-    query_w_length["seq_length_mean"] = query_w_length["seq_length"]
-
-    precision_df = (
-        query_w_length.groupby("BINID", sort=False)
-        .agg({"seq_length": "sum", "seq_length_mean": "mean", "SEQUENCEID": "count"})
-        .rename(columns={"seq_length": "total_length", "SEQUENCEID": "total_seq_counts"})
-    )
-    precision_df = pd.merge(precision_df, most_abundant_genome_df, on="BINID")
-    precision_df.rename(columns={"genome_length": "tp_length", "genome_seq_counts": "tp_seq_counts"}, inplace=True)
-    precision_df["precision_bp"] = precision_df["tp_length"] / precision_df["total_length"]
-    precision_df["precision_seq"] = precision_df["tp_seq_counts"] / precision_df["total_seq_counts"]
-
-    """if self.options.filter_tail_percentage:
-        precision_df['total_length_pct'] = precision_df['total_length'] / precision_df['total_length'].sum()
-        precision_df.sort_values(by='total_length', inplace=True)
-        precision_df['cumsum_length_pct'] = precision_df['total_length_pct'].cumsum(axis=0)
-        precision_df['precision_bp'].mask(precision_df['cumsum_length_pct'] <= self.options.filter_tail_percentage / 100, inplace=True)
-        precision_df['precision_seq'].mask(precision_df['precision_bp'].isna(), inplace=True)
-        precision_df.drop(columns=['cumsum_length_pct', 'total_length_pct'], inplace=True)
-    if self.options.genome_to_unique_common:
-        precision_df = precision_df[~precision_df['genome_id'].isin(self.options.genome_to_unique_common)]"""
-
-    precision_avg_bp = precision_df["precision_bp"].mean()
-    precision_avg_bp_sem = precision_df["precision_bp"].sem()
-    precision_avg_bp_var = precision_df["precision_bp"].var()
-    precision_avg_seq = precision_df["precision_seq"].mean()
-    precision_avg_seq_sem = precision_df["precision_seq"].sem()
-    precision_weighted_bp = precision_df["tp_length"].sum() / precision_df["total_length"].sum()
-    precision_weighted_seq = precision_df["tp_seq_counts"].sum() / precision_df["total_seq_counts"].sum()
-
-    genome_sizes_df = (
-        gs_df.groupby("genome_id", sort=False)
-        .agg({"seq_length": "sum", "SEQUENCEID": "count"})
-        .rename(columns={"seq_length": "length_gs", "SEQUENCEID": "seq_counts_gs"})
-    )
-    precision_df = (
-        precision_df.reset_index().join(genome_sizes_df, on="genome_id", how="left", sort=False).set_index("BINID")
-    )
-    precision_df["recall_bp"] = precision_df["tp_length"] / precision_df["length_gs"]
-    precision_df["recall_seq"] = precision_df["tp_seq_counts"] / precision_df["seq_counts_gs"]
-    precision_df["rank"] = "NA"
-
-    recall_df = confusion_df.loc[confusion_df.groupby("genome_id", sort=False)["genome_length"].idxmax()]
-    recall_df = (
-        recall_df.reset_index().join(genome_sizes_df, on="genome_id", how="right", sort=False).set_index("BINID")
-    )
-    recall_df.fillna({"genome_length": 0, "genome_seq_counts": 0}, inplace=True)
-    recall_df["recall_bp"] = recall_df["genome_length"] / recall_df["length_gs"]
-    recall_df["recall_seq"] = recall_df["genome_seq_counts"] / recall_df["seq_counts_gs"]
-
-    recall_df = recall_df.join(precision_df[["total_length", "seq_length_mean"]], how="left", sort=False)
-
-    # if self.options.genome_to_unique_common:
-    #    recall_df = recall_df[~recall_df["genome_id"].isin(self.options.genome_to_unique_common)]
-
-    recall_avg_bp = recall_df["recall_bp"].mean()
-    recall_avg_bp_var = recall_df["recall_bp"].var()
-    recall_avg_bp_sem = recall_df["recall_bp"].sem()
-    recall_avg_seq = recall_df["recall_seq"].mean()
-    recall_avg_seq_sem = recall_df["recall_seq"].sem()
-    recall_weighted_bp = recall_df["genome_length"].sum() / recall_df["length_gs"].sum()
-    recall_weighted_seq = recall_df["genome_seq_counts"].sum() / recall_df["seq_counts_gs"].sum()
-
-    # Compute recall as in CAMI 1
-    """unmapped_genomes = set(gs_df["genome_id"].unique()) - set(precision_df["genome_id"].unique())
-    #if self.options.genome_to_unique_common:
-    #    unmapped_genomes -= set(self.options.genome_to_unique_common)
-    num_unmapped_genomes = len(unmapped_genomes)
-    prec_copy = precision_df.reset_index()
-    if num_unmapped_genomes:
-        prec_copy = prec_copy.reindex(
-            prec_copy.index.tolist() + list(range(len(prec_copy), len(prec_copy) + num_unmapped_genomes))
-        ).fillna(0.0)
-    self.metrics.recall_avg_bp_cami1 = prec_copy["recall_bp"].mean()
-    self.metrics.recall_avg_seq_cami1 = prec_copy["recall_seq"].mean()
-    self.metrics.recall_avg_bp_sem_cami1 = prec_copy["recall_bp"].sem()
-    self.metrics.recall_avg_seq_sem_cami1 = prec_copy["recall_seq"].sem()
-    self.metrics.recall_avg_bp_var_cami1 = prec_copy["recall_bp"].var()
-    self.recall_df_cami1 = prec_copy"""
-    # End Compute recall as in CAMI 1
-
-    accuracy_bp = precision_df["tp_length"].sum() / recall_df["length_gs"].sum()
-    accuracy_seq = precision_df["tp_seq_counts"].sum() / recall_df["seq_counts_gs"].sum()
-
-    precision_df = precision_df.sort_values(by=["recall_bp"], axis=0, ascending=False)
-    recall_df = recall_df
-    metrics = {
-        "precision_avg_bp": precision_avg_bp,
-        "precision_avg_bp_sem": precision_avg_bp_sem,
-        "precision_avg_bp_var": precision_avg_bp_var,
-        "precision_avg_seq": precision_avg_seq,
-        "precision_avg_seq_sem": precision_avg_seq_sem,
-        "precision_weighted_bp": precision_weighted_bp,
-        "precision_weighted_seq": precision_weighted_seq,
-        "recall_avg_bp": recall_avg_bp,
-        "recall_avg_bp_sem": recall_avg_bp_sem,
-        "recall_avg_bp_var": recall_avg_bp_var,
-        "recall_avg_seq": recall_avg_seq,
-        "recall_avg_seq_sem": recall_avg_seq_sem,
-        "recall_weighted_bp": recall_weighted_bp,
-        "recall_weighted_seq": recall_weighted_seq,
-        "accuracy_bp": accuracy_bp,
-        "accuracy_seq": accuracy_seq,
-        "f1_avg_bp": (2*precision_avg_bp*recall_avg_bp)/(precision_avg_bp+recall_avg_bp) if (precision_avg_bp+recall_avg_bp) > 0 else 0
-    }
-    bins_eval = calc_num_recovered_genomes(precision_df, [0.9, 0.5], [0.05, 0.1])
-    return metrics, bins_eval
-
-
-def calc_num_recovered_genomes(bins, min_completeness, max_contamination):
-    counts_list = []
-    for x in itertools.product(min_completeness, max_contamination):
-        count = bins[(bins["recall_bp"] > x[0]) & (bins["precision_bp"] > (1 - x[1]))].shape[0]
-        counts_list.append(("> " + str(int(x[0] * 100)) + "% completeness", "< " + str(int(x[1] * 100)) + "%", count))
-
-    pd_counts = pd.DataFrame(counts_list, columns=["Completeness", "Contamination", "count"])
-    pd_counts = pd.pivot_table(
-        pd_counts,
-        values="count",
-        index=["Contamination"],
-        columns=["Completeness"],
-    ).reset_index()
-    return pd_counts
+from collections import OrderedDict
+from collections import defaultdict
+import itertools
+import pandas as pd
+from graphmb.contigsdataset import process_node_name
+
+
+def write_amber_bins(contig_to_bin, outputfile):
+    with open(outputfile, "w") as f:
+        f.write("#\n@Version:0.9.0\n@SampleID:SAMPLEID\n@@SEQUENCEID\tBINID\n")
+        for c in contig_to_bin:
+            f.write(f"{str(c)}\t{str(contig_to_bin[c])}\n")
+
+# adapt eval scripts from amber but simplified
+
+
+def load_binnings(file_path_query, assemblytype, columns=["SEQUENCEID", "BINID"]):
+    # columns = ["SEQUENCEID", "BINID", "TAXID", "LENGTH", "_LENGTH"]
+    # sample_id_to_query_df = OrderedDict()
+    #for metadata in columns:
+        # logging.getLogger('amber').info('Loading ' + metadata[2]['SAMPLEID'])
+        # nrows = metadata[1] - metadata[0] + 1
+        # col_indices = [k for k, v in metadata[3].items() if v in columns]
+        # amber files start with 4 header lines
+    df = pd.read_csv(file_path_query, sep="\t", comment="#", skiprows=3, header=0)  # , usecols=col_indices)
+    df = df.rename(columns={df.columns[i]: c for i, c in enumerate(columns)}, inplace=False)
+    df = df.astype({'SEQUENCEID':'string'})
+    df["SEQUENCEID"]= df["SEQUENCEID"].apply(process_node_name, assembly_type=assemblytype)
+    if "_LENGTH" in columns:
+        df.rename(columns={"_LENGTH": "LENGTH"}, inplace=True)
+        df["LENGTH"] = pd.to_numeric(df["LENGTH"])
+    return df
+
+
+def amber_eval(gs_path, bin_path, labels=["graphmb"], assemblytype="flye"):
+    gs_df = load_binnings(gs_path, columns=["SEQUENCEID", "BINID", "_LENGTH"], assemblytype=assemblytype)
+    bin_df = load_binnings(bin_path, assemblytype=assemblytype)
+    # load_queries(gs_df, bin_df, labels=labels, options, options_gs)
+    gs_df = gs_df[["SEQUENCEID", "BINID", "LENGTH"]].rename(columns={"LENGTH": "seq_length",
+                                                                       "BINID": "genome_id",
+                                                                       "SEQUENCEID": "SEQUENCEID"})
+    bin_df = bin_df[["SEQUENCEID", "BINID"]].rename(columns={"SEQUENCEID": "SEQUENCEID"})
+    gs_df["seq_length"] = pd.to_numeric(gs_df["seq_length"])
+    query_df = bin_df[["SEQUENCEID", "BINID"]]
+    query_w_length = pd.merge(query_df, gs_df.drop_duplicates("SEQUENCEID"), on="SEQUENCEID", sort=False)
+    query_w_length_no_dups = query_w_length.drop_duplicates("SEQUENCEID")
+    gs_df_no_dups = gs_df.drop_duplicates("SEQUENCEID")
+    percentage_of_assigned_bps = query_w_length_no_dups["seq_length"].sum() / gs_df_no_dups["seq_length"].sum()
+    percentage_of_assigned_seqs = query_w_length_no_dups.shape[0] / gs_df_no_dups["SEQUENCEID"].shape[0]
+    query_w_length_mult_seqs = query_df.reset_index().merge(gs_df, on="SEQUENCEID", sort=False)
+    """if query_w_length.shape[0] < query_w_length_mult_seqs.shape[0]:
+        query_w_length_mult_seqs.drop_duplicates(['index', 'genome_id'], inplace=True)
+        confusion_df = query_w_length_mult_seqs.groupby(['BINID', 'genome_id'], sort=False).agg({'seq_length': 'sum', 'SEQUENCEID': 'count'}).rename(columns={'seq_length': 'genome_length', 'SEQUENCEID': 'genome_seq_counts'})
+
+        most_abundant_genome_df = confusion_df.loc[confusion_df.groupby('BINID', sort=False)['genome_length'].idxmax()]
+        most_abundant_genome_df = most_abundant_genome_df.reset_index()[['BINID', 'genome_id']]
+
+        matching_genomes_df = pd.merge(query_w_length_mult_seqs, most_abundant_genome_df, on=['BINID', 'genome_id']).set_index('index')
+        query_w_length_mult_seqs.set_index('index', inplace=True)
+        difference_df = query_w_length_mult_seqs.drop(matching_genomes_df.index).groupby(['index'], sort=False).first()
+        query_w_length = pd.concat([matching_genomes_df, difference_df])
+
+        # Modify gs such that multiple binnings of the same sequence are not required
+        matching_genomes_df = pd.merge(gs_df, query_w_length[['SEQUENCEID', 'genome_id']], on=['SEQUENCEID', 'genome_id'])
+        matching_genomes_df = matching_genomes_df[['SEQUENCEID', 'genome_id', 'seq_length']].drop_duplicates(['SEQUENCEID', 'genome_id'])
+        condition = gs_df_no_dups['SEQUENCEID'].isin(matching_genomes_df['SEQUENCEID'])
+        difference_df = gs_df_no_dups[~condition]
+        gs_df = pd.concat([difference_df, matching_genomes_df])"""
+
+    # query_w_length_mult_seqs.reset_index(inplace=True)
+    # query_w_length_mult_seqs = pd.merge(query_w_length_mult_seqs, most_abundant_genome_df, on=['BINID'])
+    # grouped = query_w_length_mult_seqs.groupby(['index'], sort=False, as_index=False)
+    # query_w_length = grouped.apply(lambda x: x[x['genome_id_x'] == x['genome_id_y'] if any(x['genome_id_x'] == x['genome_id_y']) else len(x) * [True]])
+    # query_w_length = query_w_length.groupby(['index'], sort=False).first().drop(columns='genome_id_y').rename(columns={'genome_id_x': 'genome_id'})
+
+    df = query_w_length
+
+    confusion_df = (
+        query_w_length.groupby(["BINID", "genome_id"], sort=False)
+        .agg({"seq_length": "sum", "SEQUENCEID": "count"})
+        .rename(columns={"seq_length": "genome_length", "SEQUENCEID": "genome_seq_counts"})
+    )
+    # self.confusion_df = confusion_df
+
+    # rand_index_bp, adjusted_rand_index_bp = Metrics.compute_rand_index(
+    #    confusion_df, "BINID", "genome_id", "genome_length"
+    # )
+    # rand_index_seq, adjusted_rand_index_seq = Metrics.compute_rand_index(
+    #    confusion_df, "BINID", "genome_id", "genome_seq_counts"
+    # )
+
+    most_abundant_genome_df = (
+        confusion_df.loc[confusion_df.groupby("BINID", sort=False)["genome_length"].idxmax()]
+        .reset_index()
+        .set_index("BINID")
+    )
+
+    query_w_length["seq_length_mean"] = query_w_length["seq_length"]
+
+    precision_df = (
+        query_w_length.groupby("BINID", sort=False)
+        .agg({"seq_length": "sum", "seq_length_mean": "mean", "SEQUENCEID": "count"})
+        .rename(columns={"seq_length": "total_length", "SEQUENCEID": "total_seq_counts"})
+    )
+    precision_df = pd.merge(precision_df, most_abundant_genome_df, on="BINID")
+    precision_df.rename(columns={"genome_length": "tp_length", "genome_seq_counts": "tp_seq_counts"}, inplace=True)
+    precision_df["precision_bp"] = precision_df["tp_length"] / precision_df["total_length"]
+    precision_df["precision_seq"] = precision_df["tp_seq_counts"] / precision_df["total_seq_counts"]
+
+    """if self.options.filter_tail_percentage:
+        precision_df['total_length_pct'] = precision_df['total_length'] / precision_df['total_length'].sum()
+        precision_df.sort_values(by='total_length', inplace=True)
+        precision_df['cumsum_length_pct'] = precision_df['total_length_pct'].cumsum(axis=0)
+        precision_df['precision_bp'].mask(precision_df['cumsum_length_pct'] <= self.options.filter_tail_percentage / 100, inplace=True)
+        precision_df['precision_seq'].mask(precision_df['precision_bp'].isna(), inplace=True)
+        precision_df.drop(columns=['cumsum_length_pct', 'total_length_pct'], inplace=True)
+    if self.options.genome_to_unique_common:
+        precision_df = precision_df[~precision_df['genome_id'].isin(self.options.genome_to_unique_common)]"""
+
+    precision_avg_bp = precision_df["precision_bp"].mean()
+    precision_avg_bp_sem = precision_df["precision_bp"].sem()
+    precision_avg_bp_var = precision_df["precision_bp"].var()
+    precision_avg_seq = precision_df["precision_seq"].mean()
+    precision_avg_seq_sem = precision_df["precision_seq"].sem()
+    precision_weighted_bp = precision_df["tp_length"].sum() / precision_df["total_length"].sum()
+    precision_weighted_seq = precision_df["tp_seq_counts"].sum() / precision_df["total_seq_counts"].sum()
+
+    genome_sizes_df = (
+        gs_df.groupby("genome_id", sort=False)
+        .agg({"seq_length": "sum", "SEQUENCEID": "count"})
+        .rename(columns={"seq_length": "length_gs", "SEQUENCEID": "seq_counts_gs"})
+    )
+    precision_df = (
+        precision_df.reset_index().join(genome_sizes_df, on="genome_id", how="left", sort=False).set_index("BINID")
+    )
+    precision_df["recall_bp"] = precision_df["tp_length"] / precision_df["length_gs"]
+    precision_df["recall_seq"] = precision_df["tp_seq_counts"] / precision_df["seq_counts_gs"]
+    precision_df["rank"] = "NA"
+
+    recall_df = confusion_df.loc[confusion_df.groupby("genome_id", sort=False)["genome_length"].idxmax()]
+    recall_df = (
+        recall_df.reset_index().join(genome_sizes_df, on="genome_id", how="right", sort=False).set_index("BINID")
+    )
+    recall_df.fillna({"genome_length": 0, "genome_seq_counts": 0}, inplace=True)
+    recall_df["recall_bp"] = recall_df["genome_length"] / recall_df["length_gs"]
+    recall_df["recall_seq"] = recall_df["genome_seq_counts"] / recall_df["seq_counts_gs"]
+
+    recall_df = recall_df.join(precision_df[["total_length", "seq_length_mean"]], how="left", sort=False)
+
+    # if self.options.genome_to_unique_common:
+    #    recall_df = recall_df[~recall_df["genome_id"].isin(self.options.genome_to_unique_common)]
+
+    recall_avg_bp = recall_df["recall_bp"].mean()
+    recall_avg_bp_var = recall_df["recall_bp"].var()
+    recall_avg_bp_sem = recall_df["recall_bp"].sem()
+    recall_avg_seq = recall_df["recall_seq"].mean()
+    recall_avg_seq_sem = recall_df["recall_seq"].sem()
+    recall_weighted_bp = recall_df["genome_length"].sum() / recall_df["length_gs"].sum()
+    recall_weighted_seq = recall_df["genome_seq_counts"].sum() / recall_df["seq_counts_gs"].sum()
+
+    # Compute recall as in CAMI 1
+    """unmapped_genomes = set(gs_df["genome_id"].unique()) - set(precision_df["genome_id"].unique())
+    #if self.options.genome_to_unique_common:
+    #    unmapped_genomes -= set(self.options.genome_to_unique_common)
+    num_unmapped_genomes = len(unmapped_genomes)
+    prec_copy = precision_df.reset_index()
+    if num_unmapped_genomes:
+        prec_copy = prec_copy.reindex(
+            prec_copy.index.tolist() + list(range(len(prec_copy), len(prec_copy) + num_unmapped_genomes))
+        ).fillna(0.0)
+    self.metrics.recall_avg_bp_cami1 = prec_copy["recall_bp"].mean()
+    self.metrics.recall_avg_seq_cami1 = prec_copy["recall_seq"].mean()
+    self.metrics.recall_avg_bp_sem_cami1 = prec_copy["recall_bp"].sem()
+    self.metrics.recall_avg_seq_sem_cami1 = prec_copy["recall_seq"].sem()
+    self.metrics.recall_avg_bp_var_cami1 = prec_copy["recall_bp"].var()
+    self.recall_df_cami1 = prec_copy"""
+    # End Compute recall as in CAMI 1
+
+    accuracy_bp = precision_df["tp_length"].sum() / recall_df["length_gs"].sum()
+    accuracy_seq = precision_df["tp_seq_counts"].sum() / recall_df["seq_counts_gs"].sum()
+
+    precision_df = precision_df.sort_values(by=["recall_bp"], axis=0, ascending=False)
+    recall_df = recall_df
+    metrics = {
+        "precision_avg_bp": precision_avg_bp,
+        "precision_avg_bp_sem": precision_avg_bp_sem,
+        "precision_avg_bp_var": precision_avg_bp_var,
+        "precision_avg_seq": precision_avg_seq,
+        "precision_avg_seq_sem": precision_avg_seq_sem,
+        "precision_weighted_bp": precision_weighted_bp,
+        "precision_weighted_seq": precision_weighted_seq,
+        "recall_avg_bp": recall_avg_bp,
+        "recall_avg_bp_sem": recall_avg_bp_sem,
+        "recall_avg_bp_var": recall_avg_bp_var,
+        "recall_avg_seq": recall_avg_seq,
+        "recall_avg_seq_sem": recall_avg_seq_sem,
+        "recall_weighted_bp": recall_weighted_bp,
+        "recall_weighted_seq": recall_weighted_seq,
+        "accuracy_bp": accuracy_bp,
+        "accuracy_seq": accuracy_seq,
+        "f1_avg_bp": (2*precision_avg_bp*recall_avg_bp)/(precision_avg_bp+recall_avg_bp) if (precision_avg_bp+recall_avg_bp) > 0 else 0
+    }
+    bins_eval = calc_num_recovered_genomes(precision_df, [0.9, 0.5], [0.05, 0.1])
+    return metrics, bins_eval
+
+
+def calc_num_recovered_genomes(bins, min_completeness, max_contamination):
+    counts_list = []
+    for x in itertools.product(min_completeness, max_contamination):
+        count = bins[(bins["recall_bp"] > x[0]) & (bins["precision_bp"] > (1 - x[1]))].shape[0]
+        counts_list.append(("> " + str(int(x[0] * 100)) + "% completeness", "< " + str(int(x[1] * 100)) + "%", count))
+
+    pd_counts = pd.DataFrame(counts_list, columns=["Completeness", "Contamination", "count"])
+    pd_counts = pd.pivot_table(
+        pd_counts,
+        values="count",
+        index=["Contamination"],
+        columns=["Completeness"],
+    ).reset_index()
+    return pd_counts
```

### Comparing `graphmb-0.2.4/src/graphmb/arg_options.py` & `graphmb-0.2.5/src/graphmb/arg_options.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,116 +1,118 @@
-import argparse
-
-class LoadFromFile (argparse.Action):
-    def __call__ (self, parser, namespace, values, option_string = None):
-        with values as f:
-            contents = f.read()
-        # parse arguments in the file and store them in a blank namespace
-        data = parser.parse_args(contents.split(), namespace=None)
-        for k, v in vars(data).items():
-            # set arguments in the target namespace if they haven’t been set yet
-            #if getattr(namespace, k, None) is None:
-            #print(f"using args {k}={v}")
-            setattr(namespace, k, v)
-
-def create_parser():
-    parser = argparse.ArgumentParser(description="Train graph embedding model")
-    # input files
-    parser.add_argument("--assembly", type=str, help="Assembly base path", required=False)
-    parser.add_argument("--assembly_name", type=str, help="File name with contigs", default="assembly.fasta")
-    parser.add_argument("--graph_file", type=str, help="File name with graph", default="assembly_graph.gfa")
-    parser.add_argument("--edge_threshold", type=float, help="Remove edges with weight lower than this (keep only >=)",
-                        default=None)
-    parser.add_argument("--depth", type=str, help="Depth file from jgi", default="assembly_depth.txt")
-    parser.add_argument("--features", type=str, help="Features file mapping contig name to features",
-                        default="features.tsv")
-    parser.add_argument("--labels", type=str, help="File mapping contig to label", default=None)
-    parser.add_argument("--embs", type=str, help="No train, load embs", default=None)
-
-    # model specification
-    parser.add_argument("--model_name", type=str,
-                        help="One of the implemented models: gcn, gat, sage, sage_lstm, _ccvae variation",
-                        default="gcn")
-    parser.add_argument("--activation", type=str, help="Activation function to use(relu, prelu, sigmoid, tanh)",
-                        default="relu")
-    parser.add_argument("--layers_vae", type=int, help="Number of layers of the VAE", default=2)
-    parser.add_argument("--layers_gnn", type=int, help="Number of layers of the GNN", default=3)
-    parser.add_argument("--hidden_gnn", type=int, help="Dimension of hidden layers of GNN", default=128)
-    parser.add_argument("--hidden_vae", type=int, help="Dimension of hidden layers of VAE", default=512)
-    parser.add_argument("--embsize_gnn", "--zg", type=int, help="Output embedding dimension of GNN", default=32)
-    parser.add_argument("--embsize_vae", "--zl", type=int, help="Output embedding dimension of VAE", default=64)
-    parser.add_argument("--batchsize", type=int, help="batchsize to train the VAE", default=256)
-    parser.add_argument("--batchtype", type=str, help="Batch type, nodes or edges", default="auto")
-    parser.add_argument("--dropout_gnn", type=float, help="dropout of the GNN", default=0.1)
-    parser.add_argument("--dropout_vae", type=float, help="dropout of the VAE", default=0.2)
-    parser.add_argument("--lr_gnn", type=float, help="learning rate", default=1e-2)
-    parser.add_argument("--lr_vae", type=float, help="learning rate", default=1e-3)
-    parser.add_argument("--graph_alpha", type=float, help="Coeficient for graph loss", default=1)
-    parser.add_argument("--kld_alpha", type=float, help="Coeficient for KLD loss", default=200)
-    parser.add_argument("--ae_alpha", type=float, help="Coeficient for AE loss", default=1)
-    parser.add_argument("--scg_alpha", type=float, help="Coeficient for SCG loss", default=1)
-    parser.add_argument("--clusteringalgo", help="clustering algorithm: vamb, kmeans", default="vamb")
-    parser.add_argument("--kclusters", help="Number of clusters (only for some clustering methods)", default=None)
-    # GraphSAGE params
-    parser.add_argument("--aggtype", help="Aggregation type for GraphSAGE (mean, pool, lstm, gcn)", default="lstm")
-    parser.add_argument("--decoder_input", help="What to use for input to the decoder", default="vae")
-    parser.add_argument("--vaepretrain", help="How many epochs to pretrain VAE", default=500, type=int)
-    parser.add_argument("--ae_only", help="Do not use GNN (ae model must be used and decoder input must be ae", action="store_true")
-    parser.add_argument("--negatives", help="Number of negatives to train GraphSAGE", default=10, type=int)
-    parser.add_argument("--quick", help="Reduce number of nodes to run quicker", action="store_true")
-    parser.add_argument("--classify", help="Run classification instead of clustering", action="store_true")
-    parser.add_argument(
-        "--fanout", help="Fan out, number of positive neighbors sampled at each level", default="10,25"
-    )
-    # other training params
-    parser.add_argument("--epoch", type=int, help="Number of epochs to train model", default=500)
-    parser.add_argument("--print", type=int, help="Print interval during training", default=10)
-    parser.add_argument("--evalepochs", type=int, help="Epoch interval to run eval", default=20)
-    parser.add_argument("--evalskip", type=int, help="Skip eval of these epochs", default=50)
-    parser.add_argument("--eval_split", type=float, help="Percentage of dataset to use for eval", default=0.0)
-    parser.add_argument("--kmer", default=4)
-    parser.add_argument("--rawfeatures", help="Use raw features", action="store_true")
-    parser.add_argument("--clusteringloss", help="Train with clustering loss", action="store_true")
-    parser.add_argument("--targetmetric", help="Metric to pick best epoch", default="hq")
-    parser.add_argument("--concatfeatures", help="Concat learned and original features before clustering",
-                        action="store_true")
-    parser.add_argument("--no_loss_weights", action="store_false", help="Using edge weights for loss (positive only)")
-    parser.add_argument("--no_sample_weights", action="store_false", help="Using edge weights to sample negatives")
-    parser.add_argument(
-        "--early_stopping",
-        type=float,
-        help="Stop training if delta between last two losses is less than this",
-        default="0.1",
-    )
-    parser.add_argument("--nruns", type=int, help="Number of runs", default=1)
-    # data processing
-    parser.add_argument("--mincontig", type=int, help="Minimum size of input contigs", default=1000)
-    parser.add_argument("--minbin", type=int, help="Minimum size of clusters in bp", default=200000)
-    parser.add_argument("--mincomp", type=int, help="Minimum size of connected components", default=1)
-    parser.add_argument("--randomize", help="Randomize graph", action="store_true")
-    parser.add_argument("--labelgraph", help="Create graph based on labels (ignore assembly graph)", action="store_true")
-    parser.add_argument("--binarize", help="Binarize adj matrix", action="store_true")
-    parser.add_argument("--noedges", help="Remove all but self edges from adj matrix", action="store_true")
-    parser.add_argument("--read_embs", help="Read embeddings from file", action="store_true")
-    parser.add_argument("--reload", help="Reload data", action="store_true")
-
-    parser.add_argument("--markers", type=str, help="File with precomputed checkm results to eval",
-                        default="marker_gene_stats.tsv")
-    parser.add_argument("--post", help="Output options", default="writeembs_contig2bin")
-    parser.add_argument("--skip_preclustering", help="Use precomputed checkm results to eval", action="store_true")
-    parser.add_argument("--outname", "--outputname", help="Output (experiment) name", default="graphmb")
-    parser.add_argument("--cuda", help="Use gpu", action="store_true")
-    parser.add_argument("--noise", help="Use noise generator", action="store_true")
-    parser.add_argument("--savemodel", help="Save best model to disk", action="store_true")
-    parser.add_argument("--tsne", help="Plot tsne at checkpoints", action="store_true")
-    parser.add_argument("--numcores", help="Number of cores to use", default=1, type=int)
-    parser.add_argument(
-        "--outdir", "--outputdir", help="Output dir (same as input assembly dir if not defined", default=None
-    )
-    parser.add_argument("--assembly_type", help="flye or spades", default="flye")
-    parser.add_argument("--contignodes", help="Use contigs as nodes instead of edges", action="store_true")
-    parser.add_argument("--seed", help="Set seed", default=1, type=int)
-    parser.add_argument("--quiet", "-q", help="Do not output epoch progress", action="store_true")
-    parser.add_argument("--read_cache", help="Do not check assembly files, read cached files only", action="store_true")
-    parser.add_argument("--version", "-v", help="Print version and exit", action="store_true")
-    parser.add_argument("--loglevel", "-l", help="Log level", default="info")
-    return parser
+import argparse
+
+class LoadFromFile (argparse.Action):
+    def __call__ (self, parser, namespace, values, option_string = None):
+        with values as f:
+            contents = f.read()
+        # parse arguments in the file and store them in a blank namespace
+        data = parser.parse_args(contents.split(), namespace=None)
+        for k, v in vars(data).items():
+            # set arguments in the target namespace if they haven’t been set yet
+            #if getattr(namespace, k, None) is None:
+            #print(f"using args {k}={v}")
+            setattr(namespace, k, v)
+
+def create_parser():
+    parser = argparse.ArgumentParser(description="Train graph embedding model")
+    # input files
+    parser.add_argument("--assembly", type=str, help="Assembly base path", required=False)
+    parser.add_argument("--assembly_name", type=str, help="File name with contigs", default="assembly.fasta")
+    parser.add_argument("--graph_file", type=str, help="File name with graph", default="assembly_graph.gfa")
+    parser.add_argument("--edge_threshold", type=float, help="Remove edges with weight lower than this (keep only >=)",
+                        default=None)
+    parser.add_argument("--depth", type=str, help="Depth file from jgi", default="assembly_depth.txt")
+    parser.add_argument("--features", type=str, help="Features file mapping contig name to features",
+                        default="features.tsv")
+    parser.add_argument("--labels", type=str, help="File mapping contig to label", default=None)
+    parser.add_argument("--embs", type=str, help="No train, load embs", default=None)
+
+    # model specification
+    parser.add_argument("--model_name", type=str,
+                        help="One of the implemented models: gcn, gat, sage, sage_lstm, _ccvae variation",
+                        default="gcn")
+    parser.add_argument("--activation", type=str, help="Activation function to use(relu, prelu, sigmoid, tanh)",
+                        default="relu")
+    parser.add_argument("--layers_vae", type=int, help="Number of layers of the VAE", default=2)
+    parser.add_argument("--layers_gnn", type=int, help="Number of layers of the GNN", default=3)
+    parser.add_argument("--hidden_gnn", type=int, help="Dimension of hidden layers of GNN", default=128)
+    parser.add_argument("--hidden_vae", type=int, help="Dimension of hidden layers of VAE", default=512)
+    parser.add_argument("--embsize_gnn", "--zg", type=int, help="Output embedding dimension of GNN", default=32)
+    parser.add_argument("--embsize_vae", "--zl", type=int, help="Output embedding dimension of VAE", default=64)
+    parser.add_argument("--batchsize", type=int, help="batchsize to train the VAE", default=256)
+    parser.add_argument("--batchtype", type=str, help="Batch type, nodes or edges", default="auto")
+    parser.add_argument("--dropout_gnn", type=float, help="dropout of the GNN", default=0.1)
+    parser.add_argument("--dropout_vae", type=float, help="dropout of the VAE", default=0.2)
+    parser.add_argument("--lr_gnn", type=float, help="learning rate", default=1e-2)
+    parser.add_argument("--lr_vae", type=float, help="learning rate", default=1e-3)
+    parser.add_argument("--graph_alpha", type=float, help="Coeficient for graph loss", default=1)
+    parser.add_argument("--kld_alpha", type=float, help="Coeficient for KLD loss", default=200)
+    parser.add_argument("--ae_alpha", type=float, help="Coeficient for AE loss", default=1)
+    parser.add_argument("--scg_alpha", type=float, help="Coeficient for SCG loss", default=1)
+    parser.add_argument("--clusteringalgo", help="clustering algorithm: vamb, kmeans", default="vamb")
+    parser.add_argument("--kclusters", help="Number of clusters (only for some clustering methods)", default=None)
+    # GraphSAGE params
+    parser.add_argument("--aggtype", help="Aggregation type for GraphSAGE (mean, pool, lstm, gcn)", default="lstm")
+    parser.add_argument("--decoder_input", help="What to use for input to the decoder", default="vae")
+    parser.add_argument("--vaepretrain", help="How many epochs to pretrain VAE", default=500, type=int)
+    parser.add_argument("--ae_only", help="Do not use GNN (ae model must be used and decoder input must be ae", action="store_true")
+    parser.add_argument("--negatives", help="Number of negatives to train GraphSAGE", default=10, type=int)
+    parser.add_argument("--quick", help="Reduce number of nodes to run quicker", action="store_true")
+    parser.add_argument("--classify", help="Run classification instead of clustering", action="store_true")
+    parser.add_argument(
+        "--fanout", help="Fan out, number of positive neighbors sampled at each level", default="10,25"
+    )
+    # other training params
+    parser.add_argument("--epoch", type=int, help="Number of epochs to train model", default=500)
+    parser.add_argument("--print", type=int, help="Print interval during training", default=10)
+    parser.add_argument("--evalepochs", type=int, help="Epoch interval to run eval", default=20)
+    parser.add_argument("--evalskip", type=int, help="Skip eval of these epochs", default=50)
+    parser.add_argument("--eval_split", type=float, help="Percentage of dataset to use for eval", default=0.0)
+    parser.add_argument("--kmer", default=4)
+    parser.add_argument("--rawfeatures", help="Use raw features", action="store_true")
+    parser.add_argument("--clusteringloss", help="Train with clustering loss", action="store_true")
+    parser.add_argument("--targetmetric", help="Metric to pick best epoch", default="hq")
+    parser.add_argument("--concatfeatures", help="Concat learned and original features before clustering",
+                        action="store_true")
+    parser.add_argument("--no_loss_weights", action="store_false", help="Using edge weights for loss (positive only)")
+    parser.add_argument("--no_sample_weights", action="store_false", help="Using edge weights to sample negatives")
+    parser.add_argument(
+        "--early_stopping",
+        type=float,
+        help="Stop training if delta between last two losses is less than this",
+        default="0.1",
+    )
+    parser.add_argument("--nruns", type=int, help="Number of runs", default=1)
+    # data processing
+    parser.add_argument("--mincontig", type=int, help="Minimum size of input contigs", default=1000)
+    parser.add_argument("--minbin", type=int, help="Minimum size of clusters in bp", default=200000)
+    parser.add_argument("--mincomp", type=int, help="Minimum size of connected components", default=1)
+    parser.add_argument("--randomize", help="Randomize graph", action="store_true")
+    parser.add_argument("--labelgraph", help="Create graph based on labels (ignore assembly graph)", action="store_true")
+    parser.add_argument("--binarize", help="Binarize adj matrix", action="store_true")
+    parser.add_argument("--noedges", help="Remove all but self edges from adj matrix", action="store_true")
+    parser.add_argument("--read_embs", help="Read embeddings from file", action="store_true")
+    parser.add_argument("--reload", help="Reload data", action="store_true")
+
+    parser.add_argument("--markers", type=str, help="""File with precomputed checkm results to eval.
+                                                    If not found, it will assume it does not exist.""",
+                        default="marker_gene_stats.tsv")
+    parser.add_argument("--post", help="Output options", default="writeembs_contig2bin")
+    parser.add_argument("--writebins", help="Write bins to fasta files", action="store_true")
+    parser.add_argument("--skip_preclustering", help="Use precomputed checkm results to eval", action="store_true")
+    parser.add_argument("--outname", "--outputname", help="Output (experiment) name", default="graphmb")
+    parser.add_argument("--cuda", help="Use gpu", action="store_true")
+    parser.add_argument("--noise", help="Use noise generator", action="store_true")
+    parser.add_argument("--savemodel", help="Save best model to disk", action="store_true")
+    parser.add_argument("--tsne", help="Plot tsne at checkpoints", action="store_true")
+    parser.add_argument("--numcores", help="Number of cores to use", default=1, type=int)
+    parser.add_argument(
+        "--outdir", "--outputdir", help="Output dir (same as input assembly dir if not defined", default=None
+    )
+    parser.add_argument("--assembly_type", help="flye or spades", default="flye")
+    parser.add_argument("--contignodes", help="Use contigs as nodes instead of edges", action="store_true")
+    parser.add_argument("--seed", help="Set seed", default=1, type=int)
+    parser.add_argument("--quiet", "-q", help="Do not output epoch progress", action="store_true")
+    parser.add_argument("--read_cache", help="Do not check assembly files, read cached files only", action="store_true")
+    parser.add_argument("--version", "-v", help="Print version and exit", action="store_true")
+    parser.add_argument("--loglevel", "-l", help="Log level", default="info")
+    return parser
```

### Comparing `graphmb-0.2.4/src/graphmb/contigsdataset.py` & `graphmb-0.2.5/src/graphmb/contigsdataset.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,813 +1,813 @@
-from glob import escape
-#from importlib.resources import files #3.9 only
-from importlib_resources import files
-import itertools
-import random
-import os
-import pickle
-import pdb
-import shutil
-from typing import Dict, List, Tuple, Sequence
-from collections import Counter
-import numpy as np
-import networkx as nx
-import scipy.stats as stats
-import scipy.sparse
-from graphmb.evaluate import (
-    read_marker_gene_sets,
-    read_contig_genes,
-    get_markers_to_contigs,
-)
-
-
-#BACTERIA_MARKERS = "data/Bacteria.ms"
-#kernel = np.load("data/kernel.npz")['arr_0']
-BACTERIA_MARKERS = files('graphmb.data').joinpath('Bacteria.ms')
-kernel = np.load(files('graphmb.data').joinpath('kernel.npz'))['arr_0']
-
-def count_kmers(seq, k, kmer_to_id, canonical_k):
-    # Used in case kmers are used as input features
-    # https://stackoverflow.com/q/22428020
-    #breakpoint()
-    kmer_letters = set(["A", "T", "C", "G"])
-    kmers = [seq[i : i + k] for i in range(len(seq) - k + 1) if set(seq[i : i + k]).issubset(kmer_letters)]
-    kmers = [kmer_to_id[k] for k in kmers]
-    kmer_counts = Counter(kmers)
-    counts = np.array([kmer_counts[k] for k in range(canonical_k)])
-    counts = counts / counts.sum()
-    counts += -(1/(4**k))
-    counts = np.dot(counts, kernel)
-    return counts
-
-def get_kmer_to_id(kmer, combine_revcomp=False):
-    kmer_to_ids = {}
-    BASE_COMPLEMENT = {"A": "T", "T": "A", "G": "C", "C": "G"}
-    all_kmers = itertools.product("ACGT", repeat=kmer)
-    all_kmers = ["".join(k) for k in all_kmers]
-    new_id = 0
-    for kmer in all_kmers:
-        if kmer not in kmer_to_ids:
-            kmer_to_ids[kmer] = new_id
-            if combine_revcomp:
-                rev_compl = "".join(tuple([BASE_COMPLEMENT[x] for x in reversed(kmer)]))
-                kmer_to_ids[rev_compl] = new_id
-            new_id += 1
-    return kmer_to_ids, new_id
-
-def process_node_name(name: str, assembly_type: str="flye") -> str:
-    contig_name = name.strip().split(" ")[0]
-    #if assembly_type == "spades":
-    contig_name = "_".join(contig_name.split("_")[:2])
-    return contig_name
-
-
-class AssemblyDataset:
-    # Read contig names from fasta file and save to disk
-    # read graph
-    # other features are loaded by functions
-    # everything as numpy to make it easier to convert
-    def __init__(
-        self,
-        name,
-        logger,
-        data_dir,
-        fastafile,
-        graphfile,
-        depthfile,
-        scgfile,
-        labelsfile,
-        featuresfile,
-        cache_dir,
-        assemblytype="flye",
-        min_contig_length=0,
-        contignodes=False
-    ):
-        self.name = name
-        self.logger = logger
-        self.data_dir = data_dir
-        self.fastafile = fastafile
-        self.graphfile = graphfile
-        self.depthfile = depthfile
-        self.assembly_type = assemblytype
-        self.cache_dir = cache_dir
-        self.labelsfile = labelsfile
-        self.featuresfile = featuresfile
-        self.scgfile = scgfile
-        self.load_kmer = True
-        self.kmer = 4
-        self.min_contig_length = min_contig_length
-        self.contignodes = contignodes
-        if self.load_kmer:
-            self.kmer_to_ids, self.canonical_k = get_kmer_to_id(self.kmer)
-
-        # initialize data features which can be cached as numpy or pickle
-        self.node_names = []
-        self.node_seqs = {}  # should it be saved?
-        self.graph_nodes = []  # nodes that are part of the assembly graph
-        self.graph_paths = {} # contig paths identified by assembler
-        self.node_lengths = []
-        self.node_kmers = []
-        self.node_depths = []
-        self.edges_src = []
-        self.edges_dst = []
-        self.edge_weights = []
-        self.adj_matrix = None
-        self.neg_pairs_idx = None  # cached on the main function, only necessary for TF models
-
-        # initialize labels
-        self.labels = []
-        self.node_to_label = {}
-        self.label_to_node = {}
-        
-        self.contig_markers = {}
-        self.ref_marker_sets = {}
-
-    def read_assembly(self):
-        """Read assembly files, convert to numpy arrays and save to disk"""
-        self.logger.info("processing sequences {}".format(os.path.join(self.data_dir, self.fastafile)))
-        self.read_seqs()
-        self.logger.info(f"read {len(self.node_seqs)} seqs")
-        np.save(os.path.join(self.cache_dir, "node_names.npy"), self.node_names)
-        np.save(os.path.join(self.cache_dir, "node_lengths.npy"), self.node_lengths)
-        np.save(os.path.join(self.cache_dir, "node_attributes_kmer.npy"), self.node_kmers.astype(float))
-        pickle.dump(self.node_seqs, open(os.path.join(self.cache_dir, "node_seqs.pkl"), "wb"))
-        if os.path.exists(os.path.join(self.data_dir, self.graphfile)):
-            if not self.contignodes:
-                self.logger.info("processing GFA file (edge nodes) {}".format(os.path.join(self.data_dir, self.graphfile)))
-                self.read_gfa()
-            else:
-                self.logger.info("processing GFA file (contig nodes) {}".format(os.path.join(self.data_dir, self.graphfile)))
-                self.read_gfa_contigs()
-            self.logger.info(f"read {len(self.edges_src)}, edges")
-            np.save(os.path.join(self.cache_dir, "edge_weights.npy"), self.edge_weights)
-            scipy.sparse.save_npz(os.path.join(self.cache_dir, "adj_sparse.npz"), self.adj_matrix)
-            np.save(os.path.join(self.cache_dir, "graph_nodes.npy"), self.graph_nodes)
-            pickle.dump(self.graph_paths, open(os.path.join(self.cache_dir, "graph_paths.pkl"), 'wb'))
-        # self.filter_contigs()
-        # self.rename_nodes_to_index()
-        # self.nodes_depths = np.array(self.nodes_depths)
-        # read lengths
-        self.logger.info("reading depths")
-        self.read_depths()
-        np.save(os.path.join(self.cache_dir, "node_attributes_depth.npy"), np.array(self.node_depths))
-        self.logger.info("reading labels")
-        self.read_labels()
-        np.save(os.path.join(self.cache_dir, "node_to_label.npy"), self.node_to_label)
-        np.save(os.path.join(self.cache_dir, "label_to_node.npy"), self.label_to_node)
-        np.save(os.path.join(self.cache_dir, "labels.npy"), self.labels)
-        self.logger.info("Saved cache to {}".format(self.cache_dir))
-        # print("reading SCGs")
-        # self.read_scgs()
-
-    def print_stats(self):
-        print("==============================")
-        print("DATASET STATS:")
-        # get:
-        #   number of sequences
-        #   number of contigs
-        #   length of contigs (sum and average and N50)
-        #   coverage samples from jgi file
-        #   assembly_graph.file exists, number of edges, number of paths
-        print("number of sequences: {}".format(len(self.node_names)))
-        print("assembly length: {} Gb".format(round(sum(self.node_lengths) / 1000000000, 3)))
-        print("assembly N50: {} Mb".format(round(self.calculate_n50()/1000000, 3)))
-        print("assembly average length (Mb): {} max: {} min: {}".format(round(np.mean(self.node_lengths)/1000000, 3),
-                                                                   round(np.max(self.node_lengths)/1000000, 3),
-                                                                   round(np.min(self.node_lengths)/1000000, 3)))
-        print("coverage samples: {}".format(len(self.node_depths[0])))
-        if os.path.exists(os.path.join(self.data_dir, self.graphfile)) or \
-            len(self.edges_src) > 0:
-            print("Graph file found and read")
-            print("graph edges: {}".format(len(self.edges_src)))
-            print("contig paths: {}".format(len(self.graph_paths)))
-        else:
-            print("No assembly graph loaded")
-        #   contigs with markers on marker_gene_stats
-        #   stats with SCGs (max/min # of contigs, etc)
-
-        if len(self.contig_markers) > 0:
-            print("total ref markers sets: {}".format(len(self.ref_marker_sets)))
-            print("total ref markers: {}".format(len(self.markers)))
-            n_of_markers = [len(x) for x in self.contig_markers.values() if len(x) > 0]
-            print("contigs with one or more markers: {}/{}".format(len(n_of_markers),
-                                                                    len(self.node_names)))
-            
-            print("max SCGs on one contig: {}, average(excluding 0): {}".format(max(n_of_markers),
-                                                            round(np.mean(n_of_markers), 3)))
-            self.estimate_n_genomes()
-            print("SCG contig count min: {} contigs".format(min(self.scg_counts.values())))
-            self.get_edges_with_same_scgs()
-        else:
-            print("No SCG markers")
-        # labels
-        if self.labelsfile is not None or len(self.labels) > 1:
-            print("number of GS labels: {}".format(len(self.labels)))
-            nodes_not_na = [n for n in self.node_names if n in self.node_to_label and \
-                                                     self.node_to_label[n] != "NA"]
-            print("nodes with labels: {}".format(len(nodes_not_na)))
-        print("==============================")
-                                                          
-    def calculate_n50(self):
-        # https://eaton-lab.org/slides/genomics/answers/nb-4.1-numpy.html
-        contig_sizes = self.node_lengths.copy()
-        contig_sizes.sort()
-        contig_sizes = contig_sizes[::-1]
-        total_len = contig_sizes.sum()
-        half_total_len = total_len / 2
-        contig_sum_lens = np.zeros(contig_sizes.size, dtype=int)
-        for i in range(contig_sizes.size):
-            contig_sum_lens[i] = contig_sizes[i:].sum()
-        which_contigs_longer_than_half = contig_sum_lens > half_total_len
-        contigs_longer_than_half = contig_sizes[which_contigs_longer_than_half]
-        n50 = contigs_longer_than_half.min()
-        return n50
-
-    def read_cache(self, load_graph=True):
-        prefix = os.path.join(self.cache_dir, "{}")
-        self.node_names = list(np.load(prefix.format("node_names.npy")))
-        self.node_seqs = pickle.load(open(prefix.format("node_seqs.pkl"), "rb"))
-        # graph nodes
-        self.node_lengths = np.load(prefix.format("node_lengths.npy"))
-        if load_graph:
-            self.graph_nodes = np.load(prefix.format("graph_nodes.npy"))
-            self.graph_paths = pickle.load(open(prefix.format("graph_paths.pkl"), 'rb'))
-            self.adj_matrix = scipy.sparse.load_npz(prefix.format("adj_sparse.npz"))
-            self.edge_weights = self.adj_matrix.data
-            self.edges_src = self.adj_matrix.row
-            self.edges_dst = self.adj_matrix.col
-        self.node_kmers = np.load(prefix.format("node_attributes_kmer.npy"))
-        self.node_depths = np.load(prefix.format("node_attributes_depth.npy"))
-        # self.edge_weights = np.load(prefix.format("edge_weights.npy"))
-        
-        # labels
-        self.node_to_label = np.load("{}/node_to_label.npy".format(self.cache_dir), allow_pickle=True)[()]
-        self.label_to_node = np.load("{}/label_to_node.npy".format(self.cache_dir), allow_pickle=True)[()]
-        self.labels = list(np.load("{}/labels.npy".format(self.cache_dir)))
-        if os.path.exists(prefix.format("true_adj_sparse.npz")):
-            self.true_adj_matrix = scipy.sparse.load_npz(prefix.format("true_adj_sparse.npz"))
-
-    def check_cache(self, require_graph=True):
-        """check if all necessary files exist in cache"""
-        prefix = os.path.join(self.cache_dir, "{}")
-        if require_graph:
-            return (
-                os.path.exists(prefix.format("node_names.npy"))
-                and os.path.exists(prefix.format("node_lengths.npy"))
-                and os.path.exists(prefix.format("node_attributes_kmer.npy"))
-                #and os.path.exists(prefix.format("node_attributes_depth.npy"))
-                and os.path.exists(prefix.format("edge_weights.npy"))
-                and os.path.exists(prefix.format("adj_sparse.npz"))
-                and os.path.exists(prefix.format("graph_nodes.npy"))
-                and os.path.exists(prefix.format("graph_paths.pkl"))
-                and os.path.exists(prefix.format("node_to_label.npy"))
-                and os.path.exists(prefix.format("label_to_node.npy"))
-                and os.path.exists(prefix.format("labels.npy"))
-            )
-        else:
-            return (
-                os.path.exists(prefix.format("node_names.npy"))
-                and os.path.exists(prefix.format("node_lengths.npy"))
-                and os.path.exists(prefix.format("node_attributes_kmer.npy"))
-                #and os.path.exists(prefix.format("node_attributes_depth.npy"))
-                and os.path.exists(prefix.format("node_to_label.npy"))
-                and os.path.exists(prefix.format("label_to_node.npy"))
-                and os.path.exists(prefix.format("labels.npy"))
-            )
-
-    def read_seqs(self):
-        """Read sequences from fasta file, write to self.node_seqs"""
-        node_lengths = {}
-        node_kmers = {}
-        contig_name = None
-        with open(os.path.join(self.data_dir, self.fastafile), "r") as f:
-            for line in f:
-                if line.startswith(">"):
-                    if len(self.node_names) > 0:
-                        # finish last contig
-                        node_lengths[contig_name] = len(self.node_seqs[contig_name])
-                        if self.load_kmer:
-                            kmers = count_kmers(
-                                self.node_seqs[contig_name], self.kmer, self.kmer_to_ids, self.canonical_k
-                            )
-                            node_kmers[contig_name] = kmers
-                    contig_name = process_node_name(line[1:], self.assembly_type)
-                    self.node_names.append(contig_name)
-                    self.node_seqs[contig_name] = ""
-                else:
-                    self.node_seqs[contig_name] += line.strip()
-        # add last
-        node_lengths[contig_name] = len(self.node_seqs[contig_name])
-        if self.load_kmer:
-            kmers = count_kmers(self.node_seqs[contig_name], self.kmer, self.kmer_to_ids, self.canonical_k)
-            node_kmers[contig_name] = kmers
-            # convert kmers to numpy
-            self.node_kmers = np.array(stats.zscore([node_kmers[n] for n in self.node_names], axis=0))
-        self.node_lengths = np.array([node_lengths[n] for n in self.node_names])    
-
-    def read_gfa(self):
-        """Read graph file from GFA format, save list of start and end nodes to self.edges_src and self.edges_dst
-        Check if contig names match the fasta file from self.node_seqs
-        """
-        skipped_contigs = set()
-        with open(os.path.join(self.data_dir, self.graphfile), "r") as f:
-            for line in f:
-                if line.startswith("S"):  # sequence
-                    values = line.strip().split()
-                    node_name = process_node_name(values[1], self.assembly_type)
-                    if node_name not in self.node_names:
-                        skipped_contigs.add(node_name)
-                        continue
-                    contig_seq = self.node_seqs.get(node_name, "")  # discard missing contigs
-                    contiglen = len(contig_seq)
-
-                    if contiglen < self.min_contig_length:
-                        skipped_contigs.add(node_name)
-                    else:
-                        self.graph_nodes.append(node_name)
-                        # self.nodes_data.append([])
-                elif line.startswith("L"):  # link/edge
-                    values = line.strip().split()  # TAG, SRC, SIGN, DEST, SIGN, 0M, RC
-                    src_node_name = process_node_name(values[1], self.assembly_type)
-                    dst_node_name = process_node_name(values[3], self.assembly_type)
-                    if src_node_name in skipped_contigs or dst_node_name in skipped_contigs:
-                        # skipped_edges.add((contig_names.index(values[1]), contig_names.index(values[3])))
-                        continue
-                    src_index = self.node_names.index(src_node_name)
-                    dst_index = self.node_names.index(dst_node_name)
-                    self.edges_src.append(src_index)
-                    self.edges_dst.append(dst_index)
-                    if len(values) > 6:
-                        rc = int(values[6].split(":")[-1])
-                    else:
-                        rc = 1
-                    self.edge_weights.append(rc)
-                    # reverse too
-                    if values[1] != values[3]:
-                        self.edges_src.append(dst_index)
-                        self.edges_dst.append(src_index)
-                        self.edge_weights.append(rc)
-                elif line.startswith("P"):
-                    values = line.strip().split()  # P contig path
-                    self.graph_paths[values[1]] = [self.node_names.index(path_node_name[:-1]) \
-                        for path_node_name in values[2].split(",") if path_node_name[:-1] in self.node_names]
-        self.logger.info(f"skipped contigs {len(skipped_contigs)} < {self.min_contig_length}")
-        self.adj_matrix = scipy.sparse.coo_matrix(
-            (self.edge_weights, (self.edges_src, self.edges_dst)), shape=(len(self.node_names), len(self.node_names))
-        )
-        self.edge_weights = np.array(self.edge_weights)
-
-    def read_gfa_contigs(self):
-        skipped_contigs = set()
-        edge_edge_links = {}
-        contig_edge_links = {}
-        with open(os.path.join(self.data_dir, self.graphfile), "r") as f:
-            # ignore S entries (these are not contigs)
-            # the node seqs are read from the assembly file
-            for line in f:
-                if line.startswith("L"): # edge links
-                    values = line.strip().split()  # TAG, SRC, SIGN, DEST, SIGN, 0M, RC
-                    src_node_name = process_node_name(values[1], self.assembly_type)
-                    dst_node_name = process_node_name(values[3], self.assembly_type)
-                    edge_edge_links.setdefault(src_node_name,set()).add(values[3])
-                    edge_edge_links.setdefault(dst_node_name,set()).add(values[1])
-                elif line.startswith("P"): # contig to edge links
-                    values = line.strip().split()
-                    contig_name = process_node_name(values[1], self.assembly_type)
-                    if contig_name in skipped_contigs or contig_name not in self.node_names:
-                        #skipped_edges.add((contig_names.index(values[1]), contig_names.index(values[3])))
-                        continue
-                    for edge in values[2].split(","):
-                        contig_edge_links.setdefault(contig_name,set()).add(edge[:-1])
-                    self.graph_paths[values[1]] = [self.node_names.index(path_node_name[:-1]) \
-                        for path_node_name in values[2].split(",") if path_node_name[:-1] in self.node_names]
-        if len(contig_edge_links) == 0:
-            # load graph paths from assembly_info
-            self.logger.info("reading assembly_info file for graph paths...")
-            # TODO: check if file exists
-            contig_edge_links = self.read_assembly_info()
-        print("skipped contigs", len(skipped_contigs), "<", self.min_contig_length)
-        # create graph, , and to linked to adjacent edges
-        # first create edge to contig index
-        edge_contig_links = {}
-        for contig in contig_edge_links:
-            for e in contig_edge_links[contig]:
-                edge_contig_links.setdefault(e, set()).add(contig)
-        for contig in contig_edge_links:
-            src_index = self.node_names.index(contig)
-            for edge in contig_edge_links[contig]:
-                # connect contigs linked to same edge
-                for contig2 in edge_contig_links[edge]:
-                    dst_index = self.node_names.index(contig2)
-                    if contig2 != contig:
-                        self.edges_src.append(src_index)
-                        self.edges_dst.append(dst_index)
-                        self.edge_weights.append(1)
-                        # inverse is added when we get to contig2
-                for edge2 in edge_edge_links.get(edge, []):
-                    for contig2 in edge_contig_links.get(edge2, []):
-                        dst_index = self.node_names.index(contig2)
-                        self.edges_src.append(src_index)
-                        self.edges_dst.append(dst_index)
-                        self.edge_weights.append(1)
-        #self.logger.info(f"skipped contigs {len(skipped_contigs)} < {self.min_contig_length}")
-        self.adj_matrix = scipy.sparse.coo_matrix(
-            (self.edge_weights, (self.edges_src, self.edges_dst)), shape=(len(self.node_names), len(self.node_names))
-        )
-        self.edge_weights = np.array(self.edge_weights)
-
-    def read_assembly_info(self, get_graph_paths=False, circular_length=100000) -> Dict[str,list]:
-        """Read assembly_info.txt file generated by flye
-        """
-        self.circular_contigs: List[str] = []
-        self.repetitive_contigs: List[str] = []
-        self.contigs_multiplicity = {}
-        contig_edge_links = {}
-        with open(os.path.join(self.data_dir, "assembly_info.txt"), "r") as f:
-            next(f) # skip header
-            for line in f:
-                values = line.strip().split("\t")
-                contig_name = process_node_name(values[0], self.assembly_type)
-                if values[3] == "Y" and int(values[1]) > circular_length:
-                    self.circular_contigs.append(contig_name)
-                if values[4] == "Y":
-                    self.repetitive_contigs.append(contig_name)
-                #if contig_name not in self.node_names:
-                    #skipped_edges.add((contig_names.index(values[1]), contig_names.index(values[3])))
-                #    continue
-                self.contigs_multiplicity[contig_name] = int(values[5])
-                # get graph_paths
-                for edge in values[-1].split(","):
-                    if edge != "*":
-                        contig_edge_links.setdefault(contig_name,set()).add("edge_" + edge.strip("-"))
-                if get_graph_paths:
-                    self.graph_paths[contig_name] = ["edge_" + e for e in contig_edge_links[contig_name]]
-                #for edge_name in self.graph_paths[contig_name]:
-                #    self.contigs_multiplicity[self.node_names.index(edge_name)] = int(values[5])
-        return contig_edge_links
-    
-    def print_circular_contigs(self):
-        """Print circular contigs and info, based on flye
-        """
-        for contig_name in self.circular_contigs:
-            print("found circular contig", contig_name,
-                  "mult.", self.contigs_multiplicity[contig_name])
-            # get edges of this contig
-            contig_edges = self.graph_paths[contig_name]
-            print("---", "name", "depth", "markers", "label", "edges")
-            for edge_id in contig_edges:
-                #edge_id = self.node_names.index("edge_" + edge)
-                edge_name = self.node_names[edge_id]
-                print("---", edge_id, edge_name, self.node_lengths[edge_id],
-                      [round(d, 4) for d in self.node_depths[edge_id]],
-                      self.node_to_label[edge_name],
-                      len(self.contig_markers.get(edge_name, [])),
-                      list(self.adj_matrix.getrow(edge_id).data))
-
-    def read_depths(self) -> None:
-        node_depths: Dict[str, np.array] = {}
-        if self.depthfile is not None and os.path.exists(os.path.join(self.data_dir, self.depthfile)):
-            if self.depthfile.endswith(".npz"):
-                self.node_depths = np.load(open(os.path.join(self.data_dir, self.depthfile), "rb"))["arr_0"]
-                if self.node_depths.shape[0] != len(self.node_names):
-                    print("depth npz file mismatch:")
-                    breakpoint()
-            else:
-                with open(os.path.join(self.data_dir, self.depthfile)) as f:
-                    header = next(f)
-                    depth_i = [i + 3 for i, n in enumerate(header.split("\t")[3:]) if "-var" not in n]
-                    # var_i = [i + 3 for i, n in enumerate(header.split("\t")[3:]) if "-var" in n]
-                    for line in f:
-                        values = line.strip().split()
-                        node_name = process_node_name(values[0], self.assembly_type)
-                        if node_name in self.node_names:
-                            node_depths[node_name] = np.array([float(values[i]) for i in depth_i])
-                        else:
-                            self.logger.info("node name not found: {}".format(node_name))
-                if len(node_depths) != len(self.node_names):
-                    self.logger.info("missing abundance for some nodes: {}".format(len(node_depths) - len(self.node_names)))
-                self.node_depths = np.array([node_depths.get(n, [0]*len(depth_i)) for n in self.node_names])
-            if len(self.node_depths[0]) > 1:  # normalize depths
-                depthssum = self.node_depths.sum(axis=1) + 1e-10
-                self.node_depths /= depthssum.reshape((-1, 1))
-            else:
-                self.node_depths = stats.zscore(self.node_depths, axis=0)
-        else:
-            self.node_depths = np.ones(len(self.node_names), dtype=np.float)
-
-    def read_labels(self):
-        # logging.info("loading labels from {}".format(args.labels))
-        if self.labelsfile is not None:
-            node_to_label = {c: "NA" for c in self.node_names}
-            labels = set(["NA"])
-            with open(os.path.join(self.data_dir, self.labelsfile), "r") as f:
-                for line in f:
-                    # label, node = line.strip().split()
-                    if self.labelsfile.endswith(".csv"):
-                        values = line.strip().split(",")
-                    elif self.labelsfile.endswith(".tsv"):  # amber format
-                        if line.startswith("@") or line.startswith("#"):
-                            continue
-                        values = line.strip().split("\t")
-                    if len(values) < 2:
-                        breakpoint()
-                    node_name = process_node_name(values[0], self.assembly_type)
-                    label = values[1]
-                    if node_name in node_to_label:
-                        node_to_label[node_name] = label
-                        labels.add(label)
-                    else:
-                        breakpoint()
-                        self.logger.info(("unused label: {}".format(line.strip())))
-            labels = list(labels)
-            label_to_node = {s: [] for s in labels}
-            for n in node_to_label:
-                s = node_to_label[n]
-                label_to_node[s].append(n)
-            self.node_to_label = {n: l for n, l in node_to_label.items()}
-            self.labels = labels
-            self.label_to_node = label_to_node
-            # calculate homophily
-            if len(self.edge_weights) > 1:
-                self.calculate_homophily()
-        else:
-            self.labels = ["NA"]
-            self.label_to_node = {"NA": self.node_names}
-            self.node_to_label = {n: "NA" for n in self.node_names}
-
-    def calculate_homophily(self):
-        """
-        Calculate percentage of edges that connect nodes with the same label
-        """
-        positive_edges = 0
-        edges_without_label = 0
-        for u, v in zip(self.edges_src, self.edges_dst):
-            if self.node_to_label.get(self.node_names[u], "NA") == "NA" or \
-               self.node_to_label.get(self.node_names[v], "NA") == "NA":
-                edges_without_label += 1
-            if self.node_to_label[self.node_names[u]] == self.node_to_label[self.node_names[v]] and self.node_to_label[self.node_names[u]] != "NA":
-                positive_edges += 1
-        self.logger.info(
-            f"""homophily: {round(positive_edges / (len(self.edge_weights) - edges_without_label),4)} on
-            {len(self.edge_weights) - edges_without_label} edges between labeled nodes"""
-        )
-
-    def read_scgs(self):
-        # Load contig marker genes (Bacteria list)
-        if self.scgfile is not None:
-            # logging.info("loading checkm results")
-            scg_path = os.path.join(self.data_dir, self.scgfile)
-            ref_sets = read_marker_gene_sets(BACTERIA_MARKERS)
-            contig_markers = read_contig_genes(scg_path)
-            self.ref_marker_sets = ref_sets
-            self.contig_markers = contig_markers
-            marker_counts = get_markers_to_contigs(ref_sets, contig_markers)
-            self.markers = marker_counts
-        else:
-            self.ref_marker_sets = {}
-            self.contig_markers = {}
-            self.run_checkm()
-
-    def get_all_different_idx(self):
-        """
-        Returns a 2d numpy array where each row
-        corresponds to a pairs of node idx whose
-        feature must be different as they correspond
-        to the same contig (check jargon). This
-        should encourage the HQ value to be higher.
-        """
-        node_names_to_idx = {node_name: i for i, node_name in enumerate(self.node_names)}
-        pair_idx = set()
-        for n1 in self.contig_markers:
-            for gene1 in self.contig_markers[n1]:
-                for n2 in self.contig_markers:
-                    if n1 != n2 and gene1 in self.contig_markers[n2]:
-                        p1 = (node_names_to_idx[n1], node_names_to_idx[n2])
-                        p2 = (node_names_to_idx[n2], node_names_to_idx[n1])
-                        if (p1 not in pair_idx) and (p2 not in pair_idx):
-                            pair_idx.add(p1)
-        pair_idx = np.unique(np.array(list(pair_idx)), axis=0)
-        print("Number of diff cluster pairs:", len(pair_idx))
-        self.neg_pairs_idx = pair_idx
-
-    def run_vamb(self, vamb_outdir, cuda, vambdim):
-        from vamb.vamb_run import run as run_vamb
-        self.logger.info("running VAMB")
-        batchsteps = []
-        vamb_epochs = 500
-        if len(self.node_depths[0]) == 1:
-            vamb_bs = 32
-            batchsteps = [25, 75, 150]
-        else:
-            vamb_bs = 64
-            batchsteps = [25, 75, 150, 300]
-        nhiddens = [512, 512]
-        self.logger.info("using these batchsteps:{}".format(batchsteps))
-
-        vamb_logpath = os.path.join(vamb_outdir, "log.txt")
-        if os.path.exists(vamb_outdir) and os.path.isdir(vamb_outdir):
-            shutil.rmtree(vamb_outdir)
-        os.mkdir(vamb_outdir)
-        with open(vamb_logpath, "w") as vamb_logfile:
-            run_vamb(
-                outdir=vamb_outdir,
-                fastapath=os.path.join(self.data_dir, self.fastafile),
-                jgipath=os.path.join(self.data_dir, self.depthfile),
-                logfile=vamb_logfile,
-                cuda=cuda,
-                batchsteps=batchsteps,
-                batchsize=vamb_bs,
-                nepochs=vamb_epochs,
-                mincontiglength=self.min_contig_length,
-                nhiddens=nhiddens,
-                nlatent=int(vambdim),
-                norefcheck=True,
-            )
-            if self.data_dir != "" and self.featuresfile.endswith(".tsv"):
-                shutil.copyfile(os.path.join(vamb_outdir, "embs.tsv"), self.featuresfile)
-            self.logger.info("Contig features saved to {}".format(self.featuresfile))
-
-    def read_features(self):
-        node_embs = {}
-        self.logger.info("loading features from {}".format(self.featuresfile))
-        if self.featuresfile.endswith(".tsv"):
-            with open(self.featuresfile, "r") as ffile:
-                for line in ffile:
-                    values = line.strip().split()
-                    node_embs[values[0]] = [float(x) for x in values[1:]]
-            self.logger.info("loaded {} features/ {} nodes from tsv".format(len(node_embs), len(self.node_names)))
-        elif self.featuresfile.endswith(".pickle"):
-            with open(self.featuresfile, "rb") as ffile:
-                node_embs = pickle.load(ffile)
-            self.logger.info("loaded {} features/ {} nodes from pickle".format(len(node_embs), len(self.node_names)))
-        self.node_embs = [
-                node_embs.get(n, np.random.uniform(10e-5, 1.0, len(node_embs[list(node_embs.keys())[0]]))) for n in self.node_names
-            ]  # deal with missing embs
-        self.node_embs = np.array(self.node_embs)
-
-    def write_features_tsv(self):
-        self.logger.info("writing features to {}".format(self.featuresfile))
-        with open(self.featuresfile, "w") as ffile:
-            for i, emb in enumerate(self.node_embs):
-                ffile.write(f"{self.node_names[i]} {' '.join(map(str,emb.tolist()))}\n")
-
-    def get_topk_neighbors(self, k, scg_only=False):
-        """
-        Returns a list of the top k neighbors for each node. Use kmers and abundance
-
-        """
-        #breakpoint()
-        self.logger.info("getting top {} neighbors".format(k))
-        self.topk_neighbors = []
-        features = np.concatenate((self.node_kmers, self.node_depths), axis=1)
-        cosine_dists = np.dot(features, features.T)
-        for i in range(len(self.node_names)):
-            self.topk_neighbors.append(set(np.argsort(cosine_dists[i])[-k:]))
-        self.logger.info("got top {} neighbors".format(k))
-
-    def estimate_n_genomes(self):
-        self.scg_counts = {}
-        for marker_set in self.ref_marker_sets:
-            for gene in marker_set:
-                self.scg_counts[gene] = 0
-                for contig in self.contig_markers:
-                    if gene in self.contig_markers[contig]:
-                        self.scg_counts[gene] += self.contig_markers[contig][gene]
-
-        #print(self.scg_counts)
-        quartiles = np.percentile(list(self.scg_counts.values()), [25, 50, 75])
-        print("candidate k0s", sorted(set([k for k in self.scg_counts.values() if k >= quartiles[2]])))
-        return max(self.scg_counts.values())
-        
-       
-    def run_checkm(self, nthreads=10, tempdir="../temp"):
-        # check if checkm is installed
-        checkm_is_avail = shutil.which("checkm") is not None
-        # if not, print commands only
-        commands = [
-            "mkdir {}/nodes".format(self.data_dir), #; cd nodes; ",
-            "cat {0}/{1} | awk '{{ if (substr($0, 1, 1)=='>') {{filename=(substr($0,2) '.fa')}} print $0 > {0}/filename }}".format(self.data_dir, self.fastafile),
-            'find {}/nodes/ -name "* *" -type f | rename "s/ /_/g"'.format(self.data_dir),
-            "checkm taxonomy_wf --tmpdir {0} -t {1} -x fa domain Bacteria {2}/nodes/ {2}/checkm_nodes/".format(tempdir, nthreads, self.data_dir)
-        ]
-        if checkm_is_avail:
-            #run commands one by one
-            for cmd in commands:
-                os.system(cmd)
-        else:
-            print("Run this on a machine with CheckM installed")
-            for cmd in commands:
-                print(cmd)
-
-
-    def read_gtdbtk_files(self, prefix="gtdbtk", suffix_labels="summary.tsv",
-                          suffix_markers="markers_summary.tsv", reset=True):
-        # use summary to add species level labels
-        # also save full lineages
-        roots = ["bac120"] #, "ar53"]
-        no_species = 0
-        no_genus = 0
-        species_labels = set()
-        # reset labels
-        if reset:
-            self.node_to_label = {n: "NA" for n in self.node_names}
-            self.labels = ["NA"]
-        contig_markers = {n: {} for n in self.node_names}
-        ref_markers = set()
-        for root in roots:
-            # read labels
-            with open(os.path.join(self.data_dir, f"{prefix}.{root}.{suffix_labels}"), 'r') as f:
-                next(f) # skip header
-                for line in f:
-                    values = line.strip().split("\t")
-                    node_name = process_node_name(values[0], self.assembly_type)
-                    if values[1].startswith("Unclassified"):
-                        continue # do not add unclassified nodes
-                    classification = values[1].split(";")
-                    node_slabel = classification[-1]
-                    node_glabel = classification[-2]
-                    #if values[5] != "N/A":
-                    #    fast_ani = float(values[5])
-                    #    anis.append(fast_ani)
-                    if node_slabel == "s__":
-                        no_species += 1
-                    else:
-                        self.node_to_label[node_name] = node_slabel
-                        species_labels.add(node_slabel)
-                    #if node_slabel == "g__":
-                    #    no_genus += 1
-                    #else:
-                    #    node_to_glabel[node_name] = node_glabel
-                    #    genus_labels.add(node_glabel)
-
-            # read markers
-            with open(os.path.join(self.data_dir, f"{prefix}.{root}.{suffix_markers}"), 'r') as f:
-                next(f) # skip header
-                for line in f:
-                    values = line.strip().split("\t")
-                    node_name = process_node_name(values[0], self.assembly_type)
-                    if int(values[1]) > 0:
-                        contig_markers[node_name] = {g: 1 for g in values[5].split(",")}
-                        ref_markers.update(set(contig_markers[node_name]))
-                    if int(values[4]) > 0:
-                        ref_markers.update(set(values[-1].split(",")))
-        # create ref labels and ref markers
-        self.labels += list(species_labels)
-        self.label_to_node = {s: [] for s in self.labels}
-        for n in self.node_to_label:
-            s = self.node_to_label[n]
-            self.label_to_node[s].append(n)
-        assert len(ref_markers) == 120 # GTDB-tk bac and ar markers
-        if reset:
-            self.ref_marker_sets = [ref_markers]    
-            self.contig_markers = contig_markers
-            marker_counts = get_markers_to_contigs(self.ref_marker_sets, contig_markers)
-            self.markers = marker_counts
-
-    def get_edges_with_same_scgs(self):
-        """Check every edge to see if nodes have SCGs in common
-
-        :return: edges IDs (edges_src, edges_dst, edge_weight)
-        :rtype: list
-        """
-        edge_ids_with_same_scgs = []
-        scg_counter = Counter()
-        for x, (i, j) in enumerate(zip(self.edges_src, self.edges_dst)):
-            if self.node_names[i] in self.contig_markers and self.node_names[j] in self.contig_markers and \
-                len(self.contig_markers[self.node_names[i]]) > 0 and len(self.contig_markers[self.node_names[j]]) > 0:
-            
-                overlap = len(self.contig_markers[self.node_names[i]].keys() & \
-                    self.contig_markers[self.node_names[j]].keys())
-                if overlap > 0 and i != j:
-                    #remove edge
-                    scg_counter[overlap] += 1
-                    edge_ids_with_same_scgs.append(x)
-        print("edges with overlapping scgs (max=20):", scg_counter.most_common(20))
-        return edge_ids_with_same_scgs
-
-    def generate_edges_based_on_labels(self, noise=0):
-        # link nodes with same labels and create new adj_matrix/edges_src/edges_dst/edge_weights
-        #new_edges = []
-        new_srcs = []
-        new_dsts = []
-        for label in self.label_to_node:
-            # make circular graph
-            for i in range(len(self.label_to_node[label])):
-                new_src = self.node_names.index(self.label_to_node[label][i])
-                new_srcs.append(new_src)
-                if i+1 < len(self.label_to_node[label]):
-                    new_dst = self.node_names.index(self.label_to_node[label][i+1])
-                else: # connect to element 0
-                    new_dst = self.node_names.index(self.label_to_node[label][0])
-                #new_edges.append((new_src, new_dst))
-                new_dsts.append(new_dst)
-        new_weights = [1] * len(new_srcs)
-        print("creating new graph with {} edges".format(len(new_srcs)))
-        self.adj_matrix = scipy.sparse.coo_matrix(
-            (new_weights, (new_srcs, new_dsts)), shape=(len(self.node_names), len(self.node_names))
-        )
-        self.edges_src = new_srcs
-        self.edges_dst = new_dsts
-        self.edge_weights = np.array(new_weights)
-
-
-
+from glob import escape
+#from importlib.resources import files #3.9 only
+from importlib_resources import files
+import itertools
+import random
+import os
+import pickle
+import pdb
+import shutil
+from typing import Dict, List, Tuple, Sequence
+from collections import Counter
+import numpy as np
+import networkx as nx
+import scipy.stats as stats
+import scipy.sparse
+from graphmb.evaluate import (
+    read_marker_gene_sets,
+    read_contig_genes,
+    get_markers_to_contigs,
+)
+
+
+#BACTERIA_MARKERS = "data/Bacteria.ms"
+#kernel = np.load("data/kernel.npz")['arr_0']
+BACTERIA_MARKERS = files('graphmb.data').joinpath('Bacteria.ms')
+kernel = np.load(files('graphmb.data').joinpath('kernel.npz'))['arr_0']
+
+def count_kmers(seq, k, kmer_to_id, canonical_k):
+    # Used in case kmers are used as input features
+    # https://stackoverflow.com/q/22428020
+    #breakpoint()
+    kmer_letters = set(["A", "T", "C", "G"])
+    kmers = [seq[i : i + k] for i in range(len(seq) - k + 1) if set(seq[i : i + k]).issubset(kmer_letters)]
+    kmers = [kmer_to_id[k] for k in kmers]
+    kmer_counts = Counter(kmers)
+    counts = np.array([kmer_counts[k] for k in range(canonical_k)])
+    counts = counts / counts.sum()
+    counts += -(1/(4**k))
+    counts = np.dot(counts, kernel)
+    return counts
+
+def get_kmer_to_id(kmer, combine_revcomp=False):
+    kmer_to_ids = {}
+    BASE_COMPLEMENT = {"A": "T", "T": "A", "G": "C", "C": "G"}
+    all_kmers = itertools.product("ACGT", repeat=kmer)
+    all_kmers = ["".join(k) for k in all_kmers]
+    new_id = 0
+    for kmer in all_kmers:
+        if kmer not in kmer_to_ids:
+            kmer_to_ids[kmer] = new_id
+            if combine_revcomp:
+                rev_compl = "".join(tuple([BASE_COMPLEMENT[x] for x in reversed(kmer)]))
+                kmer_to_ids[rev_compl] = new_id
+            new_id += 1
+    return kmer_to_ids, new_id
+
+def process_node_name(name: str, assembly_type: str="flye") -> str:
+    contig_name = name.strip().split(" ")[0]
+    #if assembly_type == "spades":
+    contig_name = "_".join(contig_name.split("_")[:2])
+    return contig_name
+
+
+class AssemblyDataset:
+    # Read contig names from fasta file and save to disk
+    # read graph
+    # other features are loaded by functions
+    # everything as numpy to make it easier to convert
+    def __init__(
+        self,
+        name,
+        logger,
+        data_dir,
+        fastafile,
+        graphfile,
+        depthfile,
+        scgfile,
+        labelsfile,
+        featuresfile,
+        cache_dir,
+        assemblytype="flye",
+        min_contig_length=0,
+        contignodes=False
+    ):
+        self.name = name
+        self.logger = logger
+        self.data_dir = data_dir
+        self.fastafile = fastafile
+        self.graphfile = graphfile
+        self.depthfile = depthfile
+        self.assembly_type = assemblytype
+        self.cache_dir = cache_dir
+        self.labelsfile = labelsfile
+        self.featuresfile = featuresfile
+        self.scgfile = scgfile
+        self.load_kmer = True
+        self.kmer = 4
+        self.min_contig_length = min_contig_length
+        self.contignodes = contignodes
+        if self.load_kmer:
+            self.kmer_to_ids, self.canonical_k = get_kmer_to_id(self.kmer)
+
+        # initialize data features which can be cached as numpy or pickle
+        self.node_names = []
+        self.node_seqs = {}  # should it be saved?
+        self.graph_nodes = []  # nodes that are part of the assembly graph
+        self.graph_paths = {} # contig paths identified by assembler
+        self.node_lengths = []
+        self.node_kmers = []
+        self.node_depths = []
+        self.edges_src = []
+        self.edges_dst = []
+        self.edge_weights = []
+        self.adj_matrix = None
+        self.neg_pairs_idx = None  # cached on the main function, only necessary for TF models
+
+        # initialize labels
+        self.labels = []
+        self.node_to_label = {}
+        self.label_to_node = {}
+        
+        self.contig_markers = {}
+        self.ref_marker_sets = {}
+
+    def read_assembly(self):
+        """Read assembly files, convert to numpy arrays and save to disk"""
+        self.logger.info("processing sequences {}".format(os.path.join(self.data_dir, self.fastafile)))
+        self.read_seqs()
+        self.logger.info(f"read {len(self.node_seqs)} seqs")
+        np.save(os.path.join(self.cache_dir, "node_names.npy"), self.node_names)
+        np.save(os.path.join(self.cache_dir, "node_lengths.npy"), self.node_lengths)
+        np.save(os.path.join(self.cache_dir, "node_attributes_kmer.npy"), self.node_kmers.astype(float))
+        pickle.dump(self.node_seqs, open(os.path.join(self.cache_dir, "node_seqs.pkl"), "wb"))
+        if os.path.exists(os.path.join(self.data_dir, self.graphfile)):
+            if not self.contignodes:
+                self.logger.info("processing GFA file (edge nodes) {}".format(os.path.join(self.data_dir, self.graphfile)))
+                self.read_gfa()
+            else:
+                self.logger.info("processing GFA file (contig nodes) {}".format(os.path.join(self.data_dir, self.graphfile)))
+                self.read_gfa_contigs()
+            self.logger.info(f"read {len(self.edges_src)}, edges")
+            np.save(os.path.join(self.cache_dir, "edge_weights.npy"), self.edge_weights)
+            scipy.sparse.save_npz(os.path.join(self.cache_dir, "adj_sparse.npz"), self.adj_matrix)
+            np.save(os.path.join(self.cache_dir, "graph_nodes.npy"), self.graph_nodes)
+            pickle.dump(self.graph_paths, open(os.path.join(self.cache_dir, "graph_paths.pkl"), 'wb'))
+        # self.filter_contigs()
+        # self.rename_nodes_to_index()
+        # self.nodes_depths = np.array(self.nodes_depths)
+        # read lengths
+        self.logger.info("reading depths")
+        self.read_depths()
+        np.save(os.path.join(self.cache_dir, "node_attributes_depth.npy"), np.array(self.node_depths))
+        self.logger.info("reading labels")
+        self.read_labels()
+        np.save(os.path.join(self.cache_dir, "node_to_label.npy"), self.node_to_label)
+        np.save(os.path.join(self.cache_dir, "label_to_node.npy"), self.label_to_node)
+        np.save(os.path.join(self.cache_dir, "labels.npy"), self.labels)
+        self.logger.info("Saved cache to {}".format(self.cache_dir))
+        # print("reading SCGs")
+        # self.read_scgs()
+
+    def print_stats(self):
+        print("==============================")
+        print("DATASET STATS:")
+        # get:
+        #   number of sequences
+        #   number of contigs
+        #   length of contigs (sum and average and N50)
+        #   coverage samples from jgi file
+        #   assembly_graph.file exists, number of edges, number of paths
+        print("number of sequences: {}".format(len(self.node_names)))
+        print("assembly length: {} Gb".format(round(sum(self.node_lengths) / 1000000000, 3)))
+        print("assembly N50: {} Mb".format(round(self.calculate_n50()/1000000, 3)))
+        print("assembly average length (Mb): {} max: {} min: {}".format(round(np.mean(self.node_lengths)/1000000, 3),
+                                                                   round(np.max(self.node_lengths)/1000000, 3),
+                                                                   round(np.min(self.node_lengths)/1000000, 3)))
+        print("coverage samples: {}".format(len(self.node_depths[0])))
+        if os.path.exists(os.path.join(self.data_dir, self.graphfile)) or \
+            len(self.edges_src) > 0:
+            print("Graph file found and read")
+            print("graph edges: {}".format(len(self.edges_src)))
+            print("contig paths: {}".format(len(self.graph_paths)))
+        else:
+            print("No assembly graph loaded")
+        #   contigs with markers on marker_gene_stats
+        #   stats with SCGs (max/min # of contigs, etc)
+
+        if len(self.contig_markers) > 0:
+            print("total ref markers sets: {}".format(len(self.ref_marker_sets)))
+            print("total ref markers: {}".format(len(self.markers)))
+            n_of_markers = [len(x) for x in self.contig_markers.values() if len(x) > 0]
+            print("contigs with one or more markers: {}/{}".format(len(n_of_markers),
+                                                                    len(self.node_names)))
+            
+            print("max SCGs on one contig: {}, average(excluding 0): {}".format(max(n_of_markers),
+                                                            round(np.mean(n_of_markers), 3)))
+            self.estimate_n_genomes()
+            print("SCG contig count min: {} contigs".format(min(self.scg_counts.values())))
+            self.get_edges_with_same_scgs()
+        else:
+            print("No SCG markers")
+        # labels
+        if self.labelsfile is not None or len(self.labels) > 1:
+            print("number of GS labels: {}".format(len(self.labels)))
+            nodes_not_na = [n for n in self.node_names if n in self.node_to_label and \
+                                                     self.node_to_label[n] != "NA"]
+            print("nodes with labels: {}".format(len(nodes_not_na)))
+        print("==============================")
+                                                          
+    def calculate_n50(self):
+        # https://eaton-lab.org/slides/genomics/answers/nb-4.1-numpy.html
+        contig_sizes = self.node_lengths.copy()
+        contig_sizes.sort()
+        contig_sizes = contig_sizes[::-1]
+        total_len = contig_sizes.sum()
+        half_total_len = total_len / 2
+        contig_sum_lens = np.zeros(contig_sizes.size, dtype=int)
+        for i in range(contig_sizes.size):
+            contig_sum_lens[i] = contig_sizes[i:].sum()
+        which_contigs_longer_than_half = contig_sum_lens > half_total_len
+        contigs_longer_than_half = contig_sizes[which_contigs_longer_than_half]
+        n50 = contigs_longer_than_half.min()
+        return n50
+
+    def read_cache(self, load_graph=True):
+        prefix = os.path.join(self.cache_dir, "{}")
+        self.node_names = list(np.load(prefix.format("node_names.npy")))
+        self.node_seqs = pickle.load(open(prefix.format("node_seqs.pkl"), "rb"))
+        # graph nodes
+        self.node_lengths = np.load(prefix.format("node_lengths.npy"))
+        if load_graph:
+            self.graph_nodes = np.load(prefix.format("graph_nodes.npy"))
+            self.graph_paths = pickle.load(open(prefix.format("graph_paths.pkl"), 'rb'))
+            self.adj_matrix = scipy.sparse.load_npz(prefix.format("adj_sparse.npz"))
+            self.edge_weights = self.adj_matrix.data
+            self.edges_src = self.adj_matrix.row
+            self.edges_dst = self.adj_matrix.col
+        self.node_kmers = np.load(prefix.format("node_attributes_kmer.npy"))
+        self.node_depths = np.load(prefix.format("node_attributes_depth.npy"))
+        # self.edge_weights = np.load(prefix.format("edge_weights.npy"))
+        
+        # labels
+        self.node_to_label = np.load("{}/node_to_label.npy".format(self.cache_dir), allow_pickle=True)[()]
+        self.label_to_node = np.load("{}/label_to_node.npy".format(self.cache_dir), allow_pickle=True)[()]
+        self.labels = list(np.load("{}/labels.npy".format(self.cache_dir)))
+        if os.path.exists(prefix.format("true_adj_sparse.npz")):
+            self.true_adj_matrix = scipy.sparse.load_npz(prefix.format("true_adj_sparse.npz"))
+
+    def check_cache(self, require_graph=True):
+        """check if all necessary files exist in cache"""
+        prefix = os.path.join(self.cache_dir, "{}")
+        if require_graph:
+            return (
+                os.path.exists(prefix.format("node_names.npy"))
+                and os.path.exists(prefix.format("node_lengths.npy"))
+                and os.path.exists(prefix.format("node_attributes_kmer.npy"))
+                #and os.path.exists(prefix.format("node_attributes_depth.npy"))
+                and os.path.exists(prefix.format("edge_weights.npy"))
+                and os.path.exists(prefix.format("adj_sparse.npz"))
+                and os.path.exists(prefix.format("graph_nodes.npy"))
+                and os.path.exists(prefix.format("graph_paths.pkl"))
+                and os.path.exists(prefix.format("node_to_label.npy"))
+                and os.path.exists(prefix.format("label_to_node.npy"))
+                and os.path.exists(prefix.format("labels.npy"))
+            )
+        else:
+            return (
+                os.path.exists(prefix.format("node_names.npy"))
+                and os.path.exists(prefix.format("node_lengths.npy"))
+                and os.path.exists(prefix.format("node_attributes_kmer.npy"))
+                #and os.path.exists(prefix.format("node_attributes_depth.npy"))
+                and os.path.exists(prefix.format("node_to_label.npy"))
+                and os.path.exists(prefix.format("label_to_node.npy"))
+                and os.path.exists(prefix.format("labels.npy"))
+            )
+
+    def read_seqs(self):
+        """Read sequences from fasta file, write to self.node_seqs"""
+        node_lengths = {}
+        node_kmers = {}
+        contig_name = None
+        with open(os.path.join(self.data_dir, self.fastafile), "r") as f:
+            for line in f:
+                if line.startswith(">"):
+                    if len(self.node_names) > 0:
+                        # finish last contig
+                        node_lengths[contig_name] = len(self.node_seqs[contig_name])
+                        if self.load_kmer:
+                            kmers = count_kmers(
+                                self.node_seqs[contig_name], self.kmer, self.kmer_to_ids, self.canonical_k
+                            )
+                            node_kmers[contig_name] = kmers
+                    contig_name = process_node_name(line[1:], self.assembly_type)
+                    self.node_names.append(contig_name)
+                    self.node_seqs[contig_name] = ""
+                else:
+                    self.node_seqs[contig_name] += line.strip()
+        # add last
+        node_lengths[contig_name] = len(self.node_seqs[contig_name])
+        if self.load_kmer:
+            kmers = count_kmers(self.node_seqs[contig_name], self.kmer, self.kmer_to_ids, self.canonical_k)
+            node_kmers[contig_name] = kmers
+            # convert kmers to numpy
+            self.node_kmers = np.array(stats.zscore([node_kmers[n] for n in self.node_names], axis=0))
+        self.node_lengths = np.array([node_lengths[n] for n in self.node_names])    
+
+    def read_gfa(self):
+        """Read graph file from GFA format, save list of start and end nodes to self.edges_src and self.edges_dst
+        Check if contig names match the fasta file from self.node_seqs
+        """
+        skipped_contigs = set()
+        with open(os.path.join(self.data_dir, self.graphfile), "r") as f:
+            for line in f:
+                if line.startswith("S"):  # sequence
+                    values = line.strip().split()
+                    node_name = process_node_name(values[1], self.assembly_type)
+                    if node_name not in self.node_names:
+                        skipped_contigs.add(node_name)
+                        continue
+                    contig_seq = self.node_seqs.get(node_name, "")  # discard missing contigs
+                    contiglen = len(contig_seq)
+
+                    if contiglen < self.min_contig_length:
+                        skipped_contigs.add(node_name)
+                    else:
+                        self.graph_nodes.append(node_name)
+                        # self.nodes_data.append([])
+                elif line.startswith("L"):  # link/edge
+                    values = line.strip().split()  # TAG, SRC, SIGN, DEST, SIGN, 0M, RC
+                    src_node_name = process_node_name(values[1], self.assembly_type)
+                    dst_node_name = process_node_name(values[3], self.assembly_type)
+                    if src_node_name in skipped_contigs or dst_node_name in skipped_contigs:
+                        # skipped_edges.add((contig_names.index(values[1]), contig_names.index(values[3])))
+                        continue
+                    src_index = self.node_names.index(src_node_name)
+                    dst_index = self.node_names.index(dst_node_name)
+                    self.edges_src.append(src_index)
+                    self.edges_dst.append(dst_index)
+                    if len(values) > 6:
+                        rc = int(values[6].split(":")[-1])
+                    else:
+                        rc = 1
+                    self.edge_weights.append(rc)
+                    # reverse too
+                    if values[1] != values[3]:
+                        self.edges_src.append(dst_index)
+                        self.edges_dst.append(src_index)
+                        self.edge_weights.append(rc)
+                elif line.startswith("P"):
+                    values = line.strip().split()  # P contig path
+                    self.graph_paths[values[1]] = [self.node_names.index(path_node_name[:-1]) \
+                        for path_node_name in values[2].split(",") if path_node_name[:-1] in self.node_names]
+        self.logger.info(f"skipped contigs {len(skipped_contigs)} < {self.min_contig_length}")
+        self.adj_matrix = scipy.sparse.coo_matrix(
+            (self.edge_weights, (self.edges_src, self.edges_dst)), shape=(len(self.node_names), len(self.node_names))
+        )
+        self.edge_weights = np.array(self.edge_weights)
+
+    def read_gfa_contigs(self):
+        skipped_contigs = set()
+        edge_edge_links = {}
+        contig_edge_links = {}
+        with open(os.path.join(self.data_dir, self.graphfile), "r") as f:
+            # ignore S entries (these are not contigs)
+            # the node seqs are read from the assembly file
+            for line in f:
+                if line.startswith("L"): # edge links
+                    values = line.strip().split()  # TAG, SRC, SIGN, DEST, SIGN, 0M, RC
+                    src_node_name = process_node_name(values[1], self.assembly_type)
+                    dst_node_name = process_node_name(values[3], self.assembly_type)
+                    edge_edge_links.setdefault(src_node_name,set()).add(values[3])
+                    edge_edge_links.setdefault(dst_node_name,set()).add(values[1])
+                elif line.startswith("P"): # contig to edge links
+                    values = line.strip().split()
+                    contig_name = process_node_name(values[1], self.assembly_type)
+                    if contig_name in skipped_contigs or contig_name not in self.node_names:
+                        #skipped_edges.add((contig_names.index(values[1]), contig_names.index(values[3])))
+                        continue
+                    for edge in values[2].split(","):
+                        contig_edge_links.setdefault(contig_name,set()).add(edge[:-1])
+                    self.graph_paths[values[1]] = [self.node_names.index(path_node_name[:-1]) \
+                        for path_node_name in values[2].split(",") if path_node_name[:-1] in self.node_names]
+        if len(contig_edge_links) == 0:
+            # load graph paths from assembly_info
+            self.logger.info("reading assembly_info file for graph paths...")
+            # TODO: check if file exists
+            contig_edge_links = self.read_assembly_info()
+        print("skipped contigs", len(skipped_contigs), "<", self.min_contig_length)
+        # create graph, , and to linked to adjacent edges
+        # first create edge to contig index
+        edge_contig_links = {}
+        for contig in contig_edge_links:
+            for e in contig_edge_links[contig]:
+                edge_contig_links.setdefault(e, set()).add(contig)
+        for contig in contig_edge_links:
+            src_index = self.node_names.index(contig)
+            for edge in contig_edge_links[contig]:
+                # connect contigs linked to same edge
+                for contig2 in edge_contig_links[edge]:
+                    dst_index = self.node_names.index(contig2)
+                    if contig2 != contig:
+                        self.edges_src.append(src_index)
+                        self.edges_dst.append(dst_index)
+                        self.edge_weights.append(1)
+                        # inverse is added when we get to contig2
+                for edge2 in edge_edge_links.get(edge, []):
+                    for contig2 in edge_contig_links.get(edge2, []):
+                        dst_index = self.node_names.index(contig2)
+                        self.edges_src.append(src_index)
+                        self.edges_dst.append(dst_index)
+                        self.edge_weights.append(1)
+        #self.logger.info(f"skipped contigs {len(skipped_contigs)} < {self.min_contig_length}")
+        self.adj_matrix = scipy.sparse.coo_matrix(
+            (self.edge_weights, (self.edges_src, self.edges_dst)), shape=(len(self.node_names), len(self.node_names))
+        )
+        self.edge_weights = np.array(self.edge_weights)
+
+    def read_assembly_info(self, get_graph_paths=False, circular_length=100000) -> Dict[str,list]:
+        """Read assembly_info.txt file generated by flye
+        """
+        self.circular_contigs: List[str] = []
+        self.repetitive_contigs: List[str] = []
+        self.contigs_multiplicity = {}
+        contig_edge_links = {}
+        with open(os.path.join(self.data_dir, "assembly_info.txt"), "r") as f:
+            next(f) # skip header
+            for line in f:
+                values = line.strip().split("\t")
+                contig_name = process_node_name(values[0], self.assembly_type)
+                if values[3] == "Y" and int(values[1]) > circular_length:
+                    self.circular_contigs.append(contig_name)
+                if values[4] == "Y":
+                    self.repetitive_contigs.append(contig_name)
+                #if contig_name not in self.node_names:
+                    #skipped_edges.add((contig_names.index(values[1]), contig_names.index(values[3])))
+                #    continue
+                self.contigs_multiplicity[contig_name] = int(values[5])
+                # get graph_paths
+                for edge in values[-1].split(","):
+                    if edge != "*":
+                        contig_edge_links.setdefault(contig_name,set()).add("edge_" + edge.strip("-"))
+                if get_graph_paths:
+                    self.graph_paths[contig_name] = ["edge_" + e for e in contig_edge_links[contig_name]]
+                #for edge_name in self.graph_paths[contig_name]:
+                #    self.contigs_multiplicity[self.node_names.index(edge_name)] = int(values[5])
+        return contig_edge_links
+    
+    def print_circular_contigs(self):
+        """Print circular contigs and info, based on flye
+        """
+        for contig_name in self.circular_contigs:
+            print("found circular contig", contig_name,
+                  "mult.", self.contigs_multiplicity[contig_name])
+            # get edges of this contig
+            contig_edges = self.graph_paths[contig_name]
+            print("---", "name", "depth", "markers", "label", "edges")
+            for edge_id in contig_edges:
+                #edge_id = self.node_names.index("edge_" + edge)
+                edge_name = self.node_names[edge_id]
+                print("---", edge_id, edge_name, self.node_lengths[edge_id],
+                      [round(d, 4) for d in self.node_depths[edge_id]],
+                      self.node_to_label[edge_name],
+                      len(self.contig_markers.get(edge_name, [])),
+                      list(self.adj_matrix.getrow(edge_id).data))
+
+    def read_depths(self) -> None:
+        node_depths: Dict[str, np.array] = {}
+        if self.depthfile is not None and os.path.exists(os.path.join(self.data_dir, self.depthfile)):
+            if self.depthfile.endswith(".npz"):
+                self.node_depths = np.load(open(os.path.join(self.data_dir, self.depthfile), "rb"))["arr_0"]
+                if self.node_depths.shape[0] != len(self.node_names):
+                    print("depth npz file mismatch:")
+                    breakpoint()
+            else:
+                with open(os.path.join(self.data_dir, self.depthfile)) as f:
+                    header = next(f)
+                    depth_i = [i + 3 for i, n in enumerate(header.split("\t")[3:]) if "-var" not in n]
+                    # var_i = [i + 3 for i, n in enumerate(header.split("\t")[3:]) if "-var" in n]
+                    for line in f:
+                        values = line.strip().split()
+                        node_name = process_node_name(values[0], self.assembly_type)
+                        if node_name in self.node_names:
+                            node_depths[node_name] = np.array([float(values[i]) for i in depth_i])
+                        else:
+                            self.logger.info("node name not found: {}".format(node_name))
+                if len(node_depths) != len(self.node_names):
+                    self.logger.info("missing abundance for some nodes: {}".format(len(node_depths) - len(self.node_names)))
+                self.node_depths = np.array([node_depths.get(n, [0]*len(depth_i)) for n in self.node_names])
+            if len(self.node_depths[0]) > 1:  # normalize depths
+                depthssum = self.node_depths.sum(axis=1) + 1e-10
+                self.node_depths /= depthssum.reshape((-1, 1))
+            else:
+                self.node_depths = stats.zscore(self.node_depths, axis=0)
+        else:
+            self.node_depths = np.ones(len(self.node_names), dtype=np.float)
+
+    def read_labels(self):
+        # logging.info("loading labels from {}".format(args.labels))
+        if self.labelsfile is not None:
+            node_to_label = {c: "NA" for c in self.node_names}
+            labels = set(["NA"])
+            with open(os.path.join(self.data_dir, self.labelsfile), "r") as f:
+                for line in f:
+                    # label, node = line.strip().split()
+                    if self.labelsfile.endswith(".csv"):
+                        values = line.strip().split(",")
+                    elif self.labelsfile.endswith(".tsv"):  # amber format
+                        if line.startswith("@") or line.startswith("#"):
+                            continue
+                        values = line.strip().split("\t")
+                    if len(values) < 2:
+                        breakpoint()
+                    node_name = process_node_name(values[0], self.assembly_type)
+                    label = values[1]
+                    if node_name in node_to_label:
+                        node_to_label[node_name] = label
+                        labels.add(label)
+                    else:
+                        breakpoint()
+                        self.logger.info(("unused label: {}".format(line.strip())))
+            labels = list(labels)
+            label_to_node = {s: [] for s in labels}
+            for n in node_to_label:
+                s = node_to_label[n]
+                label_to_node[s].append(n)
+            self.node_to_label = {n: l for n, l in node_to_label.items()}
+            self.labels = labels
+            self.label_to_node = label_to_node
+            # calculate homophily
+            if len(self.edge_weights) > 1:
+                self.calculate_homophily()
+        else:
+            self.labels = ["NA"]
+            self.label_to_node = {"NA": self.node_names}
+            self.node_to_label = {n: "NA" for n in self.node_names}
+
+    def calculate_homophily(self):
+        """
+        Calculate percentage of edges that connect nodes with the same label
+        """
+        positive_edges = 0
+        edges_without_label = 0
+        for u, v in zip(self.edges_src, self.edges_dst):
+            if self.node_to_label.get(self.node_names[u], "NA") == "NA" or \
+               self.node_to_label.get(self.node_names[v], "NA") == "NA":
+                edges_without_label += 1
+            if self.node_to_label[self.node_names[u]] == self.node_to_label[self.node_names[v]] and self.node_to_label[self.node_names[u]] != "NA":
+                positive_edges += 1
+        self.logger.info(
+            f"""homophily: {round(positive_edges / (len(self.edge_weights) - edges_without_label),4)} on
+            {len(self.edge_weights) - edges_without_label} edges between labeled nodes"""
+        )
+
+    def read_scgs(self):
+        # Load contig marker genes (Bacteria list)
+        if self.scgfile is not None:
+            # logging.info("loading checkm results")
+            scg_path = os.path.join(self.data_dir, self.scgfile)
+            ref_sets = read_marker_gene_sets(BACTERIA_MARKERS)
+            contig_markers = read_contig_genes(scg_path)
+            self.ref_marker_sets = ref_sets
+            self.contig_markers = contig_markers
+            marker_counts = get_markers_to_contigs(ref_sets, contig_markers)
+            self.markers = marker_counts
+        else:
+            self.ref_marker_sets = {}
+            self.contig_markers = {}
+            self.run_checkm()
+
+    def get_all_different_idx(self):
+        """
+        Returns a 2d numpy array where each row
+        corresponds to a pairs of node idx whose
+        feature must be different as they correspond
+        to the same contig (check jargon). This
+        should encourage the HQ value to be higher.
+        """
+        node_names_to_idx = {node_name: i for i, node_name in enumerate(self.node_names)}
+        pair_idx = set()
+        for n1 in self.contig_markers:
+            for gene1 in self.contig_markers[n1]:
+                for n2 in self.contig_markers:
+                    if n1 != n2 and gene1 in self.contig_markers[n2]:
+                        p1 = (node_names_to_idx[n1], node_names_to_idx[n2])
+                        p2 = (node_names_to_idx[n2], node_names_to_idx[n1])
+                        if (p1 not in pair_idx) and (p2 not in pair_idx):
+                            pair_idx.add(p1)
+        pair_idx = np.unique(np.array(list(pair_idx)), axis=0)
+        print("Number of diff cluster pairs:", len(pair_idx))
+        self.neg_pairs_idx = pair_idx
+
+    def run_vamb(self, vamb_outdir, cuda, vambdim):
+        from vamb.vamb_run import run as run_vamb
+        self.logger.info("running VAMB")
+        batchsteps = []
+        vamb_epochs = 500
+        if len(self.node_depths[0]) == 1:
+            vamb_bs = 32
+            batchsteps = [25, 75, 150]
+        else:
+            vamb_bs = 64
+            batchsteps = [25, 75, 150, 300]
+        nhiddens = [512, 512]
+        self.logger.info("using these batchsteps:{}".format(batchsteps))
+
+        vamb_logpath = os.path.join(vamb_outdir, "log.txt")
+        if os.path.exists(vamb_outdir) and os.path.isdir(vamb_outdir):
+            shutil.rmtree(vamb_outdir)
+        os.mkdir(vamb_outdir)
+        with open(vamb_logpath, "w") as vamb_logfile:
+            run_vamb(
+                outdir=vamb_outdir,
+                fastapath=os.path.join(self.data_dir, self.fastafile),
+                jgipath=os.path.join(self.data_dir, self.depthfile),
+                logfile=vamb_logfile,
+                cuda=cuda,
+                batchsteps=batchsteps,
+                batchsize=vamb_bs,
+                nepochs=vamb_epochs,
+                mincontiglength=self.min_contig_length,
+                nhiddens=nhiddens,
+                nlatent=int(vambdim),
+                norefcheck=True,
+            )
+            if self.data_dir != "" and self.featuresfile.endswith(".tsv"):
+                shutil.copyfile(os.path.join(vamb_outdir, "embs.tsv"), self.featuresfile)
+            self.logger.info("Contig features saved to {}".format(self.featuresfile))
+
+    def read_features(self):
+        node_embs = {}
+        self.logger.info("loading features from {}".format(self.featuresfile))
+        if self.featuresfile.endswith(".tsv"):
+            with open(self.featuresfile, "r") as ffile:
+                for line in ffile:
+                    values = line.strip().split()
+                    node_embs[values[0]] = [float(x) for x in values[1:]]
+            self.logger.info("loaded {} features/ {} nodes from tsv".format(len(node_embs), len(self.node_names)))
+        elif self.featuresfile.endswith(".pickle"):
+            with open(self.featuresfile, "rb") as ffile:
+                node_embs = pickle.load(ffile)
+            self.logger.info("loaded {} features/ {} nodes from pickle".format(len(node_embs), len(self.node_names)))
+        self.node_embs = [
+                node_embs.get(n, np.random.uniform(10e-5, 1.0, len(node_embs[list(node_embs.keys())[0]]))) for n in self.node_names
+            ]  # deal with missing embs
+        self.node_embs = np.array(self.node_embs)
+
+    def write_features_tsv(self):
+        self.logger.info("writing features to {}".format(self.featuresfile))
+        with open(self.featuresfile, "w") as ffile:
+            for i, emb in enumerate(self.node_embs):
+                ffile.write(f"{self.node_names[i]} {' '.join(map(str,emb.tolist()))}\n")
+
+    def get_topk_neighbors(self, k, scg_only=False):
+        """
+        Returns a list of the top k neighbors for each node. Use kmers and abundance
+
+        """
+        #breakpoint()
+        self.logger.info("getting top {} neighbors".format(k))
+        self.topk_neighbors = []
+        features = np.concatenate((self.node_kmers, self.node_depths), axis=1)
+        cosine_dists = np.dot(features, features.T)
+        for i in range(len(self.node_names)):
+            self.topk_neighbors.append(set(np.argsort(cosine_dists[i])[-k:]))
+        self.logger.info("got top {} neighbors".format(k))
+
+    def estimate_n_genomes(self):
+        self.scg_counts = {}
+        for marker_set in self.ref_marker_sets:
+            for gene in marker_set:
+                self.scg_counts[gene] = 0
+                for contig in self.contig_markers:
+                    if gene in self.contig_markers[contig]:
+                        self.scg_counts[gene] += self.contig_markers[contig][gene]
+
+        #print(self.scg_counts)
+        quartiles = np.percentile(list(self.scg_counts.values()), [25, 50, 75])
+        print("candidate k0s", sorted(set([k for k in self.scg_counts.values() if k >= quartiles[2]])))
+        return max(self.scg_counts.values())
+        
+       
+    def run_checkm(self, nthreads=10, tempdir="../temp"):
+        # check if checkm is installed
+        checkm_is_avail = shutil.which("checkm") is not None
+        # if not, print commands only
+        commands = [
+            "mkdir {}/nodes".format(self.data_dir), #; cd nodes; ",
+            "cat {0}/{1} | awk '{{ if (substr($0, 1, 1)=='>') {{filename=(substr($0,2) '.fa')}} print $0 > {0}/filename }}".format(self.data_dir, self.fastafile),
+            'find {}/nodes/ -name "* *" -type f | rename "s/ /_/g"'.format(self.data_dir),
+            "checkm taxonomy_wf --tmpdir {0} -t {1} -x fa domain Bacteria {2}/nodes/ {2}/checkm_nodes/".format(tempdir, nthreads, self.data_dir)
+        ]
+        if checkm_is_avail:
+            #run commands one by one
+            for cmd in commands:
+                os.system(cmd)
+        else:
+            print("Run this on a machine with CheckM installed")
+            for cmd in commands:
+                print(cmd)
+
+
+    def read_gtdbtk_files(self, prefix="gtdbtk", suffix_labels="summary.tsv",
+                          suffix_markers="markers_summary.tsv", reset=True):
+        # use summary to add species level labels
+        # also save full lineages
+        roots = ["bac120"] #, "ar53"]
+        no_species = 0
+        no_genus = 0
+        species_labels = set()
+        # reset labels
+        if reset:
+            self.node_to_label = {n: "NA" for n in self.node_names}
+            self.labels = ["NA"]
+        contig_markers = {n: {} for n in self.node_names}
+        ref_markers = set()
+        for root in roots:
+            # read labels
+            with open(os.path.join(self.data_dir, f"{prefix}.{root}.{suffix_labels}"), 'r') as f:
+                next(f) # skip header
+                for line in f:
+                    values = line.strip().split("\t")
+                    node_name = process_node_name(values[0], self.assembly_type)
+                    if values[1].startswith("Unclassified"):
+                        continue # do not add unclassified nodes
+                    classification = values[1].split(";")
+                    node_slabel = classification[-1]
+                    node_glabel = classification[-2]
+                    #if values[5] != "N/A":
+                    #    fast_ani = float(values[5])
+                    #    anis.append(fast_ani)
+                    if node_slabel == "s__":
+                        no_species += 1
+                    else:
+                        self.node_to_label[node_name] = node_slabel
+                        species_labels.add(node_slabel)
+                    #if node_slabel == "g__":
+                    #    no_genus += 1
+                    #else:
+                    #    node_to_glabel[node_name] = node_glabel
+                    #    genus_labels.add(node_glabel)
+
+            # read markers
+            with open(os.path.join(self.data_dir, f"{prefix}.{root}.{suffix_markers}"), 'r') as f:
+                next(f) # skip header
+                for line in f:
+                    values = line.strip().split("\t")
+                    node_name = process_node_name(values[0], self.assembly_type)
+                    if int(values[1]) > 0:
+                        contig_markers[node_name] = {g: 1 for g in values[5].split(",")}
+                        ref_markers.update(set(contig_markers[node_name]))
+                    if int(values[4]) > 0:
+                        ref_markers.update(set(values[-1].split(",")))
+        # create ref labels and ref markers
+        self.labels += list(species_labels)
+        self.label_to_node = {s: [] for s in self.labels}
+        for n in self.node_to_label:
+            s = self.node_to_label[n]
+            self.label_to_node[s].append(n)
+        assert len(ref_markers) == 120 # GTDB-tk bac and ar markers
+        if reset:
+            self.ref_marker_sets = [ref_markers]    
+            self.contig_markers = contig_markers
+            marker_counts = get_markers_to_contigs(self.ref_marker_sets, contig_markers)
+            self.markers = marker_counts
+
+    def get_edges_with_same_scgs(self):
+        """Check every edge to see if nodes have SCGs in common
+
+        :return: edges IDs (edges_src, edges_dst, edge_weight)
+        :rtype: list
+        """
+        edge_ids_with_same_scgs = []
+        scg_counter = Counter()
+        for x, (i, j) in enumerate(zip(self.edges_src, self.edges_dst)):
+            if self.node_names[i] in self.contig_markers and self.node_names[j] in self.contig_markers and \
+                len(self.contig_markers[self.node_names[i]]) > 0 and len(self.contig_markers[self.node_names[j]]) > 0:
+            
+                overlap = len(self.contig_markers[self.node_names[i]].keys() & \
+                    self.contig_markers[self.node_names[j]].keys())
+                if overlap > 0 and i != j:
+                    #remove edge
+                    scg_counter[overlap] += 1
+                    edge_ids_with_same_scgs.append(x)
+        print("edges with overlapping scgs (max=20):", scg_counter.most_common(20))
+        return edge_ids_with_same_scgs
+
+    def generate_edges_based_on_labels(self, noise=0):
+        # link nodes with same labels and create new adj_matrix/edges_src/edges_dst/edge_weights
+        #new_edges = []
+        new_srcs = []
+        new_dsts = []
+        for label in self.label_to_node:
+            # make circular graph
+            for i in range(len(self.label_to_node[label])):
+                new_src = self.node_names.index(self.label_to_node[label][i])
+                new_srcs.append(new_src)
+                if i+1 < len(self.label_to_node[label]):
+                    new_dst = self.node_names.index(self.label_to_node[label][i+1])
+                else: # connect to element 0
+                    new_dst = self.node_names.index(self.label_to_node[label][0])
+                #new_edges.append((new_src, new_dst))
+                new_dsts.append(new_dst)
+        new_weights = [1] * len(new_srcs)
+        print("creating new graph with {} edges".format(len(new_srcs)))
+        self.adj_matrix = scipy.sparse.coo_matrix(
+            (new_weights, (new_srcs, new_dsts)), shape=(len(self.node_names), len(self.node_names))
+        )
+        self.edges_src = new_srcs
+        self.edges_dst = new_dsts
+        self.edge_weights = np.array(new_weights)
+
+
+
```

### Comparing `graphmb-0.2.4/src/graphmb/dgl_dataset.py` & `graphmb-0.2.5/src/graphmb/dgl_dataset.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,210 +1,210 @@
-import os
-import torch
-os.environ["DGLBACKEND"] = "pytorch"
-import dgl
-from dgl.data import DGLDataset
-import networkx as nx
-
-class DGLAssemblyDataset(DGLDataset):
-    def __init__(self, assembly):
-        self.assembly = assembly
-        self.logger = assembly.logger
-        super().__init__(name=assembly.name + "assembly_graph", save_dir=assembly.cache_dir, force_reload=False)
-
-    def __getitem__(self, i):
-        return self.graph
-
-    def __len__(self):
-        return 1
-
-    def process(self, root=False):
-        """Open GFA file to DGL format"""
-        # TODO: this should receive and assembly dataset object and initialize self.graph
-        # if root:
-        #    root_node = G.add_node("root", length=0)
-        # TODO: skip unconnected and too short/big
-        self.logger.info("creating DGL graph")
-        self.graph = dgl.graph(
-            (self.assembly.edges_src, self.assembly.edges_dst),
-            num_nodes=len(self.assembly.node_names),
-        )
-        self.graph.edata["weight"] = torch.tensor(self.assembly.edge_weights)
-
-        self.logger.info("done")
-        self.graph.ndata["label"] = torch.LongTensor(
-            [self.assembly.labels.index(self.assembly.node_to_label[n]) if self.assembly.node_to_label[n] in self.assembly.labels else 0 for n in self.assembly.node_names]
-        )
-
-        nx_graph = self.graph.to_networkx().to_undirected()
-        self.logger.info("connected components...")
-        # self.connected = [c for c in sorted(nx.connected_components(nx_graph), key=len, reverse=True) if len(c) > 1]
-        # breakpoint()
-        self.connected = [c for c in sorted(nx.connected_components(nx_graph), key=len, reverse=True) if len(c) > 0]
-        self.logger.info((len(self.connected), "connected"))
-        # for group in self.connected:
-        #    self.graphs.append(
-        #        dgl.node_subgraph(self.graph, [self.node_names.index(c) for c in group if c in self.node_names])
-        #    )
-
-        assert len([c for comp in self.connected for c in comp]) <= len(self.assembly.node_names)
-
-        # self.set_node_mask()
-
-    def save(self):
-        pass
-        # save graphs and labels
-        # save other information in python dict
-        """info_path = os.path.join(self.save_path, "cache.pkl")
-        print("saving graph", info_path)
-        if not os.path.exists(self.save_path):
-            os.makedirs(self.save_path)
-        save_info(info_path, vars(self))"""
-
-    def load(self):
-        pass
-        # load processed data from directory `self.save_path`
-        """ info_path = os.path.join(self.save_path, "cache.pkl")
-        print("loading from", info_path)
-        loaded_info = load_info(info_path)
-        for key in loaded_info:
-            setattr(self, key, loaded_info[key])"""
-
-    def has_cache(self):
-        """# check whether there are processed data in `self.save_path`
-        info_path = os.path.join(self.save_path, "cache.pkl")
-        return os.path.exists(info_path)"""
-        return False
-
-
-class ContigsDataset(DGLDataset):
-    def __init__(
-        self,
-        name,
-        assembly_path=None,
-        assembly_name="assembly.fasta",
-        graph_file="assembly_graph.gfa",
-        labels=None,
-        save_dir=None,
-        force_reload=False,
-        min_contig=1000,
-        kmer=4,
-        depth=None,
-        markers=None,
-        load_kmer=False,
-        assembly_type="flye",
-    ):
-        self.mode = "train"
-        # self.save_dir = save_dir
-        self.assembly = assembly_path
-        if self.assembly is None:
-            self.assembly = ""
-        self.readmapping = assembly_path
-        self.assembly_name = assembly_name
-        self.graph_file = graph_file
-        self.depth = depth
-        self.markers = markers
-        self.contig_names = []
-        self.contig_seqs = {}
-        self.read_names = []
-        self.node_names = []  # contig_names + read_names
-        self.nodes_len = []
-        self.nodes_depths = []
-        self.nodes_markers = []
-        self.nodes_kmer = []
-        self.graphs = []
-        self.edges_src = []
-        self.edges_dst = []
-        self.edges_weight = []
-        self.nodes_data = []
-        self.node_to_label = {}
-        self.node_labels = []
-        self.kmer = kmer
-        self.load_kmer = load_kmer
-        self.assembly_type = assembly_type
-        if self.load_kmer:
-            self.kmer_to_ids, self.canonical_k = get_kmer_to_id(self.kmer)
-
-        self.connected = []
-        self.min_contig_len = min_contig
-        if labels is None:
-            self.species = ["NA"]
-            self.add_new_species = True
-        else:
-            self.species = labels
-            self.add_new_species = False
-        super().__init__(name=name, save_dir=save_dir, force_reload=force_reload)
-
-    def filter_edges(self, weight=0):
-        """Filter edges based on weight"""
-        # print(max(self.edges_weight), min(self.edges_weight))
-        if weight < 0:
-            weight = sum(self.edges_weight) / len(self.edges_weight)
-        # for i in range(max(self.edges_weight)):
-        #    print(i, self.edges_weight.count(i))
-        keep_idx = self.graph.edata["weight"] >= weight
-        idx_to_remove = [i for i, x in enumerate(keep_idx) if not x]
-        self.edges_src = [self.edges_src[i] for i in keep_idx]
-        self.edges_dst = [self.edges_dst[i] for i in keep_idx]
-        # self.graph.edata["weight"] = self.graph.edata["weight"][keep_idx]
-        self.graph.remove_edges(idx_to_remove)
-
-    def filter_contigs(self):
-        # remove disconnected
-        keep_idx = [i for i, c in enumerate(self.contig_names) if c in self.edges_src or c in self.edges_dst]
-        # keep_idx = [i for i, c in enumerate(self.contig_names)]
-        self.contig_names = [self.contig_names[i] for i in keep_idx]
-        self.nodes_kmer = [self.nodes_kmer[i] for i in keep_idx]
-        self.nodes_depths = [self.nodes_depths[i] for i in keep_idx]
-        self.nodes_len = [self.nodes_len[i] for i in keep_idx]
-
-    def remove_nodes(self, remove_list):
-        self.graph.remove_nodes(torch.tensor(remove_list))
-        # self.contig_seqs = {}
-        self.node_names = [self.node_names[i] for i in range(len(self.node_names)) if i not in remove_list]
-        self.nodes_len = [self.nodes_len[i] for i in range(len(self.nodes_len)) if i not in remove_list]
-        self.nodes_depths = [self.nodes_depths[i] for i in range(len(self.nodes_depths)) if i not in remove_list]
-        self.nodes_markers = [self.nodes_markers[i] for i in range(len(self.nodes_markers)) if i not in remove_list]
-        self.nodes_kmer = [self.nodes_kmer[i] for i in range(len(self.nodes_kmer)) if i not in remove_list]
-        # self.edges_src = []
-        # self.edges_dst = []
-        # self.edges_weight = []
-        self.nodes_data = [self.nodes_data[i] for i in range(len(self.nodes_data)) if i not in remove_list]
-        # self.node_to_label = {}
-        self.node_labels = [self.node_labels[i] for i in range(len(self.node_labels)) if i not in remove_list]
-
-    def rename_nodes_to_index(self):
-        # self.edges_src = [self.contig_names.index(i) for i in self.edges_src if i in self.contig_names]
-        # self.edges_dst = [self.contig_names.index(i) for i in self.edges_dst if i in self.contig_names]
-        edge_name_to_index = {n: i for i, n in enumerate(self.contig_names)}
-        self.edges_src = [edge_name_to_index[n] for n in self.edges_src]
-        self.edges_dst = [edge_name_to_index[n] for n in self.edges_dst]
-
-    def set_node_mask(self):
-        """Set contig nodes"""
-        self.graph.ndata["contigs"] = torch.zeros(len(self.node_names), dtype=torch.bool)
-        self.graph.ndata["contigs"][: len(self.contig_names)] = True
-
-    def get_labels_from_reads(self, reads, add_new=True):
-        contig_to_species = {}
-        read_to_species = {}
-        # contig_lens = {}
-        for r in reads:
-            # print(r)
-            speciesname = r.split("_reads")[0]
-
-            if speciesname not in self.species:
-                if add_new:
-                    self.species.append(speciesname)
-                else:
-                    continue
-            for m in reads[r].mappings:
-                if m.contigname not in contig_to_species:  # and m.contigname in contig_lens:
-                    contig_to_species[m.contigname] = {}
-                if speciesname not in contig_to_species[m.contigname]:
-                    contig_to_species[m.contigname][speciesname] = 0
-                # contig_to_species[m.contigname][speciesname] += m.mapq  # weight mapping by quality
-                contig_to_species[m.contigname][speciesname] += 1  # weight mapping by len
-                read_to_species[r] = speciesname
-                # reads_count = int(values[0])
-            # contig_to_species[values[1]][speciesname] = reads_count
-        return contig_to_species, read_to_species
+import os
+import torch
+os.environ["DGLBACKEND"] = "pytorch"
+import dgl
+from dgl.data import DGLDataset
+import networkx as nx
+
+class DGLAssemblyDataset(DGLDataset):
+    def __init__(self, assembly):
+        self.assembly = assembly
+        self.logger = assembly.logger
+        super().__init__(name=assembly.name + "assembly_graph", save_dir=assembly.cache_dir, force_reload=False)
+
+    def __getitem__(self, i):
+        return self.graph
+
+    def __len__(self):
+        return 1
+
+    def process(self, root=False):
+        """Open GFA file to DGL format"""
+        # TODO: this should receive and assembly dataset object and initialize self.graph
+        # if root:
+        #    root_node = G.add_node("root", length=0)
+        # TODO: skip unconnected and too short/big
+        self.logger.info("creating DGL graph")
+        self.graph = dgl.graph(
+            (self.assembly.edges_src, self.assembly.edges_dst),
+            num_nodes=len(self.assembly.node_names),
+        )
+        self.graph.edata["weight"] = torch.tensor(self.assembly.edge_weights)
+
+        self.logger.info("done")
+        self.graph.ndata["label"] = torch.LongTensor(
+            [self.assembly.labels.index(self.assembly.node_to_label[n]) if self.assembly.node_to_label[n] in self.assembly.labels else 0 for n in self.assembly.node_names]
+        )
+
+        nx_graph = self.graph.to_networkx().to_undirected()
+        self.logger.info("connected components...")
+        # self.connected = [c for c in sorted(nx.connected_components(nx_graph), key=len, reverse=True) if len(c) > 1]
+        # breakpoint()
+        self.connected = [c for c in sorted(nx.connected_components(nx_graph), key=len, reverse=True) if len(c) > 0]
+        self.logger.info((len(self.connected), "connected"))
+        # for group in self.connected:
+        #    self.graphs.append(
+        #        dgl.node_subgraph(self.graph, [self.node_names.index(c) for c in group if c in self.node_names])
+        #    )
+
+        assert len([c for comp in self.connected for c in comp]) <= len(self.assembly.node_names)
+
+        # self.set_node_mask()
+
+    def save(self):
+        pass
+        # save graphs and labels
+        # save other information in python dict
+        """info_path = os.path.join(self.save_path, "cache.pkl")
+        print("saving graph", info_path)
+        if not os.path.exists(self.save_path):
+            os.makedirs(self.save_path)
+        save_info(info_path, vars(self))"""
+
+    def load(self):
+        pass
+        # load processed data from directory `self.save_path`
+        """ info_path = os.path.join(self.save_path, "cache.pkl")
+        print("loading from", info_path)
+        loaded_info = load_info(info_path)
+        for key in loaded_info:
+            setattr(self, key, loaded_info[key])"""
+
+    def has_cache(self):
+        """# check whether there are processed data in `self.save_path`
+        info_path = os.path.join(self.save_path, "cache.pkl")
+        return os.path.exists(info_path)"""
+        return False
+
+
+class ContigsDataset(DGLDataset):
+    def __init__(
+        self,
+        name,
+        assembly_path=None,
+        assembly_name="assembly.fasta",
+        graph_file="assembly_graph.gfa",
+        labels=None,
+        save_dir=None,
+        force_reload=False,
+        min_contig=1000,
+        kmer=4,
+        depth=None,
+        markers=None,
+        load_kmer=False,
+        assembly_type="flye",
+    ):
+        self.mode = "train"
+        # self.save_dir = save_dir
+        self.assembly = assembly_path
+        if self.assembly is None:
+            self.assembly = ""
+        self.readmapping = assembly_path
+        self.assembly_name = assembly_name
+        self.graph_file = graph_file
+        self.depth = depth
+        self.markers = markers
+        self.contig_names = []
+        self.contig_seqs = {}
+        self.read_names = []
+        self.node_names = []  # contig_names + read_names
+        self.nodes_len = []
+        self.nodes_depths = []
+        self.nodes_markers = []
+        self.nodes_kmer = []
+        self.graphs = []
+        self.edges_src = []
+        self.edges_dst = []
+        self.edges_weight = []
+        self.nodes_data = []
+        self.node_to_label = {}
+        self.node_labels = []
+        self.kmer = kmer
+        self.load_kmer = load_kmer
+        self.assembly_type = assembly_type
+        if self.load_kmer:
+            self.kmer_to_ids, self.canonical_k = get_kmer_to_id(self.kmer)
+
+        self.connected = []
+        self.min_contig_len = min_contig
+        if labels is None:
+            self.species = ["NA"]
+            self.add_new_species = True
+        else:
+            self.species = labels
+            self.add_new_species = False
+        super().__init__(name=name, save_dir=save_dir, force_reload=force_reload)
+
+    def filter_edges(self, weight=0):
+        """Filter edges based on weight"""
+        # print(max(self.edges_weight), min(self.edges_weight))
+        if weight < 0:
+            weight = sum(self.edges_weight) / len(self.edges_weight)
+        # for i in range(max(self.edges_weight)):
+        #    print(i, self.edges_weight.count(i))
+        keep_idx = self.graph.edata["weight"] >= weight
+        idx_to_remove = [i for i, x in enumerate(keep_idx) if not x]
+        self.edges_src = [self.edges_src[i] for i in keep_idx]
+        self.edges_dst = [self.edges_dst[i] for i in keep_idx]
+        # self.graph.edata["weight"] = self.graph.edata["weight"][keep_idx]
+        self.graph.remove_edges(idx_to_remove)
+
+    def filter_contigs(self):
+        # remove disconnected
+        keep_idx = [i for i, c in enumerate(self.contig_names) if c in self.edges_src or c in self.edges_dst]
+        # keep_idx = [i for i, c in enumerate(self.contig_names)]
+        self.contig_names = [self.contig_names[i] for i in keep_idx]
+        self.nodes_kmer = [self.nodes_kmer[i] for i in keep_idx]
+        self.nodes_depths = [self.nodes_depths[i] for i in keep_idx]
+        self.nodes_len = [self.nodes_len[i] for i in keep_idx]
+
+    def remove_nodes(self, remove_list):
+        self.graph.remove_nodes(torch.tensor(remove_list))
+        # self.contig_seqs = {}
+        self.node_names = [self.node_names[i] for i in range(len(self.node_names)) if i not in remove_list]
+        self.nodes_len = [self.nodes_len[i] for i in range(len(self.nodes_len)) if i not in remove_list]
+        self.nodes_depths = [self.nodes_depths[i] for i in range(len(self.nodes_depths)) if i not in remove_list]
+        self.nodes_markers = [self.nodes_markers[i] for i in range(len(self.nodes_markers)) if i not in remove_list]
+        self.nodes_kmer = [self.nodes_kmer[i] for i in range(len(self.nodes_kmer)) if i not in remove_list]
+        # self.edges_src = []
+        # self.edges_dst = []
+        # self.edges_weight = []
+        self.nodes_data = [self.nodes_data[i] for i in range(len(self.nodes_data)) if i not in remove_list]
+        # self.node_to_label = {}
+        self.node_labels = [self.node_labels[i] for i in range(len(self.node_labels)) if i not in remove_list]
+
+    def rename_nodes_to_index(self):
+        # self.edges_src = [self.contig_names.index(i) for i in self.edges_src if i in self.contig_names]
+        # self.edges_dst = [self.contig_names.index(i) for i in self.edges_dst if i in self.contig_names]
+        edge_name_to_index = {n: i for i, n in enumerate(self.contig_names)}
+        self.edges_src = [edge_name_to_index[n] for n in self.edges_src]
+        self.edges_dst = [edge_name_to_index[n] for n in self.edges_dst]
+
+    def set_node_mask(self):
+        """Set contig nodes"""
+        self.graph.ndata["contigs"] = torch.zeros(len(self.node_names), dtype=torch.bool)
+        self.graph.ndata["contigs"][: len(self.contig_names)] = True
+
+    def get_labels_from_reads(self, reads, add_new=True):
+        contig_to_species = {}
+        read_to_species = {}
+        # contig_lens = {}
+        for r in reads:
+            # print(r)
+            speciesname = r.split("_reads")[0]
+
+            if speciesname not in self.species:
+                if add_new:
+                    self.species.append(speciesname)
+                else:
+                    continue
+            for m in reads[r].mappings:
+                if m.contigname not in contig_to_species:  # and m.contigname in contig_lens:
+                    contig_to_species[m.contigname] = {}
+                if speciesname not in contig_to_species[m.contigname]:
+                    contig_to_species[m.contigname][speciesname] = 0
+                # contig_to_species[m.contigname][speciesname] += m.mapq  # weight mapping by quality
+                contig_to_species[m.contigname][speciesname] += 1  # weight mapping by len
+                read_to_species[r] = speciesname
+                # reads_count = int(values[0])
+            # contig_to_species[values[1]][speciesname] = reads_count
+        return contig_to_species, read_to_species
```

### Comparing `graphmb-0.2.4/src/graphmb/evaluate.py` & `graphmb-0.2.5/src/graphmb/evaluate.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,593 +1,593 @@
-import sys
-import ast
-import os
-import numpy as np
-import scipy
-import itertools
-import random
-from sklearn.metrics.pairwise import cosine_similarity
-
-from graphmb.visualize import run_tsne, plot_embs
-from graphmb.utils import run_clustering
-# code to run evaluation based on lineage.ms file (Bacteria) and marker_gene_stats.txt file
-
-# Get precicion
-def getPrecision(mat, k, s, total):
-    sum_k = 0
-    for i in range(k):
-        max_s = 0
-        for j in range(s):
-            if mat[i][j] > max_s:
-                max_s = mat[i][j]
-        sum_k += max_s  
-    return sum_k / total
-
-
-# Get recall
-def getRecall(mat, k, s, total, unclassified):
-    sum_s = 0
-    for i in range(s):
-        max_k = 0
-        for j in range(k):
-            if mat[j][i] > max_k:
-                max_k = mat[j][i]
-        sum_s += max_k
-    return sum_s / (total + unclassified)
-
-
-def getAveragePrecision(cluster_to_labels, cluster_sizes):
-    avg_precision = []
-    for c in cluster_to_labels:
-        #TP = cluster_to_labels[c][1]; TP+FP + cluster_sizes[c]
-        cluster_p = cluster_to_labels[c][1] / cluster_sizes[c]
-        avg_precision.append(cluster_p)
-    return round(sum(avg_precision) / len(avg_precision), 4)
-
-def getAverageRecall(label_to_cluster, cluster_to_contig, contig_sizes, label_to_node):
-    avg_recall = []
-    for label in label_to_cluster:
-        if label_to_cluster[label][0] == "NA":
-            avg_recall.append(0)
-        else:
-            cluster_r = label_to_cluster[label][1] / sum([contig_sizes.get(n, 1) for n in cluster_to_contig[label_to_cluster[label][0]]])
-            avg_recall.append(cluster_r)
-    return round(sum(avg_recall) / len(avg_recall), 4)
-
-
-# Get ARI
-def getARI(mat, k, s, N):
-    t1 = 0
-    for i in range(k):
-        sum_k = 0
-        for j in range(s):
-            sum_k += mat[i][j]
-        t1 += scipy.special.binom(sum_k, 2)
-    t2 = 0
-    for i in range(s):
-        sum_s = 0
-        for j in range(k):
-            sum_s += mat[j][i]
-        t2 += scipy.special.binom(sum_s, 2)
-    t3 = t1 * t2 / scipy.special.binom(N, 2)
-    t = 0
-    for i in range(k):
-        for j in range(s):
-            t += scipy.special.binom(mat[i][j], 2)
-    ari = (t - t3) / ((t1 + t2) / 2 - t3)
-    return ari
-
-
-# Get F1-score
-def getF1(prec, recall):
-    if prec == 0.0 or recall == 0.0:
-        return 0.0
-    else:
-        return 2 * prec * recall / (prec + recall)
-
-
-def calculate_overall_prf(cluster_to_contig, contig_to_cluster, node_to_label, label_to_node):
-    # calculate how many contigs are in the majority class of each cluster
-    total_binned = 0
-    # convert everything to ids
-    labels = list(label_to_node.keys())
-    clusters = list(cluster_to_contig.keys())
-    n_pred_labels = len(clusters)
-    n_true_labels = len(labels)
-    ground_truth_count = len(node_to_label)
-    # empty matrix
-    bins_species = [[0 for x in range(n_true_labels)] for y in range(n_pred_labels)]
-    # update with cluster memberships
-    for i in contig_to_cluster:
-        if i in node_to_label:
-            # breakpoint()
-            total_binned += 1
-            bins_species[clusters.index(contig_to_cluster[i])][labels.index(node_to_label[i])] += 1
-    my_precision = getPrecision(bins_species, n_pred_labels, n_true_labels, total_binned)
-    my_recall = getRecall(
-        bins_species, n_pred_labels, n_true_labels, total_binned, (ground_truth_count - total_binned)
-    )
-    #my_ari = getARI(bins_species, n_pred_labels, n_true_labels, total_binned)
-    my_f1 = getF1(my_precision, my_recall)
-    return my_precision, my_recall, my_f1, 0
-
-def calculate_sim_between_same_labels_small(node_names, embeddings, edges, label_to_node, node_to_label):
-    # divide sim between node of same label by avg sim between all nodes
-    avg_label_sims = {}
-    # use only embeddings of nodes with labels
-    edges = np.array(edges)
-    # calculate sim between all embs
-    all_cosine_sim = cosine_similarity(embeddings, embeddings)
-    #https://stackoverflow.com/a/69865919
-    i = np.ravel_multi_index(np.array(edges).T, all_cosine_sim.shape)
-    edge_sim = all_cosine_sim.take(i) # get sim between embs of edges
-    edge_sim = edge_sim.sum()
-    #all_cosine_sim = np.triu(all_cosine_sim)
-    # all sim should not include sims of edges
-    all_cosine_sim = all_cosine_sim.sum() - edge_sim
-    all_cosine_sim = all_cosine_sim / ((embeddings.shape[0]**2)-len(edges))
-    edge_sim /= len(edges)
-    for l in label_to_node:
-        label_node_idxs = [node_names.index(n) for n in label_to_node[l]]
-        label_embs = np.array(embeddings)[label_node_idxs]
-        if label_embs.shape[0] > 1: # at least two nodes
-            avg_label_sims[l] = ((cosine_similarity(label_embs, label_embs))).mean()
-        # pick a random 
-    avg = sum(avg_label_sims.values())/len(avg_label_sims.values())      
-    #print(round(avg, 4), round(all_cosine_sim, 4))
-          #[(x, round(avg_label_sims[x], 4), len(label_to_node[x])) for x in avg_label_sims][:10]])
-    return avg, edge_sim, all_cosine_sim
-
-
-def calculate_sim_between_same_labels_big(node_names, embeddings, edges, label_to_node, node_to_label):
-    # divide sim between node of same label by avg sim between all nodes
-    avg_label_sims = {}
-    # use only embeddings of nodes in edges to make it more efficient
-    edges = np.array(edges)
-    node_idx_with_edges = np.unique(edges)
-    #label_mask = np.array([node_to_label.get(n, "NA") != "NA" for n in node_names])
-    all_cosine_sim = cosine_similarity(embeddings[node_idx_with_edges], embeddings[node_idx_with_edges])
-    edges_new = np.searchsorted(node_idx_with_edges, edges)
-    #https://stackoverflow.com/a/69865919
-    i = np.ravel_multi_index(np.array(edges_new).T, all_cosine_sim.shape)
-    edge_sim = all_cosine_sim.take(i)
-    edge_sim = edge_sim.mean()
-    all_cosine_sim = np.triu(all_cosine_sim)
-    all_cosine_sim = all_cosine_sim.mean()
-    for l in label_to_node:
-        label_node_idxs = [node_names.index(n) for n in label_to_node[l] if node_names.index(n) in node_idx_with_edges]
-        label_node_idxs = np.searchsorted(node_idx_with_edges, label_node_idxs)
-        label_embs = np.array(embeddings)[label_node_idxs]
-        if label_embs.shape[0] > 1: # at least two nodes
-            avg_label_sims[l] = (np.triu(cosine_similarity(label_embs, label_embs))).mean()
-        # pick a random 
-    avg = sum(avg_label_sims.values())/len(avg_label_sims.values())      
-    #print(round(avg, 4), round(all_cosine_sim, 4))
-          #[(x, round(avg_label_sims[x], 4), len(label_to_node[x])) for x in avg_label_sims][:10]])
-    return avg, edge_sim, all_cosine_sim
-
-
-def read_marker_gene_sets(lineage_file):
-    """Open file with gene sets for a taxon
-
-    :param lineage_file: path to marker set file from CheckM (Bacteria.ms)
-    :type lineage_file: str
-    :return: Marker sets
-    :rtype: set
-    """
-    with open(lineage_file, "r") as f:
-        lines = f.readlines()
-    # consider only single taxon gene set
-    sets = lines[1].strip().split("\t")[-1]
-    sets = ast.literal_eval(sets)
-    return sets
-
-
-def read_contig_genes(contig_markers):
-    """Open file mapping contigs to genes
-
-    :param contig_markers: path to contig markers (marker stats)
-    :type contig_markers: str
-    :return: Mapping contig names to markers
-    :rtype: dict
-    """
-    contigs = {}
-    with open(contig_markers, "r") as f:
-        for line in f:
-            values = line.strip().split("\t")
-            contig_name = values[0]
-            # keep only first two elements
-            contig_name = "_".join(contig_name.split("_")[:2])
-            contigs[contig_name] = {}
-            mappings = ast.literal_eval(values[1])
-            for contig in mappings:
-                for gene in mappings[contig]:
-                    if gene not in contigs[contig_name]:
-                        contigs[contig_name][gene] = 0
-                    # else:
-                    #    breakpoint()
-                    contigs[contig_name][gene] += 1
-                    if len(mappings[contig][gene]) > 1:
-                        breakpoint()
-    return contigs
-
-
-def get_markers_to_contigs(marker_sets, contigs):
-    """Get marker to contig mapping
-
-    :param marker_sets: Marker sets from CheckM
-    :type marker_sets: set
-    :param contigs: Contig to marker mapping
-    :type contigs: dict
-    :return: Marker to contigs list mapping
-    :rtype: dict
-    """
-    marker2contigs = {}
-    for marker_set in marker_sets:
-        for gene in marker_set:
-            marker2contigs[gene] = []
-            for contig in contigs:
-                if gene in contigs[contig]:
-                    marker2contigs[gene].append(contig)
-    return marker2contigs
-
-
-def evaluate_contig_sets(marker_sets, contig_marker_counts, bin_to_contigs):
-    """Calculate completeness and contamination for each bin given a set of
-       marker gene sets and contig marker counts
-
-    :param marker_sets: reference marker sets, from Bacteria
-    :type marker_sets: list
-    :param contig_marker_counts: Counts of each gene on each contig
-    :type contig_marker_counts: dict
-    :param bin_to_contigs: Mapping bins to contigs
-    :type bin_to_contigs: dict
-    """
-    results = {}
-    for bin in bin_to_contigs:
-        bin_genes = {}
-        for contig in bin_to_contigs[bin]:
-            if contig not in contig_marker_counts:
-                print("missing", contig)
-                continue
-            for gene in contig_marker_counts[contig]:
-                if gene not in bin_genes:
-                    bin_genes[gene] = 0
-                bin_genes[gene] += contig_marker_counts[contig][gene]
-        comp = completeness(marker_sets, set(bin_genes.keys()))
-        cont = contamination(marker_sets, bin_genes)
-        results[bin] = {"comp": comp, "cont": cont, "genes": bin_genes}
-    return results
-
-def completeness(reference_markers, genes):
-    numerator = 0.0
-    for marker_set in reference_markers:
-        common = marker_set & genes
-        if len(marker_set) > 0:
-            numerator += len(common) / len(marker_set)
-    return 100 * (numerator / len(reference_markers))
-
-
-def contamination(reference_markers, genes):
-    numerator = 0.0
-    for i, marker_set in enumerate(reference_markers):
-        inner_total = 0.0
-        for gene in marker_set:
-            if gene in genes and genes[gene] > 0:
-                inner_total += genes[gene] - 1.0
-        if len(marker_set) > 0:
-            numerator += inner_total / len(marker_set)
-    return 100.0 * (numerator / len(reference_markers))
-
-
-def compute_cluster_score(reference_markers, contig_genes, node_names, node_labels):
-    labels_to_nodes = {i: node_names[node_labels == i].tolist() for i in np.unique(node_labels)}
-    results = {}
-    for label in labels_to_nodes:
-        genes = {}
-        for node_name in labels_to_nodes[label]:
-            if node_name not in contig_genes:
-                # print("missing", node_name)
-                continue
-            for gene in contig_genes[node_name]:
-                if gene not in genes:
-                    genes[gene] = 0
-                genes[gene] += contig_genes[node_name][gene]
-
-        comp = completeness(reference_markers, set(genes.keys()))
-        cont = contamination(reference_markers, genes)
-        results[label] = {"comp": comp, "cont": cont, "genes": genes}
-    return results
-
-
-def compute_hq(cluster_stats, comp_th=90, cont_th=5):
-    hq = 0
-    positive_clusters = []
-    for label in cluster_stats:
-        if cluster_stats[label]["comp"] >= comp_th and cluster_stats[label]["cont"] < cont_th:
-            hq += 1
-            positive_clusters.append(label)
-    return hq, positive_clusters
-
-def compute_unresolved(reference_markers, contig_genes, node_names, node_labels, resolved_clusters):
-    # completeness of a bin with all not HQ -> how many more bins we could get
-    unresolved_contigs = np.array([n for i,n in enumerate(node_names) if node_labels[i] not in resolved_clusters])
-    cluster_stats = compute_cluster_score(reference_markers, contig_genes,
-                                          unresolved_contigs, np.ones(len(unresolved_contigs)))
-    contamination = cluster_stats[1]["cont"]
-    potential_mags = int(contamination / 100)
-    return potential_mags, unresolved_contigs
-
-def compute_clusters_and_stats(
-    X,
-    node_names,
-    dataset,
-    k=0,
-    clustering="vamb",
-    cuda=False,
-    tsne=False,
-    tsne_path=None,
-    max_pos_pairs=None,
-    use_labels=False,
-    amber=False,
-    compute_pospairs=False,
-    unresolved=True
-):
-    reference_markers = dataset.ref_marker_sets
-    contig_genes = dataset.contig_markers
-    node_to_gt_idx_label = dataset.node_to_label
-    gt_idx_label_to_node = dataset.label_to_node
-    cluster_to_contig, contig_to_bin, labels, cluster_centroids = run_clustering(X, node_names,
-                                                                                 clustering, cuda, k=k)
-   
-    scores = {"precision": 0, "recall": 0, "f1": 0, "ari": 0, "hq": 0, "mq": 0,
-        "n_clusters": len(np.unique(labels)), "unresolved_mags": 0}
-    positive_pairs = []
-    positive_clusters = []
-    if contig_genes is not None and len(contig_genes) > 0:
-        cluster_stats = compute_cluster_score(reference_markers, contig_genes, node_names, labels)
-        hq, positive_clusters = compute_hq(cluster_stats)
-        mq, _ = compute_hq(cluster_stats, comp_th=50,cont_th=10)
-        """non_comp, _ = compute_hq(cluster_stats, comp_th=0, cont_th=10)
-        all_cont, _ = compute_hq(cluster_stats, comp_th=90, cont_th=1000)
-        """
-        scores["hq"] = hq
-        scores["mq"] = mq
-        #TODO avg comp and cont of hq bins
-        scores["hq_comp"] = np.mean([cluster_stats[c]["comp"] for c in positive_clusters])
-        scores["hq_cont"] = np.mean([cluster_stats[c]["cont"] for c in positive_clusters])
-        
-        if unresolved:
-            unresolved_mags, unresolved_contigs = compute_unresolved(reference_markers=reference_markers,
-                contig_genes=contig_genes,
-                node_names=node_names,
-                node_labels=labels,
-                resolved_clusters=positive_clusters)
-            scores["unresolved_mags"] = unresolved_mags
-            scores["unresolved_contigs"] = len(unresolved_contigs)
-            unresolved_contigs_with_scgs = np.array([n for i,n in enumerate(node_names) \
-                if labels[i] not in positive_clusters and len(dataset.contig_markers[n]) > 0])
-            scores["unresolved_contigs_with_scgs"] = len(unresolved_contigs_with_scgs)
-        # print(hq, mq, "incompete but non cont:", non_comp, "cont but complete:", all_cont)
-        positive_pairs = None
-        if compute_pospairs:
-            positive_pairs = get_positive_pairs(node_names, positive_clusters, cluster_to_contig, max_pos_pairs)
-    
-    # calculate edge similarity metrics
-    if node_to_gt_idx_label is not None and len(dataset.labels) > 1:
-        #if len(dataset.node_names) < 10_000:
-        #    sims = calculate_sim_between_same_labels_small(dataset.node_names, X,
-        #                                            list(zip(dataset.edges_src, dataset.edges_dst)),
-        #                                            dataset.label_to_node, dataset.node_to_label)
-        #elif len([n for n in dataset.node_names if dataset.node_to_label.get(n, "NA") != "NA"]) < 10_000:
-        #    sims = calculate_sim_between_same_labels_big(dataset.node_names, X,
-        #                                        list(zip(dataset.edges_src, dataset.edges_dst)),
-        #                                        dataset.label_to_node, dataset.node_to_label)
-        #else:
-        sims = 1,1,1
-        scores["avg_label_sim"], scores["avg_edge_sim"], scores["avg_total_sim"] = sims
-        scores["ratio_labelsim"] = scores["avg_label_sim"]/scores["avg_total_sim"]
-        scores["ratio_edgesim"] = scores["avg_edge_sim"]/scores["avg_total_sim"]
-        scores["ratio_labeltoedgesim"] = scores["avg_label_sim"]/scores["avg_edge_sim"]
-
-    if amber == True:
-        # TODO use p/r/ to get positive_clusters
-        import graphmb.amber_eval as amber
-        # save to file
-        output_bins_filename = dataset.cache_dir + f"/{dataset.name}_temp_contig2bin.tsv"
-        amber.write_amber_bins(contig_to_bin, output_bins_filename)
-        amber_metrics, bin_counts = amber.amber_eval(os.path.join(dataset.data_dir, dataset.labelsfile), output_bins_filename, ["graphmb"])
-        scores["precision_avg_bp"] = amber_metrics["precision_avg_bp"]
-        scores["recall_avg_bp"] = amber_metrics["recall_avg_bp"]
-        scores["f1_avg_bp"] = amber_metrics["f1_avg_bp"]
-        scores["amber_hq"] = bin_counts["> 90% completeness"][1]
-        scores["amber_mq"] = bin_counts["> 50% completeness"][0]
-    else:
-        # calculate edge metrics
-        p, r, f1, ari = calculate_overall_prf(
-            cluster_to_contig, contig_to_bin, node_to_gt_idx_label, gt_idx_label_to_node
-        )
-        scores["precision"] = p
-        scores["recall"] = r
-        scores["f1"] = f1
-        scores["ari"] = ari
-    #plot tSNE
-    if tsne:
-        cluster_to_contig = {cluster: [dataset.node_names[i] for i,x in enumerate(labels) if x == cluster] for cluster in set(labels)}
-        node_embeddings_2dim, centroids_2dim = run_tsne(X, dataset, cluster_to_contig, positive_clusters, centroids=cluster_centroids)
-        plot_embs(
-            dataset.node_names,
-            node_embeddings_2dim,
-            #dataset.label_to_node.copy(),
-            cluster_to_contig,
-            centroids=centroids_2dim,
-            hq_centroids=positive_clusters,
-            node_sizes=None,
-            outputname=tsne_path,
-        )
-    #print("calc metrics time", datetime.datetime.now() - processing_time)
-    return (
-        labels,
-        scores,
-        positive_pairs,
-        positive_clusters,
-    )
-
-def get_positive_pairs(node_names, positive_clusters, cluster_to_contig, max_pos_pairs=None):
-    positive_pairs = []
-    node_names_to_idx = {node_name: i for i, node_name in enumerate(node_names)}
-    for label in positive_clusters:
-        added_pairs = []
-        for (p1, p2) in itertools.combinations(cluster_to_contig[label], 2):
-            added_pairs.append((node_names_to_idx[p1], node_names_to_idx[p2]))    
-        if max_pos_pairs is not None and len(added_pairs) > max_pos_pairs:
-            added_pairs = random.sample(added_pairs, max_pos_pairs)
-        positive_pairs.extend(added_pairs)
-    # print("found {} positive pairs".format(len(positive_pairs)))
-    positive_pairs = np.unique(np.array(list(positive_pairs)), axis=0)
-    return positive_pairs
-
-def eval_epoch(node_new_features, cluster_mask, weights, args, dataset, epoch, scores, best_metric, 
-               best_embs, best_epoch, best_model, target_metric="hq"):
-    # used only by vgae model
-    #log_to_tensorboard(summary_writer, {"Embs average": np.mean(node_new_features), 'Embs std': np.std(node_new_features) }, step)
-    cluster_labels, stats, _, hq_bins = compute_clusters_and_stats(
-        node_new_features[cluster_mask], np.array(dataset.node_names)[cluster_mask],
-        dataset, clustering=args.clusteringalgo, k=args.kclusters, tsne=args.tsne,
-        amber=(args.labels is not None and "amber" in args.labels), cuda=args.cuda,
-        compute_pospairs=False, unresolved=True
-    )
-    
-    stats["epoch"] = epoch
-    scores.append(stats)
-    #logger.info(str(stats))
-
-    #log_to_tensorboard(summary_writer, {"hq": stats["hq"], "mq": stats["mq"]}, step)
-    #all_cluster_labels.append(cluster_labels)
-    #if dataset.contig_markers is not None and len(dataset.contig_markers) > 0 and stats["hq"] > best_metric:
-    #    best_metric, best_embs, best_epoch, best_model = stats["hq"], node_new_features, epoch, weights
-        #best_model = th.gnn_model
-        #save_model(args, e, th, th_vae)
-    if stats[target_metric] > best_metric:
-        best_metric, best_embs, best_epoch, best_model = stats[target_metric], node_new_features, epoch, weights
-
-    return best_metric, best_embs, best_epoch, scores, best_model, cluster_labels
-
-
-def eval_epoch_cluster(logger, summary_writer, node_new_features, cluster_mask, best_hq,
-               step, args, dataset, epoch, tsne, cluster=True):
-    
-    if cluster:
-        #log_to_tensorboard(summary_writer, {"Embs average": np.mean(node_new_features), 'Embs std': np.std(node_new_features) }, step)
-        tsne_path = os.path.join(args.outdir, f"{args.outname}_tsne_clusters_epoch_{epoch}.png")
-        cluster_labels, stats, positive_pairs, hq_bins = compute_clusters_and_stats(
-            node_new_features[cluster_mask], np.array(dataset.node_names)[cluster_mask],
-            dataset, clustering=args.clusteringalgo, k=args.kclusters, tsne=tsne, tsne_path=tsne_path, max_pos_pairs=None,
-            amber=(args.labels is not None and "amber" in args.labels), cuda=args.cuda,
-        )
-    else:
-        breakpoint()
-        cluster_labels = np.argmax(node_new_features[cluster_mask], axis=1)
-        hq, positive_clusters = compute_hq(reference_markers=dataset.ref_marker_sets,
-                                           contig_genes=dataset.contig_markers,
-                                           node_names=np.array(dataset.node_names)[cluster_mask],
-                                           node_labels=cluster_labels)
-        mq, _ = compute_hq(reference_markers=dataset.ref_marker_sets,
-                                           contig_genes=dataset.contig_markers,
-                                           node_names=np.array(dataset.node_names)[cluster_mask],
-                                           node_labels=cluster_labels, comp_th=50, cont_th=10,)
-        stats = {"hq": hq, "unresolved": len(positive_clusters), "mq": mq}
-        
-        cluster_to_contig = {i: [] for i in range(max(cluster_labels) + 1)}
-        for i in range(len(dataset.node_names)):
-            cluster_to_contig[cluster_labels[i]].append(dataset.node_names[i])
-        positive_pairs = None
-   
-    stats["epoch"] = epoch
-    #logger.info(str(stats))
-
-    #log_to_tensorboard(summary_writer, {"hq_bins": stats["hq"], "mq_bins": stats["mq"]}, step)
-    #all_cluster_labels.append(cluster_labels)
-    new_best = False
-    if dataset.contig_markers is not None and stats["hq"] > best_hq:
-        new_best = True
-    elif dataset.contig_markers is None and stats["f1"] > best_hq:
-        new_best = True
-    # print('--- END ---')
-    #if args.quiet:
-    #    logger.info(f"--- EPOCH {e:d} ---")
-    #    logger.info(f"[{gname} {nlayers_gnn}l] L={gnn_loss:.3f} D={diff_loss:.3f} HQ={stats['hq']} BestHQ={best_hq} Best Epoch={best_epoch} Max GPU MB={gpu_mem_alloc:.1f}")
-    #    logger.info(str(stats))
-
-    #cluster_labels, stats, _, hq_bins = compute_clusters_and_stats(
-    #    node_new_features, np.array(dataset.node_names),
-    #    dataset, clustering=args.clusteringalgo, k=args.kclusters, tsne=args.tsne, #cuda=args.cuda,
-    #)
-    #log_to_tensorboard(summary_writer, {"hq_bins_all": stats["hq"], "mq_bins_all": stats["mq"]}, step)
-
-    return stats, new_best, cluster_labels, positive_pairs
-
-def main():
-    sets = read_marker_gene_sets(sys.argv[1])
-    markers = read_contig_genes(sys.argv[2])
-    #print("Single contig bin eval")
-    if len(sys.argv) < 4:
-        print("Single contig bin eval")
-        single_contig_bins = {c: [c] for c in markers}
-        results = evaluate_contig_sets(sets, markers, single_contig_bins)
-        total_hq = 0
-        for bin in results:
-            if results[bin]["comp"] > 90 and results[bin]["cont"] < 5:
-                print(bin, results[bin]["comp"], results[bin]["cont"])
-                total_hq += 1
-        print("Total HQ", total_hq)
-        # for bin in markers:
-        #    print(bin)
-        #    print(completeness(sets, set(markers[bin].keys())))
-        #    print(contamination(sets, markers[bin]))
-    else:
-        cluster_to_contigs = {}
-        clusters_file = sys.argv[3]
-        with open(clusters_file, "r") as f:
-            for line in f:
-                if line.startswith("@") or line.startswith("#"):
-                    continue
-                values = line.strip().split()
-                contig, binname = values[0], values[1]
-                if binname not in cluster_to_contigs:
-                    cluster_to_contigs[binname] = []
-                cluster_to_contigs[binname].append(contig)
-        results = evaluate_contig_sets(sets, markers, cluster_to_contigs)
-        # print(results)
-
-        total_hq = 0
-        for bin in results:
-            if results[bin]["comp"] > 90 and results[bin]["cont"] < 5:
-                print(bin, results[bin]["comp"], results[bin]["cont"])
-                total_hq += 1
-        print("Total HQ", total_hq)
-        if len(sys.argv) > 4:
-            import graphmb.amber_eval as amber
-            scores = {}
-            amber_metrics, bin_counts = amber.amber_eval(sys.argv[4], clusters_file, ["graphmb"])
-            scores["precision_avg_bp"] = amber_metrics["precision_avg_bp"]
-            scores["recall_avg_bp"] = amber_metrics["recall_avg_bp"]
-            scores["f1_avg_bp"] = amber_metrics["f1_avg_bp"]
-            print(scores)
-        # count how many contigs per marker gene
-    scg_counts = {}
-    for marker_set in sets:
-        for gene in marker_set:
-            scg_counts[gene] = 0
-            for contig in markers:
-                if gene in markers[contig]:
-                    scg_counts[gene] += markers[contig][gene]
-
-    #print(scg_counts)
-    quartiles = np.percentile(list(scg_counts.values()), [25, 50, 75])
-    print("candidate k0s", sorted(set([k for k in scg_counts.values() if k >= quartiles[2]])))
-
-    # TODO convert SCGs to features
-
-
-if __name__ == "__main__":
-    main()
+import sys
+import ast
+import os
+import numpy as np
+import scipy
+import itertools
+import random
+from sklearn.metrics.pairwise import cosine_similarity
+
+from graphmb.visualize import run_tsne, plot_embs
+from graphmb.utils import run_clustering
+# code to run evaluation based on lineage.ms file (Bacteria) and marker_gene_stats.txt file
+
+# Get precicion
+def getPrecision(mat, k, s, total):
+    sum_k = 0
+    for i in range(k):
+        max_s = 0
+        for j in range(s):
+            if mat[i][j] > max_s:
+                max_s = mat[i][j]
+        sum_k += max_s  
+    return sum_k / total
+
+
+# Get recall
+def getRecall(mat, k, s, total, unclassified):
+    sum_s = 0
+    for i in range(s):
+        max_k = 0
+        for j in range(k):
+            if mat[j][i] > max_k:
+                max_k = mat[j][i]
+        sum_s += max_k
+    return sum_s / (total + unclassified)
+
+
+def getAveragePrecision(cluster_to_labels, cluster_sizes):
+    avg_precision = []
+    for c in cluster_to_labels:
+        #TP = cluster_to_labels[c][1]; TP+FP + cluster_sizes[c]
+        cluster_p = cluster_to_labels[c][1] / cluster_sizes[c]
+        avg_precision.append(cluster_p)
+    return round(sum(avg_precision) / len(avg_precision), 4)
+
+def getAverageRecall(label_to_cluster, cluster_to_contig, contig_sizes, label_to_node):
+    avg_recall = []
+    for label in label_to_cluster:
+        if label_to_cluster[label][0] == "NA":
+            avg_recall.append(0)
+        else:
+            cluster_r = label_to_cluster[label][1] / sum([contig_sizes.get(n, 1) for n in cluster_to_contig[label_to_cluster[label][0]]])
+            avg_recall.append(cluster_r)
+    return round(sum(avg_recall) / len(avg_recall), 4)
+
+
+# Get ARI
+def getARI(mat, k, s, N):
+    t1 = 0
+    for i in range(k):
+        sum_k = 0
+        for j in range(s):
+            sum_k += mat[i][j]
+        t1 += scipy.special.binom(sum_k, 2)
+    t2 = 0
+    for i in range(s):
+        sum_s = 0
+        for j in range(k):
+            sum_s += mat[j][i]
+        t2 += scipy.special.binom(sum_s, 2)
+    t3 = t1 * t2 / scipy.special.binom(N, 2)
+    t = 0
+    for i in range(k):
+        for j in range(s):
+            t += scipy.special.binom(mat[i][j], 2)
+    ari = (t - t3) / ((t1 + t2) / 2 - t3)
+    return ari
+
+
+# Get F1-score
+def getF1(prec, recall):
+    if prec == 0.0 or recall == 0.0:
+        return 0.0
+    else:
+        return 2 * prec * recall / (prec + recall)
+
+
+def calculate_overall_prf(cluster_to_contig, contig_to_cluster, node_to_label, label_to_node):
+    # calculate how many contigs are in the majority class of each cluster
+    total_binned = 0
+    # convert everything to ids
+    labels = list(label_to_node.keys())
+    clusters = list(cluster_to_contig.keys())
+    n_pred_labels = len(clusters)
+    n_true_labels = len(labels)
+    ground_truth_count = len(node_to_label)
+    # empty matrix
+    bins_species = [[0 for x in range(n_true_labels)] for y in range(n_pred_labels)]
+    # update with cluster memberships
+    for i in contig_to_cluster:
+        if i in node_to_label:
+            # breakpoint()
+            total_binned += 1
+            bins_species[clusters.index(contig_to_cluster[i])][labels.index(node_to_label[i])] += 1
+    my_precision = getPrecision(bins_species, n_pred_labels, n_true_labels, total_binned)
+    my_recall = getRecall(
+        bins_species, n_pred_labels, n_true_labels, total_binned, (ground_truth_count - total_binned)
+    )
+    #my_ari = getARI(bins_species, n_pred_labels, n_true_labels, total_binned)
+    my_f1 = getF1(my_precision, my_recall)
+    return my_precision, my_recall, my_f1, 0
+
+def calculate_sim_between_same_labels_small(node_names, embeddings, edges, label_to_node, node_to_label):
+    # divide sim between node of same label by avg sim between all nodes
+    avg_label_sims = {}
+    # use only embeddings of nodes with labels
+    edges = np.array(edges)
+    # calculate sim between all embs
+    all_cosine_sim = cosine_similarity(embeddings, embeddings)
+    #https://stackoverflow.com/a/69865919
+    i = np.ravel_multi_index(np.array(edges).T, all_cosine_sim.shape)
+    edge_sim = all_cosine_sim.take(i) # get sim between embs of edges
+    edge_sim = edge_sim.sum()
+    #all_cosine_sim = np.triu(all_cosine_sim)
+    # all sim should not include sims of edges
+    all_cosine_sim = all_cosine_sim.sum() - edge_sim
+    all_cosine_sim = all_cosine_sim / ((embeddings.shape[0]**2)-len(edges))
+    edge_sim /= len(edges)
+    for l in label_to_node:
+        label_node_idxs = [node_names.index(n) for n in label_to_node[l]]
+        label_embs = np.array(embeddings)[label_node_idxs]
+        if label_embs.shape[0] > 1: # at least two nodes
+            avg_label_sims[l] = ((cosine_similarity(label_embs, label_embs))).mean()
+        # pick a random 
+    avg = sum(avg_label_sims.values())/len(avg_label_sims.values())      
+    #print(round(avg, 4), round(all_cosine_sim, 4))
+          #[(x, round(avg_label_sims[x], 4), len(label_to_node[x])) for x in avg_label_sims][:10]])
+    return avg, edge_sim, all_cosine_sim
+
+
+def calculate_sim_between_same_labels_big(node_names, embeddings, edges, label_to_node, node_to_label):
+    # divide sim between node of same label by avg sim between all nodes
+    avg_label_sims = {}
+    # use only embeddings of nodes in edges to make it more efficient
+    edges = np.array(edges)
+    node_idx_with_edges = np.unique(edges)
+    #label_mask = np.array([node_to_label.get(n, "NA") != "NA" for n in node_names])
+    all_cosine_sim = cosine_similarity(embeddings[node_idx_with_edges], embeddings[node_idx_with_edges])
+    edges_new = np.searchsorted(node_idx_with_edges, edges)
+    #https://stackoverflow.com/a/69865919
+    i = np.ravel_multi_index(np.array(edges_new).T, all_cosine_sim.shape)
+    edge_sim = all_cosine_sim.take(i)
+    edge_sim = edge_sim.mean()
+    all_cosine_sim = np.triu(all_cosine_sim)
+    all_cosine_sim = all_cosine_sim.mean()
+    for l in label_to_node:
+        label_node_idxs = [node_names.index(n) for n in label_to_node[l] if node_names.index(n) in node_idx_with_edges]
+        label_node_idxs = np.searchsorted(node_idx_with_edges, label_node_idxs)
+        label_embs = np.array(embeddings)[label_node_idxs]
+        if label_embs.shape[0] > 1: # at least two nodes
+            avg_label_sims[l] = (np.triu(cosine_similarity(label_embs, label_embs))).mean()
+        # pick a random 
+    avg = sum(avg_label_sims.values())/len(avg_label_sims.values())      
+    #print(round(avg, 4), round(all_cosine_sim, 4))
+          #[(x, round(avg_label_sims[x], 4), len(label_to_node[x])) for x in avg_label_sims][:10]])
+    return avg, edge_sim, all_cosine_sim
+
+
+def read_marker_gene_sets(lineage_file):
+    """Open file with gene sets for a taxon
+
+    :param lineage_file: path to marker set file from CheckM (Bacteria.ms)
+    :type lineage_file: str
+    :return: Marker sets
+    :rtype: set
+    """
+    with open(lineage_file, "r") as f:
+        lines = f.readlines()
+    # consider only single taxon gene set
+    sets = lines[1].strip().split("\t")[-1]
+    sets = ast.literal_eval(sets)
+    return sets
+
+
+def read_contig_genes(contig_markers):
+    """Open file mapping contigs to genes
+
+    :param contig_markers: path to contig markers (marker stats)
+    :type contig_markers: str
+    :return: Mapping contig names to markers
+    :rtype: dict
+    """
+    contigs = {}
+    with open(contig_markers, "r") as f:
+        for line in f:
+            values = line.strip().split("\t")
+            contig_name = values[0]
+            # keep only first two elements
+            contig_name = "_".join(contig_name.split("_")[:2])
+            contigs[contig_name] = {}
+            mappings = ast.literal_eval(values[1])
+            for contig in mappings:
+                for gene in mappings[contig]:
+                    if gene not in contigs[contig_name]:
+                        contigs[contig_name][gene] = 0
+                    # else:
+                    #    breakpoint()
+                    contigs[contig_name][gene] += 1
+                    if len(mappings[contig][gene]) > 1:
+                        breakpoint()
+    return contigs
+
+
+def get_markers_to_contigs(marker_sets, contigs):
+    """Get marker to contig mapping
+
+    :param marker_sets: Marker sets from CheckM
+    :type marker_sets: set
+    :param contigs: Contig to marker mapping
+    :type contigs: dict
+    :return: Marker to contigs list mapping
+    :rtype: dict
+    """
+    marker2contigs = {}
+    for marker_set in marker_sets:
+        for gene in marker_set:
+            marker2contigs[gene] = []
+            for contig in contigs:
+                if gene in contigs[contig]:
+                    marker2contigs[gene].append(contig)
+    return marker2contigs
+
+
+def evaluate_contig_sets(marker_sets, contig_marker_counts, bin_to_contigs):
+    """Calculate completeness and contamination for each bin given a set of
+       marker gene sets and contig marker counts
+
+    :param marker_sets: reference marker sets, from Bacteria
+    :type marker_sets: list
+    :param contig_marker_counts: Counts of each gene on each contig
+    :type contig_marker_counts: dict
+    :param bin_to_contigs: Mapping bins to contigs
+    :type bin_to_contigs: dict
+    """
+    results = {}
+    for bin in bin_to_contigs:
+        bin_genes = {}
+        for contig in bin_to_contigs[bin]:
+            if contig not in contig_marker_counts:
+                print("missing", contig)
+                continue
+            for gene in contig_marker_counts[contig]:
+                if gene not in bin_genes:
+                    bin_genes[gene] = 0
+                bin_genes[gene] += contig_marker_counts[contig][gene]
+        comp = completeness(marker_sets, set(bin_genes.keys()))
+        cont = contamination(marker_sets, bin_genes)
+        results[bin] = {"comp": comp, "cont": cont, "genes": bin_genes}
+    return results
+
+def completeness(reference_markers, genes):
+    numerator = 0.0
+    for marker_set in reference_markers:
+        common = marker_set & genes
+        if len(marker_set) > 0:
+            numerator += len(common) / len(marker_set)
+    return 100 * (numerator / len(reference_markers))
+
+
+def contamination(reference_markers, genes):
+    numerator = 0.0
+    for i, marker_set in enumerate(reference_markers):
+        inner_total = 0.0
+        for gene in marker_set:
+            if gene in genes and genes[gene] > 0:
+                inner_total += genes[gene] - 1.0
+        if len(marker_set) > 0:
+            numerator += inner_total / len(marker_set)
+    return 100.0 * (numerator / len(reference_markers))
+
+
+def compute_cluster_score(reference_markers, contig_genes, node_names, node_labels):
+    labels_to_nodes = {i: node_names[node_labels == i].tolist() for i in np.unique(node_labels)}
+    results = {}
+    for label in labels_to_nodes:
+        genes = {}
+        for node_name in labels_to_nodes[label]:
+            if node_name not in contig_genes:
+                # print("missing", node_name)
+                continue
+            for gene in contig_genes[node_name]:
+                if gene not in genes:
+                    genes[gene] = 0
+                genes[gene] += contig_genes[node_name][gene]
+
+        comp = completeness(reference_markers, set(genes.keys()))
+        cont = contamination(reference_markers, genes)
+        results[label] = {"comp": comp, "cont": cont, "genes": genes}
+    return results
+
+
+def compute_hq(cluster_stats, comp_th=90, cont_th=5):
+    hq = 0
+    positive_clusters = []
+    for label in cluster_stats:
+        if cluster_stats[label]["comp"] >= comp_th and cluster_stats[label]["cont"] < cont_th:
+            hq += 1
+            positive_clusters.append(label)
+    return hq, positive_clusters
+
+def compute_unresolved(reference_markers, contig_genes, node_names, node_labels, resolved_clusters):
+    # completeness of a bin with all not HQ -> how many more bins we could get
+    unresolved_contigs = np.array([n for i,n in enumerate(node_names) if node_labels[i] not in resolved_clusters])
+    cluster_stats = compute_cluster_score(reference_markers, contig_genes,
+                                          unresolved_contigs, np.ones(len(unresolved_contigs)))
+    contamination = cluster_stats[1]["cont"]
+    potential_mags = int(contamination / 100)
+    return potential_mags, unresolved_contigs
+
+def compute_clusters_and_stats(
+    X,
+    node_names,
+    dataset,
+    k=0,
+    clustering="vamb",
+    cuda=False,
+    tsne=False,
+    tsne_path=None,
+    max_pos_pairs=None,
+    use_labels=False,
+    amber=False,
+    compute_pospairs=False,
+    unresolved=True
+):
+    reference_markers = dataset.ref_marker_sets
+    contig_genes = dataset.contig_markers
+    node_to_gt_idx_label = dataset.node_to_label
+    gt_idx_label_to_node = dataset.label_to_node
+    cluster_to_contig, contig_to_bin, labels, cluster_centroids = run_clustering(X, node_names,
+                                                                                 clustering, cuda, k=k)
+   
+    scores = {"precision": 0, "recall": 0, "f1": 0, "ari": 0, "hq": 0, "mq": 0,
+        "n_clusters": len(np.unique(labels)), "unresolved_mags": 0}
+    positive_pairs = []
+    positive_clusters = []
+    if contig_genes is not None and len(contig_genes) > 0:
+        cluster_stats = compute_cluster_score(reference_markers, contig_genes, node_names, labels)
+        hq, positive_clusters = compute_hq(cluster_stats)
+        mq, _ = compute_hq(cluster_stats, comp_th=50,cont_th=10)
+        """non_comp, _ = compute_hq(cluster_stats, comp_th=0, cont_th=10)
+        all_cont, _ = compute_hq(cluster_stats, comp_th=90, cont_th=1000)
+        """
+        scores["hq"] = hq
+        scores["mq"] = mq
+        #TODO avg comp and cont of hq bins
+        scores["hq_comp"] = np.mean([cluster_stats[c]["comp"] for c in positive_clusters])
+        scores["hq_cont"] = np.mean([cluster_stats[c]["cont"] for c in positive_clusters])
+        
+        if unresolved:
+            unresolved_mags, unresolved_contigs = compute_unresolved(reference_markers=reference_markers,
+                contig_genes=contig_genes,
+                node_names=node_names,
+                node_labels=labels,
+                resolved_clusters=positive_clusters)
+            scores["unresolved_mags"] = unresolved_mags
+            scores["unresolved_contigs"] = len(unresolved_contigs)
+            unresolved_contigs_with_scgs = np.array([n for i,n in enumerate(node_names) \
+                if labels[i] not in positive_clusters and len(dataset.contig_markers[n]) > 0])
+            scores["unresolved_contigs_with_scgs"] = len(unresolved_contigs_with_scgs)
+        # print(hq, mq, "incompete but non cont:", non_comp, "cont but complete:", all_cont)
+        positive_pairs = None
+        if compute_pospairs:
+            positive_pairs = get_positive_pairs(node_names, positive_clusters, cluster_to_contig, max_pos_pairs)
+    
+    # calculate edge similarity metrics
+    if node_to_gt_idx_label is not None and len(dataset.labels) > 1:
+        #if len(dataset.node_names) < 10_000:
+        #    sims = calculate_sim_between_same_labels_small(dataset.node_names, X,
+        #                                            list(zip(dataset.edges_src, dataset.edges_dst)),
+        #                                            dataset.label_to_node, dataset.node_to_label)
+        #elif len([n for n in dataset.node_names if dataset.node_to_label.get(n, "NA") != "NA"]) < 10_000:
+        #    sims = calculate_sim_between_same_labels_big(dataset.node_names, X,
+        #                                        list(zip(dataset.edges_src, dataset.edges_dst)),
+        #                                        dataset.label_to_node, dataset.node_to_label)
+        #else:
+        sims = 1,1,1
+        scores["avg_label_sim"], scores["avg_edge_sim"], scores["avg_total_sim"] = sims
+        scores["ratio_labelsim"] = scores["avg_label_sim"]/scores["avg_total_sim"]
+        scores["ratio_edgesim"] = scores["avg_edge_sim"]/scores["avg_total_sim"]
+        scores["ratio_labeltoedgesim"] = scores["avg_label_sim"]/scores["avg_edge_sim"]
+
+    if amber == True:
+        # TODO use p/r/ to get positive_clusters
+        import graphmb.amber_eval as amber
+        # save to file
+        output_bins_filename = dataset.cache_dir + f"/{dataset.name}_temp_contig2bin.tsv"
+        amber.write_amber_bins(contig_to_bin, output_bins_filename)
+        amber_metrics, bin_counts = amber.amber_eval(os.path.join(dataset.data_dir, dataset.labelsfile), output_bins_filename, ["graphmb"])
+        scores["precision_avg_bp"] = amber_metrics["precision_avg_bp"]
+        scores["recall_avg_bp"] = amber_metrics["recall_avg_bp"]
+        scores["f1_avg_bp"] = amber_metrics["f1_avg_bp"]
+        scores["amber_hq"] = bin_counts["> 90% completeness"][1]
+        scores["amber_mq"] = bin_counts["> 50% completeness"][0]
+    else:
+        # calculate edge metrics
+        p, r, f1, ari = calculate_overall_prf(
+            cluster_to_contig, contig_to_bin, node_to_gt_idx_label, gt_idx_label_to_node
+        )
+        scores["precision"] = p
+        scores["recall"] = r
+        scores["f1"] = f1
+        scores["ari"] = ari
+    #plot tSNE
+    if tsne:
+        cluster_to_contig = {cluster: [dataset.node_names[i] for i,x in enumerate(labels) if x == cluster] for cluster in set(labels)}
+        node_embeddings_2dim, centroids_2dim = run_tsne(X, dataset, cluster_to_contig, positive_clusters, centroids=cluster_centroids)
+        plot_embs(
+            dataset.node_names,
+            node_embeddings_2dim,
+            #dataset.label_to_node.copy(),
+            cluster_to_contig,
+            centroids=centroids_2dim,
+            hq_centroids=positive_clusters,
+            node_sizes=None,
+            outputname=tsne_path,
+        )
+    #print("calc metrics time", datetime.datetime.now() - processing_time)
+    return (
+        labels,
+        scores,
+        positive_pairs,
+        positive_clusters,
+    )
+
+def get_positive_pairs(node_names, positive_clusters, cluster_to_contig, max_pos_pairs=None):
+    positive_pairs = []
+    node_names_to_idx = {node_name: i for i, node_name in enumerate(node_names)}
+    for label in positive_clusters:
+        added_pairs = []
+        for (p1, p2) in itertools.combinations(cluster_to_contig[label], 2):
+            added_pairs.append((node_names_to_idx[p1], node_names_to_idx[p2]))    
+        if max_pos_pairs is not None and len(added_pairs) > max_pos_pairs:
+            added_pairs = random.sample(added_pairs, max_pos_pairs)
+        positive_pairs.extend(added_pairs)
+    # print("found {} positive pairs".format(len(positive_pairs)))
+    positive_pairs = np.unique(np.array(list(positive_pairs)), axis=0)
+    return positive_pairs
+
+def eval_epoch(node_new_features, cluster_mask, weights, args, dataset, epoch, scores, best_metric, 
+               best_embs, best_epoch, best_model, target_metric="hq"):
+    # used only by vgae model
+    #log_to_tensorboard(summary_writer, {"Embs average": np.mean(node_new_features), 'Embs std': np.std(node_new_features) }, step)
+    cluster_labels, stats, _, hq_bins = compute_clusters_and_stats(
+        node_new_features[cluster_mask], np.array(dataset.node_names)[cluster_mask],
+        dataset, clustering=args.clusteringalgo, k=args.kclusters, tsne=args.tsne,
+        amber=(args.labels is not None and "amber" in args.labels), cuda=args.cuda,
+        compute_pospairs=False, unresolved=True
+    )
+    
+    stats["epoch"] = epoch
+    scores.append(stats)
+    #logger.info(str(stats))
+
+    #log_to_tensorboard(summary_writer, {"hq": stats["hq"], "mq": stats["mq"]}, step)
+    #all_cluster_labels.append(cluster_labels)
+    #if dataset.contig_markers is not None and len(dataset.contig_markers) > 0 and stats["hq"] > best_metric:
+    #    best_metric, best_embs, best_epoch, best_model = stats["hq"], node_new_features, epoch, weights
+        #best_model = th.gnn_model
+        #save_model(args, e, th, th_vae)
+    if stats[target_metric] > best_metric:
+        best_metric, best_embs, best_epoch, best_model = stats[target_metric], node_new_features, epoch, weights
+
+    return best_metric, best_embs, best_epoch, scores, best_model, cluster_labels
+
+
+def eval_epoch_cluster(logger, summary_writer, node_new_features, cluster_mask, best_hq,
+               step, args, dataset, epoch, tsne, cluster=True):
+    
+    if cluster:
+        #log_to_tensorboard(summary_writer, {"Embs average": np.mean(node_new_features), 'Embs std': np.std(node_new_features) }, step)
+        tsne_path = os.path.join(args.outdir, f"{args.outname}_tsne_clusters_epoch_{epoch}.png")
+        cluster_labels, stats, positive_pairs, hq_bins = compute_clusters_and_stats(
+            node_new_features[cluster_mask], np.array(dataset.node_names)[cluster_mask],
+            dataset, clustering=args.clusteringalgo, k=args.kclusters, tsne=tsne, tsne_path=tsne_path, max_pos_pairs=None,
+            amber=(args.labels is not None and "amber" in args.labels), cuda=args.cuda,
+        )
+    else:
+        breakpoint()
+        cluster_labels = np.argmax(node_new_features[cluster_mask], axis=1)
+        hq, positive_clusters = compute_hq(reference_markers=dataset.ref_marker_sets,
+                                           contig_genes=dataset.contig_markers,
+                                           node_names=np.array(dataset.node_names)[cluster_mask],
+                                           node_labels=cluster_labels)
+        mq, _ = compute_hq(reference_markers=dataset.ref_marker_sets,
+                                           contig_genes=dataset.contig_markers,
+                                           node_names=np.array(dataset.node_names)[cluster_mask],
+                                           node_labels=cluster_labels, comp_th=50, cont_th=10,)
+        stats = {"hq": hq, "unresolved": len(positive_clusters), "mq": mq}
+        
+        cluster_to_contig = {i: [] for i in range(max(cluster_labels) + 1)}
+        for i in range(len(dataset.node_names)):
+            cluster_to_contig[cluster_labels[i]].append(dataset.node_names[i])
+        positive_pairs = None
+   
+    stats["epoch"] = epoch
+    #logger.info(str(stats))
+
+    #log_to_tensorboard(summary_writer, {"hq_bins": stats["hq"], "mq_bins": stats["mq"]}, step)
+    #all_cluster_labels.append(cluster_labels)
+    new_best = False
+    if dataset.contig_markers is not None and stats["hq"] > best_hq:
+        new_best = True
+    elif dataset.contig_markers is None and stats["f1"] > best_hq:
+        new_best = True
+    # print('--- END ---')
+    #if args.quiet:
+    #    logger.info(f"--- EPOCH {e:d} ---")
+    #    logger.info(f"[{gname} {nlayers_gnn}l] L={gnn_loss:.3f} D={diff_loss:.3f} HQ={stats['hq']} BestHQ={best_hq} Best Epoch={best_epoch} Max GPU MB={gpu_mem_alloc:.1f}")
+    #    logger.info(str(stats))
+
+    #cluster_labels, stats, _, hq_bins = compute_clusters_and_stats(
+    #    node_new_features, np.array(dataset.node_names),
+    #    dataset, clustering=args.clusteringalgo, k=args.kclusters, tsne=args.tsne, #cuda=args.cuda,
+    #)
+    #log_to_tensorboard(summary_writer, {"hq_bins_all": stats["hq"], "mq_bins_all": stats["mq"]}, step)
+
+    return stats, new_best, cluster_labels, positive_pairs
+
+def main():
+    sets = read_marker_gene_sets(sys.argv[1])
+    markers = read_contig_genes(sys.argv[2])
+    #print("Single contig bin eval")
+    if len(sys.argv) < 4:
+        print("Single contig bin eval")
+        single_contig_bins = {c: [c] for c in markers}
+        results = evaluate_contig_sets(sets, markers, single_contig_bins)
+        total_hq = 0
+        for bin in results:
+            if results[bin]["comp"] > 90 and results[bin]["cont"] < 5:
+                print(bin, results[bin]["comp"], results[bin]["cont"])
+                total_hq += 1
+        print("Total HQ", total_hq)
+        # for bin in markers:
+        #    print(bin)
+        #    print(completeness(sets, set(markers[bin].keys())))
+        #    print(contamination(sets, markers[bin]))
+    else:
+        cluster_to_contigs = {}
+        clusters_file = sys.argv[3]
+        with open(clusters_file, "r") as f:
+            for line in f:
+                if line.startswith("@") or line.startswith("#"):
+                    continue
+                values = line.strip().split()
+                contig, binname = values[0], values[1]
+                if binname not in cluster_to_contigs:
+                    cluster_to_contigs[binname] = []
+                cluster_to_contigs[binname].append(contig)
+        results = evaluate_contig_sets(sets, markers, cluster_to_contigs)
+        # print(results)
+
+        total_hq = 0
+        for bin in results:
+            if results[bin]["comp"] > 90 and results[bin]["cont"] < 5:
+                print(bin, results[bin]["comp"], results[bin]["cont"])
+                total_hq += 1
+        print("Total HQ", total_hq)
+        if len(sys.argv) > 4:
+            import graphmb.amber_eval as amber
+            scores = {}
+            amber_metrics, bin_counts = amber.amber_eval(sys.argv[4], clusters_file, ["graphmb"])
+            scores["precision_avg_bp"] = amber_metrics["precision_avg_bp"]
+            scores["recall_avg_bp"] = amber_metrics["recall_avg_bp"]
+            scores["f1_avg_bp"] = amber_metrics["f1_avg_bp"]
+            print(scores)
+        # count how many contigs per marker gene
+    scg_counts = {}
+    for marker_set in sets:
+        for gene in marker_set:
+            scg_counts[gene] = 0
+            for contig in markers:
+                if gene in markers[contig]:
+                    scg_counts[gene] += markers[contig][gene]
+
+    #print(scg_counts)
+    quartiles = np.percentile(list(scg_counts.values()), [25, 50, 75])
+    print("candidate k0s", sorted(set([k for k in scg_counts.values() if k >= quartiles[2]])))
+
+    # TODO convert SCGs to features
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `graphmb-0.2.4/src/graphmb/gnn_models.py` & `graphmb-0.2.5/src/graphmb/gnn_models.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,433 +1,433 @@
-import tensorflow as tf
-
-from tensorflow.keras.optimizers import Adam, SGD
-from tensorflow.keras.models import Model
-from tensorflow.keras.layers import Input, Dense, Activation, Softmax, Embedding, LayerNormalization
-#from tensorflow.keras import Sequential
-from tensorflow.keras.layers import BatchNormalization, Lambda, LeakyReLU, Flatten
-from tensorflow.keras.layers import Dropout, Add, Concatenate
-from tensorflow.keras.losses import SparseCategoricalCrossentropy
-import numpy as np
-from tensorflow.keras.regularizers import l2    
-
-from graphmb.layers import BiasLayer, LAF, GraphAttention
-
-class VGAE(Model):
-    def __init__(self, emb_dim, embeddings=None, 
-                 hidden_dim1=None, hidden_dim2=None,
-                 dropout=None, l2_reg=None,
-                 freeze_embeddings=False, lr=1e-02):
-        
-        super(VGAE, self).__init__()
-        
-        N = emb_dim[0] # Number of nodes in the graph
-        F = emb_dim[1] # Original size of node features
-        self.freeze_embeddings = freeze_embeddings
-
-        x_in = Input(shape=(1,), dtype=tf.int64)
-        a_in = Input((N,), dtype=tf.float32)
-        if embeddings is not None:
-            x = Embedding(N, F, weights=[embeddings], 
-                          trainable=not freeze_embeddings)(x_in)
-        else:
-            x = Embedding(N, F, trainable=not freeze_embeddings)(x_in)
-        x = Flatten()(x)
-        x_orig = x
-        
-#         for _ in range(2):
-#             x = Dense(256)(x)
-#             x = LeakyReLU()(x)
-#             x = BatchNormalization(epsilon=1e-3)(x)
-        
-
-        x = GCNConv( hidden_dim1,
-                     activation=None,
-                     kernel_regularizer=l2(l2_reg))([x, a_in])
-        x = LeakyReLU()(x)
-        x = LayerNormalization(epsilon=1e-6)(x)
-        x = Dropout(dropout)(x)
-
-        z_mean = GCNConv(
-            hidden_dim2,
-            activation=None,
-            kernel_regularizer=l2(l2_reg),
-        )([x, a_in])
-        
-        z_log_std = GCNConv(
-            hidden_dim2,
-            activation=None,
-            kernel_regularizer=l2(l2_reg),
-        )([x, a_in])
-        
-        self.encoder = Model([x_in, a_in], [z_mean, z_log_std, x_orig])
-        self.encoder.build([ (None,1), (None,N) ])
-        
-        z_in = Input(shape=(hidden_dim2,))
-        x = z_in
-        for _ in range(2):
-            x = Dense(256)(x)
-            x = LeakyReLU()(x)
-            x = BatchNormalization(epsilon=1e-6)(x)
-        #x = Dense(emb_dim[1])(x)
-        
-        
-        self.decoder = Model(z_in, x)
-        self.decoder.build((None, hidden_dim2))
-        
-        self.optimizer = Adam(learning_rate=lr)#, clipnorm=1.0)
-    
-    def call(self, x, indices=None, training=True):
-        x,a = x
-        z_mean, z_log_std, x_orig = self.encoder((x,a), training=training)
-        #z_log_std = tf.nn.softplus(z_log_std)
-        z_log_std = tf.clip_by_value(z_log_std, -2, 2)
-        z_sample = tf.random.normal(tf.shape(z_mean)) * tf.exp(z_log_std)
-        if training:
-            z = z_mean + z_sample
-            z = tf.gather(z, indices)
-            out = tf.matmul(z, tf.transpose(z))
-            out = tf.nn.sigmoid(out)
-        else:
-            z = z_mean
-            out = None
-        
-        return out, z, z_mean, z_log_std, x_orig
-    
-    def train_step(self, x, a, y, pos_weight, norm, indices):
-        loss = self._train_step(x, a, y, pos_weight, norm, indices)
-        return loss.numpy()
-    
-    @tf.function
-    def _train_step(self, x, a, y, pos_weight, norm, indices, loss="graph"): #loss="features"
-        with tf.GradientTape() as tape:
-            predictions, z, model_z_mean, model_z_log_std, x_orig = self((x, a), indices, training=True)            
-            pairs = []
-            for i in indices:
-                for j in indices:
-                    pairs.append((i,j))
-            pairs = tf.convert_to_tensor(pairs, dtype=tf.int32)
-            y = tf.gather_nd(a, pairs)
-            y = tf.reshape(y, [-1])
-            predictions = tf.reshape(predictions, [-1])
-            rec_loss = norm*tf.reduce_mean(tf.nn.weighted_cross_entropy_with_logits(logits=predictions, labels=y, pos_weight=pos_weight))
-
-            # latent loss
-            kl_loss = (0.5 / tf.cast(tf.shape(x)[-1], tf.float32)) * tf.reduce_mean(tf.reduce_sum(
-            1. + 2. * model_z_log_std - tf.square(model_z_mean) - tf.square(tf.exp(model_z_log_std)), 1
-            ))
-            
-            loss = rec_loss - kl_loss + tf.reduce_sum(self.encoder.losses)
-            ## Add reconstruction loss
-            if self.freeze_embeddings:
-                x_hat = self.decoder(z, training=True)
-                loss = loss + 0.5*tf.reduce_mean((x_hat - tf.gather(x_orig, indices))**2)
-                
-        tw = self.encoder.trainable_weights
-        if self.freeze_embeddings:
-            tw += self.decoder.trainable_weights
-        gradients = tape.gradient(loss,tw)
-        self.optimizer.apply_gradients(zip(gradients, tw))
-        return loss
-
-class GCN(Model):
-    def __init__(
-        self,
-        features_shape,
-        input_dim,
-        labels,
-        adj,
-        embsize=None,
-        n_labels=None,
-        hidden_units=None,
-        layers=None,
-        conv_last=None,
-        use_bn=True,
-        use_vae=False,
-        predict=False,
-        dropout=0.5
-    ):
-        super(GCN, self).__init__()
-        #assert layers > 0
-        self.features_shape = features_shape
-        self.labels = labels
-        self.adj = adj
-        self.adj_size = adj.dense_shape.numpy()
-
-        adj_in = Input(shape=self.adj_size[1:], batch_size=self.adj_size[0], dtype=tf.float32, sparse=True)
-        node_in = Input(shape=input_dim, batch_size=self.adj_size[0], dtype=tf.float32)
-
-        x = node_in
-        # first gcn layer
-        for l in range(layers):
-            x = Dense(hidden_units, use_bias=(l == 0))(x)
-            x = Lambda(lambda t: tf.sparse.sparse_dense_matmul(t[0], t[1]))([adj_in, x])
-            x = BiasLayer()(x)
-            if use_bn:
-                x = BatchNormalization(momentum=0.9, epsilon=1e-5)(x)
-            x = Activation("relu")(x)
-            x = Dropout(dropout)(x)
-
-        if use_vae:
-            mu = Dense(embsize, use_bias=True)(x)
-            log_std = Dense(embsize, use_bias=True)(x)
-            x = Concatenate(axis=1)([mu, log_std])
-        else:
-            x = Dense(embsize, use_bias=True)(x)
-            if predict:
-                x = Dense(n_labels, use_bias=False)(x)
-                x = Softmax()(x)
-                #x = Lambda(lambda t: tf.sparse.sparse_dense_matmul(t[0], t[1]))([adj_in, x])
-                #x = BiasLayer()(x)
-
-        self.model = Model([node_in, adj_in], x)
-        self.model.build([(features_shape[0], input_dim), tuple(self.adj_size)])
-
-    def call(self, features, idx, training=True):
-        output = self.model((features, self.adj), training=training)
-        if idx is None:
-            return output
-        else:
-            return tf.gather(output, idx)
-
-    def summary(self):
-        self.model.summary()
-
-
-class GCNLAF(Model):
-    def __init__(self, features_shape, input_dim, labels, adj,
-                 n_labels=None, hidden_units=None, embsize=None,
-                 layers=None, conv_last=None, dropout=0.5):
-        super(GCNLAF, self).__init__()
-        #assert layers > 0
-        self.features_shape = features_shape
-        self.labels = labels
-        self.adj = adj
-        self.adj_size = adj.dense_shape.numpy()
-
-        adj_in = Input(shape=self.adj_size[1:], batch_size=self.adj_size[0], dtype=tf.float32, sparse=True)
-        node_in = Input(shape=input_dim, batch_size=self.adj_size[0], dtype=tf.float32)
-
-        x = node_in
-        # first gcn layer
-        for l in range(layers):
-            x = Dense(hidden_units, use_bias=(l == 0))(x)
-            x = LAF(4)([adj_in, x])
-            x = BiasLayer()(x)
-            x = BatchNormalization(momentum=0.9, epsilon=1e-5)(x)
-            x = Activation("relu")(x)
-            x = Dropout(dropout)(x)
-
-        # third gcn layer
-        if conv_last:
-            x = Dense(embsize, use_bias=False)(x)
-            x = LAF(4)([adj_in, x])
-            x = BiasLayer()(x)
-        else:
-            x = Dense(embsize, use_bias=True)(x)
-
-        self.model = Model([node_in, adj_in], x)
-        self.model.build([(self.features_shape[0], input_dim), tuple(self.adj_size)])
-
-    def call(self, features, idx, training=True):
-        output = self.model((features, self.adj), training=training)
-        if idx is None:
-            return output
-        else:
-            return tf.gather(output, idx)
-
-    def summary(self):
-        self.model.summary()
-
-
-class GAT(Model):
-    def __init__(
-        self, features_shape, input_dim, labels, adj, embsize=None,
-        hidden_units=None, layers=None, conv_last=None, dropout=0.5
-    ):
-        super(GAT, self).__init__()
-        self.features_shape = features_shape
-        self.labels = labels
-        self.adj = adj
-        self.adj_size = adj.dense_shape.numpy()
-
-        adj_in = Input(shape=self.adj_size[1:], batch_size=self.adj_size[0], dtype=tf.float32, sparse=True)
-        node_in = Input(shape=input_dim, batch_size=self.adj_size[0], dtype=tf.float32)
-
-        x = node_in
-        for l in range(layers):
-            x = GraphAttention(hidden_units, dropout_rate=0.1, attn_heads=1, activation="linear")([adj_in, x])
-            x = BatchNormalization(momentum=0.9, epsilon=1e-5)(x)
-            x = Activation("relu")(x)
-            x = Dropout(dropout)(x)
-
-        # second sage layer
-        if conv_last:
-            x = GraphAttention(
-                embsize, dropout_rate=0.1, attn_heads=1, activation="linear", attn_heads_reduction="average"
-            )([adj_in, x])
-        else:
-            x = Dense(embsize, use_bias=True)(x)
-
-        self.model = Model([node_in, adj_in], x)
-        self.model.build([(features_shape[0], input_dim), tuple(self.adj_size)])
-
-    def call(self, features, idx, training=True):
-        output = self.model((features, self.adj), training=training)
-        if idx is None:
-            return output
-        else:
-            return tf.gather(output, idx)
-
-    def summary(self):
-        self.model.summary()
-
-
-class GATLAF(Model):
-    def __init__(self, features, labels, adj, n_labels=None, embsize=None,
-                hidden_units=None, layers=None, conv_last=None):
-        super(GATLAF, self).__init__()
-        self.features = features
-        self.labels = labels
-        self.adj = adj
-        self.adj_size = adj.dense_shape.numpy()
-
-        adj_in = Input(shape=self.adj_size[1:], batch_size=self.adj_size[0], dtype=tf.float32, sparse=True)
-        node_in = Input(shape=features.shape[1:], batch_size=self.adj_size[0], dtype=tf.float32)
-
-        x = node_in
-        for l in range(layers):
-            x = GraphAttention(hidden_units, dropout_rate=0.1, attn_heads=1, activation="linear", laf_units=4)(
-                [adj_in, x]
-            )
-            x = BatchNormalization(momentum=0.9, epsilon=1e-5)(x)
-            x = Activation("relu")(x)
-            x = Dropout(0.5)(x)
-
-        # second sage layer
-        if conv_last:
-            x = GraphAttention(
-                embsize,
-                dropout_rate=0.1,
-                attn_heads=1,
-                activation="linear",
-                attn_heads_reduction="average",
-                laf_units=4,
-            )([adj_in, x])
-        else:
-            x = Dense(embsize, use_bias=True)(x)
-
-        self.model = Model([node_in, adj_in], x)
-        self.model.build([tuple(self.features.shape), tuple(self.adj_size)])
-
-    def call(self, idx, training=True):
-        output = self.model((self.features, self.adj), training=training)
-        if idx is None:
-            return output
-        else:
-            return tf.gather(output, idx)
-
-    def summary(self):
-        self.model.summary()
-
-
-class SAGE(Model):
-    def __init__(
-        self, features_shape, input_dim, labels, adj, embsize=None,
-        n_labels=None, hidden_units=None, layers=None, conv_last=None,
-        dropout=0.5
-    ):
-        super(SAGE, self).__init__()
-        self.features_shape = features_shape
-        self.labels = labels
-        self.adj = adj
-        self.adj_size = adj.dense_shape.numpy()
-
-        adj_in = Input(shape=self.adj_size[1:], batch_size=self.adj_size[0], dtype=tf.float32, sparse=True)
-        node_in = Input(shape=input_dim, batch_size=self.adj_size[0], dtype=tf.float32)
-
-        x = node_in
-        # first sage layer
-        for l in range(layers):
-            x_node = Dense(hidden_units, use_bias=(l == 0))(x)
-            x_neigh = Dense(hidden_units, use_bias=(l == 0))(x)
-            x = Lambda(lambda t: tf.sparse.sparse_dense_matmul(t[0], t[1]))([adj_in, x_neigh])
-            x = BiasLayer()(x)
-            x = Add()([x_node, x])
-            x = BatchNormalization(momentum=0.9, epsilon=1e-5)(x)
-            x = Activation("relu")(x)
-            x = Dropout(dropout)(x)
-
-        # second sage layer
-        if conv_last:
-            x_node = Dense(embsize, use_bias=False)(x)
-            x_neigh = Dense(embsize, use_bias=False)(x)
-            x = Lambda(lambda t: tf.sparse.sparse_dense_matmul(t[0], t[1]))([adj_in, x_neigh])
-            x = BiasLayer()(x)
-            x = Add()([x_node, x])
-        else:
-            x = Dense(embsize, use_bias=True)(x)
-
-        self.model = Model([node_in, adj_in], x)
-        self.model.build([(self.features_shape[0], input_dim), tuple(self.adj_size)])
-
-    def call(self, features, idx, training=True):
-        output = self.model((features, self.adj), training=training)
-        if idx is None:
-            return output
-        else:
-            return tf.gather(output, idx)
-
-    def summary(self):
-        self.model.summary()
-
-
-class SAGELAF(Model):
-    def __init__(self, features_shape, labels, input_dim, adj,
-                n_labels=None, embsize=None, hidden_units=None,
-                layers=None, conv_last=None, dropout=0.5):
-        super(SAGELAF, self).__init__()
-        self.features_shape = features_shape
-        self.labels = labels
-        self.adj = adj
-        self.adj_size = adj.dense_shape.numpy()
-
-        adj_in = Input(shape=self.adj_size[1:], batch_size=self.adj_size[0], dtype=tf.float32, sparse=True)
-        node_in = Input(shape=input_dim, batch_size=self.adj_size[0], dtype=tf.float32)
-
-        x = node_in
-        # first sage layer
-        for l in range(layers):
-            x_node = Dense(hidden_units, use_bias=(l == 0))(x)
-            x_neigh = Dense(hidden_units, use_bias=(l == 0))(x)
-            x = LAF(4)([adj_in, x_neigh])
-            x = BiasLayer()(x)
-            x = Add()([x_node, x])
-            x = BatchNormalization(momentum=0.9, epsilon=1e-5)(x)
-            x = Activation("relu")(x)
-            x = Dropout(dropout)(x)
-
-        # second sage layer
-        if conv_last:
-            x_node = Dense(embsize, use_bias=False)(x)
-            x_neigh = Dense(embsize, use_bias=False)(x)
-            x = LAF(4)([adj_in, x_neigh])
-            x = BiasLayer()(x)
-            x = Add()([x_node, x])
-        else:
-            x = Dense(embsize, use_bias=True)(x)
-
-        self.model = Model([node_in, adj_in], x)
-        self.model.build([(self.features_shape[0], input_dim),
-                           tuple(self.adj_size)])
-
-    def call(self, features, idx, training=True):
-        output = self.model((features, self.adj), training=training)
-        if idx is None:
-            return output
-        else:
-            return tf.gather(output, idx)
-
-    def summary(self):
-        self.model.summary()
-
-name_to_model = {"SAGE": SAGE, "SAGELAF": SAGELAF, "GCN": GCN, "GCNLAF": GCNLAF, "GAT": GAT, "GATLAF": GATLAF}
+import tensorflow as tf
+
+from tensorflow.keras.optimizers import Adam, SGD
+from tensorflow.keras.models import Model
+from tensorflow.keras.layers import Input, Dense, Activation, Softmax, Embedding, LayerNormalization
+#from tensorflow.keras import Sequential
+from tensorflow.keras.layers import BatchNormalization, Lambda, LeakyReLU, Flatten
+from tensorflow.keras.layers import Dropout, Add, Concatenate
+from tensorflow.keras.losses import SparseCategoricalCrossentropy
+import numpy as np
+from tensorflow.keras.regularizers import l2    
+
+from graphmb.layers import BiasLayer, LAF, GraphAttention
+
+class VGAE(Model):
+    def __init__(self, emb_dim, embeddings=None, 
+                 hidden_dim1=None, hidden_dim2=None,
+                 dropout=None, l2_reg=None,
+                 freeze_embeddings=False, lr=1e-02):
+        
+        super(VGAE, self).__init__()
+        
+        N = emb_dim[0] # Number of nodes in the graph
+        F = emb_dim[1] # Original size of node features
+        self.freeze_embeddings = freeze_embeddings
+
+        x_in = Input(shape=(1,), dtype=tf.int64)
+        a_in = Input((N,), dtype=tf.float32)
+        if embeddings is not None:
+            x = Embedding(N, F, weights=[embeddings], 
+                          trainable=not freeze_embeddings)(x_in)
+        else:
+            x = Embedding(N, F, trainable=not freeze_embeddings)(x_in)
+        x = Flatten()(x)
+        x_orig = x
+        
+#         for _ in range(2):
+#             x = Dense(256)(x)
+#             x = LeakyReLU()(x)
+#             x = BatchNormalization(epsilon=1e-3)(x)
+        
+
+        x = GCNConv( hidden_dim1,
+                     activation=None,
+                     kernel_regularizer=l2(l2_reg))([x, a_in])
+        x = LeakyReLU()(x)
+        x = LayerNormalization(epsilon=1e-6)(x)
+        x = Dropout(dropout)(x)
+
+        z_mean = GCNConv(
+            hidden_dim2,
+            activation=None,
+            kernel_regularizer=l2(l2_reg),
+        )([x, a_in])
+        
+        z_log_std = GCNConv(
+            hidden_dim2,
+            activation=None,
+            kernel_regularizer=l2(l2_reg),
+        )([x, a_in])
+        
+        self.encoder = Model([x_in, a_in], [z_mean, z_log_std, x_orig])
+        self.encoder.build([ (None,1), (None,N) ])
+        
+        z_in = Input(shape=(hidden_dim2,))
+        x = z_in
+        for _ in range(2):
+            x = Dense(256)(x)
+            x = LeakyReLU()(x)
+            x = BatchNormalization(epsilon=1e-6)(x)
+        #x = Dense(emb_dim[1])(x)
+        
+        
+        self.decoder = Model(z_in, x)
+        self.decoder.build((None, hidden_dim2))
+        
+        self.optimizer = Adam(learning_rate=lr)#, clipnorm=1.0)
+    
+    def call(self, x, indices=None, training=True):
+        x,a = x
+        z_mean, z_log_std, x_orig = self.encoder((x,a), training=training)
+        #z_log_std = tf.nn.softplus(z_log_std)
+        z_log_std = tf.clip_by_value(z_log_std, -2, 2)
+        z_sample = tf.random.normal(tf.shape(z_mean)) * tf.exp(z_log_std)
+        if training:
+            z = z_mean + z_sample
+            z = tf.gather(z, indices)
+            out = tf.matmul(z, tf.transpose(z))
+            out = tf.nn.sigmoid(out)
+        else:
+            z = z_mean
+            out = None
+        
+        return out, z, z_mean, z_log_std, x_orig
+    
+    def train_step(self, x, a, y, pos_weight, norm, indices):
+        loss = self._train_step(x, a, y, pos_weight, norm, indices)
+        return loss.numpy()
+    
+    @tf.function
+    def _train_step(self, x, a, y, pos_weight, norm, indices, loss="graph"): #loss="features"
+        with tf.GradientTape() as tape:
+            predictions, z, model_z_mean, model_z_log_std, x_orig = self((x, a), indices, training=True)            
+            pairs = []
+            for i in indices:
+                for j in indices:
+                    pairs.append((i,j))
+            pairs = tf.convert_to_tensor(pairs, dtype=tf.int32)
+            y = tf.gather_nd(a, pairs)
+            y = tf.reshape(y, [-1])
+            predictions = tf.reshape(predictions, [-1])
+            rec_loss = norm*tf.reduce_mean(tf.nn.weighted_cross_entropy_with_logits(logits=predictions, labels=y, pos_weight=pos_weight))
+
+            # latent loss
+            kl_loss = (0.5 / tf.cast(tf.shape(x)[-1], tf.float32)) * tf.reduce_mean(tf.reduce_sum(
+            1. + 2. * model_z_log_std - tf.square(model_z_mean) - tf.square(tf.exp(model_z_log_std)), 1
+            ))
+            
+            loss = rec_loss - kl_loss + tf.reduce_sum(self.encoder.losses)
+            ## Add reconstruction loss
+            if self.freeze_embeddings:
+                x_hat = self.decoder(z, training=True)
+                loss = loss + 0.5*tf.reduce_mean((x_hat - tf.gather(x_orig, indices))**2)
+                
+        tw = self.encoder.trainable_weights
+        if self.freeze_embeddings:
+            tw += self.decoder.trainable_weights
+        gradients = tape.gradient(loss,tw)
+        self.optimizer.apply_gradients(zip(gradients, tw))
+        return loss
+
+class GCN(Model):
+    def __init__(
+        self,
+        features_shape,
+        input_dim,
+        labels,
+        adj,
+        embsize=None,
+        n_labels=None,
+        hidden_units=None,
+        layers=None,
+        conv_last=None,
+        use_bn=True,
+        use_vae=False,
+        predict=False,
+        dropout=0.5
+    ):
+        super(GCN, self).__init__()
+        #assert layers > 0
+        self.features_shape = features_shape
+        self.labels = labels
+        self.adj = adj
+        self.adj_size = adj.dense_shape.numpy()
+
+        adj_in = Input(shape=self.adj_size[1:], batch_size=self.adj_size[0], dtype=tf.float32, sparse=True)
+        node_in = Input(shape=input_dim, batch_size=self.adj_size[0], dtype=tf.float32)
+
+        x = node_in
+        # first gcn layer
+        for l in range(layers):
+            x = Dense(hidden_units, use_bias=(l == 0))(x)
+            x = Lambda(lambda t: tf.sparse.sparse_dense_matmul(t[0], t[1]))([adj_in, x])
+            x = BiasLayer()(x)
+            if use_bn:
+                x = BatchNormalization(momentum=0.9, epsilon=1e-5)(x)
+            x = Activation("relu")(x)
+            x = Dropout(dropout)(x)
+
+        if use_vae:
+            mu = Dense(embsize, use_bias=True)(x)
+            log_std = Dense(embsize, use_bias=True)(x)
+            x = Concatenate(axis=1)([mu, log_std])
+        else:
+            x = Dense(embsize, use_bias=True)(x)
+            if predict:
+                x = Dense(n_labels, use_bias=False)(x)
+                x = Softmax()(x)
+                #x = Lambda(lambda t: tf.sparse.sparse_dense_matmul(t[0], t[1]))([adj_in, x])
+                #x = BiasLayer()(x)
+
+        self.model = Model([node_in, adj_in], x)
+        self.model.build([(features_shape[0], input_dim), tuple(self.adj_size)])
+
+    def call(self, features, idx, training=True):
+        output = self.model((features, self.adj), training=training)
+        if idx is None:
+            return output
+        else:
+            return tf.gather(output, idx)
+
+    def summary(self):
+        self.model.summary()
+
+
+class GCNLAF(Model):
+    def __init__(self, features_shape, input_dim, labels, adj,
+                 n_labels=None, hidden_units=None, embsize=None,
+                 layers=None, conv_last=None, dropout=0.5):
+        super(GCNLAF, self).__init__()
+        #assert layers > 0
+        self.features_shape = features_shape
+        self.labels = labels
+        self.adj = adj
+        self.adj_size = adj.dense_shape.numpy()
+
+        adj_in = Input(shape=self.adj_size[1:], batch_size=self.adj_size[0], dtype=tf.float32, sparse=True)
+        node_in = Input(shape=input_dim, batch_size=self.adj_size[0], dtype=tf.float32)
+
+        x = node_in
+        # first gcn layer
+        for l in range(layers):
+            x = Dense(hidden_units, use_bias=(l == 0))(x)
+            x = LAF(4)([adj_in, x])
+            x = BiasLayer()(x)
+            x = BatchNormalization(momentum=0.9, epsilon=1e-5)(x)
+            x = Activation("relu")(x)
+            x = Dropout(dropout)(x)
+
+        # third gcn layer
+        if conv_last:
+            x = Dense(embsize, use_bias=False)(x)
+            x = LAF(4)([adj_in, x])
+            x = BiasLayer()(x)
+        else:
+            x = Dense(embsize, use_bias=True)(x)
+
+        self.model = Model([node_in, adj_in], x)
+        self.model.build([(self.features_shape[0], input_dim), tuple(self.adj_size)])
+
+    def call(self, features, idx, training=True):
+        output = self.model((features, self.adj), training=training)
+        if idx is None:
+            return output
+        else:
+            return tf.gather(output, idx)
+
+    def summary(self):
+        self.model.summary()
+
+
+class GAT(Model):
+    def __init__(
+        self, features_shape, input_dim, labels, adj, embsize=None,
+        hidden_units=None, layers=None, conv_last=None, dropout=0.5
+    ):
+        super(GAT, self).__init__()
+        self.features_shape = features_shape
+        self.labels = labels
+        self.adj = adj
+        self.adj_size = adj.dense_shape.numpy()
+
+        adj_in = Input(shape=self.adj_size[1:], batch_size=self.adj_size[0], dtype=tf.float32, sparse=True)
+        node_in = Input(shape=input_dim, batch_size=self.adj_size[0], dtype=tf.float32)
+
+        x = node_in
+        for l in range(layers):
+            x = GraphAttention(hidden_units, dropout_rate=0.1, attn_heads=1, activation="linear")([adj_in, x])
+            x = BatchNormalization(momentum=0.9, epsilon=1e-5)(x)
+            x = Activation("relu")(x)
+            x = Dropout(dropout)(x)
+
+        # second sage layer
+        if conv_last:
+            x = GraphAttention(
+                embsize, dropout_rate=0.1, attn_heads=1, activation="linear", attn_heads_reduction="average"
+            )([adj_in, x])
+        else:
+            x = Dense(embsize, use_bias=True)(x)
+
+        self.model = Model([node_in, adj_in], x)
+        self.model.build([(features_shape[0], input_dim), tuple(self.adj_size)])
+
+    def call(self, features, idx, training=True):
+        output = self.model((features, self.adj), training=training)
+        if idx is None:
+            return output
+        else:
+            return tf.gather(output, idx)
+
+    def summary(self):
+        self.model.summary()
+
+
+class GATLAF(Model):
+    def __init__(self, features, labels, adj, n_labels=None, embsize=None,
+                hidden_units=None, layers=None, conv_last=None):
+        super(GATLAF, self).__init__()
+        self.features = features
+        self.labels = labels
+        self.adj = adj
+        self.adj_size = adj.dense_shape.numpy()
+
+        adj_in = Input(shape=self.adj_size[1:], batch_size=self.adj_size[0], dtype=tf.float32, sparse=True)
+        node_in = Input(shape=features.shape[1:], batch_size=self.adj_size[0], dtype=tf.float32)
+
+        x = node_in
+        for l in range(layers):
+            x = GraphAttention(hidden_units, dropout_rate=0.1, attn_heads=1, activation="linear", laf_units=4)(
+                [adj_in, x]
+            )
+            x = BatchNormalization(momentum=0.9, epsilon=1e-5)(x)
+            x = Activation("relu")(x)
+            x = Dropout(0.5)(x)
+
+        # second sage layer
+        if conv_last:
+            x = GraphAttention(
+                embsize,
+                dropout_rate=0.1,
+                attn_heads=1,
+                activation="linear",
+                attn_heads_reduction="average",
+                laf_units=4,
+            )([adj_in, x])
+        else:
+            x = Dense(embsize, use_bias=True)(x)
+
+        self.model = Model([node_in, adj_in], x)
+        self.model.build([tuple(self.features.shape), tuple(self.adj_size)])
+
+    def call(self, idx, training=True):
+        output = self.model((self.features, self.adj), training=training)
+        if idx is None:
+            return output
+        else:
+            return tf.gather(output, idx)
+
+    def summary(self):
+        self.model.summary()
+
+
+class SAGE(Model):
+    def __init__(
+        self, features_shape, input_dim, labels, adj, embsize=None,
+        n_labels=None, hidden_units=None, layers=None, conv_last=None,
+        dropout=0.5
+    ):
+        super(SAGE, self).__init__()
+        self.features_shape = features_shape
+        self.labels = labels
+        self.adj = adj
+        self.adj_size = adj.dense_shape.numpy()
+
+        adj_in = Input(shape=self.adj_size[1:], batch_size=self.adj_size[0], dtype=tf.float32, sparse=True)
+        node_in = Input(shape=input_dim, batch_size=self.adj_size[0], dtype=tf.float32)
+
+        x = node_in
+        # first sage layer
+        for l in range(layers):
+            x_node = Dense(hidden_units, use_bias=(l == 0))(x)
+            x_neigh = Dense(hidden_units, use_bias=(l == 0))(x)
+            x = Lambda(lambda t: tf.sparse.sparse_dense_matmul(t[0], t[1]))([adj_in, x_neigh])
+            x = BiasLayer()(x)
+            x = Add()([x_node, x])
+            x = BatchNormalization(momentum=0.9, epsilon=1e-5)(x)
+            x = Activation("relu")(x)
+            x = Dropout(dropout)(x)
+
+        # second sage layer
+        if conv_last:
+            x_node = Dense(embsize, use_bias=False)(x)
+            x_neigh = Dense(embsize, use_bias=False)(x)
+            x = Lambda(lambda t: tf.sparse.sparse_dense_matmul(t[0], t[1]))([adj_in, x_neigh])
+            x = BiasLayer()(x)
+            x = Add()([x_node, x])
+        else:
+            x = Dense(embsize, use_bias=True)(x)
+
+        self.model = Model([node_in, adj_in], x)
+        self.model.build([(self.features_shape[0], input_dim), tuple(self.adj_size)])
+
+    def call(self, features, idx, training=True):
+        output = self.model((features, self.adj), training=training)
+        if idx is None:
+            return output
+        else:
+            return tf.gather(output, idx)
+
+    def summary(self):
+        self.model.summary()
+
+
+class SAGELAF(Model):
+    def __init__(self, features_shape, labels, input_dim, adj,
+                n_labels=None, embsize=None, hidden_units=None,
+                layers=None, conv_last=None, dropout=0.5):
+        super(SAGELAF, self).__init__()
+        self.features_shape = features_shape
+        self.labels = labels
+        self.adj = adj
+        self.adj_size = adj.dense_shape.numpy()
+
+        adj_in = Input(shape=self.adj_size[1:], batch_size=self.adj_size[0], dtype=tf.float32, sparse=True)
+        node_in = Input(shape=input_dim, batch_size=self.adj_size[0], dtype=tf.float32)
+
+        x = node_in
+        # first sage layer
+        for l in range(layers):
+            x_node = Dense(hidden_units, use_bias=(l == 0))(x)
+            x_neigh = Dense(hidden_units, use_bias=(l == 0))(x)
+            x = LAF(4)([adj_in, x_neigh])
+            x = BiasLayer()(x)
+            x = Add()([x_node, x])
+            x = BatchNormalization(momentum=0.9, epsilon=1e-5)(x)
+            x = Activation("relu")(x)
+            x = Dropout(dropout)(x)
+
+        # second sage layer
+        if conv_last:
+            x_node = Dense(embsize, use_bias=False)(x)
+            x_neigh = Dense(embsize, use_bias=False)(x)
+            x = LAF(4)([adj_in, x_neigh])
+            x = BiasLayer()(x)
+            x = Add()([x_node, x])
+        else:
+            x = Dense(embsize, use_bias=True)(x)
+
+        self.model = Model([node_in, adj_in], x)
+        self.model.build([(self.features_shape[0], input_dim),
+                           tuple(self.adj_size)])
+
+    def call(self, features, idx, training=True):
+        output = self.model((features, self.adj), training=training)
+        if idx is None:
+            return output
+        else:
+            return tf.gather(output, idx)
+
+    def summary(self):
+        self.model.summary()
+
+name_to_model = {"SAGE": SAGE, "SAGELAF": SAGELAF, "GCN": GCN, "GCNLAF": GCNLAF, "GAT": GAT, "GATLAF": GATLAF}
```

### Comparing `graphmb-0.2.4/src/graphmb/graphmb1.py` & `graphmb-0.2.5/src/graphmb/graphmb1.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,406 +1,406 @@
-
-import time
-import os
-import networkx as nx
-import numpy as np
-import operator
-
-#import tensorflow
-
-from graphmb.evaluate import read_contig_genes, read_marker_gene_sets, evaluate_contig_sets
-from graphmb.contigsdataset import get_kmer_to_id, count_kmers
-from graphmb.utils import SEED
-# import torch
-
-def open_gfa_file(filename, filter=1000, root=False, kmer=4):
-    G = nx.Graph()
-    if root:
-        root_node = G.add_node("root", length=0)
-    skipped_contigs = set()
-    skipped_edges = set()
-    kmer_to_id, canonical_k = get_kmer_to_id(kmer)
-    with open(filename, "r") as f:
-        for line in f:
-            if line.startswith("S"):
-                values = line.strip().split()
-                contigid = values[1]
-                # contiglen = int(values[3].split(":")[-1])
-                contiglen = len(values[2])
-                contig_kmers = count_kmers(values[2], kmer, kmer_to_id, canonical_k)
-                if contiglen < filter:
-                    skipped_contigs.add(contigid)
-                else:
-
-                    G.add_node(contigid, length=contiglen, kmers=contig_kmers)  # TODO: add coverage and kmer too
-                    if root:
-                        G.add_edge(contigid, "root")
-            if line.startswith("L"):
-                values = line.strip().split()
-                if values[1] in skipped_contigs or values[3] in skipped_contigs:
-                    skipped_edges.add((values[1], values[3]))
-                    continue
-                G.add_edge(values[1], values[3])
-
-    print("load graph from GFA")
-    print("skipped these contigs {} (len<{})".format(len(skipped_contigs), filter))
-    print("skipped these edges {} (len<{})".format(len(skipped_edges), filter))
-    return G
-
-
-def cluster_embs(node_embeddings, node_ids, clusteringalgo, kclusters, device="cpu", node_lens=None, seed=0):
-    #set_seed(seed)
-    if clusteringalgo == "vamb":
-        from vamb.cluster import cluster as vamb_cluster
-        it = vamb_cluster(
-            node_embeddings, node_ids, cuda=(device == "cuda:0")
-        )  # , seeds=seeds)  # contig_lens=node_lens)  #
-        cluster_to_contig = {i: c for (i, (n, c)) in enumerate(it)}
-
-        # get embs to clusters (cluster to contig has only contig names, not index)
-        """cluster_to_embs = {
-            c: np.array([node_embeddings[i] for i, n in enumerate(node_ids) if n in cluster_to_contig[c]])
-            for c in cluster_to_contig
-        }
-        cluster_centroids = np.array([cluster_to_embs[c].mean(0) for c in cluster_to_contig])"""
-        cluster_centroids = None  # not necessary for now
-    else:
-        from sklearn.cluster import (
-            KMeans,
-            DBSCAN,
-            AgglomerativeClustering,
-            MiniBatchKMeans,
-            SpectralClustering,
-            Birch,
-            OPTICS,
-        )
-        from sklearn.mixture import GaussianMixture
-
-        if clusteringalgo == "kmeans":
-            clustering = KMeans(n_clusters=kclusters, random_state=SEED)
-            cluster_labels = clustering.fit_predict(node_embeddings)
-            cluster_centroids = clustering.cluster_centers_
-        elif clusteringalgo == "kmeansgpu":
-            node_embeddings = torch.tensor(node_embeddings).cuda()
-            cluster_labels, cluster_centroids = kmeans_pytorch.kmeans(
-                X=node_embeddings, num_clusters=kclusters, device=torch.device("cuda:0")
-            )
-        elif clusteringalgo == "dbscan":
-            cluster_labels = DBSCAN(eps=1.1, min_samples=5).fit_predict(node_embeddings)
-            # cluster_centroids = clustering.cluster_centers_
-            cluster_centroids = None
-        elif clusteringalgo == "gmm":
-            cluster_model = GaussianMixture(
-                n_components=kclusters,
-                covariance_type="full",
-                max_iter=1000,
-                random_state=SEED,
-                verbose=2,
-                verbose_interval=1,
-            ).fit(node_embeddings)
-            cluster_labels = cluster_model.predict(node_embeddings)
-            cluster_centroids = cluster_model.means_
-        elif clusteringalgo == "kmeansconst":
-            cluster_labels = KMeansConstrained(
-                n_clusters=kclusters, size_min=1, size_max=5, random_state=SEED
-            ).fit_predict(node_embeddings)
-        elif clusteringalgo == "kmeansbatch":
-            kmeans = MiniBatchKMeans(n_clusters=kclusters, random_state=SEED, batch_size=100, init=seed_matrix)
-            cluster_labels = kmeans.fit_predict(node_embeddings)
-            cluster_centroids = kmeans.cluster_centers_
-        elif clusteringalgo == "spectral":
-            cluster_labels = SpectralClustering(n_clusters=kclusters, random_state=SEED).fit_predict(node_embeddings)
-            cluster_centroids = None
-        elif clusteringalgo == "birch":
-            cluster_labels = Birch(n_clusters=kclusters).fit_predict(node_embeddings)
-            cluster_centroids = None
-        elif clusteringalgo == "optics":
-            cluster_labels = OPTICS(min_samples=5, cluster_method="xi", n_jobs=-1).fit_predict(node_embeddings)
-            cluster_centroids = None
-        else:
-            print("invalid clustering algorithm")
-            return None
-        # compare clustering labels with actual labels
-        # for each cluster, get majority label, and then P/R
-        cluster_to_contig = {i: [] for i in range(kclusters)}
-        for il, l in enumerate(cluster_labels):
-            # if l not in cluster_to_contig:
-            #    cluster_to_contig[l] = []
-            cluster_to_contig[l].append(node_ids[il])
-
-    return cluster_to_contig, cluster_centroids
-
-
-def evaluate_binning(cluster_to_contig, node_to_label, label_to_node, outputclusters=False, contig_sizes=None):
-    """Evaluate binning results using contig labels (supervised scenario)
-
-    :param cluster_to_contig: mapping cluster IDs to contig names
-    :type cluster_to_contig: dict
-    :param node_to_label: mapping contig ids to labels (taxon)
-    :type node_to_label: dict
-    :param label_to_node: mapping label names to cotnigs
-    :type label_to_node: dict
-    :param outputclusters: print members of all clusters, defaults to False
-    :type outputclusters: bool, optional
-    :param contig_sizes: Provide contig sizes for balanced scores, defaults to None
-    :type contig_sizes: dict, optional
-    """
-    # uncomment if you want to plot only the biggest labels
-    # labels_to_plot = sorted(label_to_node, key = lambda key: len(label_to_node.get(key, [])), reverse=True)[:6]
-    # print(labels_to_plot)
-    avg_precision = []
-    avg_recall = []
-    avg_f1 = []
-    cluster_sizes = []
-    if contig_sizes is None:
-        contig_sizes = {c: 1 for c in node_to_label}
-    for c in cluster_to_contig:
-        cluster_labels = [node_to_label.get(n) for n in cluster_to_contig[c] if n in node_to_label]
-        cluster_counts = {}
-        for label in set(cluster_labels):
-            cluster_counts[label] = sum(
-                [contig_sizes[n] for n in cluster_to_contig[c] if node_to_label.get(n) == label]
-            )
-        if len(cluster_labels) == 0:  # we do not have labels for any of the elements of this cluster
-            continue
-        # get majority label:
-        # cluster_counter = collections.Counter(cluster_labels)
-        # cluster_majority = cluster_counter.most_common(1)
-        cluster_majority = max(cluster_counts.items(), key=operator.itemgetter(1))
-        # print(cluster_majority)
-        # if cluster_majority[0][0] not in labels_to_plot:
-        #    continue
-        if cluster_majority[0] not in label_to_node:
-            print(
-                "tie cluster",
-                f"cluster {c}, majority: {cluster_majority[0]}, cluster size {len(cluster_to_contig[c])}",
-            )
-            continue
-        # print(f"cluster {c}, majority: {cluster_majority}, cluster size {len(cluster_to_contig[c])}")
-        # print(f" {len(label_to_node.get(cluster_majority[0], []))} contigs with this label")
-        # avg_precision.append(len(cluster_to_contig) * cluster_majority[0][1]/len(cluster_to_contig[c]))
-        # avg_recall.append(len(cluster_to_contig) * cluster_majority[0][1]/len(label_to_node[cluster_majority[0][0]]))
-        cluster_size = sum([contig_sizes.get(n, 1) for n in cluster_to_contig[c]])
-        cluster_p = cluster_majority[1] / cluster_size
-        avg_precision.append(cluster_p)
-        cluster_r = cluster_majority[1] / sum([contig_sizes.get(n, 1) for n in label_to_node[cluster_majority[0]]])
-        avg_recall.append(cluster_r)
-        cluster_f1 = 2 * cluster_p * cluster_r / (cluster_p + cluster_r)
-        avg_f1.append(cluster_f1)
-        # print(cluster_p, cluster_r)
-        if outputclusters:
-            print(cluster_to_contig[c])
-        cluster_sizes.append(len(cluster_to_contig))
-    # print("average precision", sum(avg_precision)/sum(cluster_sizes)/len(avg_precision))
-    # print("average recall", sum(avg_recall)/sum(cluster_sizes)/len(avg_recall))
-    print(
-        "average precision",
-        round(sum(avg_precision) / len(avg_precision), 4),
-        "average recall",
-        round(sum(avg_recall) / len(avg_recall), 4),
-        "average f1",
-        round(sum(avg_f1) / len(avg_f1), 4),
-        "P>0.95 and R>0.9:",
-        len([i for i in range(len(avg_recall)) if avg_recall[i] >= 0.9 and avg_precision[i] >= 0.95]),
-    )
-
-
-def read_contigs_scg(ref_file, marker_file, node_names):
-    """Read marker stats and return count table
-
-    :param ref_file: path to file with reference markers (e.g. Bacteria.ms)
-    :type ref_file: str
-    :param marker_file: path to file with markers found on each contig
-    :type marker_file: str
-    :param node_names: list of node names
-    :type node_names: list
-    :return: matrix where rows are contigs, columns are markers, values are marker counts
-    :rtype: [type]
-    """
-    ref_marker_genes = read_marker_gene_sets(ref_file)
-    contigs_markers = read_contig_genes(marker_file)
-
-    # flatten ref marker gene sets
-    ref_marker_genes = [g for m in ref_marker_genes for g in m]
-    counts = []
-    for contig in node_names:
-        counts.append([contigs_markers[contig].get(g, 0) for g in ref_marker_genes])
-
-    return np.array(counts)
-
-
-def calculate_bin_metrics(results, extra_metrics=False):
-    """Calculate overall scores over a set of bins for which we already have scores
-
-    :param results: scores of each bin
-    :type results: dict
-    :param extra_metrics: Calculate more metrics, defaults to False
-    :type extra_metrics: bool, optional
-    :return: overall metrics for this bin set
-    :rtype: dict
-    """
-    hq_bins = [bin for bin in results if results[bin]["comp"] >= 90 and results[bin]["cont"] < 5]
-    mq_bins = [bin for bin in results if results[bin]["comp"] >= 50 and results[bin]["cont"] < 10]
-    metrics = {"hq": hq_bins, "mq": mq_bins, "total": results}
-    if extra_metrics and len(results) > 0:
-        metrics["avg_comp"] = sum([results[bin]["comp"] for bin in results]) / len(results)
-        metrics["avg_cont"] = sum([results[bin]["cont"] for bin in results]) / len(results)
-        cont_comp50 = [results[bin]["cont"] for bin in results if results[bin]["comp"] > 50]
-        metrics["cont_comp50"] = sum(cont_comp50) / len(cont_comp50) if len(cont_comp50) > 0 else 0
-        cont_comp90 = [results[bin]["cont"] for bin in results if results[bin]["comp"] > 90]
-        metrics["cont_comp90"] = sum(cont_comp90) / len(cont_comp90) if len(cont_comp90) > 0 else 0
-        comp_cont5 = [results[bin]["comp"] for bin in results if results[bin]["cont"] < 5]
-        metrics["comp_cont5"] = sum(comp_cont5) / len(comp_cont5) if len(comp_cont5) > 0 else 0
-    return metrics
-
-
-def cluster_eval(
-    model,
-    dataset,
-    logits,
-    clustering,
-    k,
-    loss,
-    best_hq,
-    best_hq_epoch,
-    epoch,
-    device,
-    clusteringloss=False,
-    logger=None,
-    use_marker_contigs_only=False,
-    seed=0,
-):
-    """Cluster contig embs and eval with markers
-
-    :param model: Model used to generate embs, save if better than best_hq
-    :type model: nn.Module
-    :param dataset: dataset object used to train model
-    :type dataset: ContigsDataset
-    :param logits: tensor with output of model
-    :type logits: torch.Tensor
-    :param clustering: Type of clustering to be done
-    :type clustering: str
-    :param k: Number of clusters
-    :type k: int
-    :param loss: loss (for logging)
-    :type loss: [type]
-    :param best_hq: Best HQ obtained at this point
-    :type best_hq: int
-    :param best_hq_epoch: Epoch where best HQ was obtained
-    :type best_hq_epoch: int
-    :param epoch: Current epoch
-    :type epoch: int
-    :param device: If using cuda for clustering
-    :type device: str
-    :param clusteringloss: Compute a clustering loss, defaults to False
-    :type clusteringloss: bool, optional
-    :param logger: Logger object, defaults to None
-    :type logger: [type], optional
-    :return: new best HQ and epoch, clustering loss, cluster to contig mapping
-    :rtype: list
-    """
-    import torch
-    kmeans_loss = None
-    t0_cluster = time.time()
-    model.eval()
-    #set_seed(seed)
-    if torch.is_tensor(logits):
-        embeds = logits.detach().numpy()
-    else:
-        embeds = logits
-    if use_marker_contigs_only:
-        marker_mask = [n in dataset.contig_markers and len(dataset.contig_markers[n]) > 0 for n in dataset.node_names]
-        print("clustering", sum(marker_mask), "markers", len(marker_mask))
-        cluster_embeds = embeds[marker_mask]
-        cluster_names = np.array(dataset.node_names)[marker_mask]
-    else:
-        cluster_embeds = embeds
-        cluster_names = dataset.node_names
-    cluster_to_contig, centroids = cluster_embs(
-        cluster_embeds,
-        cluster_names,
-        clustering,
-        # len(dataset.connected),
-        k,
-        device=device,
-        seed=seed,
-    )
-    contig_to_cluster = {}
-    for bin in cluster_to_contig:
-        for contig in cluster_to_contig[bin]:
-            contig_to_cluster[contig] = bin
-
-    if dataset.ref_marker_sets is not None:
-        results = evaluate_contig_sets(dataset.ref_marker_sets, dataset.contig_markers, cluster_to_contig)
-        metrics = calculate_bin_metrics(results)
-        logger.info(
-            f"HQ: {len(metrics['hq'])}, MQ:, {len(metrics['mq'])} Total bins: {len(metrics['total'])} Best HQ: {best_hq} Best HQ epoch: {best_hq_epoch}"
-        )
-        # logger.info("HQ:", hq_bins, "avg comp", avg_comp, "avg cont", avg_cont, "avg cont when comp>50", cont_comp50)
-        # logger.info(
-        #    "HQ {}, avg comp {:.2f}, avg cont {:.2f}, cont when comp>50 {:.2f}, cont when comp>90 {:.2f}, comp when cont<5 {:.2f}".format(
-        #        hq_bins, avg_comp, avg_cont, cont_comp50, cont_comp90, comp_cont5
-        #    )
-        # )
-        # print("clustering time:", time.time() - t0_cluster, embeds.shape)
-        if len(metrics["hq"]) > best_hq:
-            best_hq = len(metrics["hq"])
-            best_hq_epoch = epoch
-            logger.info("new best checkpoint, saving checkpoint to best_model_hq.pkl")
-            torch.save(model.state_dict(), os.path.join(dataset.cache_dir, "best_model_hq.pkl"))
-
-        if clusteringloss:
-            centroids = torch.tensor(centroids, device=device)
-            # get centroids of hq bins
-            # centroids = centroids[hq]
-            # get IDs of contigs of HQ bins
-            hq_node_ids = [
-                dataset.node_names.index(n)
-                for bin in metrics["hq"]
-                for n in cluster_to_contig[bin]
-                # if sum(dataset.contig_markers[n].values()) > 0
-            ]
-            # count only nodes with SCGs
-            # TODO multiply squared dist by completness of cluster
-            # cluster_comp = np.array([results[i]["comp"] / 100 for i, r in enumerate(results)])
-            # breakpoint()
-            cluster_cont = np.array([i for i, r in enumerate(results) if results[i]["cont"] > 10])
-
-            cont_node_ids = [
-                dataset.node_names.index(n)
-                for bin in cluster_cont
-                for n in cluster_to_contig[bin]
-                # if sum(dataset.contig_markers[n].values()) > 0
-            ]
-            # TODO subtract dist of contaminated bins (same num of good bins)
-            hq_logits = logits[hq_node_ids]
-            # cont_logits = logits[cont_node_ids]
-            # breakpoint()
-            # https://discuss.pytorch.org/t/k-means-loss-calculation/22041/7
-            kmeans_loss_good = ((hq_logits[:, None] - centroids[None]) ** 2).sum(2).min(1)[0].mean()
-            # kmeans_loss_bad = ((cont_logits[:, None] - centroids[None]) ** 2).sum(2).min(1)[0].mean()
-            # kmeans_loss = -kmeans_loss_bad
-            kmeans_loss = kmeans_loss_good
-            # kmeans_loss = kmeans_loss_good - kmeans_loss_bad
-            # kmeans_loss = ((logits[:, None] - centroids[None]) ** 2).sum(2).min(1)[0].mean()
-            logger.info(
-                f"Kmeans loss: {kmeans_loss.item()} on {len(hq_logits)} points {len(centroids)} total clusters",
-            )
-            # loss = kmeans_loss * alpha + (1 - alpha) * loss
-    logger.info(
-        "Epoch {:05d} | Best HQ: {} | Best epoch {} | Total loss {:.4f}".format(
-            epoch,
-            best_hq,
-            best_hq_epoch,
-            loss.detach(),
-        )
-    )
-    return best_hq, best_hq_epoch, kmeans_loss, cluster_to_contig, metrics
-
-
-def compute_loss_para(adj, device):
-    pos_weight = (adj.shape[0] * adj.shape[0] - adj.sum()) / adj.sum()
-    norm = adj.shape[0] * adj.shape[0] / float((adj.shape[0] * adj.shape[0] - adj.sum()) * 2)
-    weight_mask = adj.view(-1) == 1
-    weight_tensor = torch.ones(weight_mask.size(0)).to(device)
-    weight_tensor[weight_mask] = pos_weight
-    return weight_tensor, norm
+
+import time
+import os
+import networkx as nx
+import numpy as np
+import operator
+
+#import tensorflow
+
+from graphmb.evaluate import read_contig_genes, read_marker_gene_sets, evaluate_contig_sets
+from graphmb.contigsdataset import get_kmer_to_id, count_kmers
+from graphmb.utils import SEED
+# import torch
+
+def open_gfa_file(filename, filter=1000, root=False, kmer=4):
+    G = nx.Graph()
+    if root:
+        root_node = G.add_node("root", length=0)
+    skipped_contigs = set()
+    skipped_edges = set()
+    kmer_to_id, canonical_k = get_kmer_to_id(kmer)
+    with open(filename, "r") as f:
+        for line in f:
+            if line.startswith("S"):
+                values = line.strip().split()
+                contigid = values[1]
+                # contiglen = int(values[3].split(":")[-1])
+                contiglen = len(values[2])
+                contig_kmers = count_kmers(values[2], kmer, kmer_to_id, canonical_k)
+                if contiglen < filter:
+                    skipped_contigs.add(contigid)
+                else:
+
+                    G.add_node(contigid, length=contiglen, kmers=contig_kmers)  # TODO: add coverage and kmer too
+                    if root:
+                        G.add_edge(contigid, "root")
+            if line.startswith("L"):
+                values = line.strip().split()
+                if values[1] in skipped_contigs or values[3] in skipped_contigs:
+                    skipped_edges.add((values[1], values[3]))
+                    continue
+                G.add_edge(values[1], values[3])
+
+    print("load graph from GFA")
+    print("skipped these contigs {} (len<{})".format(len(skipped_contigs), filter))
+    print("skipped these edges {} (len<{})".format(len(skipped_edges), filter))
+    return G
+
+
+def cluster_embs(node_embeddings, node_ids, clusteringalgo, kclusters, device="cpu", node_lens=None, seed=0):
+    #set_seed(seed)
+    if clusteringalgo == "vamb":
+        from vamb.cluster import cluster as vamb_cluster
+        it = vamb_cluster(
+            node_embeddings, node_ids, cuda=(device == "cuda:0")
+        )  # , seeds=seeds)  # contig_lens=node_lens)  #
+        cluster_to_contig = {i: c for (i, (n, c)) in enumerate(it)}
+
+        # get embs to clusters (cluster to contig has only contig names, not index)
+        """cluster_to_embs = {
+            c: np.array([node_embeddings[i] for i, n in enumerate(node_ids) if n in cluster_to_contig[c]])
+            for c in cluster_to_contig
+        }
+        cluster_centroids = np.array([cluster_to_embs[c].mean(0) for c in cluster_to_contig])"""
+        cluster_centroids = None  # not necessary for now
+    else:
+        from sklearn.cluster import (
+            KMeans,
+            DBSCAN,
+            AgglomerativeClustering,
+            MiniBatchKMeans,
+            SpectralClustering,
+            Birch,
+            OPTICS,
+        )
+        from sklearn.mixture import GaussianMixture
+
+        if clusteringalgo == "kmeans":
+            clustering = KMeans(n_clusters=kclusters, random_state=SEED)
+            cluster_labels = clustering.fit_predict(node_embeddings)
+            cluster_centroids = clustering.cluster_centers_
+        elif clusteringalgo == "kmeansgpu":
+            node_embeddings = torch.tensor(node_embeddings).cuda()
+            cluster_labels, cluster_centroids = kmeans_pytorch.kmeans(
+                X=node_embeddings, num_clusters=kclusters, device=torch.device("cuda:0")
+            )
+        elif clusteringalgo == "dbscan":
+            cluster_labels = DBSCAN(eps=1.1, min_samples=5).fit_predict(node_embeddings)
+            # cluster_centroids = clustering.cluster_centers_
+            cluster_centroids = None
+        elif clusteringalgo == "gmm":
+            cluster_model = GaussianMixture(
+                n_components=kclusters,
+                covariance_type="full",
+                max_iter=1000,
+                random_state=SEED,
+                verbose=2,
+                verbose_interval=1,
+            ).fit(node_embeddings)
+            cluster_labels = cluster_model.predict(node_embeddings)
+            cluster_centroids = cluster_model.means_
+        elif clusteringalgo == "kmeansconst":
+            cluster_labels = KMeansConstrained(
+                n_clusters=kclusters, size_min=1, size_max=5, random_state=SEED
+            ).fit_predict(node_embeddings)
+        elif clusteringalgo == "kmeansbatch":
+            kmeans = MiniBatchKMeans(n_clusters=kclusters, random_state=SEED, batch_size=100, init=seed_matrix)
+            cluster_labels = kmeans.fit_predict(node_embeddings)
+            cluster_centroids = kmeans.cluster_centers_
+        elif clusteringalgo == "spectral":
+            cluster_labels = SpectralClustering(n_clusters=kclusters, random_state=SEED).fit_predict(node_embeddings)
+            cluster_centroids = None
+        elif clusteringalgo == "birch":
+            cluster_labels = Birch(n_clusters=kclusters).fit_predict(node_embeddings)
+            cluster_centroids = None
+        elif clusteringalgo == "optics":
+            cluster_labels = OPTICS(min_samples=5, cluster_method="xi", n_jobs=-1).fit_predict(node_embeddings)
+            cluster_centroids = None
+        else:
+            print("invalid clustering algorithm")
+            return None
+        # compare clustering labels with actual labels
+        # for each cluster, get majority label, and then P/R
+        cluster_to_contig = {i: [] for i in range(kclusters)}
+        for il, l in enumerate(cluster_labels):
+            # if l not in cluster_to_contig:
+            #    cluster_to_contig[l] = []
+            cluster_to_contig[l].append(node_ids[il])
+
+    return cluster_to_contig, cluster_centroids
+
+
+def evaluate_binning(cluster_to_contig, node_to_label, label_to_node, outputclusters=False, contig_sizes=None):
+    """Evaluate binning results using contig labels (supervised scenario)
+
+    :param cluster_to_contig: mapping cluster IDs to contig names
+    :type cluster_to_contig: dict
+    :param node_to_label: mapping contig ids to labels (taxon)
+    :type node_to_label: dict
+    :param label_to_node: mapping label names to cotnigs
+    :type label_to_node: dict
+    :param outputclusters: print members of all clusters, defaults to False
+    :type outputclusters: bool, optional
+    :param contig_sizes: Provide contig sizes for balanced scores, defaults to None
+    :type contig_sizes: dict, optional
+    """
+    # uncomment if you want to plot only the biggest labels
+    # labels_to_plot = sorted(label_to_node, key = lambda key: len(label_to_node.get(key, [])), reverse=True)[:6]
+    # print(labels_to_plot)
+    avg_precision = []
+    avg_recall = []
+    avg_f1 = []
+    cluster_sizes = []
+    if contig_sizes is None:
+        contig_sizes = {c: 1 for c in node_to_label}
+    for c in cluster_to_contig:
+        cluster_labels = [node_to_label.get(n) for n in cluster_to_contig[c] if n in node_to_label]
+        cluster_counts = {}
+        for label in set(cluster_labels):
+            cluster_counts[label] = sum(
+                [contig_sizes[n] for n in cluster_to_contig[c] if node_to_label.get(n) == label]
+            )
+        if len(cluster_labels) == 0:  # we do not have labels for any of the elements of this cluster
+            continue
+        # get majority label:
+        # cluster_counter = collections.Counter(cluster_labels)
+        # cluster_majority = cluster_counter.most_common(1)
+        cluster_majority = max(cluster_counts.items(), key=operator.itemgetter(1))
+        # print(cluster_majority)
+        # if cluster_majority[0][0] not in labels_to_plot:
+        #    continue
+        if cluster_majority[0] not in label_to_node:
+            print(
+                "tie cluster",
+                f"cluster {c}, majority: {cluster_majority[0]}, cluster size {len(cluster_to_contig[c])}",
+            )
+            continue
+        # print(f"cluster {c}, majority: {cluster_majority}, cluster size {len(cluster_to_contig[c])}")
+        # print(f" {len(label_to_node.get(cluster_majority[0], []))} contigs with this label")
+        # avg_precision.append(len(cluster_to_contig) * cluster_majority[0][1]/len(cluster_to_contig[c]))
+        # avg_recall.append(len(cluster_to_contig) * cluster_majority[0][1]/len(label_to_node[cluster_majority[0][0]]))
+        cluster_size = sum([contig_sizes.get(n, 1) for n in cluster_to_contig[c]])
+        cluster_p = cluster_majority[1] / cluster_size
+        avg_precision.append(cluster_p)
+        cluster_r = cluster_majority[1] / sum([contig_sizes.get(n, 1) for n in label_to_node[cluster_majority[0]]])
+        avg_recall.append(cluster_r)
+        cluster_f1 = 2 * cluster_p * cluster_r / (cluster_p + cluster_r)
+        avg_f1.append(cluster_f1)
+        # print(cluster_p, cluster_r)
+        if outputclusters:
+            print(cluster_to_contig[c])
+        cluster_sizes.append(len(cluster_to_contig))
+    # print("average precision", sum(avg_precision)/sum(cluster_sizes)/len(avg_precision))
+    # print("average recall", sum(avg_recall)/sum(cluster_sizes)/len(avg_recall))
+    print(
+        "average precision",
+        round(sum(avg_precision) / len(avg_precision), 4),
+        "average recall",
+        round(sum(avg_recall) / len(avg_recall), 4),
+        "average f1",
+        round(sum(avg_f1) / len(avg_f1), 4),
+        "P>0.95 and R>0.9:",
+        len([i for i in range(len(avg_recall)) if avg_recall[i] >= 0.9 and avg_precision[i] >= 0.95]),
+    )
+
+
+def read_contigs_scg(ref_file, marker_file, node_names):
+    """Read marker stats and return count table
+
+    :param ref_file: path to file with reference markers (e.g. Bacteria.ms)
+    :type ref_file: str
+    :param marker_file: path to file with markers found on each contig
+    :type marker_file: str
+    :param node_names: list of node names
+    :type node_names: list
+    :return: matrix where rows are contigs, columns are markers, values are marker counts
+    :rtype: [type]
+    """
+    ref_marker_genes = read_marker_gene_sets(ref_file)
+    contigs_markers = read_contig_genes(marker_file)
+
+    # flatten ref marker gene sets
+    ref_marker_genes = [g for m in ref_marker_genes for g in m]
+    counts = []
+    for contig in node_names:
+        counts.append([contigs_markers[contig].get(g, 0) for g in ref_marker_genes])
+
+    return np.array(counts)
+
+
+def calculate_bin_metrics(results, extra_metrics=False):
+    """Calculate overall scores over a set of bins for which we already have scores
+
+    :param results: scores of each bin
+    :type results: dict
+    :param extra_metrics: Calculate more metrics, defaults to False
+    :type extra_metrics: bool, optional
+    :return: overall metrics for this bin set
+    :rtype: dict
+    """
+    hq_bins = [bin for bin in results if results[bin]["comp"] >= 90 and results[bin]["cont"] < 5]
+    mq_bins = [bin for bin in results if results[bin]["comp"] >= 50 and results[bin]["cont"] < 10]
+    metrics = {"hq": hq_bins, "mq": mq_bins, "total": results}
+    if extra_metrics and len(results) > 0:
+        metrics["avg_comp"] = sum([results[bin]["comp"] for bin in results]) / len(results)
+        metrics["avg_cont"] = sum([results[bin]["cont"] for bin in results]) / len(results)
+        cont_comp50 = [results[bin]["cont"] for bin in results if results[bin]["comp"] > 50]
+        metrics["cont_comp50"] = sum(cont_comp50) / len(cont_comp50) if len(cont_comp50) > 0 else 0
+        cont_comp90 = [results[bin]["cont"] for bin in results if results[bin]["comp"] > 90]
+        metrics["cont_comp90"] = sum(cont_comp90) / len(cont_comp90) if len(cont_comp90) > 0 else 0
+        comp_cont5 = [results[bin]["comp"] for bin in results if results[bin]["cont"] < 5]
+        metrics["comp_cont5"] = sum(comp_cont5) / len(comp_cont5) if len(comp_cont5) > 0 else 0
+    return metrics
+
+
+def cluster_eval(
+    model,
+    dataset,
+    logits,
+    clustering,
+    k,
+    loss,
+    best_hq,
+    best_hq_epoch,
+    epoch,
+    device,
+    clusteringloss=False,
+    logger=None,
+    use_marker_contigs_only=False,
+    seed=0,
+):
+    """Cluster contig embs and eval with markers
+
+    :param model: Model used to generate embs, save if better than best_hq
+    :type model: nn.Module
+    :param dataset: dataset object used to train model
+    :type dataset: ContigsDataset
+    :param logits: tensor with output of model
+    :type logits: torch.Tensor
+    :param clustering: Type of clustering to be done
+    :type clustering: str
+    :param k: Number of clusters
+    :type k: int
+    :param loss: loss (for logging)
+    :type loss: [type]
+    :param best_hq: Best HQ obtained at this point
+    :type best_hq: int
+    :param best_hq_epoch: Epoch where best HQ was obtained
+    :type best_hq_epoch: int
+    :param epoch: Current epoch
+    :type epoch: int
+    :param device: If using cuda for clustering
+    :type device: str
+    :param clusteringloss: Compute a clustering loss, defaults to False
+    :type clusteringloss: bool, optional
+    :param logger: Logger object, defaults to None
+    :type logger: [type], optional
+    :return: new best HQ and epoch, clustering loss, cluster to contig mapping
+    :rtype: list
+    """
+    import torch
+    kmeans_loss = None
+    t0_cluster = time.time()
+    model.eval()
+    #set_seed(seed)
+    if torch.is_tensor(logits):
+        embeds = logits.detach().numpy()
+    else:
+        embeds = logits
+    if use_marker_contigs_only:
+        marker_mask = [n in dataset.contig_markers and len(dataset.contig_markers[n]) > 0 for n in dataset.node_names]
+        print("clustering", sum(marker_mask), "markers", len(marker_mask))
+        cluster_embeds = embeds[marker_mask]
+        cluster_names = np.array(dataset.node_names)[marker_mask]
+    else:
+        cluster_embeds = embeds
+        cluster_names = dataset.node_names
+    cluster_to_contig, centroids = cluster_embs(
+        cluster_embeds,
+        cluster_names,
+        clustering,
+        # len(dataset.connected),
+        k,
+        device=device,
+        seed=seed,
+    )
+    contig_to_cluster = {}
+    for bin in cluster_to_contig:
+        for contig in cluster_to_contig[bin]:
+            contig_to_cluster[contig] = bin
+
+    if dataset.ref_marker_sets is not None:
+        results = evaluate_contig_sets(dataset.ref_marker_sets, dataset.contig_markers, cluster_to_contig)
+        metrics = calculate_bin_metrics(results)
+        logger.info(
+            f"HQ: {len(metrics['hq'])}, MQ:, {len(metrics['mq'])} Total bins: {len(metrics['total'])} Best HQ: {best_hq} Best HQ epoch: {best_hq_epoch}"
+        )
+        # logger.info("HQ:", hq_bins, "avg comp", avg_comp, "avg cont", avg_cont, "avg cont when comp>50", cont_comp50)
+        # logger.info(
+        #    "HQ {}, avg comp {:.2f}, avg cont {:.2f}, cont when comp>50 {:.2f}, cont when comp>90 {:.2f}, comp when cont<5 {:.2f}".format(
+        #        hq_bins, avg_comp, avg_cont, cont_comp50, cont_comp90, comp_cont5
+        #    )
+        # )
+        # print("clustering time:", time.time() - t0_cluster, embeds.shape)
+        if len(metrics["hq"]) > best_hq:
+            best_hq = len(metrics["hq"])
+            best_hq_epoch = epoch
+            logger.info("new best checkpoint, saving checkpoint to best_model_hq.pkl")
+            torch.save(model.state_dict(), os.path.join(dataset.cache_dir, "best_model_hq.pkl"))
+
+        if clusteringloss:
+            centroids = torch.tensor(centroids, device=device)
+            # get centroids of hq bins
+            # centroids = centroids[hq]
+            # get IDs of contigs of HQ bins
+            hq_node_ids = [
+                dataset.node_names.index(n)
+                for bin in metrics["hq"]
+                for n in cluster_to_contig[bin]
+                # if sum(dataset.contig_markers[n].values()) > 0
+            ]
+            # count only nodes with SCGs
+            # TODO multiply squared dist by completness of cluster
+            # cluster_comp = np.array([results[i]["comp"] / 100 for i, r in enumerate(results)])
+            # breakpoint()
+            cluster_cont = np.array([i for i, r in enumerate(results) if results[i]["cont"] > 10])
+
+            cont_node_ids = [
+                dataset.node_names.index(n)
+                for bin in cluster_cont
+                for n in cluster_to_contig[bin]
+                # if sum(dataset.contig_markers[n].values()) > 0
+            ]
+            # TODO subtract dist of contaminated bins (same num of good bins)
+            hq_logits = logits[hq_node_ids]
+            # cont_logits = logits[cont_node_ids]
+            # breakpoint()
+            # https://discuss.pytorch.org/t/k-means-loss-calculation/22041/7
+            kmeans_loss_good = ((hq_logits[:, None] - centroids[None]) ** 2).sum(2).min(1)[0].mean()
+            # kmeans_loss_bad = ((cont_logits[:, None] - centroids[None]) ** 2).sum(2).min(1)[0].mean()
+            # kmeans_loss = -kmeans_loss_bad
+            kmeans_loss = kmeans_loss_good
+            # kmeans_loss = kmeans_loss_good - kmeans_loss_bad
+            # kmeans_loss = ((logits[:, None] - centroids[None]) ** 2).sum(2).min(1)[0].mean()
+            logger.info(
+                f"Kmeans loss: {kmeans_loss.item()} on {len(hq_logits)} points {len(centroids)} total clusters",
+            )
+            # loss = kmeans_loss * alpha + (1 - alpha) * loss
+    logger.info(
+        "Epoch {:05d} | Best HQ: {} | Best epoch {} | Total loss {:.4f}".format(
+            epoch,
+            best_hq,
+            best_hq_epoch,
+            loss.detach(),
+        )
+    )
+    return best_hq, best_hq_epoch, kmeans_loss, cluster_to_contig, metrics
+
+
+def compute_loss_para(adj, device):
+    pos_weight = (adj.shape[0] * adj.shape[0] - adj.sum()) / adj.sum()
+    norm = adj.shape[0] * adj.shape[0] / float((adj.shape[0] * adj.shape[0] - adj.sum()) * 2)
+    weight_mask = adj.view(-1) == 1
+    weight_tensor = torch.ones(weight_mask.size(0)).to(device)
+    weight_tensor[weight_mask] = pos_weight
+    return weight_tensor, norm
```

### Comparing `graphmb-0.2.4/src/graphmb/graphsage_unsupervised.py` & `graphmb-0.2.5/src/graphmb/graphsage_unsupervised.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,376 +1,376 @@
-import time
-import pdb
-import os
-import random
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-import torch.optim as optim
-import dgl
-from dgl.nn.pytorch.conv import SAGEConv, GATConv
-import dgl.function as fn
-import tqdm
-import numpy as np
-import copy
-import sklearn
-
-from graphmb.utils import set_seed
-from graphmb.graphmb1 import cluster_eval
-
-# Based on this implemention: https://github.com/dmlc/dgl/blob/master/examples/pytorch/graphsage/train_sampling_unsupervised.py
-
-
-class MultiLayerNeighborWeightedSampler(dgl.dataloading.MultiLayerNeighborSampler):
-    def sample_frontier(self, block_id, g, seed_nodes):
-        fanout = self.fanouts[block_id]
-        frontier = dgl.sampling.sample_neighbors(g, seed_nodes, fanout, replace=self.replace, prob="weight")
-        return frontier
-
-
-class NegativeSampler(object):
-    def __init__(self, g, k, neg_share=False):
-        self.weights = g.in_degrees().float() ** 0.75
-        self.k = k
-        self.neg_share = neg_share
-
-    def __call__(self, g, eids):
-        src, _ = g.find_edges(eids)
-        n = len(src)
-        if self.neg_share and n % self.k == 0:
-            dst = self.weights.multinomial(n, replacement=True)
-            dst = dst.view(-1, 1, self.k).expand(-1, self.k, -1).flatten()
-        else:
-            dst = self.weights.multinomial(n * self.k, replacement=True)
-        src = src.repeat_interleave(self.k)
-        return src, dst
-
-
-class NegativeSamplerWeight(object):
-    """Samples negatives according to the inverse of edge weight"""
-
-    def __init__(self, g, k, neg_share=False):
-        self.k = k
-        self.neg_share = neg_share
-
-    def __call__(self, g, eids):
-        src, dst = g.find_edges(eids)
-        new_dst = []
-        new_src = []
-        possible_dst = set(dst)
-        new_src = [src_node for src_node in src if len(g.out_edges(src_node)[1]) < 2]
-        new_dst = random.sample(possible_dst, k=len(new_src))
-        # print("adding", len(new_src), "more edges")
-        src = src.repeat_interleave(self.k)
-        expand_g = dgl.remove_self_loop(dgl.add_edges(g, new_src, new_dst))
-        expand_g.edata["weight"] = 1 / expand_g.edata["weight"]
-
-        samples_edges = dgl.sampling.sample_neighbors(
-            expand_g, src, self.k, prob="weight", replace=True, edge_dir="out"
-        )
-        src = samples_edges.edges()[0]
-        dst = samples_edges.edges()[1]
-        # src = src.repeat_interleave(self.k)
-        return src, dst
-
-
-class CrossEntropyLoss(nn.Module):
-    def forward(self, block_outputs, pos_graph, neg_graph, weights=True):
-        with pos_graph.local_scope():
-            pos_graph.ndata["h"] = block_outputs
-            pos_graph.apply_edges(fn.u_dot_v("h", "h", "score"))
-            pos_score = pos_graph.edata["score"]
-        with neg_graph.local_scope():
-            neg_graph.ndata["h"] = block_outputs
-            neg_graph.apply_edges(fn.u_dot_v("h", "h", "score"))
-            neg_score = neg_graph.edata["score"]
-
-        score = torch.cat([pos_score, neg_score])
-        pos_label = torch.ones_like(pos_score)
-        if weights:
-            pos_weights = pos_graph.edata["weight"] / max(pos_graph.edata["weight"])
-            pos_weights = pos_weights.unsqueeze(-1)
-        else:
-            pos_weights = torch.ones_like(pos_score)
-        neg_label = torch.zeros_like(neg_score)
-        neg_weights = torch.ones_like(neg_score)
-        all_weights = torch.cat([pos_weights, neg_weights])
-        label = torch.cat([pos_label, neg_label]).long()
-        loss = F.binary_cross_entropy_with_logits(score, label.float(), weight=all_weights)
-        return loss
-
-
-class SAGE(nn.Module):
-    def __init__(self, in_feats, n_hidden, n_classes, n_layers, activation, dropout, agg="mean"):
-        super().__init__()
-        self.init(in_feats, n_hidden, n_classes, n_layers, activation, dropout, agg)
-
-    def init(self, in_feats, n_hidden, n_classes, n_layers, activation, dropout, agg):
-        self.n_layers = n_layers
-        self.n_hidden = n_hidden
-        self.n_classes = n_classes
-        self.layers = nn.ModuleList()
-        # self.batchnorm = nn.BatchNorm1d(n_hidden)
-        if n_layers > 1:
-            self.layers.append(SAGEConv(in_feats, n_hidden, agg, feat_drop=dropout))
-
-            for i in range(1, n_layers - 1):
-                self.layers.append(SAGEConv(n_hidden, n_hidden, agg, feat_drop=dropout))
-                # self.layers.append(nn.BatchNorm1d(n_hidden))
-            self.layers.append(SAGEConv(n_hidden, n_classes, agg))
-        else:
-            self.layers.append(SAGEConv(in_feats, n_classes, agg, feat_drop=dropout))
-        if agg == "gcn":
-            breakpoint()
-        self.dropout = nn.Dropout(dropout)
-        self.activation = activation
-
-    def forward(self, blocks, x, edge_weight=None):
-        h = x
-        for il, (layer, block) in enumerate(zip(self.layers, blocks)):
-            # weights = F.softmax(block.edata["weight"])
-            # weights = block.edata["weight"] / max(block.edata["weight"])
-            # h = layer(block, h, edge_weight=weights)
-            h = layer(block, h)
-            if il != len(self.layers) - 1:
-                h = self.activation(h)
-        return h
-
-    def inference(self, g, x, device, batch_size, num_workers, use_weights=False):
-        """
-        Inference with the GraphSAGE model on full neighbors (i.e. without neighbor sampling).
-        g : the entire graph.
-        x : the input of entire node set.
-        The inference code is written in a fashion that it could handle any number of nodes and
-        layers.
-        """
-        # During inference with sampling, multi-layer blocks are very inefficient because
-        # lots of computations in the first few layers are repeated.
-        # Therefore, we compute the representation of all nodes layer by layer.  The nodes
-        # on each layer are of course splitted in batches.
-        # TODO: can we standardize this?
-        for il, layer in enumerate(self.layers):
-            y = torch.zeros(g.num_nodes(), self.n_hidden if il != len(self.layers) - 1 else self.n_classes)
-            sampler = dgl.dataloading.MultiLayerFullNeighborSampler(1)
-            
-            dataloader = dgl.dataloading.NodeDataLoader(
-                g,
-                torch.arange(g.num_nodes()).to(g.device),
-                sampler,
-                batch_size=batch_size,
-                shuffle=False,
-                drop_last=False,
-                num_workers=num_workers,
-            )
-
-            for input_nodes, output_nodes, blocks in dataloader:
-                block = blocks[0]
-
-                block = block.int().to(device)
-                h = x[input_nodes].to(device)
-
-                if use_weights:
-                    weights = block.edata["weight"] / max(block.edata["weight"])
-                    h = layer(block, h, edge_weight=weights)
-                else:
-                    h = layer(block, h)
-                if il != len(self.layers) - 1:
-                    h = self.activation(h)
-                    h = self.dropout(h)
-
-                y[output_nodes] = h.cpu()
-
-            x = y
-        return y
-
-
-def train_graphsage(
-    dataset,
-    model,
-    batch_size,
-    fan_out,
-    num_negs,
-    neg_share,
-    lr,
-    num_epochs,
-    num_workers=0,
-    print_interval=3,
-    device="cpu",
-    cluster_features=True,
-    clusteringalgo="kmeans",
-    k=1,
-    logger=None,
-    loss_weights=False,
-    sample_weights=False,
-    epsilon=0.1,
-    evalepochs=1,
-    seed=0,
-    eval_skip=0,
-    quick=False
-):
-    train_start_time = time.time()
-    nfeat = dataset.graph.ndata.pop("feat")
-    model = model.to(device)
-    # Create PyTorch DataLoader for constructing blocks
-    n_edges = dataset.graph.num_edges()
-    train_seeds = torch.arange(n_edges)
-    set_seed(seed)
-
-    # Create samplers
-    if not sample_weights:
-        neg_sampler = NegativeSampler(dataset.graph, num_negs, neg_share)
-        sampler = dgl.dataloading.MultiLayerNeighborSampler([int(fanout) for fanout in fan_out.split(",")])
-    else:
-        neg_sampler = NegativeSamplerWeight(dataset.graph, num_negs, neg_share)
-        sampler = MultiLayerNeighborWeightedSampler([int(fanout) for fanout in fan_out.split(",")])
-
-    if batch_size == 0:
-        batch_size = len(train_seeds)
-    dataloader = dgl.dataloading.EdgeDataLoader(
-        dataset.graph,
-        train_seeds,
-        sampler,
-        exclude="reverse_id",
-        reverse_eids=torch.cat([torch.arange(n_edges // 2, n_edges), torch.arange(0, n_edges // 2)]).to(train_seeds),
-        negative_sampler=neg_sampler,
-        device=device,
-        batch_size=batch_size,
-        shuffle=True,
-        drop_last=True,
-        num_workers=num_workers,
-    )
-
-    loss_fcn = CrossEntropyLoss()
-    optimizer_sage = optim.Adam(model.parameters(), lr=lr)
-    # Training loop
-    avg = 0
-    iter_pos = []
-    iter_neg = []
-    iter_d = []
-    iter_t = []
-    best_hq = 0
-    best_hq_epoch = 0
-    total_steps = 0
-    losses = []
-    stop_run = False
-    for epoch in range(num_epochs):
-        tic = time.time()
-        # Loop over the dataloader to sample the computation dependency graph as a list of
-        # blocks.
-        tic_step = time.time()
-        for step, (input_nodes, pos_graph, neg_graph, blocks) in enumerate(dataloader):
-            batch_inputs = nfeat[input_nodes].to(device)
-            d_step = time.time()
-            #set_seed(seed)
-            model.train()
-            pos_graph = pos_graph.to(device)
-            neg_graph = neg_graph.to(device)
-            blocks = [block.int().to(device) for block in blocks]
-            # Compute loss and prediction
-            batch_pred = model(blocks, batch_inputs)
-            loss = loss_fcn(batch_pred, pos_graph, neg_graph, weights=loss_weights)
-
-            optimizer_sage.zero_grad()
-            loss.backward()
-            optimizer_sage.step()
-
-            t = time.time()
-            pos_edges = pos_graph.num_edges()
-            neg_edges = neg_graph.num_edges()
-            iter_pos.append(pos_edges / (t - tic_step))
-            iter_neg.append(neg_edges / (t - tic_step))
-            iter_d.append(d_step - tic_step)
-            iter_t.append(t - d_step)
-            if total_steps % print_interval == 0:
-                gpu_mem_alloc = torch.cuda.max_memory_allocated() / 1000000 if torch.cuda.is_available() else 0
-                logger.info(
-                    "Epoch {:05d} | Step {:05d} | N samples {} | Loss {:.4f} | Speed (samples/sec) {:.4f}|{:.4f} | Load {:.4f}| train {:.4f} | GPU {:.1f} MB".format(
-                        epoch,
-                        step,
-                        len(input_nodes),
-                        loss.item(),
-                        np.mean(iter_pos[3:]),
-                        np.mean(iter_neg[3:]),
-                        np.mean(iter_d[3:]),
-                        np.mean(iter_t[3:]),
-                        gpu_mem_alloc,
-                    )
-                )
-            tic_step = time.time()
-            total_steps += 1
-
-        losses.append(loss.item())
-        # early stopping
-        if (
-            epsilon is not None
-            and len(losses) > 3
-            and (losses[-2] - losses[-1]) < epsilon
-            and (losses[-3] - losses[-2]) < epsilon
-        ):
-            logger.info("Early stopping {}".format(str(losses[-5:])))
-            stop_run = True
-
-        if dataset.assembly.ref_marker_sets is not None and ((epoch % evalepochs == 0 and epoch > eval_skip) or stop_run):
-            model.eval()
-            encoded = model.inference(dataset.graph, nfeat, device, batch_size, num_workers)
-            if cluster_features:
-                encoded = torch.cat((encoded, nfeat), axis=1)
-            best_hq, best_hq_epoch, kmeans_loss, clusters, epoch_metrics = cluster_eval(
-                model=model,
-                dataset=dataset.assembly,
-                logits=encoded,
-                clustering=clusteringalgo,
-                k=k,
-                loss=loss,
-                best_hq=best_hq,
-                best_hq_epoch=best_hq_epoch,
-                epoch=epoch,
-                device=device,
-                clusteringloss=False,
-                logger=logger,
-                use_marker_contigs_only=quick,
-                seed=seed,
-            )
-            if best_hq_epoch == epoch:
-                metrics = epoch_metrics
-            # compare clusters
-            new_assignments = np.zeros(len(dataset.assembly.node_names))
-            for i, cluster in enumerate(clusters):
-                for contig in clusters[cluster]:
-                    new_assignments[dataset.assembly.node_names.index(contig)] = i
-
-            old_assignments = new_assignments.copy()
-        toc = time.time()
-        if epoch >= 5:
-            avg += toc - tic
-        if stop_run:
-            break
-        # = encoded.cpu().detach().numpy()
-
-    last_train_embs = encoded
-    last_model = model
-    logger.info("saving last model")
-    torch.save(last_model.state_dict(), os.path.join(dataset.assembly.cache_dir, "last_model_hq.pkl"))
-    logger.info("Avg epoch time: {}".format(avg / (epoch - 4)))
-    logger.info("Total training time: {:.3f} seconds".format(time.time() - train_start_time))
-    logger.info("Peak memory usage: {} MB".format(torch.cuda.max_memory_allocated()/1000000))
-    model.eval()
-    logger.info(f"Best HQ {best_hq} epoch, {best_hq_epoch}")
-    if total_steps == 0:
-        print("No training was done")
-    elif dataset.assembly.ref_marker_sets is not None:
-        logger.info("loading best model")
-        best_model = copy.deepcopy(model)
-        try:
-            best_model.load_state_dict(torch.load(os.path.join(dataset.assembly.cache_dir, "best_model_hq.pkl")))
-        except RuntimeError:
-            pdb.set_trace()
-    else:
-        best_model = last_model
-    set_seed(seed)
-    print("running best or last model again")
-    best_train_embs = best_model.inference(dataset.graph, nfeat, device, batch_size, num_workers)
-
-    best_train_embs = best_train_embs.detach()
-    if cluster_features:
-        best_train_embs = torch.cat((best_train_embs, nfeat), axis=1).detach()
-    return best_train_embs, best_model, last_train_embs, last_model, metrics
+import time
+import pdb
+import os
+import random
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+import torch.optim as optim
+import dgl
+from dgl.nn.pytorch.conv import SAGEConv, GATConv
+import dgl.function as fn
+import tqdm
+import numpy as np
+import copy
+import sklearn
+
+from graphmb.utils import set_seed
+from graphmb.graphmb1 import cluster_eval
+
+# Based on this implemention: https://github.com/dmlc/dgl/blob/master/examples/pytorch/graphsage/train_sampling_unsupervised.py
+
+
+class MultiLayerNeighborWeightedSampler(dgl.dataloading.MultiLayerNeighborSampler):
+    def sample_frontier(self, block_id, g, seed_nodes):
+        fanout = self.fanouts[block_id]
+        frontier = dgl.sampling.sample_neighbors(g, seed_nodes, fanout, replace=self.replace, prob="weight")
+        return frontier
+
+
+class NegativeSampler(object):
+    def __init__(self, g, k, neg_share=False):
+        self.weights = g.in_degrees().float() ** 0.75
+        self.k = k
+        self.neg_share = neg_share
+
+    def __call__(self, g, eids):
+        src, _ = g.find_edges(eids)
+        n = len(src)
+        if self.neg_share and n % self.k == 0:
+            dst = self.weights.multinomial(n, replacement=True)
+            dst = dst.view(-1, 1, self.k).expand(-1, self.k, -1).flatten()
+        else:
+            dst = self.weights.multinomial(n * self.k, replacement=True)
+        src = src.repeat_interleave(self.k)
+        return src, dst
+
+
+class NegativeSamplerWeight(object):
+    """Samples negatives according to the inverse of edge weight"""
+
+    def __init__(self, g, k, neg_share=False):
+        self.k = k
+        self.neg_share = neg_share
+
+    def __call__(self, g, eids):
+        src, dst = g.find_edges(eids)
+        new_dst = []
+        new_src = []
+        possible_dst = set(dst)
+        new_src = [src_node for src_node in src if len(g.out_edges(src_node)[1]) < 2]
+        new_dst = random.sample(possible_dst, k=len(new_src))
+        # print("adding", len(new_src), "more edges")
+        src = src.repeat_interleave(self.k)
+        expand_g = dgl.remove_self_loop(dgl.add_edges(g, new_src, new_dst))
+        expand_g.edata["weight"] = 1 / expand_g.edata["weight"]
+
+        samples_edges = dgl.sampling.sample_neighbors(
+            expand_g, src, self.k, prob="weight", replace=True, edge_dir="out"
+        )
+        src = samples_edges.edges()[0]
+        dst = samples_edges.edges()[1]
+        # src = src.repeat_interleave(self.k)
+        return src, dst
+
+
+class CrossEntropyLoss(nn.Module):
+    def forward(self, block_outputs, pos_graph, neg_graph, weights=True):
+        with pos_graph.local_scope():
+            pos_graph.ndata["h"] = block_outputs
+            pos_graph.apply_edges(fn.u_dot_v("h", "h", "score"))
+            pos_score = pos_graph.edata["score"]
+        with neg_graph.local_scope():
+            neg_graph.ndata["h"] = block_outputs
+            neg_graph.apply_edges(fn.u_dot_v("h", "h", "score"))
+            neg_score = neg_graph.edata["score"]
+
+        score = torch.cat([pos_score, neg_score])
+        pos_label = torch.ones_like(pos_score)
+        if weights:
+            pos_weights = pos_graph.edata["weight"] / max(pos_graph.edata["weight"])
+            pos_weights = pos_weights.unsqueeze(-1)
+        else:
+            pos_weights = torch.ones_like(pos_score)
+        neg_label = torch.zeros_like(neg_score)
+        neg_weights = torch.ones_like(neg_score)
+        all_weights = torch.cat([pos_weights, neg_weights])
+        label = torch.cat([pos_label, neg_label]).long()
+        loss = F.binary_cross_entropy_with_logits(score, label.float(), weight=all_weights)
+        return loss
+
+
+class SAGE(nn.Module):
+    def __init__(self, in_feats, n_hidden, n_classes, n_layers, activation, dropout, agg="mean"):
+        super().__init__()
+        self.init(in_feats, n_hidden, n_classes, n_layers, activation, dropout, agg)
+
+    def init(self, in_feats, n_hidden, n_classes, n_layers, activation, dropout, agg):
+        self.n_layers = n_layers
+        self.n_hidden = n_hidden
+        self.n_classes = n_classes
+        self.layers = nn.ModuleList()
+        # self.batchnorm = nn.BatchNorm1d(n_hidden)
+        if n_layers > 1:
+            self.layers.append(SAGEConv(in_feats, n_hidden, agg, feat_drop=dropout))
+
+            for i in range(1, n_layers - 1):
+                self.layers.append(SAGEConv(n_hidden, n_hidden, agg, feat_drop=dropout))
+                # self.layers.append(nn.BatchNorm1d(n_hidden))
+            self.layers.append(SAGEConv(n_hidden, n_classes, agg))
+        else:
+            self.layers.append(SAGEConv(in_feats, n_classes, agg, feat_drop=dropout))
+        if agg == "gcn":
+            breakpoint()
+        self.dropout = nn.Dropout(dropout)
+        self.activation = activation
+
+    def forward(self, blocks, x, edge_weight=None):
+        h = x
+        for il, (layer, block) in enumerate(zip(self.layers, blocks)):
+            # weights = F.softmax(block.edata["weight"])
+            # weights = block.edata["weight"] / max(block.edata["weight"])
+            # h = layer(block, h, edge_weight=weights)
+            h = layer(block, h)
+            if il != len(self.layers) - 1:
+                h = self.activation(h)
+        return h
+
+    def inference(self, g, x, device, batch_size, num_workers, use_weights=False):
+        """
+        Inference with the GraphSAGE model on full neighbors (i.e. without neighbor sampling).
+        g : the entire graph.
+        x : the input of entire node set.
+        The inference code is written in a fashion that it could handle any number of nodes and
+        layers.
+        """
+        # During inference with sampling, multi-layer blocks are very inefficient because
+        # lots of computations in the first few layers are repeated.
+        # Therefore, we compute the representation of all nodes layer by layer.  The nodes
+        # on each layer are of course splitted in batches.
+        # TODO: can we standardize this?
+        for il, layer in enumerate(self.layers):
+            y = torch.zeros(g.num_nodes(), self.n_hidden if il != len(self.layers) - 1 else self.n_classes)
+            sampler = dgl.dataloading.MultiLayerFullNeighborSampler(1)
+            
+            dataloader = dgl.dataloading.NodeDataLoader(
+                g,
+                torch.arange(g.num_nodes()).to(g.device),
+                sampler,
+                batch_size=batch_size,
+                shuffle=False,
+                drop_last=False,
+                num_workers=num_workers,
+            )
+
+            for input_nodes, output_nodes, blocks in dataloader:
+                block = blocks[0]
+
+                block = block.int().to(device)
+                h = x[input_nodes].to(device)
+
+                if use_weights:
+                    weights = block.edata["weight"] / max(block.edata["weight"])
+                    h = layer(block, h, edge_weight=weights)
+                else:
+                    h = layer(block, h)
+                if il != len(self.layers) - 1:
+                    h = self.activation(h)
+                    h = self.dropout(h)
+
+                y[output_nodes] = h.cpu()
+
+            x = y
+        return y
+
+
+def train_graphsage(
+    dataset,
+    model,
+    batch_size,
+    fan_out,
+    num_negs,
+    neg_share,
+    lr,
+    num_epochs,
+    num_workers=0,
+    print_interval=3,
+    device="cpu",
+    cluster_features=True,
+    clusteringalgo="kmeans",
+    k=1,
+    logger=None,
+    loss_weights=False,
+    sample_weights=False,
+    epsilon=0.1,
+    evalepochs=1,
+    seed=0,
+    eval_skip=0,
+    quick=False
+):
+    train_start_time = time.time()
+    nfeat = dataset.graph.ndata.pop("feat")
+    model = model.to(device)
+    # Create PyTorch DataLoader for constructing blocks
+    n_edges = dataset.graph.num_edges()
+    train_seeds = torch.arange(n_edges)
+    set_seed(seed)
+
+    # Create samplers
+    if not sample_weights:
+        neg_sampler = NegativeSampler(dataset.graph, num_negs, neg_share)
+        sampler = dgl.dataloading.MultiLayerNeighborSampler([int(fanout) for fanout in fan_out.split(",")])
+    else:
+        neg_sampler = NegativeSamplerWeight(dataset.graph, num_negs, neg_share)
+        sampler = MultiLayerNeighborWeightedSampler([int(fanout) for fanout in fan_out.split(",")])
+
+    if batch_size == 0:
+        batch_size = len(train_seeds)
+    dataloader = dgl.dataloading.EdgeDataLoader(
+        dataset.graph,
+        train_seeds,
+        sampler,
+        exclude="reverse_id",
+        reverse_eids=torch.cat([torch.arange(n_edges // 2, n_edges), torch.arange(0, n_edges // 2)]).to(train_seeds),
+        negative_sampler=neg_sampler,
+        device=device,
+        batch_size=batch_size,
+        shuffle=True,
+        drop_last=True,
+        num_workers=num_workers,
+    )
+
+    loss_fcn = CrossEntropyLoss()
+    optimizer_sage = optim.Adam(model.parameters(), lr=lr)
+    # Training loop
+    avg = 0
+    iter_pos = []
+    iter_neg = []
+    iter_d = []
+    iter_t = []
+    best_hq = 0
+    best_hq_epoch = 0
+    total_steps = 0
+    losses = []
+    stop_run = False
+    for epoch in range(num_epochs):
+        tic = time.time()
+        # Loop over the dataloader to sample the computation dependency graph as a list of
+        # blocks.
+        tic_step = time.time()
+        for step, (input_nodes, pos_graph, neg_graph, blocks) in enumerate(dataloader):
+            batch_inputs = nfeat[input_nodes].to(device)
+            d_step = time.time()
+            #set_seed(seed)
+            model.train()
+            pos_graph = pos_graph.to(device)
+            neg_graph = neg_graph.to(device)
+            blocks = [block.int().to(device) for block in blocks]
+            # Compute loss and prediction
+            batch_pred = model(blocks, batch_inputs)
+            loss = loss_fcn(batch_pred, pos_graph, neg_graph, weights=loss_weights)
+
+            optimizer_sage.zero_grad()
+            loss.backward()
+            optimizer_sage.step()
+
+            t = time.time()
+            pos_edges = pos_graph.num_edges()
+            neg_edges = neg_graph.num_edges()
+            iter_pos.append(pos_edges / (t - tic_step))
+            iter_neg.append(neg_edges / (t - tic_step))
+            iter_d.append(d_step - tic_step)
+            iter_t.append(t - d_step)
+            if total_steps % print_interval == 0:
+                gpu_mem_alloc = torch.cuda.max_memory_allocated() / 1000000 if torch.cuda.is_available() else 0
+                logger.info(
+                    "Epoch {:05d} | Step {:05d} | N samples {} | Loss {:.4f} | Speed (samples/sec) {:.4f}|{:.4f} | Load {:.4f}| train {:.4f} | GPU {:.1f} MB".format(
+                        epoch,
+                        step,
+                        len(input_nodes),
+                        loss.item(),
+                        np.mean(iter_pos[3:]),
+                        np.mean(iter_neg[3:]),
+                        np.mean(iter_d[3:]),
+                        np.mean(iter_t[3:]),
+                        gpu_mem_alloc,
+                    )
+                )
+            tic_step = time.time()
+            total_steps += 1
+
+        losses.append(loss.item())
+        # early stopping
+        if (
+            epsilon is not None
+            and len(losses) > 3
+            and (losses[-2] - losses[-1]) < epsilon
+            and (losses[-3] - losses[-2]) < epsilon
+        ):
+            logger.info("Early stopping {}".format(str(losses[-5:])))
+            stop_run = True
+
+        if dataset.assembly.ref_marker_sets is not None and ((epoch % evalepochs == 0 and epoch > eval_skip) or stop_run):
+            model.eval()
+            encoded = model.inference(dataset.graph, nfeat, device, batch_size, num_workers)
+            if cluster_features:
+                encoded = torch.cat((encoded, nfeat), axis=1)
+            best_hq, best_hq_epoch, kmeans_loss, clusters, epoch_metrics = cluster_eval(
+                model=model,
+                dataset=dataset.assembly,
+                logits=encoded,
+                clustering=clusteringalgo,
+                k=k,
+                loss=loss,
+                best_hq=best_hq,
+                best_hq_epoch=best_hq_epoch,
+                epoch=epoch,
+                device=device,
+                clusteringloss=False,
+                logger=logger,
+                use_marker_contigs_only=quick,
+                seed=seed,
+            )
+            if best_hq_epoch == epoch:
+                metrics = epoch_metrics
+            # compare clusters
+            new_assignments = np.zeros(len(dataset.assembly.node_names))
+            for i, cluster in enumerate(clusters):
+                for contig in clusters[cluster]:
+                    new_assignments[dataset.assembly.node_names.index(contig)] = i
+
+            old_assignments = new_assignments.copy()
+        toc = time.time()
+        if epoch >= 5:
+            avg += toc - tic
+        if stop_run:
+            break
+        # = encoded.cpu().detach().numpy()
+
+    last_train_embs = encoded
+    last_model = model
+    logger.info("saving last model")
+    torch.save(last_model.state_dict(), os.path.join(dataset.assembly.cache_dir, "last_model_hq.pkl"))
+    logger.info("Avg epoch time: {}".format(avg / (epoch - 4)))
+    logger.info("Total training time: {:.3f} seconds".format(time.time() - train_start_time))
+    logger.info("Peak memory usage: {} MB".format(torch.cuda.max_memory_allocated()/1000000))
+    model.eval()
+    logger.info(f"Best HQ {best_hq} epoch, {best_hq_epoch}")
+    if total_steps == 0:
+        print("No training was done")
+    elif dataset.assembly.ref_marker_sets is not None:
+        logger.info("loading best model")
+        best_model = copy.deepcopy(model)
+        try:
+            best_model.load_state_dict(torch.load(os.path.join(dataset.assembly.cache_dir, "best_model_hq.pkl")))
+        except RuntimeError:
+            pdb.set_trace()
+    else:
+        best_model = last_model
+    set_seed(seed)
+    print("running best or last model again")
+    best_train_embs = best_model.inference(dataset.graph, nfeat, device, batch_size, num_workers)
+
+    best_train_embs = best_train_embs.detach()
+    if cluster_features:
+        best_train_embs = torch.cat((best_train_embs, nfeat), axis=1).detach()
+    return best_train_embs, best_model, last_train_embs, last_model, metrics
```

### Comparing `graphmb-0.2.4/src/graphmb/layers.py` & `graphmb-0.2.5/src/graphmb/layers.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,275 +1,275 @@
-import tensorflow as tf
-
-from tensorflow.keras.optimizers import Adam
-from tensorflow.keras.models import Model
-from tensorflow.keras.layers import Input, Dense, Activation
-from tensorflow.keras.layers import BatchNormalization, Lambda
-from tensorflow.keras.layers import Dropout, Layer
-
-def laf_init_uniform(shape, dtype=None):
-    a = tf.random.uniform(shape ,0,1, dtype=dtype)
-    return a
-
-def laf_init_normal(shape, dtype=None):
-    b = tf.random.normal(shape, 1.0, 0.1, dtype=dtype)
-    return b
-
-class BiasLayer(Layer):
-    def __init__(self, *args, **kwargs):
-        super(BiasLayer, self).__init__(*args, **kwargs)
-
-    def build(self, input_shape):
-        self.bias = self.add_weight('bias',
-                                    shape=input_shape[1:],
-                                    initializer='zeros',
-                                    trainable=True)
-    def call(self, x):
-        return x + self.bias
-
-class LAF(Layer):
-    def __init__(self, units=4, eps=1e-7):
-        super(LAF, self).__init__()
-        self.units = units
-        self.eps = eps
-        
-    def build(self, input_shape):
-
-        self.b = self.add_weight(shape=(1, self.units, 1),
-                                 initializer=laf_init_uniform,
-                                 trainable=True, name='b')
-        self.d = self.add_weight(shape=(1, self.units, 1),
-                                 initializer=laf_init_uniform,
-                                 trainable=True, name='d')
-        self.f = self.add_weight(shape=(1, self.units, 1),
-                                 initializer=laf_init_uniform,
-                                 trainable=True, name='f')
-        self.h = self.add_weight(shape=(1, self.units, 1),
-                                 initializer=laf_init_uniform,
-                                 trainable=True, name='h')
-
-        self.a = self.add_weight(shape=(1, self.units, 1),
-                                 initializer=laf_init_uniform,
-                                 trainable=True, name='a')
-        self.c = self.add_weight(shape=(1, self.units, 1),
-                                 initializer=laf_init_uniform,
-                                 trainable=True, name='c')
-        self.e = self.add_weight(shape=(1, self.units, 1),
-                                 initializer=laf_init_uniform,
-                                 trainable=True, name='e')
-        self.g = self.add_weight(shape=(1, self.units, 1),
-                                 initializer=laf_init_uniform,
-                                 trainable=True, name='g')
-       
-        self.alpha = self.add_weight(shape=(1, self.units, 1),
-                                 initializer=laf_init_normal,
-                                 trainable=True, name='alpha')
-        self.beta  = self.add_weight(shape=(1, self.units, 1),
-                                 initializer=laf_init_normal,
-                                 trainable=True, name='beta')
-        self.gamma = self.add_weight(shape=(1, self.units, 1),
-                                 initializer=laf_init_normal,
-                                 trainable=True, name='gamma')
-        self.delta = self.add_weight(shape=(1, self.units, 1),
-                                 initializer=laf_init_normal,
-                                 trainable=True, name='delta')
-    def call(self, inputs):
-        eps = 1e-6
-        adj, inputs = inputs
-
-        x = inputs
-        x  = tf.reshape(x, [-1, self.units, inputs.shape[-1]//self.units])
-        sig_x  = tf.clip_by_value(tf.nn.sigmoid(x), eps, 1-eps)
-        n_sig_x = 1.0 - sig_x
-
-        x_b = tf.math.pow(sig_x, tf.nn.relu(self.b))
-        x_d = tf.math.pow(n_sig_x, tf.nn.relu(self.d))
-        x_f = tf.math.pow(sig_x, tf.nn.relu(self.f))
-        x_h = tf.math.pow(n_sig_x, tf.nn.relu(self.h))
-
-        x_b = tf.reshape(x_b, [-1, inputs.shape[-1]])
-        x_d = tf.reshape(x_d, [-1, inputs.shape[-1]])
-        x_f = tf.reshape(x_f, [-1, inputs.shape[-1]])
-        x_h = tf.reshape(x_h, [-1, inputs.shape[-1]])
-
-        x_b = tf.sparse.sparse_dense_matmul(adj, x_b) + eps
-        x_d = tf.sparse.sparse_dense_matmul(adj, x_d) + eps
-        x_f = tf.sparse.sparse_dense_matmul(adj, x_f) + eps
-        x_h = tf.sparse.sparse_dense_matmul(adj, x_h) + eps
-
-        x_b = tf.reshape(x_b, [-1, self.units, inputs.shape[-1]//self.units])
-        x_d = tf.reshape(x_d, [-1, self.units, inputs.shape[-1]//self.units])
-        x_f = tf.reshape(x_f, [-1, self.units, inputs.shape[-1]//self.units])
-        x_h = tf.reshape(x_h, [-1, self.units, inputs.shape[-1]//self.units])
-
-        x_ab = tf.math.pow(x_b,tf.nn.relu(self.a) ) * self.alpha
-        x_cd = tf.math.pow(x_d,tf.nn.relu(self.c) ) * self.beta
-        x_ef = tf.math.pow(x_f,tf.nn.relu(self.e) ) * self.gamma
-        x_gh = tf.math.pow(x_h,tf.nn.relu(self.g) ) * self.delta
-
-        den = (x_ef + x_gh)
-        num = (x_ab + x_cd) * den
-
-        out = num / (den * den + 1e-3)
-        out = tf.reshape(out, (-1, inputs.shape[-1]))
-        return out
-    
-    
-# https://github.com/danielegrattarola/keras-gat/blob/master/keras_gat/graph_attention_layer.py
-# https://www.programmersought.com/article/38174813555/
-
-class GraphAttention(Layer):
-    def __init__(self,
-                 F_,
-                 attn_heads=1,
-                 attn_heads_reduction='concat',  # {'concat', 'average'}
-                 dropout_rate=0.5,
-                 activation='relu',
-                 use_bias=True,
-                 kernel_initializer='glorot_uniform',
-                 bias_initializer='zeros',
-                 attn_kernel_initializer='glorot_uniform',
-                 kernel_regularizer=None,
-                 bias_regularizer=None,
-                 attn_kernel_regularizer=None,
-                 activity_regularizer=None,
-                 kernel_constraint=None,
-                 bias_constraint=None,
-                 attn_kernel_constraint=None,
-                 laf_units=None,
-                 **kwargs):
-        if attn_heads_reduction not in {'concat', 'average'}:
-            raise ValueError('Possbile reduction methods: concat, average')
-
-        self.F_ = F_  # Number of output features (F' in the paper)
-        self.attn_heads = attn_heads  # Number of attention heads (K in the paper)
-        self.attn_heads_reduction = attn_heads_reduction  # Eq. 5 and 6 in the paper
-        self.dropout_rate = dropout_rate  # Internal dropout rate
-        self.activation = tf.keras.activations.get(activation)  # Eq. 4 in the paper
-        self.use_bias = use_bias
-
-        self.kernel_initializer = tf.keras.initializers.get(kernel_initializer)
-        self.bias_initializer = tf.keras.initializers.get(bias_initializer)
-        self.attn_kernel_initializer = tf.keras.initializers.get(attn_kernel_initializer)
-
-        self.kernel_regularizer = tf.keras.regularizers.get(kernel_regularizer)
-        self.bias_regularizer = tf.keras.regularizers.get(bias_regularizer)
-        self.attn_kernel_regularizer = tf.keras.regularizers.get(attn_kernel_regularizer)
-        self.activity_regularizer = tf.keras.regularizers.get(activity_regularizer)
-
-        self.kernel_constraint = tf.keras.constraints.get(kernel_constraint)
-        self.bias_constraint = tf.keras.constraints.get(bias_constraint)
-        self.attn_kernel_constraint = tf.keras.constraints.get(attn_kernel_constraint)
-        self.supports_masking = False
-
-        # Populated by build()
-        self.kernels = []       # Layer kernels for attention heads
-        self.biases = []        # Layer biases for attention heads
-        self.attn_kernels = []  # Attention kernels for attention heads
-
-        if attn_heads_reduction == 'concat':
-            # Output will have shape (..., K * F')
-            self.output_dim = self.F_ * self.attn_heads
-        else:
-            # Output will have shape (..., F')
-            self.output_dim = self.F_
-
-        self.laf_units = laf_units
-        if self.laf_units is not None:
-            self.laf_agg = LAF(laf_units)
-
-        super(GraphAttention, self).__init__(**kwargs)
-
-    def build(self, input_shape):
-        assert len(input_shape) >= 2
-        F = input_shape[1][-1]
-
-        # Initialize weights for each attention head
-        for head in range(self.attn_heads):
-            # Layer kernel
-            kernel = self.add_weight(shape=(F, self.F_),
-                                     initializer=self.kernel_initializer,
-                                     regularizer=self.kernel_regularizer,
-                                     constraint=self.kernel_constraint,
-                                     name='kernel_{}'.format(head))
-            self.kernels.append(kernel)
-
-            # # Layer bias
-            if self.use_bias:
-                bias = self.add_weight(shape=(self.F_, ),
-                                       initializer=self.bias_initializer,
-                                       regularizer=self.bias_regularizer,
-                                       constraint=self.bias_constraint,
-                                       name='bias_{}'.format(head))
-                self.biases.append(bias)
-
-            # Attention kernels
-            attn_kernel_self = self.add_weight(shape=(self.F_, 1),
-                                               initializer=self.attn_kernel_initializer,
-                                               regularizer=self.attn_kernel_regularizer,
-                                               constraint=self.attn_kernel_constraint,
-                                               name='attn_kernel_self_{}'.format(head),)
-            attn_kernel_neighs = self.add_weight(shape=(self.F_, 1),
-                                                 initializer=self.attn_kernel_initializer,
-                                                 regularizer=self.attn_kernel_regularizer,
-                                                 constraint=self.attn_kernel_constraint,
-                                                 name='attn_kernel_neigh_{}'.format(head))
-            self.attn_kernels.append([attn_kernel_self, attn_kernel_neighs])
-        self.built = True
-
-    def call(self, inputs, training=True):
-        A = inputs[0]  # Adjacency matrix (N x N) sparse
-        X = inputs[1]  # Node features (N x F)
-
-        outputs = []
-        for head in range(self.attn_heads):
-            kernel = self.kernels[head]  # W in the paper (F x F')
-            attention_kernel = self.attn_kernels[head]  # Attention kernel a in the paper (2F' x 1)
-
-            # Compute inputs to attention network
-            features = tf.matmul(X, kernel)  # (N x F')
-
-            # Compute feature combinations
-            # Note: [[a_1], [a_2]]^T [[Wh_i], [Wh_2]] = [a_1]^T [Wh_i] + [a_2]^T [Wh_j]
-            attn_for_self   = tf.matmul(features, attention_kernel[0])  # (N x 1), [a_1]^T [Wh_i]
-            attn_for_neighs = tf.matmul(features, attention_kernel[1])  # (N x 1), [a_2]^T [Wh_j]
-
-            # Attention head a(Wh_i, Wh_j) = a^T [[Wh_i], [Wh_j]]
-            con_sa_1 = A * attn_for_self 
-            con_sa_2 = A * tf.transpose(attn_for_neighs, [1,0])
-            
-            weights = tf.sparse.add(con_sa_1, con_sa_2)  # concatenation
-            weights_act = tf.SparseTensor(indices=weights.indices,
-                                          values=tf.nn.leaky_relu(weights.values, alpha=0.2),
-                                          dense_shape=weights.dense_shape)
-            
-            attention = tf.sparse.softmax(weights_act)
-            if training and self.dropout_rate > 0.0:
-                attention = tf.SparseTensor(indices=attention.indices,
-                                            values=tf.nn.dropout(attention.values, self.dropout_rate),
-                                            dense_shape=attention.dense_shape)
-            if training and self.dropout_rate > 0.0:
-                features = tf.nn.dropout(features, self.dropout_rate)
-            
-            if self.laf_units is not None:
-                node_features = self.laf_agg((attention, features))
-            else:
-                node_features = tf.sparse.sparse_dense_matmul(attention, features)
-            
-            if self.use_bias:
-                node_features = node_features + self.biases[head]
-                
-            # Add output of attention head to final output
-            outputs.append(node_features)
-
-        # Aggregate the heads' output according to the reduction method
-        output = tf.concat(outputs, axis=1)  # (N x KF')
-        if self.attn_heads_reduction != 'concat':
-            output = tf.reshape(output, [-1, self.attn_heads, self.F_])
-            output = tf.reduce_mean(output, axis=-2)
-
-        output = self.activation(output)
-        return output
-
-    def compute_output_shape(self, input_shape):
-        output_shape = input_shape[0][0], self.output_dim
-        return output_shape
+import tensorflow as tf
+
+from tensorflow.keras.optimizers import Adam
+from tensorflow.keras.models import Model
+from tensorflow.keras.layers import Input, Dense, Activation
+from tensorflow.keras.layers import BatchNormalization, Lambda
+from tensorflow.keras.layers import Dropout, Layer
+
+def laf_init_uniform(shape, dtype=None):
+    a = tf.random.uniform(shape ,0,1, dtype=dtype)
+    return a
+
+def laf_init_normal(shape, dtype=None):
+    b = tf.random.normal(shape, 1.0, 0.1, dtype=dtype)
+    return b
+
+class BiasLayer(Layer):
+    def __init__(self, *args, **kwargs):
+        super(BiasLayer, self).__init__(*args, **kwargs)
+
+    def build(self, input_shape):
+        self.bias = self.add_weight('bias',
+                                    shape=input_shape[1:],
+                                    initializer='zeros',
+                                    trainable=True)
+    def call(self, x):
+        return x + self.bias
+
+class LAF(Layer):
+    def __init__(self, units=4, eps=1e-7):
+        super(LAF, self).__init__()
+        self.units = units
+        self.eps = eps
+        
+    def build(self, input_shape):
+
+        self.b = self.add_weight(shape=(1, self.units, 1),
+                                 initializer=laf_init_uniform,
+                                 trainable=True, name='b')
+        self.d = self.add_weight(shape=(1, self.units, 1),
+                                 initializer=laf_init_uniform,
+                                 trainable=True, name='d')
+        self.f = self.add_weight(shape=(1, self.units, 1),
+                                 initializer=laf_init_uniform,
+                                 trainable=True, name='f')
+        self.h = self.add_weight(shape=(1, self.units, 1),
+                                 initializer=laf_init_uniform,
+                                 trainable=True, name='h')
+
+        self.a = self.add_weight(shape=(1, self.units, 1),
+                                 initializer=laf_init_uniform,
+                                 trainable=True, name='a')
+        self.c = self.add_weight(shape=(1, self.units, 1),
+                                 initializer=laf_init_uniform,
+                                 trainable=True, name='c')
+        self.e = self.add_weight(shape=(1, self.units, 1),
+                                 initializer=laf_init_uniform,
+                                 trainable=True, name='e')
+        self.g = self.add_weight(shape=(1, self.units, 1),
+                                 initializer=laf_init_uniform,
+                                 trainable=True, name='g')
+       
+        self.alpha = self.add_weight(shape=(1, self.units, 1),
+                                 initializer=laf_init_normal,
+                                 trainable=True, name='alpha')
+        self.beta  = self.add_weight(shape=(1, self.units, 1),
+                                 initializer=laf_init_normal,
+                                 trainable=True, name='beta')
+        self.gamma = self.add_weight(shape=(1, self.units, 1),
+                                 initializer=laf_init_normal,
+                                 trainable=True, name='gamma')
+        self.delta = self.add_weight(shape=(1, self.units, 1),
+                                 initializer=laf_init_normal,
+                                 trainable=True, name='delta')
+    def call(self, inputs):
+        eps = 1e-6
+        adj, inputs = inputs
+
+        x = inputs
+        x  = tf.reshape(x, [-1, self.units, inputs.shape[-1]//self.units])
+        sig_x  = tf.clip_by_value(tf.nn.sigmoid(x), eps, 1-eps)
+        n_sig_x = 1.0 - sig_x
+
+        x_b = tf.math.pow(sig_x, tf.nn.relu(self.b))
+        x_d = tf.math.pow(n_sig_x, tf.nn.relu(self.d))
+        x_f = tf.math.pow(sig_x, tf.nn.relu(self.f))
+        x_h = tf.math.pow(n_sig_x, tf.nn.relu(self.h))
+
+        x_b = tf.reshape(x_b, [-1, inputs.shape[-1]])
+        x_d = tf.reshape(x_d, [-1, inputs.shape[-1]])
+        x_f = tf.reshape(x_f, [-1, inputs.shape[-1]])
+        x_h = tf.reshape(x_h, [-1, inputs.shape[-1]])
+
+        x_b = tf.sparse.sparse_dense_matmul(adj, x_b) + eps
+        x_d = tf.sparse.sparse_dense_matmul(adj, x_d) + eps
+        x_f = tf.sparse.sparse_dense_matmul(adj, x_f) + eps
+        x_h = tf.sparse.sparse_dense_matmul(adj, x_h) + eps
+
+        x_b = tf.reshape(x_b, [-1, self.units, inputs.shape[-1]//self.units])
+        x_d = tf.reshape(x_d, [-1, self.units, inputs.shape[-1]//self.units])
+        x_f = tf.reshape(x_f, [-1, self.units, inputs.shape[-1]//self.units])
+        x_h = tf.reshape(x_h, [-1, self.units, inputs.shape[-1]//self.units])
+
+        x_ab = tf.math.pow(x_b,tf.nn.relu(self.a) ) * self.alpha
+        x_cd = tf.math.pow(x_d,tf.nn.relu(self.c) ) * self.beta
+        x_ef = tf.math.pow(x_f,tf.nn.relu(self.e) ) * self.gamma
+        x_gh = tf.math.pow(x_h,tf.nn.relu(self.g) ) * self.delta
+
+        den = (x_ef + x_gh)
+        num = (x_ab + x_cd) * den
+
+        out = num / (den * den + 1e-3)
+        out = tf.reshape(out, (-1, inputs.shape[-1]))
+        return out
+    
+    
+# https://github.com/danielegrattarola/keras-gat/blob/master/keras_gat/graph_attention_layer.py
+# https://www.programmersought.com/article/38174813555/
+
+class GraphAttention(Layer):
+    def __init__(self,
+                 F_,
+                 attn_heads=1,
+                 attn_heads_reduction='concat',  # {'concat', 'average'}
+                 dropout_rate=0.5,
+                 activation='relu',
+                 use_bias=True,
+                 kernel_initializer='glorot_uniform',
+                 bias_initializer='zeros',
+                 attn_kernel_initializer='glorot_uniform',
+                 kernel_regularizer=None,
+                 bias_regularizer=None,
+                 attn_kernel_regularizer=None,
+                 activity_regularizer=None,
+                 kernel_constraint=None,
+                 bias_constraint=None,
+                 attn_kernel_constraint=None,
+                 laf_units=None,
+                 **kwargs):
+        if attn_heads_reduction not in {'concat', 'average'}:
+            raise ValueError('Possbile reduction methods: concat, average')
+
+        self.F_ = F_  # Number of output features (F' in the paper)
+        self.attn_heads = attn_heads  # Number of attention heads (K in the paper)
+        self.attn_heads_reduction = attn_heads_reduction  # Eq. 5 and 6 in the paper
+        self.dropout_rate = dropout_rate  # Internal dropout rate
+        self.activation = tf.keras.activations.get(activation)  # Eq. 4 in the paper
+        self.use_bias = use_bias
+
+        self.kernel_initializer = tf.keras.initializers.get(kernel_initializer)
+        self.bias_initializer = tf.keras.initializers.get(bias_initializer)
+        self.attn_kernel_initializer = tf.keras.initializers.get(attn_kernel_initializer)
+
+        self.kernel_regularizer = tf.keras.regularizers.get(kernel_regularizer)
+        self.bias_regularizer = tf.keras.regularizers.get(bias_regularizer)
+        self.attn_kernel_regularizer = tf.keras.regularizers.get(attn_kernel_regularizer)
+        self.activity_regularizer = tf.keras.regularizers.get(activity_regularizer)
+
+        self.kernel_constraint = tf.keras.constraints.get(kernel_constraint)
+        self.bias_constraint = tf.keras.constraints.get(bias_constraint)
+        self.attn_kernel_constraint = tf.keras.constraints.get(attn_kernel_constraint)
+        self.supports_masking = False
+
+        # Populated by build()
+        self.kernels = []       # Layer kernels for attention heads
+        self.biases = []        # Layer biases for attention heads
+        self.attn_kernels = []  # Attention kernels for attention heads
+
+        if attn_heads_reduction == 'concat':
+            # Output will have shape (..., K * F')
+            self.output_dim = self.F_ * self.attn_heads
+        else:
+            # Output will have shape (..., F')
+            self.output_dim = self.F_
+
+        self.laf_units = laf_units
+        if self.laf_units is not None:
+            self.laf_agg = LAF(laf_units)
+
+        super(GraphAttention, self).__init__(**kwargs)
+
+    def build(self, input_shape):
+        assert len(input_shape) >= 2
+        F = input_shape[1][-1]
+
+        # Initialize weights for each attention head
+        for head in range(self.attn_heads):
+            # Layer kernel
+            kernel = self.add_weight(shape=(F, self.F_),
+                                     initializer=self.kernel_initializer,
+                                     regularizer=self.kernel_regularizer,
+                                     constraint=self.kernel_constraint,
+                                     name='kernel_{}'.format(head))
+            self.kernels.append(kernel)
+
+            # # Layer bias
+            if self.use_bias:
+                bias = self.add_weight(shape=(self.F_, ),
+                                       initializer=self.bias_initializer,
+                                       regularizer=self.bias_regularizer,
+                                       constraint=self.bias_constraint,
+                                       name='bias_{}'.format(head))
+                self.biases.append(bias)
+
+            # Attention kernels
+            attn_kernel_self = self.add_weight(shape=(self.F_, 1),
+                                               initializer=self.attn_kernel_initializer,
+                                               regularizer=self.attn_kernel_regularizer,
+                                               constraint=self.attn_kernel_constraint,
+                                               name='attn_kernel_self_{}'.format(head),)
+            attn_kernel_neighs = self.add_weight(shape=(self.F_, 1),
+                                                 initializer=self.attn_kernel_initializer,
+                                                 regularizer=self.attn_kernel_regularizer,
+                                                 constraint=self.attn_kernel_constraint,
+                                                 name='attn_kernel_neigh_{}'.format(head))
+            self.attn_kernels.append([attn_kernel_self, attn_kernel_neighs])
+        self.built = True
+
+    def call(self, inputs, training=True):
+        A = inputs[0]  # Adjacency matrix (N x N) sparse
+        X = inputs[1]  # Node features (N x F)
+
+        outputs = []
+        for head in range(self.attn_heads):
+            kernel = self.kernels[head]  # W in the paper (F x F')
+            attention_kernel = self.attn_kernels[head]  # Attention kernel a in the paper (2F' x 1)
+
+            # Compute inputs to attention network
+            features = tf.matmul(X, kernel)  # (N x F')
+
+            # Compute feature combinations
+            # Note: [[a_1], [a_2]]^T [[Wh_i], [Wh_2]] = [a_1]^T [Wh_i] + [a_2]^T [Wh_j]
+            attn_for_self   = tf.matmul(features, attention_kernel[0])  # (N x 1), [a_1]^T [Wh_i]
+            attn_for_neighs = tf.matmul(features, attention_kernel[1])  # (N x 1), [a_2]^T [Wh_j]
+
+            # Attention head a(Wh_i, Wh_j) = a^T [[Wh_i], [Wh_j]]
+            con_sa_1 = A * attn_for_self 
+            con_sa_2 = A * tf.transpose(attn_for_neighs, [1,0])
+            
+            weights = tf.sparse.add(con_sa_1, con_sa_2)  # concatenation
+            weights_act = tf.SparseTensor(indices=weights.indices,
+                                          values=tf.nn.leaky_relu(weights.values, alpha=0.2),
+                                          dense_shape=weights.dense_shape)
+            
+            attention = tf.sparse.softmax(weights_act)
+            if training and self.dropout_rate > 0.0:
+                attention = tf.SparseTensor(indices=attention.indices,
+                                            values=tf.nn.dropout(attention.values, self.dropout_rate),
+                                            dense_shape=attention.dense_shape)
+            if training and self.dropout_rate > 0.0:
+                features = tf.nn.dropout(features, self.dropout_rate)
+            
+            if self.laf_units is not None:
+                node_features = self.laf_agg((attention, features))
+            else:
+                node_features = tf.sparse.sparse_dense_matmul(attention, features)
+            
+            if self.use_bias:
+                node_features = node_features + self.biases[head]
+                
+            # Add output of attention head to final output
+            outputs.append(node_features)
+
+        # Aggregate the heads' output according to the reduction method
+        output = tf.concat(outputs, axis=1)  # (N x KF')
+        if self.attn_heads_reduction != 'concat':
+            output = tf.reshape(output, [-1, self.attn_heads, self.F_])
+            output = tf.reduce_mean(output, axis=-2)
+
+        output = self.activation(output)
+        return output
+
+    def compute_output_shape(self, input_shape):
+        output_shape = input_shape[0][0], self.output_dim
+        return output_shape
```

### Comparing `graphmb-0.2.4/src/graphmb/main.py` & `graphmb-0.2.5/src/graphmb/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,601 +1,609 @@
-
-import logging
-from datetime import datetime
-from collections import Counter
-import numpy as np
-import sys
-import os
-import copy
-import pickle
-import shutil
-import pdb
-import networkx as nx
-
-from pathlib import Path
-from graphmb.arg_options import create_parser
-from graphmb.evaluate import (
-    evaluate_contig_sets,
-    calculate_overall_prf,
-)
-from graphmb.contigsdataset import AssemblyDataset
-from graphmb.visualize import draw_nx_graph, run_tsne, plot_embs
-from graphmb.utils import set_seed, get_cluster_mask
-from graphmb.graphmb1 import (cluster_embs,
-    evaluate_binning,
-    calculate_bin_metrics,
-    )
-
-from graphmb.version import __version__
-
-def run_model(dataset, args, logger, nrun, target_metric):
-    if args.model_name.endswith("_ccvae"):
-        from graphmb import train_ccvae
-        return train_ccvae.run_model_ccvae(dataset, args, logger, nrun, target_metric)
-    elif args.model_name == "vae":
-        from graphmb import train_vae
-        return train_vae.run_model_vae(dataset, args, logger, nrun)
-    elif args.model_name in ("gcn", "sage", "gat"):
-        from graphmb import train_gnn
-        return train_gnn.run_model_gnn(dataset, args, logger, nrun, target_metric)
-
-def draw(dataset, node_to_label, label_to_node, cluster_to_contig, outname, graph=None):
-    # properties of all nodes
-    nodeid_to_label = {i: node_to_label.get(n, "NA") for i, n in enumerate(dataset.node_names)}
-    contig_lens = {i: dataset.node_lengths[i] for i in range(len(dataset.node_names))}
-    nodes_titles = {
-        i: str(dataset.node_names[i]) + "<br>Length: " + str(contig_lens[i]) for i in range(len(dataset.contig_names))
-    }
-    if dataset.depth is not None:
-        nodes_titles = {
-            i: nodes_titles[i] + "<br>Depth: " + ", ".join(["{:.4}".format(x) for x in dataset.nodes_depths[i]])
-            for i in range(len(dataset.contig_names))
-        }
-    if cluster_to_contig:
-        contig_to_cluster = {contig: cluster for cluster, contigs in cluster_to_contig.items() for contig in contigs}
-        nodes_titles = {
-            i: nodes_titles[i] + "<br>Cluster: " + str(contig_to_cluster[n])
-            for i, n in enumerate(dataset.contig_names)
-        }
-
-    # convert DGL graph to networkx
-    nx_graph = graph.cpu().to_networkx(edge_attrs=["weight"]).to_undirected()
-    connected_comp = [c for c in sorted(nx.connected_components(nx_graph), key=len, reverse=True) if len(c) > 0]
-    # draw connected components to separate files
-    for i in range(10, 50):
-        # without_largest_comp = [item for sublist in connected_comp[10:110] for item in sublist if len(sublist) > 2]
-        this_comp = connected_comp[i]
-        nx_graph = nx.subgraph(nx_graph, this_comp)
-
-        draw_nx_graph(
-            nx_graph,
-            nodeid_to_label,
-            label_to_node,
-            outname + "_" + str(i),
-            contig_sizes=contig_lens,
-            node_titles=nodes_titles,
-        )
-
-
-def write_embs(embs, node_names, outname):
-    # write embs as dict node_name: embs
-    embs_dict = {node_names[i]: embs[i] for i in range(len(embs))}
-    with open(outname, "wb") as f:
-        pickle.dump(embs_dict, f)
-
-def write_edges(graph, outname):
-    with open(outname, "w") as graphf:
-        for e in zip(graph.edges()[0], graph.edges()[1]):
-            graphf.write(str(e[0].item()) + "\t" + str(e[1].item()) + "\n")
-
-
-def check_dirs(args, use_features=True):
-    """Check if files necessary to run exist, other wise print message and exit"""
-    if args.outdir is None:
-        if args.assembly is None:
-            print("Please specify assembly path or outdir with --assembly or --outdir")
-            exit()
-        else:
-            args.outdir = args.assembly
-    else:
-        Path(args.outdir).mkdir(parents=True, exist_ok=True)
-
-    # check if other dirs exists
-    if not os.path.exists(os.path.join(args.assembly, args.graph_file)):
-        print(f"Assembly Graph file {args.graph_file} not found, check --graph_file option")
-    if not os.path.exists(os.path.join(args.assembly, args.features)) or not use_features:
-
-        # needs assembly files to calculate features
-        if not os.path.exists(os.path.join(args.assembly, args.assembly_name)):
-            print(f"Assembly {args.assembly_name} not found, check --assembly_name option")
-            exit()
-        if not os.path.exists(os.path.join(args.assembly, args.depth)):
-            print(f"Depth file {args.depth} not found, check --depth option, not using depths")
-            #exit()
-
-
-def get_activation(args):
-    # pick activation function
-    import torch.nn as nn
-    if args.activation == "prelu":
-        activation = nn.PReLU(args.hidden_gnn)
-    elif args.activation == "relu":
-        activation = nn.ReLU()
-    elif args.activation == "tanh":
-        activation = nn.Tanh()
-    elif args.activation == "sigmoid":
-        activation = nn.Sigmoid()
-    elif args.activation == "lrelu":
-        activation = nn.LeakyReLU()
-    return activation
-
-
-def run_graphmb(dataset, args, device, logger):
-    from graphmb.graphsage_unsupervised import train_graphsage, SAGE
-    activation = get_activation(args)
-    model = SAGE(
-        dataset.graph.ndata["feat"].shape[1],
-        args.hidden_gnn,
-        args.embsize_gnn,
-        args.layers_gnn,
-        activation,
-        args.dropout_gnn,
-        agg=args.aggtype
-    )
-    model = model.to(device)
-
-    if model is not None:
-        model = model.to(device)
-
-    cluster_mask = get_cluster_mask(args.quick, dataset.assembly)
-    logging.info(model)
-    if (
-        dataset.assembly.ref_marker_sets is not None
-        and args.clusteringalgo is not None
-        and not args.skip_preclustering
-    ):
-        # cluster using only input features
-        logger.info("pre train clustering:")
-        pre_cluster_to_contig, centroids = cluster_embs(
-            dataset.graph.ndata["feat"].detach().cpu().numpy()[cluster_mask],
-            np.array(dataset.assembly.node_names)[cluster_mask],
-            args.clusteringalgo,
-            args.kclusters,
-            device=device,
-            # node_lens=np.array([c[0] for c in dataset.assembly.nodes_len]),
-            node_lens=np.array(dataset.assembly.node_lengths)[cluster_mask],
-            seed=args.seed,
-        )
-        results = evaluate_contig_sets(
-            dataset.assembly.ref_marker_sets, dataset.assembly.contig_markers, pre_cluster_to_contig
-        )
-        metrics = calculate_bin_metrics(results)
-        logger.info(f"HQ: {len(metrics['hq'])}, MQ:, {len(metrics['mq'])} Total bins: {len(metrics['total'])}")
-
-    best_train_embs, best_model, last_train_embs, last_model, metrics = train_graphsage(
-        dataset,
-        model,
-        batch_size=args.batchsize,
-        fan_out=args.fanout,
-        num_negs=args.negatives,
-        neg_share=False,
-        num_epochs=args.epoch,
-        lr=args.lr_gnn,
-        k=args.kclusters,
-        clusteringalgo=args.clusteringalgo,
-        cluster_features=args.concatfeatures,
-        print_interval=args.print,
-        loss_weights=(not args.no_loss_weights),
-        sample_weights=(not args.no_sample_weights),
-        logger=logger,
-        device=device,
-        epsilon=args.early_stopping,
-        evalepochs=args.evalepochs,
-        seed=args.seed,
-        eval_skip=args.evalskip,
-        quick=args.quick
-    )
-    return best_train_embs, best_model, last_train_embs, last_model, metrics
-
-
-def write_bins(args, dataset, cluster_to_contig, logger):
-    bin_dir = Path(args.outdir + "/{}_bins/".format(args.outname))
-    bin_dir.mkdir(parents=True, exist_ok=True)
-    [f.unlink() for f in bin_dir.glob("*.fa") if f.is_file()]
-    clustered_contigs = set()
-    multi_contig_clusters = 0
-    logger.info(f"{len(cluster_to_contig)} clusters")
-    short_contigs = set()
-    skipped_clusters = 0
-    for c in cluster_to_contig:
-        cluster_size = sum([dataset.node_lengths[dataset.node_names.index(contig)] for contig in cluster_to_contig[c]])
-        if cluster_size < args.minbin:
-            # print("skipped small cluster", len(cluster_to_contig[c]), "contig")
-            for contig in cluster_to_contig[c]:
-                short_contigs.add(contig)
-            skipped_clusters += 1
-            continue
-        multi_contig_clusters += 1
-        with open(bin_dir / f"{c}.fa", "w") as binfile:
-            for contig in cluster_to_contig[c]:
-                binfile.write(">" + contig + "\n")
-                binfile.write(dataset.node_seqs[contig] + "\n")
-                clustered_contigs.add(contig)
-        # print("multi cluster", c, "size", cluster_size, "contigs", len(cluster_to_contig[c]))
-    logger.info("### skipped {} clusters while writing to file".format(skipped_clusters))
-    single_clusters = multi_contig_clusters
-    left_over = set(dataset.node_names) - clustered_contigs - short_contigs
-    for c in left_over:
-        if c not in clustered_contigs and len(dataset.node_seqs[c]) > args.minbin:
-
-            with open(bin_dir / f"{single_clusters}.fna", "w") as binfile:
-                binfile.write(">" + c + "\n")
-                binfile.write(dataset.node_seqs[c] + "\n")
-                single_clusters += 1
-            # print("contig", single_clusters, "size", len(dataset.contig_seqs[c]))
-    logger.info(f"### wrote {single_clusters} clusters {multi_contig_clusters} >= #contig {args.mincomp}")
-
-
-def run_post_processing(final_embs, args, logger, dataset, device, label_to_node, node_to_label, seed):
-    metrics = {}
-    if "cluster" in args.post or "kmeans" in args.post:
-        logger.info("#### clustering embs with {} ({})".format(args.clusteringalgo, args.kclusters))
-        # train_embs = last_train_embs
-
-        if args.clusteringalgo is False:
-            args.clusteringalgo = "kmeans"
-        if not isinstance(final_embs, np.ndarray):
-            if args.cuda:
-                final_embs = final_embs.cpu()
-            final_embs = final_embs.numpy()
-
-            # last_train_embs should already be detached and on cpu
-        best_cluster_to_contig, best_centroids = cluster_embs(
-            final_embs,
-            dataset.node_names,
-            args.clusteringalgo,
-            # len(dataset.connected),
-            args.kclusters,
-            device=device,
-            seed=seed,
-        )
-        cluster_sizes = {}
-        for c in best_cluster_to_contig:
-            cluster_size = sum([len(dataset.node_seqs[contig]) for contig in best_cluster_to_contig[c]])
-            cluster_sizes[c] = cluster_size
-        best_contig_to_bin = {}
-        for bin in best_cluster_to_contig:
-            for contig in best_cluster_to_contig[bin]:
-                best_contig_to_bin[contig] = bin
-        # run for best epoch only
-        if args.markers is not None:
-            total_hq = 0
-            total_mq = 0
-            results = evaluate_contig_sets(dataset.ref_marker_sets, dataset.contig_markers, best_cluster_to_contig)
-            hq_bins = set()
-            for binid in results:
-                if results[binid]["comp"] > 90 and results[binid]["cont"] < 5:
-                    contig_labels = [dataset.node_to_label.get(node, 0) for node in best_cluster_to_contig[binid]]
-                    labels_count = Counter(contig_labels)
-                    # logger.debug(
-                    #    f"{binid}, {round(results[binid]['comp'],4)}, {round(results[binid]['cont'],4)}, "
-                    #    f"{len(best_cluster_to_contig[binid])} {labels_count}"
-                    # )
-                    hq_bins.add(binid)
-                    total_hq += 1
-                if results[binid]["comp"] > 50 and results[binid]["cont"] < 10:
-                    total_mq += 1
-            logger.info("#### Total HQ {} ####".format(total_hq))
-            logger.info("#### Total MQ {} ####".format(total_mq))
-            metrics["hq_bins"] = total_hq
-            metrics["mq_bins"] = total_mq
-        contig_lens = {dataset.node_names[i]: dataset.node_lengths[i] for i in range(len(dataset.node_names))}
-        if len(dataset.labels) > 1:
-            evaluate_binning(best_cluster_to_contig, node_to_label, label_to_node, contig_sizes=contig_lens)
-            # calculate overall P/R/F
-            calculate_overall_prf(best_cluster_to_contig, best_contig_to_bin, node_to_label, label_to_node, contig_lens)
-            calculate_overall_prf(
-                {
-                    cluster: best_cluster_to_contig[cluster]
-                    for cluster in best_cluster_to_contig
-                    if cluster_sizes[cluster] > args.minbin
-                },
-                {
-                    contig: best_contig_to_bin[contig]
-                    for contig in best_contig_to_bin
-                    if cluster_sizes[best_contig_to_bin[contig]] > args.minbin
-                },
-                node_to_label,
-                label_to_node,
-                contig_lens
-            )
-        if "writebins" in args.post:
-            logger.info(f"### writing bins to {args.outdir}/{args.outname}_bins/")
-            write_bins(args, dataset, best_cluster_to_contig, logger)
-        if "contig2bin" in args.post:
-            # invert cluster_to_contig
-            logger.info("### Writing contig2bin to {}/{}".format(args.outdir, args.outname))
-            with open(args.outdir + f"/{args.outname}_best_contig2bin.tsv", "w") as f:
-                f.write("@Version:0.9.0\n@SampleID:SAMPLEID\n@@SEQUENCEID\tBINID\n")
-                for c in best_contig_to_bin:
-                    f.write(f"{str(c)}\t{str(best_contig_to_bin[c])}\n")
-
-    # plot tsne embs
-    if "tsne" in args.post:
-        node_embeddings_2dim, centroids_2dim = run_tsne(final_embs, dataset, best_cluster_to_contig, hq_bins)
-        plot_embs(
-            dataset.node_names,
-            node_embeddings_2dim,
-            label_to_node,
-            centroids=centroids_2dim,
-            hq_centroids=hq_bins,
-            node_sizes=None,
-            outputname=os.path.join(args.outdir, args.outname + "_tsne_clusters.png"),
-        )
-
-        # node_sizes=[dataset.nodes_len[i][0] * 100 for i in range(len(dataset.contig_names))],
-    if "draw" in args.post:
-        print("drawing graph")
-        draw(
-            dataset,
-            node_to_label,
-            label_to_node,
-            best_cluster_to_contig,
-            os.path.join(args.outdir, args.outname + "_graph.png"),
-            graph=graph,
-        )
-
-    if "edges" in args.post:
-        logger.info(f"### writing edges to {args.outdir + args.outname}_edges")
-        write_edges(graph, os.path.join(args.outdir, args.outname + "_edges"))
-
-    if "writeembs" in args.post:
-        logger.info("### writing best and last embs to {}".format(args.outdir))
-        write_embs(final_embs, dataset.node_names, os.path.join(args.outdir, f"{args.outname}_best_embs.pickle"))
-        # write_embs(best_train_embs, dataset.node_names, os.path.join(args.outdir, f"{args.outname}_last_embs.pickle"))
-    return metrics
-
-def main():
-    parser = create_parser()
-    args = parser.parse_args()
-
-    if args.version:
-        print(f"GraphMB {__version__}")
-        exit(0)
-    if not args.read_cache:
-        check_dirs(args)
-    # set up logging
-    now = datetime.now()
-    logger = logging.getLogger(__name__)
-    loglevel = getattr(logging, args.loglevel.upper())
-    logger.setLevel(loglevel)
-    logfile = os.path.join(args.outdir, now.strftime("%Y%m%d-%H%M%S") + "{}_output.log".format(args.outname))
-    output_file_handler = logging.FileHandler(logfile)
-    print("logging to {}".format(logfile))
-    stdout_handler = logging.StreamHandler(sys.stdout)
-    logger.addHandler(output_file_handler)
-    logger.addHandler(stdout_handler)
-    logging.getLogger('matplotlib.font_manager').setLevel(logging.ERROR)
-    logging.getLogger("matplotlib").disabled = True
-    logging.getLogger("matplotlib.pyplot").disabled = True
-
-    def handle_exception(exc_type, exc_value, exc_traceback):
-        if issubclass(exc_type, KeyboardInterrupt):
-            sys.__excepthook__(exc_type, exc_value, exc_traceback)
-            return
-
-        logger.error("Uncaught exception", exc_info=(exc_type, exc_value, exc_traceback))
-
-    sys.excepthook = handle_exception
-
-    # setup tensorflow
-    if args.model_name != "sage_lstm":
-        if "torch" in sys.modules:
-            sys.modules.pop('torch')
-        os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"  # FATAL
-        import tensorflow as tf
-        #tf.get_logger().setLevel(logging.INFO)
-        clustering_device = "cpu" # avoid tf vs torch issues
-        logging.getLogger("tensorflow").setLevel(logging.INFO)
-        if not args.cuda:
-            tf.config.set_visible_devices([], "GPU")
-
-    logger.info(f"Running GraphMB {__version__}")
-    logger.debug(args)
-    # setup cuda and cpu
-    logger.info("using cuda: {}".format(str(args.cuda)))
-    device = "cuda:0" if args.cuda else "cpu"
-    clustering_device = "cuda:0" if args.cuda else "cpu"
-    logger.info("setting seed to {}".format(args.seed))
-    set_seed(args.seed)
-    use_graph = os.path.exists(os.path.join(args.assembly, args.graph_file)) or args.read_cache
-    # specify data properties for caching
-    if args.features is None:
-        if args.assembly != "":
-            features_path = os.path.join(args.assembly, "features.tsv")
-        else:
-            features_path = os.path.join(args.outdir, "features.tsv")
-    else:
-        features_path = os.path.join(args.assembly, args.features)
-
-    # create assembly object
-    dataset = AssemblyDataset(
-        name=args.outname,
-        logger=logger,
-        data_dir=args.assembly, #every file is appended to this this
-        fastafile=args.assembly_name,
-        graphfile=args.graph_file,
-        depthfile=args.depth,
-        scgfile=args.markers,
-        labelsfile=args.labels,
-        featuresfile=features_path,
-        cache_dir=args.outdir,
-        min_contig_length=args.mincontig,
-        contignodes=args.contignodes
-    )
-    if args.read_cache or (dataset.check_cache(use_graph) and not args.reload):
-        logger.info("Reading cache from".format(args.outdir))
-        dataset.read_cache(use_graph)
-    else:
-        check_dirs(args, use_features=False)
-        logger.info("Cache not found on {}".format(args.outdir))
-        dataset.read_assembly()
-        logger.info("")
-    
-    if args.markers.startswith("gtdb"):
-        dataset.read_gtdbtk_files()
-    elif args.markers != "":
-        dataset.read_scgs()
-    else:
-        args.markers = None
-
-    # load precomputed contigs with same SCGs (diff genomes)
-    if os.path.exists(f"{dataset.cache_dir}/all_different.npy"):
-        dataset.neg_pairs_idx = np.load(f"{dataset.cache_dir}/all_different.npy")
-    elif args.markers is not None:
-        dataset.get_all_different_idx()
-        np.save(f"{dataset.cache_dir}/all_different.npy", dataset.neg_pairs_idx)
-    else:
-        dataset.neg_pairs_idx = np.array([])
-        args.scg_alpha = 0
-    
-    if os.path.exists(os.path.join(args.assembly, "assembly_info.txt")):
-        logger.info("Reading assembly info file")
-        dataset.read_assembly_info()
-        dataset.print_circular_contigs()
-    # k can be user defined or dependent on the dataset
-    if args.kclusters is None:
-        args.kclusters = len(dataset.labels)
-    args.kclusters = int(args.kclusters)
-
-    # reload labels from file anyway
-    if args.labels is not None:
-        dataset.read_labels()
-    
-    if args.labelgraph:
-        dataset.generate_edges_based_on_labels()
-        dataset.calculate_homophily()
-    
-    dataset.print_stats()
-
-    target_metric = "f1"
-    if args.markers is not None:
-        target_metric = "hq"
-    elif args.labels is not None and "amber" in args.labels:
-        target_metric = "f1_avg_bp"
-    elif args.labels is None:
-        target_metric = "noeval"
-
-    # graph transformations
-    # Filter edges according to weight (could be from read overlap count or depth sim)
-    if (not args.rawfeatures and args.model_name != "vae") or args.reload:
-        if not os.path.exists(dataset.featuresfile) or args.reload:
-            from graphmb import train_ccvae
-            logger.info("==============Running VAE model=====================")
-            old_args = copy.deepcopy(args)
-            args.graph_alpha = 0 # do not use edges 
-            args.outname = "ccvae"
-            vae_embs, _ = train_ccvae.run_model_ccvae(dataset, args, logger, 0,
-                                                      use_gnn=False, epochs=args.vaepretrain,
-                                                      target_metric=target_metric)
-            logger.info("===================================================")
-            dataset.node_embs = np.array(vae_embs)
-            dataset.write_features_tsv()
-            args = old_args
-        else:
-            dataset.read_features()
-    
-    # Prepare for running multiple runs and aggregate scores
-    metrics_per_run = []
-    amber_metrics_per_run = []
-    for n in range(args.nruns):
-        logger.info("RUN {}".format(n))
-        if args.embs is not None:  # no training, just run post processing
-            emb_file = args.embs
-            with open(emb_file, "rb") as embsf:
-                best_embs_dict = pickle.load(embsf)
-                best_train_embs = np.array([best_embs_dict[i] for i in dataset.node_names])
-
-        # DGL specific code - GraphMB1
-        elif args.model_name == "sage_lstm":
-            import torch
-            from graphmb.dgl_dataset import DGLAssemblyDataset
-            torch.set_num_threads(args.numcores)
-            dgl_dataset = DGLAssemblyDataset(dataset)
-            # initialize empty features vector
-            nodes_data = torch.FloatTensor(len(dataset.node_names), 0)
-            if args.rawfeatures:
-                nodes_data = torch.cat(
-                    (nodes_data, torch.FloatTensor(dataset.node_kmers), torch.FloatTensor(dataset.node_depths)), dim=1
-                )
-            # if args.depth is not None:
-            #    dataset.nodes_data = torch.cat((dataset.nodes_data, dataset.nodes_depths), dim=1)
-            elif args.features is not None:  # append embs
-                node_embs = torch.FloatTensor(dataset.node_embs)
-                nodes_data = torch.cat((nodes_data, node_embs), dim=1)
-            dgl_dataset.graph.ndata["feat"] = nodes_data
-            # dataset.graph.ndata["len"] = torch.Tensor(dataset.nodes_len)
-
-            dgl_dataset.graph.edata["weight"] = dgl_dataset.graph.edata["weight"].float()
-            graph = dgl_dataset[0]
-            logger.info(graph)
-            graph = graph.to(device)
-
-            model = None
-            if args.embs is None and args.read_embs is False:
-                best_train_embs, model, last_train_embs, last_model, metrics = run_graphmb(dgl_dataset, args, device, logger)
-                emb_file = args.outdir + f"/{args.outname}_train_embs.pickle"
-                metrics = {k: len(v) for k, v in metrics.items()}
-            if model is None:
-                best_train_embs = graph.ndata["feat"]
-                last_train_embs = graph.ndata["feat"]
-        
-        elif args.model_name in ("sage", "gcn", "gat", "vae", "vgae") or args.model_name.endswith("_ccvae") or \
-             args.model_name.endswith("_decode") or args.model_name.endswith("_aug"):
-            best_train_embs, metrics = run_model(dataset, args, logger, nrun=n, target_metric=target_metric)
-            tf.keras.backend.clear_session()
-
-        run_post_processing(
-            best_train_embs,
-            args,
-            logger,
-            dataset,
-            clustering_device,
-            dataset.label_to_node,
-            dataset.node_to_label,
-            seed=args.seed,
-        )
-
-        if args.labels is not None: # or "contig2bin" in args.post:
-            from graphmb.amber_eval import amber_eval
-            amber_metrics, bin_counts = amber_eval(
-                os.path.join(args.assembly, args.labels), args.outdir + f"/{args.outname}_{n}_best_contig2bin.tsv", ["graphmb"]
-            )
-        #if args.labels is not None:
-            hq = bin_counts["> 90% completeness"][1]
-            mq = bin_counts["> 50% completeness"][1]
-            amber_metrics["hq"] = hq
-            amber_metrics["mq"] = mq
-            amber_metrics_per_run.append(amber_metrics)
-        metrics_per_run.append(metrics)
-        args.seed += 1
-        set_seed(args.seed)
-
-    metrics_names = metrics_per_run[0].keys()
-    for mname in metrics_names:
-        values = [m.get(mname, 0) for m in metrics_per_run]
-        logger.info("### {}: {:.3f} {:.3f}".format(mname, np.mean(values), np.std(values)))
-    hqs = [m["hq"] for m in metrics_per_run]
-    mqs = [m["mq"] for m in metrics_per_run]
-    logger.info("{:.1f} {:.1f} {:.1f} {:.1f}".format(np.mean(hqs), np.std(hqs), np.mean(mqs), np.std(mqs)))
-    if args.labels is not None:
-        #amber_metrics_names = amber_metrics_per_run[0].keys()
-        amber_metrics_names = ["precision_avg_bp", "recall_avg_bp", "f1_avg_bp", "hq", "mq"]
-        for mname in amber_metrics_names:
-            values = [m[mname] for m in amber_metrics_per_run]
-            logger.info("### amber eval {}: {:.4f} {:.4f} ###".format(mname, np.mean(values), np.std(values)))
-    total_time = datetime.now() - now
-    print("Total run time: {}".format(total_time))
-    print("Seconds per run: {:.2f}".format(total_time.total_seconds() / args.nruns))
-
-if __name__ == "__main__":
-    main()
+
+import logging
+from datetime import datetime
+from collections import Counter
+import numpy as np
+import sys
+import os
+import copy
+import pickle
+import shutil
+import pdb
+import networkx as nx
+
+from pathlib import Path
+from graphmb.arg_options import create_parser
+from graphmb.evaluate import (
+    evaluate_contig_sets,
+    calculate_overall_prf,
+)
+from graphmb.contigsdataset import AssemblyDataset
+from graphmb.visualize import draw_nx_graph, run_tsne, plot_embs
+from graphmb.utils import set_seed, get_cluster_mask
+from graphmb.graphmb1 import (cluster_embs,
+    evaluate_binning,
+    calculate_bin_metrics,
+    )
+
+from graphmb.version import __version__
+
+def run_model(dataset, args, logger, nrun, target_metric):
+    if args.model_name.endswith("_ccvae"):
+        from graphmb import train_ccvae
+        return train_ccvae.run_model_ccvae(dataset, args, logger, nrun, target_metric)
+    # TODO: this should be equivalent to running ccvae with both alpha params set to 0
+    #elif args.model_name == "vae":
+    #    from graphmb import train_vae
+    #    return train_vae.run_model_vae(dataset, args, logger, nrun)
+    elif args.model_name in ("gcn", "sage", "gat"):
+        from graphmb import train_gnn
+        return train_gnn.run_model_gnn(dataset, args, logger, nrun, target_metric)
+
+def draw(dataset, node_to_label, label_to_node, cluster_to_contig, outname, graph=None):
+    # properties of all nodes
+    nodeid_to_label = {i: node_to_label.get(n, "NA") for i, n in enumerate(dataset.node_names)}
+    contig_lens = {i: dataset.node_lengths[i] for i in range(len(dataset.node_names))}
+    nodes_titles = {
+        i: str(dataset.node_names[i]) + "<br>Length: " + str(contig_lens[i]) for i in range(len(dataset.contig_names))
+    }
+    if dataset.depth is not None:
+        nodes_titles = {
+            i: nodes_titles[i] + "<br>Depth: " + ", ".join(["{:.4}".format(x) for x in dataset.nodes_depths[i]])
+            for i in range(len(dataset.contig_names))
+        }
+    if cluster_to_contig:
+        contig_to_cluster = {contig: cluster for cluster, contigs in cluster_to_contig.items() for contig in contigs}
+        nodes_titles = {
+            i: nodes_titles[i] + "<br>Cluster: " + str(contig_to_cluster[n])
+            for i, n in enumerate(dataset.contig_names)
+        }
+
+    # convert DGL graph to networkx
+    nx_graph = graph.cpu().to_networkx(edge_attrs=["weight"]).to_undirected()
+    connected_comp = [c for c in sorted(nx.connected_components(nx_graph), key=len, reverse=True) if len(c) > 0]
+    # draw connected components to separate files
+    for i in range(10, 50):
+        # without_largest_comp = [item for sublist in connected_comp[10:110] for item in sublist if len(sublist) > 2]
+        this_comp = connected_comp[i]
+        nx_graph = nx.subgraph(nx_graph, this_comp)
+
+        draw_nx_graph(
+            nx_graph,
+            nodeid_to_label,
+            label_to_node,
+            outname + "_" + str(i),
+            contig_sizes=contig_lens,
+            node_titles=nodes_titles,
+        )
+
+
+def write_embs(embs, node_names, outname):
+    # write embs as dict node_name: embs
+    embs_dict = {node_names[i]: embs[i] for i in range(len(embs))}
+    with open(outname, "wb") as f:
+        pickle.dump(embs_dict, f)
+
+def write_edges(graph, outname):
+    with open(outname, "w") as graphf:
+        for e in zip(graph.edges()[0], graph.edges()[1]):
+            graphf.write(str(e[0].item()) + "\t" + str(e[1].item()) + "\n")
+
+
+def check_dirs(args, use_features=True):
+    """Check if files necessary to run exist, other wise print message and exit"""
+    if args.outdir is None:
+        if args.assembly is None:
+            print("Please specify assembly path or outdir with --assembly or --outdir")
+            exit()
+        else:
+            args.outdir = args.assembly
+    else:
+        Path(args.outdir).mkdir(parents=True, exist_ok=True)
+
+    # check if other dirs exists
+    if not os.path.exists(os.path.join(args.assembly, args.graph_file)):
+        print(f"Assembly Graph file {args.graph_file} not found, check --graph_file option")
+    if not os.path.exists(os.path.join(args.assembly, args.features)) or not use_features:
+
+        # needs assembly files to calculate features
+        if not os.path.exists(os.path.join(args.assembly, args.assembly_name)):
+            print(f"Assembly {args.assembly_name} not found, check --assembly_name option")
+            exit()
+        if not os.path.exists(os.path.join(args.assembly, args.depth)):
+            print(f"Depth file {args.depth} not found, check --depth option, not using depths")
+            #exit()
+
+
+def get_activation(args):
+    # pick activation function
+    import torch.nn as nn
+    if args.activation == "prelu":
+        activation = nn.PReLU(args.hidden_gnn)
+    elif args.activation == "relu":
+        activation = nn.ReLU()
+    elif args.activation == "tanh":
+        activation = nn.Tanh()
+    elif args.activation == "sigmoid":
+        activation = nn.Sigmoid()
+    elif args.activation == "lrelu":
+        activation = nn.LeakyReLU()
+    return activation
+
+
+def run_graphmb(dataset, args, device, logger):
+    from graphmb.graphsage_unsupervised import train_graphsage, SAGE
+    activation = get_activation(args)
+    model = SAGE(
+        dataset.graph.ndata["feat"].shape[1],
+        args.hidden_gnn,
+        args.embsize_gnn,
+        args.layers_gnn,
+        activation,
+        args.dropout_gnn,
+        agg=args.aggtype
+    )
+    model = model.to(device)
+
+    if model is not None:
+        model = model.to(device)
+
+    cluster_mask = get_cluster_mask(args.quick, dataset.assembly)
+    logging.info(model)
+    if (
+        dataset.assembly.ref_marker_sets is not None
+        and args.clusteringalgo is not None
+        and not args.skip_preclustering
+    ):
+        # cluster using only input features
+        logger.info("pre train clustering:")
+        pre_cluster_to_contig, centroids = cluster_embs(
+            dataset.graph.ndata["feat"].detach().cpu().numpy()[cluster_mask],
+            np.array(dataset.assembly.node_names)[cluster_mask],
+            args.clusteringalgo,
+            args.kclusters,
+            device=device,
+            # node_lens=np.array([c[0] for c in dataset.assembly.nodes_len]),
+            node_lens=np.array(dataset.assembly.node_lengths)[cluster_mask],
+            seed=args.seed,
+        )
+        results = evaluate_contig_sets(
+            dataset.assembly.ref_marker_sets, dataset.assembly.contig_markers, pre_cluster_to_contig
+        )
+        metrics = calculate_bin_metrics(results)
+        logger.info(f"HQ: {len(metrics['hq'])}, MQ:, {len(metrics['mq'])} Total bins: {len(metrics['total'])}")
+
+    best_train_embs, best_model, last_train_embs, last_model, metrics = train_graphsage(
+        dataset,
+        model,
+        batch_size=args.batchsize,
+        fan_out=args.fanout,
+        num_negs=args.negatives,
+        neg_share=False,
+        num_epochs=args.epoch,
+        lr=args.lr_gnn,
+        k=args.kclusters,
+        clusteringalgo=args.clusteringalgo,
+        cluster_features=args.concatfeatures,
+        print_interval=args.print,
+        loss_weights=(not args.no_loss_weights),
+        sample_weights=(not args.no_sample_weights),
+        logger=logger,
+        device=device,
+        epsilon=args.early_stopping,
+        evalepochs=args.evalepochs,
+        seed=args.seed,
+        eval_skip=args.evalskip,
+        quick=args.quick
+    )
+    return best_train_embs, best_model, last_train_embs, last_model, metrics
+
+
+def write_bins(args, dataset, cluster_to_contig, logger):
+    bin_dir = Path(args.outdir + "/{}_bins/".format(args.outname))
+    bin_dir.mkdir(parents=True, exist_ok=True)
+    [f.unlink() for f in bin_dir.glob("*.fa") if f.is_file()]
+    clustered_contigs = set()
+    multi_contig_clusters = 0
+    logger.info(f"{len(cluster_to_contig)} clusters")
+    short_contigs = set()
+    skipped_clusters = 0
+    for c in cluster_to_contig:
+        cluster_size = sum([dataset.node_lengths[dataset.node_names.index(contig)] for contig in cluster_to_contig[c]])
+        if cluster_size < args.minbin:
+            # print("skipped small cluster", len(cluster_to_contig[c]), "contig")
+            for contig in cluster_to_contig[c]:
+                short_contigs.add(contig)
+            skipped_clusters += 1
+            continue
+        multi_contig_clusters += 1
+        with open(bin_dir / f"{c}.fa", "w") as binfile:
+            for contig in cluster_to_contig[c]:
+                binfile.write(">" + contig + "\n")
+                binfile.write(dataset.node_seqs[contig] + "\n")
+                clustered_contigs.add(contig)
+        # print("multi cluster", c, "size", cluster_size, "contigs", len(cluster_to_contig[c]))
+    logger.info("### skipped {} clusters while writing to file".format(skipped_clusters))
+    single_clusters = multi_contig_clusters
+    left_over = set(dataset.node_names) - clustered_contigs - short_contigs
+    for c in left_over:
+        if c not in clustered_contigs and len(dataset.node_seqs[c]) > args.minbin:
+
+            with open(bin_dir / f"{single_clusters}.fna", "w") as binfile:
+                binfile.write(">" + c + "\n")
+                binfile.write(dataset.node_seqs[c] + "\n")
+                single_clusters += 1
+            # print("contig", single_clusters, "size", len(dataset.contig_seqs[c]))
+    logger.info(f"### wrote {single_clusters} clusters {multi_contig_clusters} >= #contig {args.mincomp}")
+
+
+def run_post_processing(final_embs, args, logger, dataset, device, label_to_node, node_to_label, seed):
+    metrics = {}
+    if "cluster" in args.post or "kmeans" in args.post:
+        logger.info("#### clustering embs with {} ({})".format(args.clusteringalgo, args.kclusters))
+        # train_embs = last_train_embs
+
+        if args.clusteringalgo is False:
+            args.clusteringalgo = "kmeans"
+        if not isinstance(final_embs, np.ndarray):
+            if args.cuda:
+                final_embs = final_embs.cpu()
+            final_embs = final_embs.numpy()
+
+            # last_train_embs should already be detached and on cpu
+        best_cluster_to_contig, best_centroids = cluster_embs(
+            final_embs,
+            dataset.node_names,
+            args.clusteringalgo,
+            # len(dataset.connected),
+            args.kclusters,
+            device=device,
+            seed=seed,
+        )
+        cluster_sizes = {}
+        for c in best_cluster_to_contig:
+            cluster_size = sum([len(dataset.node_seqs[contig]) for contig in best_cluster_to_contig[c]])
+            cluster_sizes[c] = cluster_size
+        best_contig_to_bin = {}
+        for bin in best_cluster_to_contig:
+            for contig in best_cluster_to_contig[bin]:
+                best_contig_to_bin[contig] = bin
+        # run for best epoch only
+        if args.markers is not None:
+            total_hq = 0
+            total_mq = 0
+            results = evaluate_contig_sets(dataset.ref_marker_sets, dataset.contig_markers, best_cluster_to_contig)
+            hq_bins = set()
+            for binid in results:
+                if results[binid]["comp"] > 90 and results[binid]["cont"] < 5:
+                    contig_labels = [dataset.node_to_label.get(node, 0) for node in best_cluster_to_contig[binid]]
+                    labels_count = Counter(contig_labels)
+                    # logger.debug(
+                    #    f"{binid}, {round(results[binid]['comp'],4)}, {round(results[binid]['cont'],4)}, "
+                    #    f"{len(best_cluster_to_contig[binid])} {labels_count}"
+                    # )
+                    hq_bins.add(binid)
+                    total_hq += 1
+                if results[binid]["comp"] > 50 and results[binid]["cont"] < 10:
+                    total_mq += 1
+            logger.info("#### Total HQ {} ####".format(total_hq))
+            logger.info("#### Total MQ {} ####".format(total_mq))
+            metrics["hq_bins"] = total_hq
+            metrics["mq_bins"] = total_mq
+        contig_lens = {dataset.node_names[i]: dataset.node_lengths[i] for i in range(len(dataset.node_names))}
+        if len(dataset.labels) > 1:
+            evaluate_binning(best_cluster_to_contig, node_to_label, label_to_node, contig_sizes=contig_lens)
+            # calculate overall P/R/F
+            calculate_overall_prf(best_cluster_to_contig, best_contig_to_bin, node_to_label, label_to_node, contig_lens)
+            calculate_overall_prf(
+                {
+                    cluster: best_cluster_to_contig[cluster]
+                    for cluster in best_cluster_to_contig
+                    if cluster_sizes[cluster] > args.minbin
+                },
+                {
+                    contig: best_contig_to_bin[contig]
+                    for contig in best_contig_to_bin
+                    if cluster_sizes[best_contig_to_bin[contig]] > args.minbin
+                },
+                node_to_label,
+                label_to_node,
+                contig_lens
+            )
+        if "writebins" in args.post:
+            logger.info(f"### writing bins to {args.outdir}/{args.outname}_bins/")
+            write_bins(args, dataset, best_cluster_to_contig, logger)
+        if "contig2bin" in args.post:
+            # invert cluster_to_contig
+            logger.info("### Writing contig2bin to {}/{}".format(args.outdir, args.outname))
+            with open(args.outdir + f"/{args.outname}_best_contig2bin.tsv", "w") as f:
+                f.write("@Version:0.9.0\n@SampleID:SAMPLEID\n@@SEQUENCEID\tBINID\n")
+                for c in best_contig_to_bin:
+                    f.write(f"{str(c)}\t{str(best_contig_to_bin[c])}\n")
+
+    # plot tsne embs
+    if "tsne" in args.post:
+        node_embeddings_2dim, centroids_2dim = run_tsne(final_embs, dataset, best_cluster_to_contig, hq_bins)
+        plot_embs(
+            dataset.node_names,
+            node_embeddings_2dim,
+            label_to_node,
+            centroids=centroids_2dim,
+            hq_centroids=hq_bins,
+            node_sizes=None,
+            outputname=os.path.join(args.outdir, args.outname + "_tsne_clusters.png"),
+        )
+
+        # node_sizes=[dataset.nodes_len[i][0] * 100 for i in range(len(dataset.contig_names))],
+    if "draw" in args.post:
+        print("drawing graph")
+        draw(
+            dataset,
+            node_to_label,
+            label_to_node,
+            best_cluster_to_contig,
+            os.path.join(args.outdir, args.outname + "_graph.png"),
+            graph=graph,
+        )
+
+    if "edges" in args.post:
+        logger.info(f"### writing edges to {args.outdir + args.outname}_edges")
+        write_edges(graph, os.path.join(args.outdir, args.outname + "_edges"))
+
+    if "writeembs" in args.post:
+        logger.info("### writing best and last embs to {}".format(args.outdir))
+        write_embs(final_embs, dataset.node_names, os.path.join(args.outdir, f"{args.outname}_best_embs.pickle"))
+        # write_embs(best_train_embs, dataset.node_names, os.path.join(args.outdir, f"{args.outname}_last_embs.pickle"))
+    return metrics
+
+def main():
+    parser = create_parser()
+    args = parser.parse_args()
+
+    if args.version:
+        print(f"GraphMB {__version__}")
+        exit(0)
+    if not args.read_cache:
+        check_dirs(args)
+    # set up logging
+    now = datetime.now()
+    logger = logging.getLogger(__name__)
+    loglevel = getattr(logging, args.loglevel.upper())
+    logger.setLevel(loglevel)
+    logfile = os.path.join(args.outdir, now.strftime("%Y%m%d-%H%M%S") + "{}_output.log".format(args.outname))
+    output_file_handler = logging.FileHandler(logfile)
+    print("logging to {}".format(logfile))
+    stdout_handler = logging.StreamHandler(sys.stdout)
+    logger.addHandler(output_file_handler)
+    logger.addHandler(stdout_handler)
+    logging.getLogger('matplotlib.font_manager').setLevel(logging.ERROR)
+    logging.getLogger("matplotlib").disabled = True
+    logging.getLogger("matplotlib.pyplot").disabled = True
+
+    def handle_exception(exc_type, exc_value, exc_traceback):
+        if issubclass(exc_type, KeyboardInterrupt):
+            sys.__excepthook__(exc_type, exc_value, exc_traceback)
+            return
+
+        logger.error("Uncaught exception", exc_info=(exc_type, exc_value, exc_traceback))
+
+    sys.excepthook = handle_exception
+
+    # setup tensorflow
+    if args.model_name != "sage_lstm":
+        if "torch" in sys.modules:
+            sys.modules.pop('torch')
+        os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"  # FATAL
+        import tensorflow as tf
+        #tf.get_logger().setLevel(logging.INFO)
+        clustering_device = "cpu" # avoid tf vs torch issues
+        logging.getLogger("tensorflow").setLevel(logging.INFO)
+        if not args.cuda:
+            tf.config.set_visible_devices([], "GPU")
+
+    logger.info(f"Running GraphMB {__version__}")
+    logger.debug(args)
+    # setup cuda and cpu
+    logger.info("using cuda: {}".format(str(args.cuda)))
+    device = "cuda:0" if args.cuda else "cpu"
+    clustering_device = "cuda:0" if args.cuda else "cpu"
+    logger.info("setting seed to {}".format(args.seed))
+    set_seed(args.seed)
+    use_graph = os.path.exists(os.path.join(args.assembly, args.graph_file)) or args.read_cache
+    # specify data properties for caching
+    if args.features is None:
+        if args.assembly != "":
+            features_path = os.path.join(args.assembly, "features.tsv")
+        else:
+            features_path = os.path.join(args.outdir, "features.tsv")
+    else:
+        features_path = os.path.join(args.assembly, args.features)
+
+    # create assembly object
+    dataset = AssemblyDataset(
+        name=args.outname,
+        logger=logger,
+        data_dir=args.assembly, #every file is appended to this this
+        fastafile=args.assembly_name,
+        graphfile=args.graph_file,
+        depthfile=args.depth,
+        scgfile=args.markers,
+        labelsfile=args.labels,
+        featuresfile=features_path,
+        cache_dir=args.outdir,
+        min_contig_length=args.mincontig,
+        contignodes=args.contignodes
+    )
+    if args.read_cache or (dataset.check_cache(use_graph) and not args.reload):
+        logger.info("Reading cache from".format(args.outdir))
+        dataset.read_cache(use_graph)
+    else:
+        check_dirs(args, use_features=False)
+        logger.info("Cache not found on {}".format(args.outdir))
+        dataset.read_assembly()
+        logger.info("")
+    
+    if args.markers.startswith("gtdb"):
+        dataset.read_gtdbtk_files()
+    elif args.markers != "" and os.path.exists(os.path.join(args.assembly, args.markers)):
+        dataset.read_scgs()
+    else:
+        logger.info(f"Not using SCG file: {args.markers} (not found)")
+        args.markers = None
+
+    # load precomputed contigs with same SCGs (diff genomes)
+    if os.path.exists(f"{dataset.cache_dir}/all_different.npy"):
+        dataset.neg_pairs_idx = np.load(f"{dataset.cache_dir}/all_different.npy")
+    elif args.markers is not None:
+        dataset.get_all_different_idx()
+        np.save(f"{dataset.cache_dir}/all_different.npy", dataset.neg_pairs_idx)
+    else:
+        dataset.neg_pairs_idx = np.array([])
+        args.scg_alpha = 0
+    
+    if os.path.exists(os.path.join(args.assembly, "assembly_info.txt")):
+        logger.info("Reading assembly info file")
+        dataset.read_assembly_info()
+        dataset.print_circular_contigs()
+    # k can be user defined or dependent on the dataset
+    if args.kclusters is None:
+        args.kclusters = len(dataset.labels)
+    args.kclusters = int(args.kclusters)
+
+    # reload labels from file anyway
+    if args.labels is not None:
+        dataset.read_labels()
+    
+    if args.labelgraph:
+        dataset.generate_edges_based_on_labels()
+        dataset.calculate_homophily()
+    
+    dataset.print_stats()
+
+    target_metric = "f1"
+    if args.markers is not None:
+        target_metric = "hq"
+    elif args.labels is not None and "amber" in args.labels:
+        target_metric = "f1_avg_bp"
+    elif args.labels is None:
+        target_metric = "noeval"
+
+    # graph transformations
+    # Filter edges according to weight (could be from read overlap count or depth sim)
+    if (not args.rawfeatures and args.model_name != "vae") or args.reload:
+        if not os.path.exists(dataset.featuresfile) or args.reload:
+            from graphmb import train_ccvae
+            logger.info("==============Running VAE model=====================")
+            old_args = copy.deepcopy(args)
+            args.graph_alpha = 0 # do not use edges 
+            args.outname = "ccvae"
+            vae_embs, _ = train_ccvae.run_model_ccvae(dataset, args, logger, 0,
+                                                      use_gnn=False, epochs=args.vaepretrain,
+                                                      target_metric=target_metric)
+            logger.info("===================================================")
+            dataset.node_embs = np.array(vae_embs)
+            dataset.write_features_tsv()
+            args = old_args
+        else:
+            dataset.read_features()
+    
+    # Prepare for running multiple runs and aggregate scores
+    metrics_per_run = []
+    amber_metrics_per_run = []
+    for n in range(args.nruns):
+        logger.info("RUN {}".format(n))
+        if args.embs is not None:  # no training, just run post processing
+            emb_file = args.embs
+            with open(emb_file, "rb") as embsf:
+                best_embs_dict = pickle.load(embsf)
+                best_train_embs = np.array([best_embs_dict[i] for i in dataset.node_names])
+
+        # DGL specific code - GraphMB1
+        elif args.model_name == "sage_lstm":
+            import torch
+            from graphmb.dgl_dataset import DGLAssemblyDataset
+            torch.set_num_threads(args.numcores)
+            dgl_dataset = DGLAssemblyDataset(dataset)
+            # initialize empty features vector
+            nodes_data = torch.FloatTensor(len(dataset.node_names), 0)
+            if args.rawfeatures:
+                nodes_data = torch.cat(
+                    (nodes_data, torch.FloatTensor(dataset.node_kmers), torch.FloatTensor(dataset.node_depths)), dim=1
+                )
+            # if args.depth is not None:
+            #    dataset.nodes_data = torch.cat((dataset.nodes_data, dataset.nodes_depths), dim=1)
+            elif args.features is not None:  # append embs
+                node_embs = torch.FloatTensor(dataset.node_embs)
+                nodes_data = torch.cat((nodes_data, node_embs), dim=1)
+            dgl_dataset.graph.ndata["feat"] = nodes_data
+            # dataset.graph.ndata["len"] = torch.Tensor(dataset.nodes_len)
+
+            dgl_dataset.graph.edata["weight"] = dgl_dataset.graph.edata["weight"].float()
+            graph = dgl_dataset[0]
+            logger.info(graph)
+            graph = graph.to(device)
+
+            model = None
+            if args.embs is None and args.read_embs is False:
+                best_train_embs, model, last_train_embs, last_model, metrics = run_graphmb(dgl_dataset, args, device, logger)
+                emb_file = args.outdir + f"/{args.outname}_train_embs.pickle"
+                metrics = {k: len(v) for k, v in metrics.items()}
+            if model is None:
+                best_train_embs = graph.ndata["feat"]
+                last_train_embs = graph.ndata["feat"]
+        
+        elif args.model_name in ("sage", "gcn", "gat", "vae", "vgae") or args.model_name.endswith("_ccvae") or \
+             args.model_name.endswith("_decode") or args.model_name.endswith("_aug"):
+            best_train_embs, metrics, contig_labels = run_model(dataset, args, logger, nrun=n, target_metric=target_metric)
+            tf.keras.backend.clear_session()
+
+        run_post_processing(
+            best_train_embs,
+            args,
+            logger,
+            dataset,
+            clustering_device,
+            dataset.label_to_node,
+            dataset.node_to_label,
+            seed=args.seed,
+        )
+        breakpoint()
+        if args.writebins:
+            cluster_to_contig = {k: [] for k in set(contig_labels)}
+            for contig, label in enumerate(contig_labels):
+                cluster_to_contig[label].append(dataset.node_names[contig])
+            write_bins(args, dataset, cluster_to_contig, logger)
+
+        if args.labels is not None: # or "contig2bin" in args.post:
+            from graphmb.amber_eval import amber_eval
+            amber_metrics, bin_counts = amber_eval(
+                os.path.join(args.assembly, args.labels), args.outdir + f"/{args.outname}_{n}_best_contig2bin.tsv", ["graphmb"]
+            )
+        #if args.labels is not None:
+            hq = bin_counts["> 90% completeness"][1]
+            mq = bin_counts["> 50% completeness"][1]
+            amber_metrics["hq"] = hq
+            amber_metrics["mq"] = mq
+            amber_metrics_per_run.append(amber_metrics)
+        metrics_per_run.append(metrics)
+        args.seed += 1
+        set_seed(args.seed)
+
+    metrics_names = metrics_per_run[0].keys()
+    for mname in metrics_names:
+        values = [m.get(mname, 0) for m in metrics_per_run]
+        logger.info("### {}: {:.3f} {:.3f}".format(mname, np.mean(values), np.std(values)))
+    hqs = [m["hq"] for m in metrics_per_run]
+    mqs = [m["mq"] for m in metrics_per_run]
+    logger.info("{:.1f} {:.1f} {:.1f} {:.1f}".format(np.mean(hqs), np.std(hqs), np.mean(mqs), np.std(mqs)))
+    if args.labels is not None:
+        #amber_metrics_names = amber_metrics_per_run[0].keys()
+        amber_metrics_names = ["precision_avg_bp", "recall_avg_bp", "f1_avg_bp", "hq", "mq"]
+        for mname in amber_metrics_names:
+            values = [m[mname] for m in amber_metrics_per_run]
+            logger.info("### amber eval {}: {:.4f} {:.4f} ###".format(mname, np.mean(values), np.std(values)))
+    total_time = datetime.now() - now
+    print("Total run time: {}".format(total_time))
+    print("Seconds per run: {:.2f}".format(total_time.total_seconds() / args.nruns))
+
+if __name__ == "__main__":
+    main()
```

### Comparing `graphmb-0.2.4/src/graphmb/models.py` & `graphmb-0.2.5/src/graphmb/models.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,642 +1,642 @@
-from os import uname
-import tensorflow as tf
-
-from tensorflow.keras.optimizers import Adam, SGD
-from tensorflow.keras.models import Model
-from tensorflow.keras.layers import Input, Dense, Activation, Softmax, Embedding, LayerNormalization
-#from tensorflow.keras import Sequential
-from tensorflow.keras.layers import BatchNormalization, Lambda, LeakyReLU, Flatten
-from tensorflow.keras.layers import Dropout, Add, Concatenate
-from tensorflow.keras.losses import SparseCategoricalCrossentropy
-import numpy as np
-from tensorflow.keras.regularizers import l2    
-from tqdm import tqdm
-
-#import tensorflow_probability as tfp
-
-class VAEEncoder(Model):
-    def __init__(self, abundance_dim, kmers_dim, hiddendim, zdim=64, dropout=0, layers=2):
-        super(VAEEncoder, self).__init__()
-        self.abundance_dim = abundance_dim
-        self.kmers_dim = kmers_dim
-        self.zdim = zdim
-        in_ = Input(shape=(abundance_dim+kmers_dim,))
-        x = in_
-        for i in range(layers):
-            x = Dense(hiddendim, activation='linear', name=f"encoder_{i}")(x)
-            x = LeakyReLU(0.01)(x)
-            if dropout > 0:
-                x = Dropout(dropout)(x)
-            x = BatchNormalization()(x)
-        mu = Dense(zdim, name="mu")(x)
-        logvar = Dense(zdim, kernel_initializer='zeros', name="logvar")(x)
-        self.model = Model(in_, [mu, logvar])
- 
-    def call(self, x, training=False):
-        mu, sigma = self.model(x, training=training)
-        return mu, sigma
-
-    
-class VAEDecoder(Model):
-    def __init__(self, abundance_dim, kmers_dim, hiddendim, zdim=64, dropout=0, layers=2):
-        super(VAEDecoder, self).__init__()
-        self.abundance_dim = abundance_dim
-        self.kmers_dim = kmers_dim
-        self.zdim = zdim
-        in_ = Input(shape=(zdim,))
-        x = in_
-        for i in range(layers):
-            x = Dense(hiddendim, activation='linear', name=f"decoder_{i}")(x)
-            x = LeakyReLU(0.01)(x)
-            if dropout > 0:
-                x = Dropout(dropout)(x)
-            x = BatchNormalization()(x)
-            
-        x1 = Dense(abundance_dim, name="decoder_ab")(x)
-        x2 = Dense(kmers_dim, name="decoder_kmer")(x)
-        if self.abundance_dim > 1:
-            x1 = Softmax()(x1)
-        x = Concatenate()((x1,x2))
-        
-        self.model = Model(in_, x)
- 
-    def call(self, z, training=False):
-        x_hat = self.model(z, training=training)
-        return x_hat
-
-class Encoder(Model):
-    def __init__(self, features_dim, hiddendim, zdim=64, dropout=0, layers=2):
-        super(VAEEncoder, self).__init__()
-        self.zdim = zdim
-        in_ = Input(shape=(features_dim,))
-        x = in_
-        for i in range(layers):
-            x = Dense(hiddendim, activation='linear', name=f"encoder_{i}")(x)
-            x = LeakyReLU(0.01)(x)
-            if dropout > 0:
-                x = Dropout(dropout)(x)
-            x = BatchNormalization()(x)
-        mu = Dense(zdim, name="mu")(x)
-        logvar = Dense(zdim, kernel_initializer='zeros', name="logvar")(x)
-        self.model = Model(in_, [mu, logvar])
- 
-    def call(self, x, training=False):
-        mu, sigma = self.model(x, training=training)
-        return mu, sigma
-
-    
-class Decoder(Model):
-    def __init__(self, features_dim, hiddendim, zdim=64, dropout=0, layers=2):
-        super(VAEDecoder, self).__init__()
-        self.features_dim = features_dim
-        self.zdim = zdim
-        in_ = Input(shape=(zdim,))
-        x = in_
-        for i in range(layers):
-            x = Dense(hiddendim, activation='linear', name=f"decoder_{i}")(x)
-            x = LeakyReLU(0.01)(x)
-            if dropout > 0:
-                x = Dropout(dropout)(x)
-            x = BatchNormalization()(x)
-            
-        x = Dense(features_dim, name="decoder_ab")(x)
-        #x2 = Dense(kmers_dim, name="decoder_kmer")(x)
-        #if self.abundance_dim > 1:
-        #    x1 = Softmax()(x1)
-        #x = Concatenate()((x1,x2))
-        
-        self.model = Model(in_, x)
- 
-    def call(self, z, training=False):
-        x_hat = self.model(z, training=training)
-        return x_hat
-
-
-class LabelClassifier(Model):
-    def __init__(self, n_classes, hiddendim=128, zdim=64, dropout=0, layers=1):
-        super(LabelClassifier, self).__init__()
-        in_ = Input(shape=(zdim,))
-        x = in_
-        for nl in range(layers):
-            if nl == layers-1:
-                x = Dense(n_classes, activation='softmax')(x)
-            else:
-                x = Dense(hiddendim, activation='linear')(x)
-                #x = LeakyReLU(0.01)(x)
-                if dropout > 0:
-                    x = Dropout(dropout)(x)
-
-        self.model = Model(in_, x)
-        self.loss_fn = SparseCategoricalCrossentropy()
- 
-    def call(self, z, mask, training=False):
-        predictions = self.model(tf.gather(params=z, indices=mask), training=training)
-        return predictions
-
-    def loss(self, gold_labels, predicted_labels):
-        return self.loss_fn(y_true=gold_labels,y_pred=predicted_labels)
-
-class TrainHelperVAE:
-    def __init__(self, encoder, decoder, learning_rate=1e-3,  kld_weight=1/200.,
-                train_weights=False, classification=False, n_classes=0,
-                gold_labels=None, mask_labels=0.0, ae_alpha=1):
-        self.encoder = encoder
-        self.decoder = decoder
-        self.train_weights = train_weights
-        self.abundance_dim = self.encoder.abundance_dim
-        self.kmers_dim = self.encoder.kmers_dim
-        self.ae_alpha = ae_alpha
-        if train_weights:
-            #self.kld_weight = tf.Variable(kld_weight)
-            self.kld_weight = kld_weight
-            #self.abundance_weight = tf.Variable(0.5)
-            self.kmer_weight = tf.Variable(0.1)
-        else:
-            self.kld_weight = kld_weight
-            if self.abundance_dim > 1:
-                #self.abundance_weight = 0.85 / tf.math.log(float(self.abundance_dim))
-                self.kmer_weight = 0.15
-            else:
-                #self.abundance_weight = 0.5
-                self.kmer_weight = 0.5
-        self.opt = tf.keras.optimizers.Adam(learning_rate=learning_rate)
-        self.logvar = None
-        self.mu = None
-        self.z = None
-        self.classify = classification
-        if self.classify:
-            self.classifier = LabelClassifier(n_classes, zdim=encoder.zdim)
-            self.gold_labels = gold_labels
-            self.mask_labels = mask_labels
-            
-    def train_step(self, x, writer=None, epoch=0, vae=True, gold_labels=None):
-        losses = self._train_step(x, vae=vae, writer=writer, epoch=epoch, gold_labels=gold_labels)
-        if writer is not None:
-            with writer.as_default():
-                tf.summary.scalar('mean logvar', self.logvar, step=epoch)
-                tf.summary.scalar('mean mu', self.mu, step=epoch)
-        losses = [loss.numpy() for loss in losses]
-        return losses
-    
-    @tf.function
-    def loss(self, x, mu, logvar, vae, training=True, writer=None, epoch=0, gold_labels=None):
-        if vae:
-            epsilon = tf.random.normal(tf.shape(mu))
-            z = mu + epsilon * tf.math.exp(0.5 * logvar)
-            kld  = 0.5*tf.math.reduce_mean(tf.math.reduce_mean(1.0 + logvar - tf.math.pow(mu, 2) - tf.math.exp(logvar), axis=1))
-            kld  = kld * self.kld_weight
-        else:
-            z = mu
-            kld = tf.convert_to_tensor(0.0)
-        x_hat = self.decoder(z, training=training)
-        if self.classify:
-            if self.mask_labels > 0:
-                use_labels = np.random.choice(z.shape[0], int(z.shape[0]*(1-self.mask_labels)))
-            else:
-                use_labels = np.arange(z.shape[0])
-            predictions = self.classifier(z, mask=use_labels)
-            prediction_loss = self.classifier.loss(gold_labels[use_labels], predictions)
-        else:
-            prediction_loss = tf.convert_to_tensor(0.0)
-        if writer is not None:
-            with writer.as_default():
-                tf.summary.scalar('min ab', tf.reduce_min(x_hat[:, :self.abundance_dim]), step=epoch)
-        if self.abundance_dim > 1:
-            mse1 = -tf.reduce_mean(tf.reduce_sum((tf.math.log(x_hat[:, :self.abundance_dim] + 1e-9) * x[:, :self.abundance_dim]), axis=1))
-        else:
-            mse1 = tf.reduce_mean( (x[:, :self.abundance_dim] - x_hat[:, :self.abundance_dim])**2)
-        if self.train_weights:
-            kmer_weight = tf.math.sigmoid(self.kmer_weight)
-        else:
-            kmer_weight = self.kmer_weight
-        mse1 *= (1-kmer_weight)
-        mse2 = kmer_weight*tf.reduce_mean( tf.reduce_mean((x[:, self.abundance_dim:] - x_hat[:, self.abundance_dim:])**2, axis=1))
-
-        return mse1, mse2, kld, prediction_loss
-
-    @tf.function
-    def _train_step(self, x, vae=True, writer=None, epoch=0, gold_labels=None):
-        with tf.GradientTape() as tape:
-            mu, logvar = self.encoder(x, training=True)
-            logvar = tf.clip_by_value(logvar, -2, 2)
-            self.logvar = tf.cast(tf.math.reduce_mean(logvar), float)
-            self.mu = tf.cast(tf.math.reduce_mean(mu), float)
-            mse1, mse2, kld, predl = self.loss(x, mu, logvar, vae, training=True,
-                                               writer=writer, epoch=epoch,
-                                               gold_labels=gold_labels)
-            loss = mse1 + mse2 - kld + predl
-            loss *= self.ae_alpha
-        tw = self.encoder.trainable_weights + self.decoder.trainable_weights 
-        if self.train_weights:
-            tw += [self.kmer_weight] # self.kld_weight
-        if self.classify:
-            tw += self.classifier.trainable_weights
-        grads = tape.gradient(loss, tw)
-        grad_norm = tf.linalg.global_norm(grads)
-        clip_grads, _ = tf.clip_by_global_norm(grads, 5,  use_norm=grad_norm)
-        new_grad_norm = tf.linalg.global_norm(clip_grads)
-        self.opt.apply_gradients(zip(clip_grads, tw))
-
-        if writer is not None:
-            with writer.as_default():
-                tf.summary.scalar('grad norm', grad_norm, step=epoch)
-                tf.summary.scalar('clipped grad norm', new_grad_norm, step=epoch)
-
-        return loss, mse2, mse1, kld, predl
-
-
-class NoiseModel(Model):
-    def __init__(self, abundance_dim, emb_dim, hiddendim=128, dropout=0, layers=1):
-        super(NoiseModel, self).__init__()
-        self.abundance_dim = abundance_dim
-        self.kmers_dim = emb_dim
-        in_ = Input(shape=((abundance_dim+emb_dim)*2,))
-        x = in_
-        for i in range(layers):
-            x = Dense(hiddendim, activation='linear', name=f"noise_{i}")(x)
-            x = LeakyReLU(0.01)(x)
-            if dropout > 0:
-                x = Dropout(dropout)(x)
-            x = BatchNormalization()(x)
-        noise = Dense(1, name="mu")(x)
-        self.model = Model(in_, noise)
- 
-    def call(self, x, training=False):
-        noise = self.model(x, training=training)
-        return noise
-
-class TH:
-    def __init__(
-        self,
-        input_features,
-        gnn_model,
-        lr=0.01,
-        all_different_idx=None,
-        all_same_idx=None,
-        ae_encoder=None,
-        ae_decoder=None,
-        decoder_input="gnn",
-        classifier=None,
-        latentdim=32,
-        graph_weight=1.0,
-        ae_weight=1.0,
-        kld_weight = 1/200,
-        scg_weight=100.0,
-        kmer_weight=0.15,
-        abundance_weight=0.85,
-        kmer_dim=103,
-        kmer_alpha=0.5,
-        num_negatives=50,
-        kmers_dim=103,
-        abundance_dim=4,
-        labels=None,
-        use_gnn=True,
-        use_noise=False,
-        loglevel="warning",
-        pretrainvae=0
-    ):
-        self.opt = Adam(learning_rate=lr, epsilon=1e-8)
-        # self.opt = SGD(learning_rate=lr)
-        self.gnn_model = gnn_model
-        self.features = input_features
-        # self.dense_adj = tf.sparse.to_dense(self.model.adj)
-        if gnn_model is not None:
-            self.adj_shape = self.gnn_model.adj.dense_shape
-        self.kmer_dim = kmer_dim
-        self.ab_dim = input_features.shape[1] - kmer_dim
-        self.kmer_alpha = kmer_alpha
-        self.num_negatives = num_negatives
-        self.nlatent = latentdim
-        self.scg_pairs = all_different_idx
-        self.all_same_idx = all_same_idx
-        self.classifier = classifier
-        self.encoder = ae_encoder
-        self.decoder = ae_decoder
-        self.decoder_input = decoder_input
-        self.use_ae = ae_encoder is not None
-        self.mse_loss = tf.keras.losses.MeanSquaredError()
-        self.graph_weight = graph_weight
-        self.ae_weight = ae_weight
-        self.kld_weight = kld_weight
-        self.scg_weight = scg_weight
-        self.kmer_weight = kmer_weight
-        self.noise_reg = 1
-        self.abundance_weight = abundance_weight
-        self.no_gnn = gnn_model is None
-        self.train_ae = False
-        self.abundance_dim = abundance_dim
-        self.kmers_dim = kmers_dim
-        self.use_gnn = use_gnn
-        self.use_noise = use_noise
-        self.loglevel = loglevel
-        self.pretrainvae = pretrainvae
-        self.epoch = 0
-
-    @tf.function
-    def sample_negatives(self, edge_idx, node_idx):
-        # for 5 negatives and batchsize 256, this should give 1% or less false negatives
-        neg_idx = tf.random.uniform(shape=(2, len(edge_idx)*self.num_negatives),
-                                    maxval=node_idx.shape[0], dtype=tf.int32)
-        # get neg idx relative to node_idx (of this batch)
-        neg_idx_row = tf.gather(params=node_idx, indices=neg_idx[0,:])
-        neg_idx_col = tf.gather(params=node_idx, indices=neg_idx[1,:])
-        return neg_idx_row, neg_idx_col
-        #return neg_idx[0,:], neg_idx[1,:]
-
-    @tf.function
-    def nodedist(self, u, v):
-        #breakpoint()
-        #return tf.reduce_sum((tf.expand_dims(x, 0) - tf.expand_dims(y, 1)**2), axis=-1)
-        u = tf.nn.l2_normalize(u, axis=1)
-        v = tf.nn.l2_normalize(v, axis=1)
-        pairwise = tf.reduce_sum(tf.math.multiply(u, v), axis=1)
-        #pairwise = -tf.norm(tf.math.subtract(u, v) + + 1.0e-12, ord='euclidean', axis=1,)
-        return pairwise
-    
-    @tf.function
-    def edge_loss(self, pos_dists, neg_dists):
-        #breakpoint()
-        y_true = tf.concat((tf.ones_like(pos_dists), tf.zeros_like(neg_dists)), axis=0)
-        y_pred = tf.concat((pos_dists, neg_dists), axis=0)
-        gnn_loss = tf.keras.metrics.binary_crossentropy(y_true, y_pred, from_logits=True)
-        return gnn_loss
-    
-    def train_vae(self, nodes_idx, vae=True):
-        if not vae: # not variational, no kld loss
-            # make logvar non trainable
-            layer_names = [layer.name for layer in self.encoder.layers[0].layers]
-            logvar_idx = layer_names.index("logvar")
-            self.encoder.layers[0].layers[logvar_idx].trainable = False
-            #ae_embs = tf.concat((self.features[:,:self.abundance_dim], self.encoder(self.features)[0]), axis=1)
-
-        ae_mu, ae_logvar = self.encoder(tf.gather(self.features, nodes_idx), training=(self.epoch < self.pretrainvae or self.pretrainvae == 0))
-        #ae_mu, ae_logvar = self.encoder(tf.gather(self.features, nodes_idx), training=True)
-        if self.decoder_input == "gnn" and self.use_gnn and (self.epoch > self.pretrainvae or self.pretrainvae == 0):
-            ae_mu = tf.scatter_nd(indices=nodes_idx[:,None],
-                                     updates=ae_mu,
-                                     shape=(self.features.shape[0], ae_mu.shape[1]))
-            ae_mu = self.gnn_model(ae_mu, nodes_idx, training=True)
-        ae_recon = self.decoder(ae_mu, training=(self.epoch < self.pretrainvae or self.pretrainvae == 0))
-        #ae_recon = self.decoder(ae_mu, training=True)
-        ae_logvar = tf.clip_by_value(ae_logvar, -2, 2)
-        try:
-            losses = self.ae_loss(tf.gather(self.features, nodes_idx), ae_recon, ae_mu, ae_logvar, vae=vae)
-        except:
-            breakpoint()
-        ae_loss = tf.reduce_sum(losses) * self.ae_weight
-        ae_losses = {"kmer_loss": losses[0],
-                        "ab_loss": losses[1],
-                        "kld": losses[2],
-                        "vae_loss": ae_loss,
-                        "mean_logvar": tf.reduce_mean(ae_logvar)}
-        if ae_losses["kld"] < -1:
-            breakpoint()
-        #logvar_idx = layer_names.index("logvar")
-        #self.encoder.layers[0].layers[logvar_idx].trainable = False
-        #ae_embs = tf.concat((self.features[:,:self.abundance_dim], self.encoder(self.features)[0]), axis=1)
-        #ae_embs = self.encoder(self.features)[0]
-        return ae_mu, ae_losses
-
-    def train_edges(self, node_hat, nodes_idx, edges_idx, train_pairs):
-        """_summary_
-
-        :param node_hat: node embeddings
-        :type node_hat: _type_
-        :param nodes_idx: node idx to be considered in this batch
-        :type nodes_idx: _type_
-        :param edges_idx: edge idx to be considered in this batch
-        :type edges_idx: _type_
-        :param train_pairs: graph edges, pairs of node idxs of this batch
-        :type train_pairs: 
-        :return: _description_
-        :rtype: _type_
-        """
-        gnn_losses = {"gnn_loss": tf.constant(0, dtype=tf.float32),
-                      "pos": tf.constant(0, dtype=tf.float32),
-                      "neg": tf.constant(0, dtype=tf.float32)}
-        if self.graph_weight > 0:
-            #breakpoint()
-            src_embs = tf.gather(indices=train_pairs[0], params=node_hat)
-            dst_embs = tf.gather(indices=train_pairs[1], params=node_hat)
-            positive_pairwise_dist = self.nodedist(src_embs, dst_embs)
-            # create random negatives for gnn_loss
-            batch_neg_idx_src, batch_neg_idx_dst = self.sample_negatives(edge_idx=edges_idx,
-                                                                node_idx=nodes_idx)
-            if self.loglevel == "debug":
-                pset = set(zip(train_pairs[0].numpy(), train_pairs[1].numpy()))
-                nset = set(zip(batch_neg_idx_src.numpy(), batch_neg_idx_dst.numpy()))
-                print("false random negatives", round(len(pset & nset)/len(edges_idx), 4))
-            
-            try:
-                #negative_pairs = tf.gather_nd(pairwise_similarity, neg_idx)
-                neg_row_embs = tf.gather(indices=batch_neg_idx_src, params=node_hat)
-                neg_col_embs = tf.gather(indices=batch_neg_idx_dst, params=node_hat)
-                negative_pairwise_dist = self.nodedist(neg_row_embs, neg_col_embs)
-            except:
-                breakpoint()
-
-            pos_dist = tf.reduce_mean(positive_pairwise_dist)
-            if self.num_negatives > 0:
-                neg_dist = tf.reduce_mean(negative_pairwise_dist)
-            else:
-                neg_dist = tf.constant(0)
-
-            gnn_losses["pos"] = pos_dist
-            gnn_losses["neg"] = neg_dist
-            gnn_loss = self.edge_loss(positive_pairwise_dist, negative_pairwise_dist)
-            gnn_loss = gnn_loss * self.graph_weight
-            gnn_losses["gnn_loss"] = gnn_loss
-        #loss = gnn_loss
-        return gnn_losses
-
-    def train_scg(self, node_hat, scgs_idx):
-        scg_loss = tf.constant(0, dtype=tf.float32)
-        if self.scg_pairs is not None and self.scg_weight > 0:
-            scg_row_embs = tf.gather(node_hat, self.scg_pairs[scgs_idx, 0])
-            scg_col_embs = tf.gather(node_hat, self.scg_pairs[scgs_idx, 1])
-            scg_pairwise = self.nodedist(scg_row_embs, scg_col_embs)
-            scg_loss = self.edge_loss(tf.ones_like([0.0]), scg_pairwise)
-            scg_loss *= self.scg_weight
-        return scg_loss
-
-    @tf.function
-    def train_scg_only(self):
-        scgs_idx = range(0, len(self.scg_pairs))
-        layer_names = [layer.name for layer in self.encoder.layers[0].layers]
-        logvar_idx = layer_names.index("logvar")
-        self.encoder.layers[0].layers[logvar_idx].trainable = False
-        with tf.GradientTape() as tape:
-
-            node_hat, _ = self.encoder(self.features, training=True)
-            scg_loss = self.train_scg(node_hat, scgs_idx)
-            # aggregate model weights
-            if self.use_gnn and (self.epoch > self.pretrainvae or self.pretrainvae ==  0) :
-                tw = self.gnn_model.trainable_weights
-            else:
-                tw = []
-            if self.use_ae:
-                if self.pretrainvae == 0 or self.epoch < self.pretrainvae:
-                    tw += self.encoder.trainable_weights
-                #self.encoder.layers[0].layers[logvar_idx].trainable = True
-            grads = tape.gradient(scg_loss, tw)
-
-            self.opt.apply_gradients(zip(grads, tw))
-        self.encoder.layers[0].layers[logvar_idx].trainable = True
-        return scg_loss
-
-
-    @tf.function
-    def train_unsupervised(self, nodes_idx=None, edges_idx=None,
-                            scgs_idx=None,training=True, vae=True,
-                            mask_labels=None, gold_labels=None, last_batch=False, scg=False):
-        #### get node indices to be used for this batch
-        if edges_idx is None:
-            edges_idx = range(0,self.gnn_model.adj.indices.shape[0])
-        if nodes_idx is None:
-            # get nodes_idx from edges_idx
-            # this are the node pairs with their original indices, e.g. (1,2), (2,3), (3,1)
-            train_src_original = tf.gather(indices=edges_idx, params=self.gnn_model.adj.indices[:,0])
-            train_dst_original = tf.gather(indices=edges_idx, params=self.gnn_model.adj.indices[:,1])
-            unique_nodes = tf.unique(tf.concat((train_src_original, train_dst_original), axis=0))
-            nodes_idx = unique_nodes.y # e.g. (A,B,C)
-            # get new indices for edges in relation to current node list(A,B), (B,C), (C,A)
-            #train_src_new = unique_nodes.idx[:train_src_original.shape[0]] 
-            #train_dst_new = unique_nodes.idx[train_src_original.shape[0]:]
-            #train_idx_new = (train_src_new, train_dst_new)
-            if self.loglevel == "debug":
-                print(f"using {nodes_idx.shape} nodes for this batch")
-        else:
-            train_idx_new = (self.gnn_model.adj.indices[:,0], self.gnn_model.adj.indices[:,1])
-            train_src_original = self.gnn_model.adj.indices[:,0]
-            train_dst_original = self.gnn_model.adj.indices[:,1]
-        if scgs_idx is None:
-            scgs_idx = range(0, len(self.scg_pairs))
-        #####
-        
-        with tf.GradientTape() as tape:
-            #####   run encoder first on nodes of this batch
-            if self.use_ae:
-                # only nodes in nodes_idx are processed, the output may have a different dimension
-                ae_embs, ae_losses = self.train_vae(nodes_idx)
-                # ae_embs is only nodes in node_idx
-                #reverse gather, expand so that ae_embs has the same dim as self.features
-                ae_embs = tf.scatter_nd(indices=nodes_idx[:,None],
-                                     updates=ae_embs,
-                                     shape=(self.features.shape[0], ae_embs.shape[1]))
-            else:
-                ae_embs = self.features # ae_embs is all nodes
-                ae_losses = {}
-            ######
-            ###### run gnn model
-            if self.use_gnn and self.decoder_input == "vae" and (self.epoch > self.pretrainvae or self.pretrainvae ==  0):
-                gnn_embs = self.gnn_model(ae_embs, nodes_idx, training=True)
-                node_hat = tf.scatter_nd(indices=nodes_idx[:,None],
-                                     updates=gnn_embs,
-                                     shape=(self.features.shape[0], gnn_embs.shape[1]))
-            else:
-                node_hat = ae_embs
-            gnn_losses = self.train_edges(node_hat, nodes_idx, edges_idx,
-                                          (train_src_original, train_dst_original))
-            scg_loss = tf.convert_to_tensor(0.0)
-            if scg:
-                scg_loss = self.train_scg(node_hat, scgs_idx)
-            gnn_losses["scg_loss"] = scg_loss
-
-            # classification loss
-            if self.classifier is not None:
-                if mask_labels is not None and mask_labels > 0:
-                    use_labels = np.random.choice(node_hat.shape[0], int(node_hat.shape[0]*(1-self.mask_labels)))
-                else:
-                    use_labels = np.arange(node_hat.shape[0])
-                predictions = self.classifier(node_hat, mask=use_labels)
-                pred_loss = self.classifier.loss(gold_labels[use_labels], predictions)
-            else:
-                pred_loss = tf.convert_to_tensor(0.0)
-            gnn_losses["pred_loss"] = pred_loss
-            
-            # combine losses and update model
-            loss = gnn_losses["gnn_loss"] + scg_loss
-            if training:
-                # aggregate model weights
-                if self.use_gnn and (self.epoch > self.pretrainvae or self.pretrainvae ==  0) :
-                    tw = self.gnn_model.trainable_weights
-                else:
-                    tw = []
-                if self.use_ae:
-                    loss += ae_losses["vae_loss"]
-                    if self.pretrainvae == 0 or self.epoch < self.pretrainvae:
-                        tw += self.encoder.trainable_weights + self.decoder.trainable_weights # skip logvar 
-                    #self.encoder.layers[0].layers[logvar_idx].trainable = True
-
-                if self.classifier is not None:
-                    tw += self.classifier.trainable_weights
-                    loss += pred_loss
-                #################
-                #grads = tape.gradient([ae_losses.get("vae_loss", tf.convert_to_tensor(0.0)), gnn_losses["gnn_loss"], scg_loss, pred_loss], tw)
-                grads = tape.gradient([ae_losses.get("vae_loss", tf.convert_to_tensor(0.0)), gnn_losses["gnn_loss"], pred_loss], tw)
-                grad_norm = tf.linalg.global_norm(grads)
-                #clip_grads, _ = tf.clip_by_global_norm(grads, 2,  use_norm=grad_norm)
-                #new_grad_norm = tf.linalg.global_norm(clip_grads)
-                self.opt.apply_gradients(zip(grads, tw))
-                ae_losses["grad_norm"] = grad_norm.numpy()
-                #ae_losses["grad_norm_clip"] = new_grad_norm.numpy()
-        return loss, gnn_losses, ae_losses
-        
-        
-    #@tf.function
-    def ae_loss(self, x, x_hat, mu, logvar, vae):
-        if vae:
-            epsilon = tf.random.normal(tf.shape(mu))
-            z = mu + epsilon * tf.math.exp(0.5 * logvar)
-            kld  = 0.5*tf.math.reduce_mean(tf.math.reduce_mean(1.0 + logvar - tf.math.pow(mu, 2) - tf.math.exp(logvar), axis=1))
-            kld  = -kld * self.kld_weight
-        else:
-            z = mu
-            kld = tf.convert_to_tensor(0.0)
-        if self.abundance_dim > 1:
-            mse1 = - tf.reduce_mean(tf.reduce_sum((tf.math.log(x_hat[:, :self.abundance_dim] + 1e-9) * x[:, :self.abundance_dim]), axis=1))
-        else:
-            mse1 = tf.reduce_mean( (x[:, :self.abundance_dim] - x_hat[:, :self.abundance_dim])**2)
-        mse1 *= (1-self.kmer_weight)
-        mse2 = self.kmer_weight*tf.reduce_mean( tf.reduce_mean((x[:, self.abundance_dim:] - x_hat[:, self.abundance_dim:])**2, axis=1))
-
-        return mse2, mse1, kld
-
-    @tf.function
-    def train_unsupervised_decode(self, idx):
-        with tf.GradientTape() as tape:
-            # run gnn model
-            z_sample, mu, logvar, x_orginal, x_hat = self.gnn_model(self.features, self.adj,
-                                                           indices=idx, training=True)
- 
-
-            loss = 0
-            gnn_loss = tf.constant(0, dtype=tf.float32)
-            # SCG loss
-            scg_loss = tf.constant(0, dtype=tf.float32)
-            if self.scg_pairs is not None and self.scg_weight > 0:
-                ns1 = tf.gather(z_sample, self.scg_pairs[:, 0])
-                ns2 = tf.gather(z_sample, self.scg_pairs[:, 1])
-                all_diff_pairs = tf.math.exp(-0.5 * tf.reduce_sum((ns1 - ns2) ** 2, axis=-1))
-                scg_loss = tf.reduce_mean(all_diff_pairs) * self.scg_weight
-                loss += scg_loss
-
-            # decode
-            kmer_loss, ab_loss, kld_loss = self.ae_loss(tf.gather(self.features, idx), x_hat, mu, logvar, vae=True)
-            loss += kmer_loss + ab_loss - kld_loss
-
-        tw = self.gnn_model.trainable_weights
-        #tw += self.encoder.trainable_weights
-        #tw += self.decoder.trainable_weights
-        grads = tape.gradient(loss, tw)
-        self.opt.apply_gradients(zip(grads, tw))
-        return loss, gnn_loss, scg_loss, kmer_loss, ab_loss, kld_loss
-
-    @staticmethod
-    def sample_idx(idx, n):
-        n = tf.cast(n, tf.int64)
-        N = tf.cast(tf.shape(idx)[0], tf.int64)
-        random_idx = tf.random.uniform(shape=(n,), minval=0, maxval=N, dtype=tf.int64)
-        s_idx = tf.gather_nd(idx, random_idx)
-        return s_idx
-
+from os import uname
+import tensorflow as tf
+
+from tensorflow.keras.optimizers import Adam, SGD
+from tensorflow.keras.models import Model
+from tensorflow.keras.layers import Input, Dense, Activation, Softmax, Embedding, LayerNormalization
+#from tensorflow.keras import Sequential
+from tensorflow.keras.layers import BatchNormalization, Lambda, LeakyReLU, Flatten
+from tensorflow.keras.layers import Dropout, Add, Concatenate
+from tensorflow.keras.losses import SparseCategoricalCrossentropy
+import numpy as np
+from tensorflow.keras.regularizers import l2    
+from tqdm import tqdm
+
+#import tensorflow_probability as tfp
+
+class VAEEncoder(Model):
+    def __init__(self, abundance_dim, kmers_dim, hiddendim, zdim=64, dropout=0, layers=2):
+        super(VAEEncoder, self).__init__()
+        self.abundance_dim = abundance_dim
+        self.kmers_dim = kmers_dim
+        self.zdim = zdim
+        in_ = Input(shape=(abundance_dim+kmers_dim,))
+        x = in_
+        for i in range(layers):
+            x = Dense(hiddendim, activation='linear', name=f"encoder_{i}")(x)
+            x = LeakyReLU(0.01)(x)
+            if dropout > 0:
+                x = Dropout(dropout)(x)
+            x = BatchNormalization()(x)
+        mu = Dense(zdim, name="mu")(x)
+        logvar = Dense(zdim, kernel_initializer='zeros', name="logvar")(x)
+        self.model = Model(in_, [mu, logvar])
+ 
+    def call(self, x, training=False):
+        mu, sigma = self.model(x, training=training)
+        return mu, sigma
+
+    
+class VAEDecoder(Model):
+    def __init__(self, abundance_dim, kmers_dim, hiddendim, zdim=64, dropout=0, layers=2):
+        super(VAEDecoder, self).__init__()
+        self.abundance_dim = abundance_dim
+        self.kmers_dim = kmers_dim
+        self.zdim = zdim
+        in_ = Input(shape=(zdim,))
+        x = in_
+        for i in range(layers):
+            x = Dense(hiddendim, activation='linear', name=f"decoder_{i}")(x)
+            x = LeakyReLU(0.01)(x)
+            if dropout > 0:
+                x = Dropout(dropout)(x)
+            x = BatchNormalization()(x)
+            
+        x1 = Dense(abundance_dim, name="decoder_ab")(x)
+        x2 = Dense(kmers_dim, name="decoder_kmer")(x)
+        if self.abundance_dim > 1:
+            x1 = Softmax()(x1)
+        x = Concatenate()((x1,x2))
+        
+        self.model = Model(in_, x)
+ 
+    def call(self, z, training=False):
+        x_hat = self.model(z, training=training)
+        return x_hat
+
+class Encoder(Model):
+    def __init__(self, features_dim, hiddendim, zdim=64, dropout=0, layers=2):
+        super(VAEEncoder, self).__init__()
+        self.zdim = zdim
+        in_ = Input(shape=(features_dim,))
+        x = in_
+        for i in range(layers):
+            x = Dense(hiddendim, activation='linear', name=f"encoder_{i}")(x)
+            x = LeakyReLU(0.01)(x)
+            if dropout > 0:
+                x = Dropout(dropout)(x)
+            x = BatchNormalization()(x)
+        mu = Dense(zdim, name="mu")(x)
+        logvar = Dense(zdim, kernel_initializer='zeros', name="logvar")(x)
+        self.model = Model(in_, [mu, logvar])
+ 
+    def call(self, x, training=False):
+        mu, sigma = self.model(x, training=training)
+        return mu, sigma
+
+    
+class Decoder(Model):
+    def __init__(self, features_dim, hiddendim, zdim=64, dropout=0, layers=2):
+        super(VAEDecoder, self).__init__()
+        self.features_dim = features_dim
+        self.zdim = zdim
+        in_ = Input(shape=(zdim,))
+        x = in_
+        for i in range(layers):
+            x = Dense(hiddendim, activation='linear', name=f"decoder_{i}")(x)
+            x = LeakyReLU(0.01)(x)
+            if dropout > 0:
+                x = Dropout(dropout)(x)
+            x = BatchNormalization()(x)
+            
+        x = Dense(features_dim, name="decoder_ab")(x)
+        #x2 = Dense(kmers_dim, name="decoder_kmer")(x)
+        #if self.abundance_dim > 1:
+        #    x1 = Softmax()(x1)
+        #x = Concatenate()((x1,x2))
+        
+        self.model = Model(in_, x)
+ 
+    def call(self, z, training=False):
+        x_hat = self.model(z, training=training)
+        return x_hat
+
+
+class LabelClassifier(Model):
+    def __init__(self, n_classes, hiddendim=128, zdim=64, dropout=0, layers=1):
+        super(LabelClassifier, self).__init__()
+        in_ = Input(shape=(zdim,))
+        x = in_
+        for nl in range(layers):
+            if nl == layers-1:
+                x = Dense(n_classes, activation='softmax')(x)
+            else:
+                x = Dense(hiddendim, activation='linear')(x)
+                #x = LeakyReLU(0.01)(x)
+                if dropout > 0:
+                    x = Dropout(dropout)(x)
+
+        self.model = Model(in_, x)
+        self.loss_fn = SparseCategoricalCrossentropy()
+ 
+    def call(self, z, mask, training=False):
+        predictions = self.model(tf.gather(params=z, indices=mask), training=training)
+        return predictions
+
+    def loss(self, gold_labels, predicted_labels):
+        return self.loss_fn(y_true=gold_labels,y_pred=predicted_labels)
+
+class TrainHelperVAE:
+    def __init__(self, encoder, decoder, learning_rate=1e-3,  kld_weight=1/200.,
+                train_weights=False, classification=False, n_classes=0,
+                gold_labels=None, mask_labels=0.0, ae_alpha=1):
+        self.encoder = encoder
+        self.decoder = decoder
+        self.train_weights = train_weights
+        self.abundance_dim = self.encoder.abundance_dim
+        self.kmers_dim = self.encoder.kmers_dim
+        self.ae_alpha = ae_alpha
+        if train_weights:
+            #self.kld_weight = tf.Variable(kld_weight)
+            self.kld_weight = kld_weight
+            #self.abundance_weight = tf.Variable(0.5)
+            self.kmer_weight = tf.Variable(0.1)
+        else:
+            self.kld_weight = kld_weight
+            if self.abundance_dim > 1:
+                #self.abundance_weight = 0.85 / tf.math.log(float(self.abundance_dim))
+                self.kmer_weight = 0.15
+            else:
+                #self.abundance_weight = 0.5
+                self.kmer_weight = 0.5
+        self.opt = tf.keras.optimizers.Adam(learning_rate=learning_rate)
+        self.logvar = None
+        self.mu = None
+        self.z = None
+        self.classify = classification
+        if self.classify:
+            self.classifier = LabelClassifier(n_classes, zdim=encoder.zdim)
+            self.gold_labels = gold_labels
+            self.mask_labels = mask_labels
+            
+    def train_step(self, x, writer=None, epoch=0, vae=True, gold_labels=None):
+        losses = self._train_step(x, vae=vae, writer=writer, epoch=epoch, gold_labels=gold_labels)
+        if writer is not None:
+            with writer.as_default():
+                tf.summary.scalar('mean logvar', self.logvar, step=epoch)
+                tf.summary.scalar('mean mu', self.mu, step=epoch)
+        losses = [loss.numpy() for loss in losses]
+        return losses
+    
+    @tf.function
+    def loss(self, x, mu, logvar, vae, training=True, writer=None, epoch=0, gold_labels=None):
+        if vae:
+            epsilon = tf.random.normal(tf.shape(mu))
+            z = mu + epsilon * tf.math.exp(0.5 * logvar)
+            kld  = 0.5*tf.math.reduce_mean(tf.math.reduce_mean(1.0 + logvar - tf.math.pow(mu, 2) - tf.math.exp(logvar), axis=1))
+            kld  = kld * self.kld_weight
+        else:
+            z = mu
+            kld = tf.convert_to_tensor(0.0)
+        x_hat = self.decoder(z, training=training)
+        if self.classify:
+            if self.mask_labels > 0:
+                use_labels = np.random.choice(z.shape[0], int(z.shape[0]*(1-self.mask_labels)))
+            else:
+                use_labels = np.arange(z.shape[0])
+            predictions = self.classifier(z, mask=use_labels)
+            prediction_loss = self.classifier.loss(gold_labels[use_labels], predictions)
+        else:
+            prediction_loss = tf.convert_to_tensor(0.0)
+        if writer is not None:
+            with writer.as_default():
+                tf.summary.scalar('min ab', tf.reduce_min(x_hat[:, :self.abundance_dim]), step=epoch)
+        if self.abundance_dim > 1:
+            mse1 = -tf.reduce_mean(tf.reduce_sum((tf.math.log(x_hat[:, :self.abundance_dim] + 1e-9) * x[:, :self.abundance_dim]), axis=1))
+        else:
+            mse1 = tf.reduce_mean( (x[:, :self.abundance_dim] - x_hat[:, :self.abundance_dim])**2)
+        if self.train_weights:
+            kmer_weight = tf.math.sigmoid(self.kmer_weight)
+        else:
+            kmer_weight = self.kmer_weight
+        mse1 *= (1-kmer_weight)
+        mse2 = kmer_weight*tf.reduce_mean( tf.reduce_mean((x[:, self.abundance_dim:] - x_hat[:, self.abundance_dim:])**2, axis=1))
+
+        return mse1, mse2, kld, prediction_loss
+
+    @tf.function
+    def _train_step(self, x, vae=True, writer=None, epoch=0, gold_labels=None):
+        with tf.GradientTape() as tape:
+            mu, logvar = self.encoder(x, training=True)
+            logvar = tf.clip_by_value(logvar, -2, 2)
+            self.logvar = tf.cast(tf.math.reduce_mean(logvar), float)
+            self.mu = tf.cast(tf.math.reduce_mean(mu), float)
+            mse1, mse2, kld, predl = self.loss(x, mu, logvar, vae, training=True,
+                                               writer=writer, epoch=epoch,
+                                               gold_labels=gold_labels)
+            loss = mse1 + mse2 - kld + predl
+            loss *= self.ae_alpha
+        tw = self.encoder.trainable_weights + self.decoder.trainable_weights 
+        if self.train_weights:
+            tw += [self.kmer_weight] # self.kld_weight
+        if self.classify:
+            tw += self.classifier.trainable_weights
+        grads = tape.gradient(loss, tw)
+        grad_norm = tf.linalg.global_norm(grads)
+        clip_grads, _ = tf.clip_by_global_norm(grads, 5,  use_norm=grad_norm)
+        new_grad_norm = tf.linalg.global_norm(clip_grads)
+        self.opt.apply_gradients(zip(clip_grads, tw))
+
+        if writer is not None:
+            with writer.as_default():
+                tf.summary.scalar('grad norm', grad_norm, step=epoch)
+                tf.summary.scalar('clipped grad norm', new_grad_norm, step=epoch)
+
+        return loss, mse2, mse1, kld, predl
+
+
+class NoiseModel(Model):
+    def __init__(self, abundance_dim, emb_dim, hiddendim=128, dropout=0, layers=1):
+        super(NoiseModel, self).__init__()
+        self.abundance_dim = abundance_dim
+        self.kmers_dim = emb_dim
+        in_ = Input(shape=((abundance_dim+emb_dim)*2,))
+        x = in_
+        for i in range(layers):
+            x = Dense(hiddendim, activation='linear', name=f"noise_{i}")(x)
+            x = LeakyReLU(0.01)(x)
+            if dropout > 0:
+                x = Dropout(dropout)(x)
+            x = BatchNormalization()(x)
+        noise = Dense(1, name="mu")(x)
+        self.model = Model(in_, noise)
+ 
+    def call(self, x, training=False):
+        noise = self.model(x, training=training)
+        return noise
+
+class TH:
+    def __init__(
+        self,
+        input_features,
+        gnn_model,
+        lr=0.01,
+        all_different_idx=None,
+        all_same_idx=None,
+        ae_encoder=None,
+        ae_decoder=None,
+        decoder_input="gnn",
+        classifier=None,
+        latentdim=32,
+        graph_weight=1.0,
+        ae_weight=1.0,
+        kld_weight = 1/200,
+        scg_weight=100.0,
+        kmer_weight=0.15,
+        abundance_weight=0.85,
+        kmer_dim=103,
+        kmer_alpha=0.5,
+        num_negatives=50,
+        kmers_dim=103,
+        abundance_dim=4,
+        labels=None,
+        use_gnn=True,
+        use_noise=False,
+        loglevel="warning",
+        pretrainvae=0
+    ):
+        self.opt = Adam(learning_rate=lr, epsilon=1e-8)
+        # self.opt = SGD(learning_rate=lr)
+        self.gnn_model = gnn_model
+        self.features = input_features
+        # self.dense_adj = tf.sparse.to_dense(self.model.adj)
+        if gnn_model is not None:
+            self.adj_shape = self.gnn_model.adj.dense_shape
+        self.kmer_dim = kmer_dim
+        self.ab_dim = input_features.shape[1] - kmer_dim
+        self.kmer_alpha = kmer_alpha
+        self.num_negatives = num_negatives
+        self.nlatent = latentdim
+        self.scg_pairs = all_different_idx
+        self.all_same_idx = all_same_idx
+        self.classifier = classifier
+        self.encoder = ae_encoder
+        self.decoder = ae_decoder
+        self.decoder_input = decoder_input
+        self.use_ae = ae_encoder is not None
+        self.mse_loss = tf.keras.losses.MeanSquaredError()
+        self.graph_weight = graph_weight
+        self.ae_weight = ae_weight
+        self.kld_weight = kld_weight
+        self.scg_weight = scg_weight
+        self.kmer_weight = kmer_weight
+        self.noise_reg = 1
+        self.abundance_weight = abundance_weight
+        self.no_gnn = gnn_model is None
+        self.train_ae = False
+        self.abundance_dim = abundance_dim
+        self.kmers_dim = kmers_dim
+        self.use_gnn = use_gnn
+        self.use_noise = use_noise
+        self.loglevel = loglevel
+        self.pretrainvae = pretrainvae
+        self.epoch = 0
+
+    @tf.function
+    def sample_negatives(self, edge_idx, node_idx):
+        # for 5 negatives and batchsize 256, this should give 1% or less false negatives
+        neg_idx = tf.random.uniform(shape=(2, len(edge_idx)*self.num_negatives),
+                                    maxval=node_idx.shape[0], dtype=tf.int32)
+        # get neg idx relative to node_idx (of this batch)
+        neg_idx_row = tf.gather(params=node_idx, indices=neg_idx[0,:])
+        neg_idx_col = tf.gather(params=node_idx, indices=neg_idx[1,:])
+        return neg_idx_row, neg_idx_col
+        #return neg_idx[0,:], neg_idx[1,:]
+
+    @tf.function
+    def nodedist(self, u, v):
+        #breakpoint()
+        #return tf.reduce_sum((tf.expand_dims(x, 0) - tf.expand_dims(y, 1)**2), axis=-1)
+        u = tf.nn.l2_normalize(u, axis=1)
+        v = tf.nn.l2_normalize(v, axis=1)
+        pairwise = tf.reduce_sum(tf.math.multiply(u, v), axis=1)
+        #pairwise = -tf.norm(tf.math.subtract(u, v) + + 1.0e-12, ord='euclidean', axis=1,)
+        return pairwise
+    
+    @tf.function
+    def edge_loss(self, pos_dists, neg_dists):
+        #breakpoint()
+        y_true = tf.concat((tf.ones_like(pos_dists), tf.zeros_like(neg_dists)), axis=0)
+        y_pred = tf.concat((pos_dists, neg_dists), axis=0)
+        gnn_loss = tf.keras.metrics.binary_crossentropy(y_true, y_pred, from_logits=True)
+        return gnn_loss
+    
+    def train_vae(self, nodes_idx, vae=True):
+        if not vae: # not variational, no kld loss
+            # make logvar non trainable
+            layer_names = [layer.name for layer in self.encoder.layers[0].layers]
+            logvar_idx = layer_names.index("logvar")
+            self.encoder.layers[0].layers[logvar_idx].trainable = False
+            #ae_embs = tf.concat((self.features[:,:self.abundance_dim], self.encoder(self.features)[0]), axis=1)
+
+        ae_mu, ae_logvar = self.encoder(tf.gather(self.features, nodes_idx), training=(self.epoch < self.pretrainvae or self.pretrainvae == 0))
+        #ae_mu, ae_logvar = self.encoder(tf.gather(self.features, nodes_idx), training=True)
+        if self.decoder_input == "gnn" and self.use_gnn and (self.epoch > self.pretrainvae or self.pretrainvae == 0):
+            ae_mu = tf.scatter_nd(indices=nodes_idx[:,None],
+                                     updates=ae_mu,
+                                     shape=(self.features.shape[0], ae_mu.shape[1]))
+            ae_mu = self.gnn_model(ae_mu, nodes_idx, training=True)
+        ae_recon = self.decoder(ae_mu, training=(self.epoch < self.pretrainvae or self.pretrainvae == 0))
+        #ae_recon = self.decoder(ae_mu, training=True)
+        ae_logvar = tf.clip_by_value(ae_logvar, -2, 2)
+        try:
+            losses = self.ae_loss(tf.gather(self.features, nodes_idx), ae_recon, ae_mu, ae_logvar, vae=vae)
+        except:
+            breakpoint()
+        ae_loss = tf.reduce_sum(losses) * self.ae_weight
+        ae_losses = {"kmer_loss": losses[0],
+                        "ab_loss": losses[1],
+                        "kld": losses[2],
+                        "vae_loss": ae_loss,
+                        "mean_logvar": tf.reduce_mean(ae_logvar)}
+        if ae_losses["kld"] < -1:
+            breakpoint()
+        #logvar_idx = layer_names.index("logvar")
+        #self.encoder.layers[0].layers[logvar_idx].trainable = False
+        #ae_embs = tf.concat((self.features[:,:self.abundance_dim], self.encoder(self.features)[0]), axis=1)
+        #ae_embs = self.encoder(self.features)[0]
+        return ae_mu, ae_losses
+
+    def train_edges(self, node_hat, nodes_idx, edges_idx, train_pairs):
+        """_summary_
+
+        :param node_hat: node embeddings
+        :type node_hat: _type_
+        :param nodes_idx: node idx to be considered in this batch
+        :type nodes_idx: _type_
+        :param edges_idx: edge idx to be considered in this batch
+        :type edges_idx: _type_
+        :param train_pairs: graph edges, pairs of node idxs of this batch
+        :type train_pairs: 
+        :return: _description_
+        :rtype: _type_
+        """
+        gnn_losses = {"gnn_loss": tf.constant(0, dtype=tf.float32),
+                      "pos": tf.constant(0, dtype=tf.float32),
+                      "neg": tf.constant(0, dtype=tf.float32)}
+        if self.graph_weight > 0:
+            #breakpoint()
+            src_embs = tf.gather(indices=train_pairs[0], params=node_hat)
+            dst_embs = tf.gather(indices=train_pairs[1], params=node_hat)
+            positive_pairwise_dist = self.nodedist(src_embs, dst_embs)
+            # create random negatives for gnn_loss
+            batch_neg_idx_src, batch_neg_idx_dst = self.sample_negatives(edge_idx=edges_idx,
+                                                                node_idx=nodes_idx)
+            if self.loglevel == "debug":
+                pset = set(zip(train_pairs[0].numpy(), train_pairs[1].numpy()))
+                nset = set(zip(batch_neg_idx_src.numpy(), batch_neg_idx_dst.numpy()))
+                print("false random negatives", round(len(pset & nset)/len(edges_idx), 4))
+            
+            try:
+                #negative_pairs = tf.gather_nd(pairwise_similarity, neg_idx)
+                neg_row_embs = tf.gather(indices=batch_neg_idx_src, params=node_hat)
+                neg_col_embs = tf.gather(indices=batch_neg_idx_dst, params=node_hat)
+                negative_pairwise_dist = self.nodedist(neg_row_embs, neg_col_embs)
+            except:
+                breakpoint()
+
+            pos_dist = tf.reduce_mean(positive_pairwise_dist)
+            if self.num_negatives > 0:
+                neg_dist = tf.reduce_mean(negative_pairwise_dist)
+            else:
+                neg_dist = tf.constant(0)
+
+            gnn_losses["pos"] = pos_dist
+            gnn_losses["neg"] = neg_dist
+            gnn_loss = self.edge_loss(positive_pairwise_dist, negative_pairwise_dist)
+            gnn_loss = gnn_loss * self.graph_weight
+            gnn_losses["gnn_loss"] = gnn_loss
+        #loss = gnn_loss
+        return gnn_losses
+
+    def train_scg(self, node_hat, scgs_idx):
+        scg_loss = tf.constant(0, dtype=tf.float32)
+        if self.scg_pairs is not None and self.scg_weight > 0:
+            scg_row_embs = tf.gather(node_hat, self.scg_pairs[scgs_idx, 0])
+            scg_col_embs = tf.gather(node_hat, self.scg_pairs[scgs_idx, 1])
+            scg_pairwise = self.nodedist(scg_row_embs, scg_col_embs)
+            scg_loss = self.edge_loss(tf.ones_like([0.0]), scg_pairwise)
+            scg_loss *= self.scg_weight
+        return scg_loss
+
+    @tf.function
+    def train_scg_only(self):
+        scgs_idx = range(0, len(self.scg_pairs))
+        layer_names = [layer.name for layer in self.encoder.layers[0].layers]
+        logvar_idx = layer_names.index("logvar")
+        self.encoder.layers[0].layers[logvar_idx].trainable = False
+        with tf.GradientTape() as tape:
+
+            node_hat, _ = self.encoder(self.features, training=True)
+            scg_loss = self.train_scg(node_hat, scgs_idx)
+            # aggregate model weights
+            if self.use_gnn and (self.epoch > self.pretrainvae or self.pretrainvae ==  0) :
+                tw = self.gnn_model.trainable_weights
+            else:
+                tw = []
+            if self.use_ae:
+                if self.pretrainvae == 0 or self.epoch < self.pretrainvae:
+                    tw += self.encoder.trainable_weights
+                #self.encoder.layers[0].layers[logvar_idx].trainable = True
+            grads = tape.gradient(scg_loss, tw)
+
+            self.opt.apply_gradients(zip(grads, tw))
+        self.encoder.layers[0].layers[logvar_idx].trainable = True
+        return scg_loss
+
+
+    @tf.function
+    def train_unsupervised(self, nodes_idx=None, edges_idx=None,
+                            scgs_idx=None,training=True, vae=True,
+                            mask_labels=None, gold_labels=None, last_batch=False, scg=False):
+        #### get node indices to be used for this batch
+        if edges_idx is None:
+            edges_idx = range(0,self.gnn_model.adj.indices.shape[0])
+        if nodes_idx is None:
+            # get nodes_idx from edges_idx
+            # this are the node pairs with their original indices, e.g. (1,2), (2,3), (3,1)
+            train_src_original = tf.gather(indices=edges_idx, params=self.gnn_model.adj.indices[:,0])
+            train_dst_original = tf.gather(indices=edges_idx, params=self.gnn_model.adj.indices[:,1])
+            unique_nodes = tf.unique(tf.concat((train_src_original, train_dst_original), axis=0))
+            nodes_idx = unique_nodes.y # e.g. (A,B,C)
+            # get new indices for edges in relation to current node list(A,B), (B,C), (C,A)
+            #train_src_new = unique_nodes.idx[:train_src_original.shape[0]] 
+            #train_dst_new = unique_nodes.idx[train_src_original.shape[0]:]
+            #train_idx_new = (train_src_new, train_dst_new)
+            if self.loglevel == "debug":
+                print(f"using {nodes_idx.shape} nodes for this batch")
+        else:
+            train_idx_new = (self.gnn_model.adj.indices[:,0], self.gnn_model.adj.indices[:,1])
+            train_src_original = self.gnn_model.adj.indices[:,0]
+            train_dst_original = self.gnn_model.adj.indices[:,1]
+        if scgs_idx is None:
+            scgs_idx = range(0, len(self.scg_pairs))
+        #####
+        
+        with tf.GradientTape() as tape:
+            #####   run encoder first on nodes of this batch
+            if self.use_ae:
+                # only nodes in nodes_idx are processed, the output may have a different dimension
+                ae_embs, ae_losses = self.train_vae(nodes_idx)
+                # ae_embs is only nodes in node_idx
+                #reverse gather, expand so that ae_embs has the same dim as self.features
+                ae_embs = tf.scatter_nd(indices=nodes_idx[:,None],
+                                     updates=ae_embs,
+                                     shape=(self.features.shape[0], ae_embs.shape[1]))
+            else:
+                ae_embs = self.features # ae_embs is all nodes
+                ae_losses = {}
+            ######
+            ###### run gnn model
+            if self.use_gnn and self.decoder_input == "vae" and (self.epoch > self.pretrainvae or self.pretrainvae ==  0):
+                gnn_embs = self.gnn_model(ae_embs, nodes_idx, training=True)
+                node_hat = tf.scatter_nd(indices=nodes_idx[:,None],
+                                     updates=gnn_embs,
+                                     shape=(self.features.shape[0], gnn_embs.shape[1]))
+            else:
+                node_hat = ae_embs
+            gnn_losses = self.train_edges(node_hat, nodes_idx, edges_idx,
+                                          (train_src_original, train_dst_original))
+            scg_loss = tf.convert_to_tensor(0.0)
+            if scg:
+                scg_loss = self.train_scg(node_hat, scgs_idx)
+            gnn_losses["scg_loss"] = scg_loss
+
+            # classification loss
+            if self.classifier is not None:
+                if mask_labels is not None and mask_labels > 0:
+                    use_labels = np.random.choice(node_hat.shape[0], int(node_hat.shape[0]*(1-self.mask_labels)))
+                else:
+                    use_labels = np.arange(node_hat.shape[0])
+                predictions = self.classifier(node_hat, mask=use_labels)
+                pred_loss = self.classifier.loss(gold_labels[use_labels], predictions)
+            else:
+                pred_loss = tf.convert_to_tensor(0.0)
+            gnn_losses["pred_loss"] = pred_loss
+            
+            # combine losses and update model
+            loss = gnn_losses["gnn_loss"] + scg_loss
+            if training:
+                # aggregate model weights
+                if self.use_gnn and (self.epoch > self.pretrainvae or self.pretrainvae ==  0) :
+                    tw = self.gnn_model.trainable_weights
+                else:
+                    tw = []
+                if self.use_ae:
+                    loss += ae_losses["vae_loss"]
+                    if self.pretrainvae == 0 or self.epoch < self.pretrainvae:
+                        tw += self.encoder.trainable_weights + self.decoder.trainable_weights # skip logvar 
+                    #self.encoder.layers[0].layers[logvar_idx].trainable = True
+
+                if self.classifier is not None:
+                    tw += self.classifier.trainable_weights
+                    loss += pred_loss
+                #################
+                #grads = tape.gradient([ae_losses.get("vae_loss", tf.convert_to_tensor(0.0)), gnn_losses["gnn_loss"], scg_loss, pred_loss], tw)
+                grads = tape.gradient([ae_losses.get("vae_loss", tf.convert_to_tensor(0.0)), gnn_losses["gnn_loss"], pred_loss], tw)
+                grad_norm = tf.linalg.global_norm(grads)
+                #clip_grads, _ = tf.clip_by_global_norm(grads, 2,  use_norm=grad_norm)
+                #new_grad_norm = tf.linalg.global_norm(clip_grads)
+                self.opt.apply_gradients(zip(grads, tw))
+                ae_losses["grad_norm"] = grad_norm.numpy()
+                #ae_losses["grad_norm_clip"] = new_grad_norm.numpy()
+        return loss, gnn_losses, ae_losses
+        
+        
+    #@tf.function
+    def ae_loss(self, x, x_hat, mu, logvar, vae):
+        if vae:
+            epsilon = tf.random.normal(tf.shape(mu))
+            z = mu + epsilon * tf.math.exp(0.5 * logvar)
+            kld  = 0.5*tf.math.reduce_mean(tf.math.reduce_mean(1.0 + logvar - tf.math.pow(mu, 2) - tf.math.exp(logvar), axis=1))
+            kld  = -kld * self.kld_weight
+        else:
+            z = mu
+            kld = tf.convert_to_tensor(0.0)
+        if self.abundance_dim > 1:
+            mse1 = - tf.reduce_mean(tf.reduce_sum((tf.math.log(x_hat[:, :self.abundance_dim] + 1e-9) * x[:, :self.abundance_dim]), axis=1))
+        else:
+            mse1 = tf.reduce_mean( (x[:, :self.abundance_dim] - x_hat[:, :self.abundance_dim])**2)
+        mse1 *= (1-self.kmer_weight)
+        mse2 = self.kmer_weight*tf.reduce_mean( tf.reduce_mean((x[:, self.abundance_dim:] - x_hat[:, self.abundance_dim:])**2, axis=1))
+
+        return mse2, mse1, kld
+
+    @tf.function
+    def train_unsupervised_decode(self, idx):
+        with tf.GradientTape() as tape:
+            # run gnn model
+            z_sample, mu, logvar, x_orginal, x_hat = self.gnn_model(self.features, self.adj,
+                                                           indices=idx, training=True)
+ 
+
+            loss = 0
+            gnn_loss = tf.constant(0, dtype=tf.float32)
+            # SCG loss
+            scg_loss = tf.constant(0, dtype=tf.float32)
+            if self.scg_pairs is not None and self.scg_weight > 0:
+                ns1 = tf.gather(z_sample, self.scg_pairs[:, 0])
+                ns2 = tf.gather(z_sample, self.scg_pairs[:, 1])
+                all_diff_pairs = tf.math.exp(-0.5 * tf.reduce_sum((ns1 - ns2) ** 2, axis=-1))
+                scg_loss = tf.reduce_mean(all_diff_pairs) * self.scg_weight
+                loss += scg_loss
+
+            # decode
+            kmer_loss, ab_loss, kld_loss = self.ae_loss(tf.gather(self.features, idx), x_hat, mu, logvar, vae=True)
+            loss += kmer_loss + ab_loss - kld_loss
+
+        tw = self.gnn_model.trainable_weights
+        #tw += self.encoder.trainable_weights
+        #tw += self.decoder.trainable_weights
+        grads = tape.gradient(loss, tw)
+        self.opt.apply_gradients(zip(grads, tw))
+        return loss, gnn_loss, scg_loss, kmer_loss, ab_loss, kld_loss
+
+    @staticmethod
+    def sample_idx(idx, n):
+        n = tf.cast(n, tf.int64)
+        N = tf.cast(tf.shape(idx)[0], tf.int64)
+        random_idx = tf.random.uniform(shape=(n,), minval=0, maxval=N, dtype=tf.int64)
+        s_idx = tf.gather_nd(idx, random_idx)
+        return s_idx
+
```

### Comparing `graphmb-0.2.4/src/graphmb/train_ccvae.py` & `graphmb-0.2.5/src/graphmb/train_ccvae.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,445 +1,445 @@
-import numpy as np
-import datetime
-import os
-import tensorflow as tf
-import random
-import logging
-from tqdm import tqdm
-import mlflow
-from scipy.sparse import coo_matrix, diags
-
-from tensorflow.keras.optimizers import Adam, SGD
-
-from graphmb.models import  TH, TrainHelperVAE, VAEDecoder, VAEEncoder, LabelClassifier
-from graphmb.utils import set_seed
-from graphmb.visualize import plot_edges_sim
-from graphmb.evaluate import compute_clusters_and_stats, eval_epoch
-from graphmb.utils import get_cluster_mask
-from graphmb.gnn_models import name_to_model
-
-
-def normalize_adj_sparse(A):
-    #breakpoint()
-    # https://github.com/tkipf/gcn/blob/master/gcn/utils.py
-    A.setdiag(1)
-    rowsum = np.array(A.sum(1))
-    d_inv_sqrt = np.power(rowsum, -0.5).flatten()
-    d_inv_sqrt[np.isinf(d_inv_sqrt)] = 0.0
-    d_mat_inv_sqrt = diags(d_inv_sqrt)
-    return A.dot(d_mat_inv_sqrt).transpose().dot(d_mat_inv_sqrt).tocoo()
-
-
-def prepare_data_for_gnn(
-    dataset, use_edge_weights=True, cluster_markers_only=False, use_raw=False,
-    binarize=False, remove_edges=False, remove_same_scg=True
-):
-
-    if use_raw: # use raw features instead of precomputed embeddings
-        node_raw = np.hstack((dataset.node_depths, dataset.node_kmers))
-        # features are already normalized
-        #node_raw = (node_raw - node_raw.mean(axis=0, keepdims=True)) / node_raw.std(axis=0, keepdims=True)
-        X = node_raw
-    else:
-        node_features = (dataset.node_embs - dataset.node_embs.mean(axis=0, keepdims=True)) / dataset.node_embs.std(
-            axis=0, keepdims=True
-        )
-        X = node_features
-
-    depth = 2
-    # adjacency_matrix_sparse, edge_features = filter_graph_with_markers(adjacency_matrix_sparse, node_names, contig_genes, edge_features, depth=depth) 
-    cluster_mask = get_cluster_mask(cluster_markers_only, dataset)
-    #connected_marker_nodes = set(range(len(dataset.node_names)))
-    
-    adj_matrix = dataset.adj_matrix.copy()
-    edge_weights = dataset.edge_weights.copy()
-    if binarize:
-        # both dataset.adj_matrix and dataset.edge_weights
-        #breakpoint()
-        percentile = 90
-        threshold = np.percentile(dataset.edge_weights, percentile)
-        print(f"using this threshold ({percentile} percentile) {threshold} on adj matrix with {len(dataset.adj_matrix.row)} edges")
-        #dataset.adj_matrix = dataset.adj_matrix
-        adj_matrix.data[adj_matrix.data < threshold] = 0
-        adj_matrix.data[adj_matrix.data >= threshold] = 1
-        adj_matrix.eliminate_zeros()
-        edge_weights = adj_matrix.data 
-        #dataset.edge_weights = np.ones(len(dataset.adj_matrix.row))
-        print(f"reduce matrix to {len(edge_weights)} edges")
-    
-    if remove_same_scg:
-        edges_with_same_scgs = dataset.get_edges_with_same_scgs()
-        for x in edges_with_same_scgs:
-                adj_matrix.data[x] = 0
-                edge_weights[x] = 0
-        adj_matrix.eliminate_zeros()
-        print(f"deleted {len(edges_with_same_scgs)} edges with same SCGs")
-    
-    if remove_edges:
-        # create self loops only sparse adj matrix
-        n = len(dataset.node_names)
-        adj_matrix = coo_matrix((np.ones(n), (np.array(range(n)), np.array(range(n)))), shape=(n,n))
-        edge_weights = np.ones(len(adj_matrix.row))
-        print(f"reduce matrix to {len(edge_weights)} edges")
-    
-    # gcn transform
-    adj_norm = normalize_adj_sparse(adj_matrix)
-    
-    if use_edge_weights:
-        #edge_features = (dataset.edge_weights - dataset.edge_weights.min()) / (
-        #    dataset.edge_weights.max() - dataset.edge_weights.min()
-        #)
-        edge_features = edge_weights / edge_weights.max()
-        # multiply normalized values by edge weights
-        old_rows, old_cols = adj_matrix.row, adj_matrix.col
-        old_idx_to_edge_idx = {(r, c): i for i, (r, c) in enumerate(zip(old_rows, old_cols))}
-        old_values = adj_norm.data.astype(np.float32)
-        new_values = []
-        for i, j, ov in zip(adj_norm.row, adj_norm.col, old_values):
-            if i == j:
-                new_values.append(1.0)
-            else:
-                try:
-                    eidx = old_idx_to_edge_idx[(i, j)]
-                    new_values.append(ov * edge_features[eidx])
-                except:
-                    new_values.append(ov)
-        new_values = np.array(new_values).astype(np.float32)
-    
-    else:
-        adj_norm.data = np.ones(len(adj_norm.row))
-        new_values = adj_norm.data.astype(np.float32)
-    
-    # convert to tf.SparseTensor
-    adj = tf.SparseTensor(
-        indices=np.array([adj_norm.row, adj_norm.col]).T, values=new_values, dense_shape=adj_norm.shape
-    )
-    adj = tf.sparse.reorder(adj)
-
-    # neg_pair_idx = None
-    pos_pair_idx = None
-    print("**** Num of edges:", adj.indices.shape[0])
-    return X, adj, cluster_mask, dataset.neg_pairs_idx, pos_pair_idx
-
-def run_model_ccvae(dataset, args, logger, nrun, epochs=None, 
-                    plot=False, use_last_batch=False, use_gnn=False,
-                    target_metric="hq"):
-    set_seed(args.seed)
-    node_names = np.array(dataset.node_names)
-    RESULT_EVERY = args.evalepochs
-    hidden_gnn = args.hidden_gnn
-    hidden_vae = args.hidden_vae
-    output_dim_gnn = args.embsize_gnn
-    output_dim_vae = args.embsize_vae
-    epochs = args.epoch if not epochs else epochs
-    lr_vae = args.lr_vae
-    lr_gnn = args.lr_gnn
-    nlayers_gnn = args.layers_gnn
-    gname = args.model_name
-    use_gnn = args.layers_gnn > 0 and use_gnn
-    if not use_gnn:
-        lr_gnn = lr_vae
-    with mlflow.start_run(run_name=args.assembly.split("/")[-1] + "-" + args.outname):
-        mlflow.log_params(vars(args))
-        
-        # pick one of the LAF models
-        gmodel_type = name_to_model[gname.split("_")[0].upper()] 
-        clustering = args.clusteringalgo
-        k = args.kclusters
-        
-        use_edge_weights = True
-        cluster_markers_only = args.quick
-        use_ae = True
-
-        current_time = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
-        X, adj, cluster_mask, neg_pair_idx, pos_pair_idx = prepare_data_for_gnn(
-            dataset, use_edge_weights, cluster_markers_only, use_raw=True,
-            binarize=args.binarize, remove_edges=args.noedges)
-
-        if nrun == 0:
-            logger.info("******* Running model: CCVAE {}**********".format(gname if use_gnn else ""))
-            logger.info("***** using edge weights: {} ******".format(use_edge_weights))
-            logger.info("***** cluster markers only: {} *****".format(cluster_markers_only))
-            logger.info("***** self edges only: {} *****".format(args.noedges))
-            logger.info("***** Using raw kmer+abund features: {}".format(True))
-            logger.info("***** SCG neg pairs: {}".format(neg_pair_idx.shape))
-            logger.info("***** input features dimension: {}".format(X[cluster_mask].shape))
-        tf.config.run_functions_eagerly(True)
-        
-        # pre train clustering
-        if not args.skip_preclustering and nrun == 0:
-            cluster_labels, stats, _, hq_bins = compute_clusters_and_stats(
-                        X[cluster_mask], node_names[cluster_mask],
-                        dataset, clustering=clustering, k=k, tsne=args.tsne,
-                        amber=(args.labels is not None and "amber" in args.labels),
-                        cuda=args.cuda,
-                    )
-            #mlflow.log_metrics(stats, step=0)
-            logger.info(f">>> Pre train stats: {str(stats)}")
-        else:
-            stats = {"epoch":0, target_metric: 0, "hq": 0 }
-            cluster_labels = []
-        
-        pname = ""
-
-        #plot edges vs initial embs
-        if plot:
-            id_to_scg = {i: set(dataset.contig_markers[node_name].keys()) for i, node_name in enumerate(dataset.node_names)}
-            plot_edges_sim(X, dataset.adj_matrix, id_to_scg, f"{args.outdir}/{args.outname}_pretrain_")
-
-        # initialize variables
-        scores = [stats]
-        all_cluster_labels = []
-        all_cluster_labels.append(cluster_labels)
-        losses = {"total": [], "ae": [], "gnn": [], "scg": []}
-        X = X.astype(np.float32)
-        features = tf.constant(X)
-        input_dim_gnn = output_dim_vae #+ dataset.node_depths.shape[1]
-        if args.graph_alpha > 0:
-            clustering_dim = output_dim_gnn
-        elif not args.concatfeatures:
-            clustering_dim = output_dim_vae
-        else:
-            clustering_dim = output_dim_vae + output_dim_gnn
-        logger.info(f"*** Model input dim {X.shape[1]}, GNN input dim {input_dim_gnn}")
-        logger.info(f"use_ae: {use_ae}, run AE only: {args.ae_only} output clustering dim {clustering_dim}")
-
-        gnn_model = gmodel_type(
-            features_shape=features.shape,
-            input_dim=input_dim_gnn,
-            labels=None,
-            adj=adj,
-            embsize=output_dim_gnn,
-            hidden_units=hidden_gnn,
-            layers=nlayers_gnn,
-            conv_last=False,
-            dropout=args.dropout_gnn
-        )  # , use_bn=True, use_vae=False)
-
-        encoder = VAEEncoder(dataset.node_depths.shape[1], dataset.node_kmers.shape[1],
-                             hidden_vae, zdim=output_dim_vae, dropout=args.dropout_vae,
-                             layers=args.layers_vae)
-        decoder = VAEDecoder(dataset.node_depths.shape[1], dataset.node_kmers.shape[1],
-                             hidden_vae, zdim=output_dim_vae, dropout=args.dropout_vae,
-                             layers=args.layers_vae)
-
-        if args.classify:
-            classifier = LabelClassifier(len(dataset.labels), zdim=encoder.zdim)
-        else:
-            classifier = None
-        trainer = TH(
-            features,
-            gnn_model=gnn_model,
-            lr=lr_gnn,
-            all_different_idx=neg_pair_idx,
-            all_same_idx=pos_pair_idx,
-            ae_encoder=encoder,
-            ae_decoder=decoder,
-            decoder_input=args.decoder_input,
-            classifier=classifier,
-            latentdim=output_dim_gnn,
-            graph_weight=float(args.graph_alpha),
-            ae_weight=float(args.ae_alpha),
-            scg_weight=float(args.scg_alpha),
-            num_negatives=args.negatives,
-            kmers_dim=dataset.node_kmers.shape[1],
-            abundance_dim=dataset.node_depths.shape[1],
-            use_gnn=use_gnn,
-            use_noise=args.noise, # not being used
-            loglevel=args.loglevel,
-            pretrainvae=0
-        )
-
-        if args.batchtype == "auto":
-            if args.ae_alpha > 0 and args.graph_alpha == 0 and args.scg_alpha == 0:
-                args.batchtype = "nodes"
-            else:
-                args.batchtype = "edges"
-        scg_idx = np.arange(len(neg_pair_idx))
-        # create eval split
-        if args.eval_split == 0:
-            if "node" in args.batchtype:
-                train_idx = np.arange(len(features))
-            elif "edge" in args.batchtype:
-                train_idx = np.arange(gnn_model.adj.indices.shape[0])
-            eval_idx = []
-        else:
-            if "node" in args.batchtype:
-                train_idx = np.array(random.sample(list(range(gnn_model.adj.indices.shape[0])), int(gnn_model.adj.indices.shape[0]*(1-args.eval_split))))
-                eval_idx = np.array([x for x in np.arange(gnn_model.adj.indices.shape[0]) if x not in train_idx])
-            elif "edge" in args.batchtype:
-                train_idx = np.array(random.sample(list(range(gnn_model.adj.indices.shape[0])), int(gnn_model.adj.indices.shape[0]*(1-args.eval_split))))
-                eval_idx = np.array([x for x in np.arange(gnn_model.adj.indices.shape[0]) if x not in train_idx])
-            logging.info(f"**** using {gnn_model.adj.indices.shape[0]} for training and {gnn_model.adj.indices.shape[0]} for eval")
-        #edges_idx = np.arange(gnn_model.adj.indices.shape[0])
-        features = np.array(features)
-        pbar_epoch = tqdm(range(epochs), disable=args.quiet, position=0)
-        scores = [stats]
-        best_embs, best_vae_embs, best_model, best_score, best_epoch = None, None, None, 0, 0
-        
-        # increasing batch size
-        batch_size = args.batchsize
-        if batch_size == 0:
-            batch_size = len(train_idx)
-        logger.info("**** initial {} batch size: {} ****".format(args.batchtype, batch_size))
-        mlflow.log_metric("cur_batch_size", batch_size, 0)
-        batch_steps = [25, 75, 150, 300]
-        batch_steps = [x for i, x in enumerate(batch_steps) if (2 ** (i+1))*batch_size < len(train_idx)]
-        logger.info("**** epoch batch size doubles: {} ****".format(str(batch_steps)))
-        gold_labels = np.array([dataset.labels.index(dataset.node_to_label[n]) for n in dataset.node_names])
-        step = 0
-        scores_string = ""
-        
-        for e in pbar_epoch:
-            #vae_epoch_losses = {"kld_loss": [], "vae_loss": [], "kmer_loss": [], "ab_loss": []}
-            recon_loss = 0
-            trainer.epoch = e
-            # train VAE in batches
-            if e in batch_steps:
-                print(f'Increasing {args.batchtype} batch size from {batch_size:d} to {batch_size*2:d}')
-                batch_size = batch_size * 2
-                mlflow.log_metric("cur_batch_size", batch_size, e )
-
-            ############################################################
-            vae_losses_epoch = {}
-            gnn_losses_epoch = {}
-            total_losses_epoch = []
-
-            # train model ################################################
-            np.random.shuffle(train_idx)
-
-            #graph_batch_size = 256
-            #graph_batch_size = len(edges_idx)
-            n_batches = len(train_idx)//batch_size
-            if use_last_batch and n_batches < len(train_idx)/batch_size:
-                n_batches += 1 # add final batch
-            if args.scg_alpha > 0:
-                scg_batch_size = len(neg_pair_idx)//n_batches
-            pbar_gnnbatch = tqdm(range(n_batches),
-                                 disable=(args.quiet or batch_size == len(train_idx) or n_batches < 1000),
-                                 position=1, ascii=' =')
-            for b in pbar_gnnbatch:
-                if "edge" in args.batchtype:
-                    nodes_batch, edges_batch = None, train_idx[b*batch_size:(b+1)*batch_size]
-                elif "node" in args.batchtype:
-                    nodes_batch, edges_batch = train_idx[b*batch_size:(b+1)*batch_size], None
-                if args.scg_alpha > 0:
-                    scg_batch = scg_idx #[b*scg_batch_size:(b+1)*scg_batch_size]
-                else:
-                    scg_batch = None
-                losses = trainer.train_unsupervised(edges_idx=edges_batch,
-                                                    nodes_idx=nodes_batch,
-                                                    scgs_idx=scg_batch, vae=True,
-                                                    gold_labels=gold_labels)
-                total_loss, gnn_losses, ae_losses = losses
-                total_losses_epoch.append(total_loss.numpy())
-                for l in gnn_losses: gnn_losses_epoch.setdefault(l,[]).append(gnn_losses[l])
-                for l in ae_losses: vae_losses_epoch.setdefault(l,[]).append(ae_losses[l])
-
-                #add losses to get epoch avg
-            if args.scg_alpha > 0:
-                scg_loss = trainer.train_scg_only()
-                scg_loss = scg_loss.numpy()
-            else:
-                scg_loss = 0
-            epoch_metrics = {"Total": np.average(total_losses_epoch),
-                             "gnn": np.average(gnn_losses_epoch["gnn_loss"]),
-                             #"SCG": np.average(gnn_losses_epoch["scg_loss"]),
-                             "SCG": scg_loss,
-                             "pred": np.average(gnn_losses_epoch["pred_loss"]),
-                            #'GNN  LR': float(trainer.opt._decayed_lr(float)),
-                            "pos": np.average(gnn_losses_epoch["pos"]),
-                            "neg": np.average(gnn_losses_epoch["neg"]),
-                            "kld": np.average(vae_losses_epoch["kld"]),
-                            "vae": np.average(vae_losses_epoch["vae_loss"]),
-                            "kmer": np.average(vae_losses_epoch["kmer_loss"]),
-                            "ab": np.average( vae_losses_epoch["ab_loss"])}
-                            #"logvar": ae_losses["mean_logvar"],
-                            #"grad_norm": ae_losses["grad_norm"],
-                            #"grad_norm_clip": ae_losses["grad_norm_clip"]}
-            #print(float(gnn_trainer.opt._decayed_lr(float)))
-            mlflow.log_metrics(epoch_metrics, step=e)
-            ##############################################################
-
-
-            # eval loss:TODO #######################################################
-
-            gpu_mem_alloc = tf.config.experimental.get_memory_info('GPU:0')["peak"] / 1000000 if args.cuda else 0
-            #gpu_mem_alloc = tf.config.experimental.get_memory_usage('GPU:0') / 1000000 if args.cuda else 0
-            # eval checkpoint ##############################################################
-            if (e + 1) % RESULT_EVERY == 0 and e > args.evalskip and target_metric != "noeval":
-                evalstarttime = datetime.datetime.now()
-               
-                gnn_input_features = trainer.encoder(features)[0]
-                #trainer.features = gnn_input_features
-                logger.debug("encoder output " + str(gnn_input_features[0][:5].numpy()))
-                if use_gnn:
-                    node_new_features = trainer.gnn_model(gnn_input_features, None, training=False)
-                    
-                    if args.concatfeatures:
-                        node_new_features = tf.concat((gnn_input_features,
-                                                        node_new_features), axis=1).numpy()
-                    else:
-                        node_new_features = node_new_features.numpy()
-                        #node_new_features = gnn_input_features.numpy()
-                else:
-                    node_new_features = gnn_input_features.numpy()
-
-                    
-                weights = (trainer.encoder.get_weights(), trainer.gnn_model.get_weights())
-                eval_output = eval_epoch(node_new_features, cluster_mask, weights,
-                                         args, dataset, e, scores, best_score, best_embs,
-                                         best_epoch, best_model, target_metric)
-                best_score, best_embs, best_epoch, scores, best_model, cluster_labels = eval_output
-                stats = scores[-1]
-                all_cluster_labels.append(cluster_labels)
-                if args.quiet:
-                    logger.info(f"--- EPOCH {e:d} ---")
-                    scores_string = f"HQ={stats['hq']}  Best{target_metric}={round(best_score, 3)} Best Epoch={best_epoch} Cur={round(stats.get(target_metric,0), 3)}"
-                    losses_string = " ".join([f"{k}={v:.3f}" for k, v in epoch_metrics.items()])
-                    logger.info(f"[{args.outname} {nlayers_gnn}l {pname}]{losses_string} {scores_string} GPU={gpu_mem_alloc:.1f}MB")
-                    logger.info(str(stats))
-                mlflow.log_metrics(stats, step=e)
-                #print("total eval time", datetime.datetime.now() - evalstarttime)
-            losses_string = " ".join([f"{k}={v:.3f}" for k, v in epoch_metrics.items() if v != 0])
-            scores_string = f"Best{target_metric}={round(best_score, 3)} BestEpoch={best_epoch} Cur{target_metric}={round(stats.get(target_metric,0), 3)}"
-            pbar_epoch.set_description(
-                f"[{args.outname} {pname}] {losses_string} {scores_string} GPU={gpu_mem_alloc:.1f}MB"
-            )
-
-        #################################################################
-        if best_embs is None and target_metric != "noeval":
-            best_embs = node_new_features
-        else:
-            node_new_features = trainer.encoder(features)[0]
-        if tf.is_tensor(node_new_features):
-            node_new_features = node_new_features.numpy()
-        cluster_labels, stats, _, _ = compute_clusters_and_stats(
-            node_new_features, node_names, dataset, clustering=clustering, k=k,
-            amber=(args.labels is not None and "amber" in args.labels),
-            cuda=args.cuda,
-        )
-        
-        all_cluster_labels.append(cluster_labels)
-        stats["epoch"] = e
-        scores.append(stats)
-        # get best stats:
-        if target_metric != "noeval":
-            # get best stats:
-            target_scores = [s[target_metric] for s in scores]
-            best_idx = np.argmax(target_scores)
-        else:
-            best_embs = node_new_features
-            best_idx = -1
-        mlflow.log_metrics(scores[best_idx], step=e+1)
-        logger.info(f">>> Last epoch: {RESULT_EVERY + (best_idx*RESULT_EVERY)} : {stats} <<<")
-        logger.info(f">>> best epoch: {RESULT_EVERY + (best_idx*RESULT_EVERY)} : {scores[best_idx]} <<<")
-        with open(f"{args.outdir}/{args.outname}_{nrun}_best_contig2bin.tsv", "w") as f:
-            f.write("@Version:0.9.0\n@SampleID:SAMPLEID\n@@SEQUENCEID\tBINID\n")
-            for i in range(len(all_cluster_labels[best_idx])):
-                f.write(f"{node_names[i]}\t{all_cluster_labels[best_idx][i]}\n")
-     
-        #plot edges vs initial embs
-        #plot_edges_sim(best_vae_embs, dataset.adj_matrix, id_to_scg, "vae_")
-        if plot:
-            plot_edges_sim(best_embs, dataset.adj_matrix, id_to_scg, "posttrain_")
-        return best_embs, scores[best_idx]
+import numpy as np
+import datetime
+import os
+import tensorflow as tf
+import random
+import logging
+from tqdm import tqdm
+import mlflow
+from scipy.sparse import coo_matrix, diags
+
+from tensorflow.keras.optimizers import Adam, SGD
+
+from graphmb.models import  TH, TrainHelperVAE, VAEDecoder, VAEEncoder, LabelClassifier
+from graphmb.utils import set_seed
+from graphmb.visualize import plot_edges_sim
+from graphmb.evaluate import compute_clusters_and_stats, eval_epoch
+from graphmb.utils import get_cluster_mask
+from graphmb.gnn_models import name_to_model
+
+
+def normalize_adj_sparse(A):
+    #breakpoint()
+    # https://github.com/tkipf/gcn/blob/master/gcn/utils.py
+    A.setdiag(1)
+    rowsum = np.array(A.sum(1))
+    d_inv_sqrt = np.power(rowsum, -0.5).flatten()
+    d_inv_sqrt[np.isinf(d_inv_sqrt)] = 0.0
+    d_mat_inv_sqrt = diags(d_inv_sqrt)
+    return A.dot(d_mat_inv_sqrt).transpose().dot(d_mat_inv_sqrt).tocoo()
+
+
+def prepare_data_for_gnn(
+    dataset, use_edge_weights=True, cluster_markers_only=False, use_raw=False,
+    binarize=False, remove_edges=False, remove_same_scg=True
+):
+
+    if use_raw: # use raw features instead of precomputed embeddings
+        node_raw = np.hstack((dataset.node_depths, dataset.node_kmers))
+        # features are already normalized
+        #node_raw = (node_raw - node_raw.mean(axis=0, keepdims=True)) / node_raw.std(axis=0, keepdims=True)
+        X = node_raw
+    else:
+        node_features = (dataset.node_embs - dataset.node_embs.mean(axis=0, keepdims=True)) / dataset.node_embs.std(
+            axis=0, keepdims=True
+        )
+        X = node_features
+
+    depth = 2
+    # adjacency_matrix_sparse, edge_features = filter_graph_with_markers(adjacency_matrix_sparse, node_names, contig_genes, edge_features, depth=depth) 
+    cluster_mask = get_cluster_mask(cluster_markers_only, dataset)
+    #connected_marker_nodes = set(range(len(dataset.node_names)))
+    
+    adj_matrix = dataset.adj_matrix.copy()
+    edge_weights = dataset.edge_weights.copy()
+    if binarize:
+        # both dataset.adj_matrix and dataset.edge_weights
+        #breakpoint()
+        percentile = 90
+        threshold = np.percentile(dataset.edge_weights, percentile)
+        print(f"using this threshold ({percentile} percentile) {threshold} on adj matrix with {len(dataset.adj_matrix.row)} edges")
+        #dataset.adj_matrix = dataset.adj_matrix
+        adj_matrix.data[adj_matrix.data < threshold] = 0
+        adj_matrix.data[adj_matrix.data >= threshold] = 1
+        adj_matrix.eliminate_zeros()
+        edge_weights = adj_matrix.data 
+        #dataset.edge_weights = np.ones(len(dataset.adj_matrix.row))
+        print(f"reduce matrix to {len(edge_weights)} edges")
+    
+    if remove_same_scg:
+        edges_with_same_scgs = dataset.get_edges_with_same_scgs()
+        for x in edges_with_same_scgs:
+                adj_matrix.data[x] = 0
+                edge_weights[x] = 0
+        adj_matrix.eliminate_zeros()
+        print(f"deleted {len(edges_with_same_scgs)} edges with same SCGs")
+    
+    if remove_edges:
+        # create self loops only sparse adj matrix
+        n = len(dataset.node_names)
+        adj_matrix = coo_matrix((np.ones(n), (np.array(range(n)), np.array(range(n)))), shape=(n,n))
+        edge_weights = np.ones(len(adj_matrix.row))
+        print(f"reduce matrix to {len(edge_weights)} edges")
+    
+    # gcn transform
+    adj_norm = normalize_adj_sparse(adj_matrix)
+    
+    if use_edge_weights:
+        #edge_features = (dataset.edge_weights - dataset.edge_weights.min()) / (
+        #    dataset.edge_weights.max() - dataset.edge_weights.min()
+        #)
+        edge_features = edge_weights / edge_weights.max()
+        # multiply normalized values by edge weights
+        old_rows, old_cols = adj_matrix.row, adj_matrix.col
+        old_idx_to_edge_idx = {(r, c): i for i, (r, c) in enumerate(zip(old_rows, old_cols))}
+        old_values = adj_norm.data.astype(np.float32)
+        new_values = []
+        for i, j, ov in zip(adj_norm.row, adj_norm.col, old_values):
+            if i == j:
+                new_values.append(1.0)
+            else:
+                try:
+                    eidx = old_idx_to_edge_idx[(i, j)]
+                    new_values.append(ov * edge_features[eidx])
+                except:
+                    new_values.append(ov)
+        new_values = np.array(new_values).astype(np.float32)
+    
+    else:
+        adj_norm.data = np.ones(len(adj_norm.row))
+        new_values = adj_norm.data.astype(np.float32)
+    
+    # convert to tf.SparseTensor
+    adj = tf.SparseTensor(
+        indices=np.array([adj_norm.row, adj_norm.col]).T, values=new_values, dense_shape=adj_norm.shape
+    )
+    adj = tf.sparse.reorder(adj)
+
+    # neg_pair_idx = None
+    pos_pair_idx = None
+    print("**** Num of edges:", adj.indices.shape[0])
+    return X, adj, cluster_mask, dataset.neg_pairs_idx, pos_pair_idx
+
+def run_model_ccvae(dataset, args, logger, nrun, epochs=None, 
+                    plot=False, use_last_batch=False, use_gnn=False,
+                    target_metric="hq"):
+    set_seed(args.seed)
+    node_names = np.array(dataset.node_names)
+    RESULT_EVERY = args.evalepochs
+    hidden_gnn = args.hidden_gnn
+    hidden_vae = args.hidden_vae
+    output_dim_gnn = args.embsize_gnn
+    output_dim_vae = args.embsize_vae
+    epochs = args.epoch if not epochs else epochs
+    lr_vae = args.lr_vae
+    lr_gnn = args.lr_gnn
+    nlayers_gnn = args.layers_gnn
+    gname = args.model_name
+    use_gnn = args.layers_gnn > 0 and use_gnn
+    if not use_gnn:
+        lr_gnn = lr_vae
+    with mlflow.start_run(run_name=args.assembly.split("/")[-1] + "-" + args.outname):
+        mlflow.log_params(vars(args))
+        
+        # pick one of the LAF models
+        gmodel_type = name_to_model[gname.split("_")[0].upper()] 
+        clustering = args.clusteringalgo
+        k = args.kclusters
+        
+        use_edge_weights = True
+        cluster_markers_only = args.quick
+        use_ae = True
+
+        current_time = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
+        X, adj, cluster_mask, neg_pair_idx, pos_pair_idx = prepare_data_for_gnn(
+            dataset, use_edge_weights, cluster_markers_only, use_raw=True,
+            binarize=args.binarize, remove_edges=args.noedges)
+
+        if nrun == 0:
+            logger.info("******* Running model: CCVAE {}**********".format(gname if use_gnn else ""))
+            logger.info("***** using edge weights: {} ******".format(use_edge_weights))
+            logger.info("***** cluster markers only: {} *****".format(cluster_markers_only))
+            logger.info("***** self edges only: {} *****".format(args.noedges))
+            logger.info("***** Using raw kmer+abund features: {}".format(True))
+            logger.info("***** SCG neg pairs: {}".format(neg_pair_idx.shape))
+            logger.info("***** input features dimension: {}".format(X[cluster_mask].shape))
+        tf.config.run_functions_eagerly(True)
+        
+        # pre train clustering
+        if not args.skip_preclustering and nrun == 0:
+            cluster_labels, stats, _, hq_bins = compute_clusters_and_stats(
+                        X[cluster_mask], node_names[cluster_mask],
+                        dataset, clustering=clustering, k=k, tsne=args.tsne,
+                        amber=(args.labels is not None and "amber" in args.labels),
+                        cuda=args.cuda,
+                    )
+            #mlflow.log_metrics(stats, step=0)
+            logger.info(f">>> Pre train stats: {str(stats)}")
+        else:
+            stats = {"epoch":0, target_metric: 0, "hq": 0 }
+            cluster_labels = []
+        
+        pname = ""
+
+        #plot edges vs initial embs
+        if plot:
+            id_to_scg = {i: set(dataset.contig_markers[node_name].keys()) for i, node_name in enumerate(dataset.node_names)}
+            plot_edges_sim(X, dataset.adj_matrix, id_to_scg, f"{args.outdir}/{args.outname}_pretrain_")
+
+        # initialize variables
+        scores = [stats]
+        all_cluster_labels = []
+        all_cluster_labels.append(cluster_labels)
+        losses = {"total": [], "ae": [], "gnn": [], "scg": []}
+        X = X.astype(np.float32)
+        features = tf.constant(X)
+        input_dim_gnn = output_dim_vae #+ dataset.node_depths.shape[1]
+        if args.graph_alpha > 0:
+            clustering_dim = output_dim_gnn
+        elif not args.concatfeatures:
+            clustering_dim = output_dim_vae
+        else:
+            clustering_dim = output_dim_vae + output_dim_gnn
+        logger.info(f"*** Model input dim {X.shape[1]}, GNN input dim {input_dim_gnn}")
+        logger.info(f"use_ae: {use_ae}, run AE only: {args.ae_only} output clustering dim {clustering_dim}")
+
+        gnn_model = gmodel_type(
+            features_shape=features.shape,
+            input_dim=input_dim_gnn,
+            labels=None,
+            adj=adj,
+            embsize=output_dim_gnn,
+            hidden_units=hidden_gnn,
+            layers=nlayers_gnn,
+            conv_last=False,
+            dropout=args.dropout_gnn
+        )  # , use_bn=True, use_vae=False)
+
+        encoder = VAEEncoder(dataset.node_depths.shape[1], dataset.node_kmers.shape[1],
+                             hidden_vae, zdim=output_dim_vae, dropout=args.dropout_vae,
+                             layers=args.layers_vae)
+        decoder = VAEDecoder(dataset.node_depths.shape[1], dataset.node_kmers.shape[1],
+                             hidden_vae, zdim=output_dim_vae, dropout=args.dropout_vae,
+                             layers=args.layers_vae)
+
+        if args.classify:
+            classifier = LabelClassifier(len(dataset.labels), zdim=encoder.zdim)
+        else:
+            classifier = None
+        trainer = TH(
+            features,
+            gnn_model=gnn_model,
+            lr=lr_gnn,
+            all_different_idx=neg_pair_idx,
+            all_same_idx=pos_pair_idx,
+            ae_encoder=encoder,
+            ae_decoder=decoder,
+            decoder_input=args.decoder_input,
+            classifier=classifier,
+            latentdim=output_dim_gnn,
+            graph_weight=float(args.graph_alpha),
+            ae_weight=float(args.ae_alpha),
+            scg_weight=float(args.scg_alpha),
+            num_negatives=args.negatives,
+            kmers_dim=dataset.node_kmers.shape[1],
+            abundance_dim=dataset.node_depths.shape[1],
+            use_gnn=use_gnn,
+            use_noise=args.noise, # not being used
+            loglevel=args.loglevel,
+            pretrainvae=0
+        )
+
+        if args.batchtype == "auto":
+            if args.ae_alpha > 0 and args.graph_alpha == 0 and args.scg_alpha == 0:
+                args.batchtype = "nodes"
+            else:
+                args.batchtype = "edges"
+        scg_idx = np.arange(len(neg_pair_idx))
+        # create eval split
+        if args.eval_split == 0:
+            if "node" in args.batchtype:
+                train_idx = np.arange(len(features))
+            elif "edge" in args.batchtype:
+                train_idx = np.arange(gnn_model.adj.indices.shape[0])
+            eval_idx = []
+        else:
+            if "node" in args.batchtype:
+                train_idx = np.array(random.sample(list(range(gnn_model.adj.indices.shape[0])), int(gnn_model.adj.indices.shape[0]*(1-args.eval_split))))
+                eval_idx = np.array([x for x in np.arange(gnn_model.adj.indices.shape[0]) if x not in train_idx])
+            elif "edge" in args.batchtype:
+                train_idx = np.array(random.sample(list(range(gnn_model.adj.indices.shape[0])), int(gnn_model.adj.indices.shape[0]*(1-args.eval_split))))
+                eval_idx = np.array([x for x in np.arange(gnn_model.adj.indices.shape[0]) if x not in train_idx])
+            logging.info(f"**** using {gnn_model.adj.indices.shape[0]} for training and {gnn_model.adj.indices.shape[0]} for eval")
+        #edges_idx = np.arange(gnn_model.adj.indices.shape[0])
+        features = np.array(features)
+        pbar_epoch = tqdm(range(epochs), disable=args.quiet, position=0)
+        scores = [stats]
+        best_embs, best_vae_embs, best_model, best_score, best_epoch = None, None, None, 0, 0
+        
+        # increasing batch size
+        batch_size = args.batchsize
+        if batch_size == 0:
+            batch_size = len(train_idx)
+        logger.info("**** initial {} batch size: {} ****".format(args.batchtype, batch_size))
+        mlflow.log_metric("cur_batch_size", batch_size, 0)
+        batch_steps = [25, 75, 150, 300]
+        batch_steps = [x for i, x in enumerate(batch_steps) if (2 ** (i+1))*batch_size < len(train_idx)]
+        logger.info("**** epoch batch size doubles: {} ****".format(str(batch_steps)))
+        gold_labels = np.array([dataset.labels.index(dataset.node_to_label[n]) for n in dataset.node_names])
+        step = 0
+        scores_string = ""
+        
+        for e in pbar_epoch:
+            #vae_epoch_losses = {"kld_loss": [], "vae_loss": [], "kmer_loss": [], "ab_loss": []}
+            recon_loss = 0
+            trainer.epoch = e
+            # train VAE in batches
+            if e in batch_steps:
+                print(f'Increasing {args.batchtype} batch size from {batch_size:d} to {batch_size*2:d}')
+                batch_size = batch_size * 2
+                mlflow.log_metric("cur_batch_size", batch_size, e )
+
+            ############################################################
+            vae_losses_epoch = {}
+            gnn_losses_epoch = {}
+            total_losses_epoch = []
+
+            # train model ################################################
+            np.random.shuffle(train_idx)
+
+            #graph_batch_size = 256
+            #graph_batch_size = len(edges_idx)
+            n_batches = len(train_idx)//batch_size
+            if use_last_batch and n_batches < len(train_idx)/batch_size:
+                n_batches += 1 # add final batch
+            if args.scg_alpha > 0:
+                scg_batch_size = len(neg_pair_idx)//n_batches
+            pbar_gnnbatch = tqdm(range(n_batches),
+                                 disable=(args.quiet or batch_size == len(train_idx) or n_batches < 1000),
+                                 position=1, ascii=' =')
+            for b in pbar_gnnbatch:
+                if "edge" in args.batchtype:
+                    nodes_batch, edges_batch = None, train_idx[b*batch_size:(b+1)*batch_size]
+                elif "node" in args.batchtype:
+                    nodes_batch, edges_batch = train_idx[b*batch_size:(b+1)*batch_size], None
+                if args.scg_alpha > 0:
+                    scg_batch = scg_idx #[b*scg_batch_size:(b+1)*scg_batch_size]
+                else:
+                    scg_batch = None
+                losses = trainer.train_unsupervised(edges_idx=edges_batch,
+                                                    nodes_idx=nodes_batch,
+                                                    scgs_idx=scg_batch, vae=True,
+                                                    gold_labels=gold_labels)
+                total_loss, gnn_losses, ae_losses = losses
+                total_losses_epoch.append(total_loss.numpy())
+                for l in gnn_losses: gnn_losses_epoch.setdefault(l,[]).append(gnn_losses[l])
+                for l in ae_losses: vae_losses_epoch.setdefault(l,[]).append(ae_losses[l])
+
+                #add losses to get epoch avg
+            if args.scg_alpha > 0:
+                scg_loss = trainer.train_scg_only()
+                scg_loss = scg_loss.numpy()
+            else:
+                scg_loss = 0
+            epoch_metrics = {"Total": np.average(total_losses_epoch),
+                             "gnn": np.average(gnn_losses_epoch["gnn_loss"]),
+                             #"SCG": np.average(gnn_losses_epoch["scg_loss"]),
+                             "SCG": scg_loss,
+                             "pred": np.average(gnn_losses_epoch["pred_loss"]),
+                            #'GNN  LR': float(trainer.opt._decayed_lr(float)),
+                            "pos": np.average(gnn_losses_epoch["pos"]),
+                            "neg": np.average(gnn_losses_epoch["neg"]),
+                            "kld": np.average(vae_losses_epoch["kld"]),
+                            "vae": np.average(vae_losses_epoch["vae_loss"]),
+                            "kmer": np.average(vae_losses_epoch["kmer_loss"]),
+                            "ab": np.average( vae_losses_epoch["ab_loss"])}
+                            #"logvar": ae_losses["mean_logvar"],
+                            #"grad_norm": ae_losses["grad_norm"],
+                            #"grad_norm_clip": ae_losses["grad_norm_clip"]}
+            #print(float(gnn_trainer.opt._decayed_lr(float)))
+            mlflow.log_metrics(epoch_metrics, step=e)
+            ##############################################################
+
+
+            # eval loss:TODO #######################################################
+
+            gpu_mem_alloc = tf.config.experimental.get_memory_info('GPU:0')["peak"] / 1000000 if args.cuda else 0
+            #gpu_mem_alloc = tf.config.experimental.get_memory_usage('GPU:0') / 1000000 if args.cuda else 0
+            # eval checkpoint ##############################################################
+            if (e + 1) % RESULT_EVERY == 0 and e > args.evalskip and target_metric != "noeval":
+                evalstarttime = datetime.datetime.now()
+               
+                gnn_input_features = trainer.encoder(features)[0]
+                #trainer.features = gnn_input_features
+                logger.debug("encoder output " + str(gnn_input_features[0][:5].numpy()))
+                if use_gnn:
+                    node_new_features = trainer.gnn_model(gnn_input_features, None, training=False)
+                    
+                    if args.concatfeatures:
+                        node_new_features = tf.concat((gnn_input_features,
+                                                        node_new_features), axis=1).numpy()
+                    else:
+                        node_new_features = node_new_features.numpy()
+                        #node_new_features = gnn_input_features.numpy()
+                else:
+                    node_new_features = gnn_input_features.numpy()
+
+                    
+                weights = (trainer.encoder.get_weights(), trainer.gnn_model.get_weights())
+                eval_output = eval_epoch(node_new_features, cluster_mask, weights,
+                                         args, dataset, e, scores, best_score, best_embs,
+                                         best_epoch, best_model, target_metric)
+                best_score, best_embs, best_epoch, scores, best_model, cluster_labels = eval_output
+                stats = scores[-1]
+                all_cluster_labels.append(cluster_labels)
+                if args.quiet:
+                    logger.info(f"--- EPOCH {e:d} ---")
+                    scores_string = f"HQ={stats['hq']}  Best{target_metric}={round(best_score, 3)} Best Epoch={best_epoch} Cur={round(stats.get(target_metric,0), 3)}"
+                    losses_string = " ".join([f"{k}={v:.3f}" for k, v in epoch_metrics.items()])
+                    logger.info(f"[{args.outname} {nlayers_gnn}l {pname}]{losses_string} {scores_string} GPU={gpu_mem_alloc:.1f}MB")
+                    logger.info(str(stats))
+                mlflow.log_metrics(stats, step=e)
+                #print("total eval time", datetime.datetime.now() - evalstarttime)
+            losses_string = " ".join([f"{k}={v:.3f}" for k, v in epoch_metrics.items() if v != 0])
+            scores_string = f"Best{target_metric}={round(best_score, 3)} BestEpoch={best_epoch} Cur{target_metric}={round(stats.get(target_metric,0), 3)}"
+            pbar_epoch.set_description(
+                f"[{args.outname} {pname}] {losses_string} {scores_string} GPU={gpu_mem_alloc:.1f}MB"
+            )
+
+        #################################################################
+        if best_embs is None and target_metric != "noeval":
+            best_embs = node_new_features
+        else:
+            node_new_features = trainer.encoder(features)[0]
+        if tf.is_tensor(node_new_features):
+            node_new_features = node_new_features.numpy()
+        cluster_labels, stats, _, _ = compute_clusters_and_stats(
+            node_new_features, node_names, dataset, clustering=clustering, k=k,
+            amber=(args.labels is not None and "amber" in args.labels),
+            cuda=args.cuda,
+        )
+        
+        all_cluster_labels.append(cluster_labels)
+        stats["epoch"] = e
+        scores.append(stats)
+        # get best stats:
+        if target_metric != "noeval":
+            # get best stats:
+            target_scores = [s[target_metric] for s in scores]
+            best_idx = np.argmax(target_scores)
+        else:
+            best_embs = node_new_features
+            best_idx = -1
+        mlflow.log_metrics(scores[best_idx], step=e+1)
+        logger.info(f">>> Last epoch: {RESULT_EVERY + (best_idx*RESULT_EVERY)} : {stats} <<<")
+        logger.info(f">>> best epoch: {RESULT_EVERY + (best_idx*RESULT_EVERY)} : {scores[best_idx]} <<<")
+        with open(f"{args.outdir}/{args.outname}_{nrun}_best_contig2bin.tsv", "w") as f:
+            f.write("@Version:0.9.0\n@SampleID:SAMPLEID\n@@SEQUENCEID\tBINID\n")
+            for i in range(len(all_cluster_labels[best_idx])):
+                f.write(f"{node_names[i]}\t{all_cluster_labels[best_idx][i]}\n")
+     
+        #plot edges vs initial embs
+        #plot_edges_sim(best_vae_embs, dataset.adj_matrix, id_to_scg, "vae_")
+        if plot:
+            plot_edges_sim(best_embs, dataset.adj_matrix, id_to_scg, "posttrain_")
+        return best_embs, scores[best_idx], all_cluster_labels[best_idx]
```

### Comparing `graphmb-0.2.4/src/graphmb/train_gnn.py` & `graphmb-0.2.5/src/graphmb/train_gnn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,220 +1,220 @@
-import numpy as np
-import datetime
-import os
-import tensorflow as tf
-import random
-import logging
-from tqdm import tqdm
-import mlflow
-from graphmb.models import  TH
-from graphmb.utils import set_seed # , run_tsne, plot_embs, plot_edges_sim
-from graphmb.train_ccvae import prepare_data_for_gnn
-from graphmb.visualize import plot_edges_sim
-from graphmb.evaluate import compute_clusters_and_stats, eval_epoch
-from graphmb.utils import get_cluster_mask
-from graphmb.gnn_models import name_to_model
-
-
-def run_model_gnn(dataset, args, logger, nrun, target_metric):
-    set_seed(args.seed)
-    node_names = np.array(dataset.node_names)
-    RESULT_EVERY = args.evalepochs
-    hidden_gnn = args.hidden_gnn
-    output_dim_gnn = args.embsize_gnn
-    epochs = args.epoch
-    lr_gnn = args.lr_gnn
-    nlayers_gnn = args.layers_gnn
-    gname = args.model_name
-    gmodel_type = name_to_model[gname.split("_")[0].upper()]
-    clustering = args.clusteringalgo
-    k = args.kclusters
-    use_disconnected = not args.quick
-    cluster_markers_only = args.quick
-    use_edge_weights = True
-    concat_features = True # bypass args, otherwise results are bad
-    
-    with mlflow.start_run(run_name=args.assembly.split("/")[-1] + "-" + args.outname):
-        mlflow.log_params(vars(args))
-        current_time = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
-        tf.config.run_functions_eagerly(True)
-
-        X, adj, cluster_mask, neg_pair_idx, pos_pair_idx = prepare_data_for_gnn(
-                dataset, use_edge_weights, cluster_markers_only, use_raw=args.rawfeatures,
-                binarize=args.binarize, remove_edges=args.noedges)
-        if nrun == 0:
-            print("logging to mlflow")
-            logger.info("******* Running model: {} **********".format(gname))
-            logger.info("***** using edge weights: {} ******".format(use_edge_weights))
-            logger.info("***** using disconnected: {} ******".format(use_disconnected))
-            logger.info("***** concat features: {} *****".format(concat_features))
-            logger.info("***** cluster markers only: {} *****".format(cluster_markers_only))
-            logger.info("***** threshold adj matrix: {} *****".format(args.binarize))
-            logger.info("***** self edges only: {} *****".format(args.noedges))
-            logger.info("***** Using raw kmer+abund features: {}".format(args.rawfeatures))
-        
-            logger.info("***** SCG neg pairs: {}".format(neg_pair_idx.shape))
-            logger.info("***** input features dimension: {}".format(X[cluster_mask].shape[1]))
-            logger.info("***** Nodes used for clustering: {}".format(X[cluster_mask].shape[0]))
-
-        #plot edges vs initial embs
-        #id_to_scg = {i: set(dataset.contig_markers.get(node_name, {}).keys()) for i, node_name in enumerate(dataset.node_names)}
-        #plot_edges_sim(X, dataset.adj_matrix, id_to_scg, f"{args.outdir}/{args.outname}_pretrain_")
-
-        # pre train clustering
-        if not args.skip_preclustering and nrun == 0:
-            cluster_labels, stats, _, hq_bins = compute_clusters_and_stats(
-                        X[cluster_mask], node_names[cluster_mask],
-                        dataset, clustering=clustering, k=k,
-                        amber=(args.labels is not None and "amber" in args.labels),
-                        cuda=args.cuda,
-                    )
-            logger.info(f">>> Pre train stats: {str(stats)}")
-        else:
-            stats = {"hq": 0, "epoch":0, target_metric: 0}
-        
-        scores = [stats]
-        losses = {"total": [], "ae": [], "gnn": [], "scg": []}
-        X = X.astype(np.float32)
-        features = tf.constant(X)
-        input_dim_gnn = X.shape[1]
-    
-        logger.info(f"*** Model input dim {X.shape[1]}, GNN input dim {input_dim_gnn}")
-
-        gnn_model = gmodel_type(
-            features_shape=features.shape,
-            input_dim=input_dim_gnn,
-            labels=None,
-            adj=adj,
-            embsize=output_dim_gnn,
-            hidden_units=hidden_gnn,
-            layers=nlayers_gnn,
-            conv_last=False,
-        )
-        logger.info(f"*** output clustering dim {output_dim_gnn}")
-
-        th = TH(
-            features,
-            gnn_model=gnn_model,
-            lr=lr_gnn,
-            all_different_idx=neg_pair_idx,
-            all_same_idx=pos_pair_idx,
-            ae_encoder=None,
-            ae_decoder=None,
-            latentdim=output_dim_gnn,
-            graph_weight=float(args.graph_alpha),
-            ae_weight=float(args.ae_alpha),
-            scg_weight=float(args.scg_alpha),
-            num_negatives=args.negatives,
-            decoder_input=args.decoder_input,
-        )
-
-        #gnn_model.summary()
-        if args.eval_split == 0:
-            train_idx = np.arange(len(features))
-            eval_idx = []
-        else:
-            train_idx = np.array(random.sample(list(range(len(features))), int(len(features)*(1-args.eval_split))))
-            eval_idx = np.array([x for x in np.arange(len(features)) if x not in train_idx])
-            logging.info(f"**** using {len(train_idx)} for training and {len(eval_idx)} for eval")
-        features = np.array(features)
-        pbar_epoch = tqdm(range(epochs), disable=args.quiet, position=0)
-        scores = []
-        best_embs = None
-        best_model = th.gnn_model.get_weights()
-        best_score = 0
-        best_epoch = 0
-        batch_size = args.batchsize
-        scores_string = ""
-        if batch_size == 0:
-            batch_size = len(train_idx)
-        all_cluster_labels = []
-        step = 0
-        for e in pbar_epoch:
-            np.random.shuffle(train_idx)
-            step += 1
-            loss, gnn_losses, ae_losses = th.train_unsupervised(train_idx, scg=True)
-            epoch_losses = {"Total": loss.numpy(),
-                            "gnn": gnn_losses["gnn_loss"].numpy(),
-                             "SCG": gnn_losses["scg_loss"].numpy(),
-                             #"pred": gnn_losses["pred_loss"],
-                            #'GNN  LR': float(trainer.opt._decayed_lr(float)),
-                            "pos": gnn_losses["pos"].numpy(),
-                            "neg": gnn_losses["neg"].numpy()}
-            mlflow.log_metrics(epoch_losses, step=step)
-            gnn_loss = epoch_losses["gnn"]
-            diff_loss = epoch_losses["SCG"]
-
-            if args.eval_split > 0:
-                eval_total_loss, eval_gnn_loss, eval_diff_loss, eval_pos_loss, \
-                    eval_neg_loss = th.train_unsupervised(eval_idx, training=False)
-                eval_epoch_losses = {"Eval gnn loss": float(eval_gnn_loss), "Eval SCG loss": float(eval_diff_loss),
-                                     "Eval GNN loss": float(eval_total_loss),
-                                     "Eval pos loss": float(eval_pos_loss),
-                                     "Eval neg_loss": float(eval_neg_loss)}
-                mlflow.log_metrics(eval_epoch_losses, step=step)
-            #else:
-            #    eval_loss, eval_mse1, eval_mse2, eval_kld = 0, 0, 0, 0
-
-            gpu_mem_alloc = tf.config.experimental.get_memory_info('GPU:0')["peak"] / 1000000 if args.cuda else 0
-            #gpu_mem_alloc = tf.config.experimental.get_memory_usage('GPU:0') / 1000000 if args.cuda else 0
-            if (e + 1) % RESULT_EVERY == 0 and e > args.evalskip and target_metric != "noeval":
-                gnn_input_features = features
-                node_new_features = th.gnn_model(gnn_input_features, None, training=False)
-                node_new_features = node_new_features.numpy()
-                if concat_features:
-                    node_new_features = tf.concat([gnn_input_features, node_new_features], axis=1).numpy()
-                eval_output = eval_epoch(node_new_features, cluster_mask, th.gnn_model.get_weights(),
-                                         args, dataset, e, scores, best_score, best_embs, best_epoch,
-                                         best_model, target_metric=target_metric)
-                
-                best_score, best_embs, best_epoch, scores, best_model, cluster_labels = eval_output
-                stats = scores[-1]
-                if args.quiet:
-                    logger.info(f"--- EPOCH {e:d} ---")
-                    scores_string = f"HQ={stats['hq']}   Best{target_metric}={round(best_score, 3)} Best Epoch={best_epoch}"
-                    logger.info(f"[{gname} {nlayers_gnn}l] L={gnn_loss:.3f} D={diff_loss:.3f} {scores_string} GPU={gpu_mem_alloc:.1f}MB")
-                    logger.info(str(stats))
-                mlflow.log_metrics(stats, step=step)
-                all_cluster_labels.append(cluster_labels)
-                scores_string = f"HQ={stats['hq']}  Best{target_metric}={round(best_score, 3)}  Best Epoch={best_epoch}"
-            pbar_epoch.set_description(
-                f"[{args.outname} {nlayers_gnn}l] L={gnn_loss:.3f} D={diff_loss:.3f} {scores_string} GPU={gpu_mem_alloc:.1f}MB"
-            )
-            total_loss = gnn_loss + diff_loss
-            losses["gnn"].append(gnn_loss)
-            losses["scg"].append(diff_loss)
-            losses["total"].append(total_loss)
-
-        gnn_model.set_weights(best_model)
-        node_new_features = th.gnn_model(features, None, training=False)
-        node_new_features = node_new_features.numpy()
-        if best_embs is None or target_metric != "noeval":
-            best_embs = node_new_features
-        if concat_features:
-            node_new_features = tf.concat([features, node_new_features], axis=1).numpy()
-        cluster_labels, stats, _, _ = compute_clusters_and_stats(
-            node_new_features, node_names, dataset,
-            clustering=clustering, k=k, amber=(args.labels is not None and "amber" in args.labels),
-            cuda=args.cuda,
-        )
-        all_cluster_labels.append(cluster_labels)
-        stats["epoch"] = e
-        scores.append(stats)
-        if target_metric != "noeval":
-            # get best stats:
-            target_scores = [s[target_metric] for s in scores]
-            best_idx = np.argmax(target_scores)
-        else:
-            best_embs = node_new_features
-            best_idx = -1
-        mlflow.log_metrics(scores[best_idx], step=step+1)
-    logger.info(f">>> best epoch all contigs: {RESULT_EVERY + (best_idx*RESULT_EVERY)} : {stats} <<<")
-    logger.info(f">>> best epoch: {RESULT_EVERY + (best_idx*RESULT_EVERY)} : {scores[best_idx]} <<<")
-    with open(f"{args.outdir}/{args.outname}_{nrun}_best_contig2bin.tsv", "w") as f:
-        f.write("@Version:0.9.0\n@SampleID:SAMPLEID\n@@SEQUENCEID\tBINID\n")
-        for i in range(len(all_cluster_labels[best_idx])):
-            f.write(f"{node_names[i]}\t{all_cluster_labels[best_idx][i]}\n")
-    #plot edges vs final embs
-    #plot_edges_sim(best_embs, dataset.adj_matrix, id_to_scg, f"{args.outdir}/{args.outname}_posttrain_")
-    return best_embs, scores[best_idx]
-
+import numpy as np
+import datetime
+import os
+import tensorflow as tf
+import random
+import logging
+from tqdm import tqdm
+import mlflow
+from graphmb.models import  TH
+from graphmb.utils import set_seed # , run_tsne, plot_embs, plot_edges_sim
+from graphmb.train_ccvae import prepare_data_for_gnn
+from graphmb.visualize import plot_edges_sim
+from graphmb.evaluate import compute_clusters_and_stats, eval_epoch
+from graphmb.utils import get_cluster_mask
+from graphmb.gnn_models import name_to_model
+
+
+def run_model_gnn(dataset, args, logger, nrun, target_metric):
+    set_seed(args.seed)
+    node_names = np.array(dataset.node_names)
+    RESULT_EVERY = args.evalepochs
+    hidden_gnn = args.hidden_gnn
+    output_dim_gnn = args.embsize_gnn
+    epochs = args.epoch
+    lr_gnn = args.lr_gnn
+    nlayers_gnn = args.layers_gnn
+    gname = args.model_name
+    gmodel_type = name_to_model[gname.split("_")[0].upper()]
+    clustering = args.clusteringalgo
+    k = args.kclusters
+    use_disconnected = not args.quick
+    cluster_markers_only = args.quick
+    use_edge_weights = True
+    concat_features = True # bypass args, otherwise results are bad
+    
+    with mlflow.start_run(run_name=args.assembly.split("/")[-1] + "-" + args.outname):
+        mlflow.log_params(vars(args))
+        current_time = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
+        tf.config.run_functions_eagerly(True)
+
+        X, adj, cluster_mask, neg_pair_idx, pos_pair_idx = prepare_data_for_gnn(
+                dataset, use_edge_weights, cluster_markers_only, use_raw=args.rawfeatures,
+                binarize=args.binarize, remove_edges=args.noedges)
+        if nrun == 0:
+            print("logging to mlflow")
+            logger.info("******* Running model: {} **********".format(gname))
+            logger.info("***** using edge weights: {} ******".format(use_edge_weights))
+            logger.info("***** using disconnected: {} ******".format(use_disconnected))
+            logger.info("***** concat features: {} *****".format(concat_features))
+            logger.info("***** cluster markers only: {} *****".format(cluster_markers_only))
+            logger.info("***** threshold adj matrix: {} *****".format(args.binarize))
+            logger.info("***** self edges only: {} *****".format(args.noedges))
+            logger.info("***** Using raw kmer+abund features: {}".format(args.rawfeatures))
+        
+            logger.info("***** SCG neg pairs: {}".format(neg_pair_idx.shape))
+            logger.info("***** input features dimension: {}".format(X[cluster_mask].shape[1]))
+            logger.info("***** Nodes used for clustering: {}".format(X[cluster_mask].shape[0]))
+
+        #plot edges vs initial embs
+        #id_to_scg = {i: set(dataset.contig_markers.get(node_name, {}).keys()) for i, node_name in enumerate(dataset.node_names)}
+        #plot_edges_sim(X, dataset.adj_matrix, id_to_scg, f"{args.outdir}/{args.outname}_pretrain_")
+
+        # pre train clustering
+        if not args.skip_preclustering and nrun == 0:
+            cluster_labels, stats, _, hq_bins = compute_clusters_and_stats(
+                        X[cluster_mask], node_names[cluster_mask],
+                        dataset, clustering=clustering, k=k,
+                        amber=(args.labels is not None and "amber" in args.labels),
+                        cuda=args.cuda,
+                    )
+            logger.info(f">>> Pre train stats: {str(stats)}")
+        else:
+            stats = {"hq": 0, "epoch":0, target_metric: 0}
+        
+        scores = [stats]
+        losses = {"total": [], "ae": [], "gnn": [], "scg": []}
+        X = X.astype(np.float32)
+        features = tf.constant(X)
+        input_dim_gnn = X.shape[1]
+    
+        logger.info(f"*** Model input dim {X.shape[1]}, GNN input dim {input_dim_gnn}")
+
+        gnn_model = gmodel_type(
+            features_shape=features.shape,
+            input_dim=input_dim_gnn,
+            labels=None,
+            adj=adj,
+            embsize=output_dim_gnn,
+            hidden_units=hidden_gnn,
+            layers=nlayers_gnn,
+            conv_last=False,
+        )
+        logger.info(f"*** output clustering dim {output_dim_gnn}")
+
+        th = TH(
+            features,
+            gnn_model=gnn_model,
+            lr=lr_gnn,
+            all_different_idx=neg_pair_idx,
+            all_same_idx=pos_pair_idx,
+            ae_encoder=None,
+            ae_decoder=None,
+            latentdim=output_dim_gnn,
+            graph_weight=float(args.graph_alpha),
+            ae_weight=float(args.ae_alpha),
+            scg_weight=float(args.scg_alpha),
+            num_negatives=args.negatives,
+            decoder_input=args.decoder_input,
+        )
+
+        #gnn_model.summary()
+        if args.eval_split == 0:
+            train_idx = np.arange(len(features))
+            eval_idx = []
+        else:
+            train_idx = np.array(random.sample(list(range(len(features))), int(len(features)*(1-args.eval_split))))
+            eval_idx = np.array([x for x in np.arange(len(features)) if x not in train_idx])
+            logging.info(f"**** using {len(train_idx)} for training and {len(eval_idx)} for eval")
+        features = np.array(features)
+        pbar_epoch = tqdm(range(epochs), disable=args.quiet, position=0)
+        scores = []
+        best_embs = None
+        best_model = th.gnn_model.get_weights()
+        best_score = 0
+        best_epoch = 0
+        batch_size = args.batchsize
+        scores_string = ""
+        if batch_size == 0:
+            batch_size = len(train_idx)
+        all_cluster_labels = []
+        step = 0
+        for e in pbar_epoch:
+            np.random.shuffle(train_idx)
+            step += 1
+            loss, gnn_losses, ae_losses = th.train_unsupervised(train_idx, scg=True)
+            epoch_losses = {"Total": loss.numpy(),
+                            "gnn": gnn_losses["gnn_loss"].numpy(),
+                             "SCG": gnn_losses["scg_loss"].numpy(),
+                             #"pred": gnn_losses["pred_loss"],
+                            #'GNN  LR': float(trainer.opt._decayed_lr(float)),
+                            "pos": gnn_losses["pos"].numpy(),
+                            "neg": gnn_losses["neg"].numpy()}
+            mlflow.log_metrics(epoch_losses, step=step)
+            gnn_loss = epoch_losses["gnn"]
+            diff_loss = epoch_losses["SCG"]
+
+            if args.eval_split > 0:
+                eval_total_loss, eval_gnn_loss, eval_diff_loss, eval_pos_loss, \
+                    eval_neg_loss = th.train_unsupervised(eval_idx, training=False)
+                eval_epoch_losses = {"Eval gnn loss": float(eval_gnn_loss), "Eval SCG loss": float(eval_diff_loss),
+                                     "Eval GNN loss": float(eval_total_loss),
+                                     "Eval pos loss": float(eval_pos_loss),
+                                     "Eval neg_loss": float(eval_neg_loss)}
+                mlflow.log_metrics(eval_epoch_losses, step=step)
+            #else:
+            #    eval_loss, eval_mse1, eval_mse2, eval_kld = 0, 0, 0, 0
+
+            gpu_mem_alloc = tf.config.experimental.get_memory_info('GPU:0')["peak"] / 1000000 if args.cuda else 0
+            #gpu_mem_alloc = tf.config.experimental.get_memory_usage('GPU:0') / 1000000 if args.cuda else 0
+            if (e + 1) % RESULT_EVERY == 0 and e > args.evalskip and target_metric != "noeval":
+                gnn_input_features = features
+                node_new_features = th.gnn_model(gnn_input_features, None, training=False)
+                node_new_features = node_new_features.numpy()
+                if concat_features:
+                    node_new_features = tf.concat([gnn_input_features, node_new_features], axis=1).numpy()
+                eval_output = eval_epoch(node_new_features, cluster_mask, th.gnn_model.get_weights(),
+                                         args, dataset, e, scores, best_score, best_embs, best_epoch,
+                                         best_model, target_metric=target_metric)
+                
+                best_score, best_embs, best_epoch, scores, best_model, cluster_labels = eval_output
+                stats = scores[-1]
+                if args.quiet:
+                    logger.info(f"--- EPOCH {e:d} ---")
+                    scores_string = f"HQ={stats['hq']}   Best{target_metric}={round(best_score, 3)} Best Epoch={best_epoch}"
+                    logger.info(f"[{gname} {nlayers_gnn}l] L={gnn_loss:.3f} D={diff_loss:.3f} {scores_string} GPU={gpu_mem_alloc:.1f}MB")
+                    logger.info(str(stats))
+                mlflow.log_metrics(stats, step=step)
+                all_cluster_labels.append(cluster_labels)
+                scores_string = f"HQ={stats['hq']}  Best{target_metric}={round(best_score, 3)}  Best Epoch={best_epoch}"
+            pbar_epoch.set_description(
+                f"[{args.outname} {nlayers_gnn}l] L={gnn_loss:.3f} D={diff_loss:.3f} {scores_string} GPU={gpu_mem_alloc:.1f}MB"
+            )
+            total_loss = gnn_loss + diff_loss
+            losses["gnn"].append(gnn_loss)
+            losses["scg"].append(diff_loss)
+            losses["total"].append(total_loss)
+
+        gnn_model.set_weights(best_model)
+        node_new_features = th.gnn_model(features, None, training=False)
+        node_new_features = node_new_features.numpy()
+        if best_embs is None or target_metric != "noeval":
+            best_embs = node_new_features
+        if concat_features:
+            node_new_features = tf.concat([features, node_new_features], axis=1).numpy()
+        cluster_labels, stats, _, _ = compute_clusters_and_stats(
+            node_new_features, node_names, dataset,
+            clustering=clustering, k=k, amber=(args.labels is not None and "amber" in args.labels),
+            cuda=args.cuda,
+        )
+        all_cluster_labels.append(cluster_labels)
+        stats["epoch"] = e
+        scores.append(stats)
+        if target_metric != "noeval":
+            # get best stats:
+            target_scores = [s[target_metric] for s in scores]
+            best_idx = np.argmax(target_scores)
+        else:
+            best_embs = node_new_features
+            best_idx = -1
+        mlflow.log_metrics(scores[best_idx], step=step+1)
+    logger.info(f">>> best epoch all contigs: {RESULT_EVERY + (best_idx*RESULT_EVERY)} : {stats} <<<")
+    logger.info(f">>> best epoch: {RESULT_EVERY + (best_idx*RESULT_EVERY)} : {scores[best_idx]} <<<")
+    with open(f"{args.outdir}/{args.outname}_{nrun}_best_contig2bin.tsv", "w") as f:
+        f.write("@Version:0.9.0\n@SampleID:SAMPLEID\n@@SEQUENCEID\tBINID\n")
+        for i in range(len(all_cluster_labels[best_idx])):
+            f.write(f"{node_names[i]}\t{all_cluster_labels[best_idx][i]}\n")
+    #plot edges vs final embs
+    #plot_edges_sim(best_embs, dataset.adj_matrix, id_to_scg, f"{args.outdir}/{args.outname}_posttrain_")
+    return best_embs, scores[best_idx], all_cluster_labels[best_idx]
+
```

### Comparing `graphmb-0.2.4/src/graphmb/utils.py` & `graphmb-0.2.5/src/graphmb/utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-from pathlib import Path
-import time
-import os
-import sys
-import math
-import pdb
-import itertools
-from collections import Counter
-import networkx as nx
-import numpy as np
-from tqdm import tqdm
-import datetime
-import operator
-import scipy
-import logging
-# import dgl
-import random
-from sklearn.cluster import KMeans
-#import tensorflow as tf
-
-SEED = 0
-
-def set_seed(seed=0):
-    if "dgl" in sys.modules:
-        import dgl
-        print("setting dgl seed")
-        dgl.random.seed(seed)
-    if "torch" in sys.modules:
-        import torch
-        print("setting torch seed")
-        torch.manual_seed(seed)
-    random.seed(seed)
-    np.random.seed(seed)
-    if "tensorflow" in sys.modules:
-        import tensorflow
-        print("setting tf seed")
-        tensorflow.random.set_seed(seed)
-
-
-
-class Read:
-    def __init__(self, readid, species=None):
-        self.readid = readid
-        self.species = species
-        self.mappings = set()
-
-
-class ReadMapping:
-    def __init__(self, readid, bitflag, contigname, pos, mapq, seq):
-        self.readid = readid
-        self.bitflag = bitflag
-        self.contigname = contigname
-        self.pos = pos
-        self.mapq = mapq
-
-
-def get_cluster_mask(quick, dataset):
-    if quick and dataset.contig_markers is not None:
-        #connected_marker_nodes = filter_disconnected(dataset.adj_matrix, dataset.node_names, dataset.contig_markers)
-        nodes_with_markers = [
-            i
-            for i, n in enumerate(dataset.node_names)
-            if n in dataset.contig_markers and len(dataset.contig_markers[n]) > 0
-        ]
-        print("eval cluster with ", len(nodes_with_markers), "contigds with markers")
-        cluster_mask = [n in nodes_with_markers for n in range(len(dataset.node_names))]
-    else:
-        cluster_mask = [True] * len(dataset.node_names)
-    return cluster_mask
-
-def save_model(args, epoch, th, th_vae):
-    if th_vae is not None:
-        # save encoder and decoder
-        th_vae.encoder.save(os.path.join(args.outdir, args.outname + "_best_encoder"))
-        th_vae.decoder.save(os.path.join(args.outdir, args.outname + "_best_decoder"))
-    if th is not None:
-        th.gnn_model.save(os.path.join(args.outdir, args.outname + "_best_gnn"))
-
-
-def run_clustering(X, node_names, clustering_algo, cuda, k=0, tsne=False):
-    
-    if clustering_algo == "vamb":
-        from graphmb.vamb_clustering import cluster as vamb_cluster
-        starttime = datetime.datetime.now()
-        X = X.astype(np.float32)
-        cluster_to_contig = {
-            i: c for (i, (n, c)) in enumerate(vamb_cluster(X, node_names, cuda=cuda))
-        }
-        clustering_time = datetime.datetime.now()
-        #print("clustering time", clustering_time-starttime)
-        contig_to_bin = {}
-        #for b in cluster_to_contig:
-        #    for contig in cluster_to_contig[b]:
-        #        contig_to_bin[contig] = b
-        for k, v in cluster_to_contig.items():
-            contig_to_bin.update({n: k for n in v})
-        labels = np.array([contig_to_bin[n] for n in node_names])
-        # very slow code:
-        cluster_centroids = None
-        if tsne:
-            cluster_to_embs = {
-                c: np.array([X[i] for i, n in enumerate(node_names) if n in cluster_to_contig[c]])
-                for c in cluster_to_contig
-            }
-            cluster_centroids = np.array([cluster_to_embs[c].mean(0) for c in cluster_to_contig])
-        processing_time = datetime.datetime.now()
-        #print("processing time",  processing_time - clustering_time)
-    elif clustering_algo == "kmeansbatch":
-        kmeans = MiniBatchKMeans(n_clusters=k, random_state=0, batch_size=2048, verbose=0) #, init=seed_matrix)
-        labels = kmeans.fit_predict(X)
-        contig_to_bin = {node_names[i]: labels[i] for i in range(len(node_names))}
-        cluster_to_contig = {i: [] for i in range(k)}
-        for i in range(len(node_names)):
-            cluster_to_contig[labels[i]].append(node_names[i])
-        #cluster_centroids = kmeans.cluster_centers_
-    elif clustering_algo == "kmeansgpu":
-        pass
-    elif clustering_algo == "kmedoids":
-        import kmedoids
-        breakpoint()
-        # TODO do this on gpu if avail
-        D = np.sum((X[:,None]-X[None])**2, axis=-1)
-        # TODO find best k
-        km = kmedoids.KMedoids(20, method='fasterpam')
-        cluster_labels = km.fit_predict(D).astype(np.int64)
-    elif clustering_algo == "kmeans":
-        clf = KMeans(k, random_state=1234)
-        labels = clf.fit_predict(X)
-        contig_to_bin = {node_names[i]: labels[i] for i in range(len(node_names))}
-        cluster_to_contig = {i: [] for i in range(k)}
-        for i in range(len(node_names)):
-            cluster_to_contig[labels[i]].append(node_names[i])
-        cluster_centroids = None
-    return cluster_to_contig, contig_to_bin, labels, cluster_centroids
-
-def filter_disconnected(adj, node_names, markers):
-    # get idx of nodes that are connected or have at least one marker
-    graph = nx.convert_matrix.from_scipy_sparse_matrix(adj, edge_attribute="weight")
-    # breakpoint()
-    nodes_to_remove = set()
-    for n1 in graph.nodes:
-        if len(list(graph.neighbors(n1))) == 0 or (
-            node_names[n1] not in markers or len(markers[node_names[n1]]) == 0
-        ):
-            nodes_to_remove.add(n1)
-
-    graph.remove_nodes_from(list(nodes_to_remove))
-    assert len(graph.nodes()) == (len(node_names)-len(nodes_to_remove))
-    print(f"{len(nodes_to_remove)} nodes without edges nor markers, keeping {len(graph.nodes())} nodes")
-    return set(graph.nodes())
-
-def run_model_vgae(dataset, args, logger, nrun):
-    node_names = np.array(dataset.node_names)
-    RESULT_EVERY = args.evalepochs
-    hidden_gnn = args.hidden_gnn
-    hidden_vae = args.hidden_vae
-    output_dim_gnn = args.embsize_gnn
-    output_dim_vae = args.embsize_vae
-    epochs = args.epoch
-    lr_vae = args.lr_vae
-    lr_gnn = args.lr_gnn
-    nlayers_gnn = args.layers_gnn
-    clustering = args.clusteringalgo
-    k = args.kclusters
-    use_edge_weights = True
-    cluster_markers_only = args.quick
-    decay = 0.5 ** (2.0 / epochs)
-    concat_features = args.concat_features
-
-    current_time = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
-    train_log_dir = os.path.join(args.outdir, 'logs/' + args.outname + current_time + '/train')
-    summary_writer = tf.summary.create_file_writer(train_log_dir)
-    print("logging to tensorboard")
-    tb_handler = TensorboardLogger(summary_writer, runname=args.outname + current_time)
-    logger.addHandler(tb_handler)
-    #tf.summary.trace_on(graph=True)
-
-    logger.info("******* Running model: VGAE **********")
-    logger.info("***** using edge weights: {} ******".format(use_edge_weights))
-    logger.info("***** concat features: {} *****".format(concat_features))
-    logger.info("***** cluster markers only: {} *****".format(cluster_markers_only))
-    logger.info("***** threshold adj matrix: {} *****".format(args.binarize))
-    logger.info("***** self edges only: {} *****".format(args.noedges))
-    logger.info("***** Using raw kmer+abund features: {}".format(args.rawfeatures))
-    tf.config.experimental_run_functions_eagerly(True)
-
-
-    X, adj, cluster_mask, neg_pair_idx, pos_pair_idx = prepare_data_for_gnn(
-            dataset, use_edge_weights, cluster_markers_only, use_raw=True,
-            binarize=args.binarize, remove_edges=args.noedges)
-    logger.info("***** SCG neg pairs: {}".format(neg_pair_idx.shape))
-    logger.info("***** input features dimension: {}".format(X[cluster_mask].shape))
-    # pre train clustering
-    if not args.skip_preclustering:
-        cluster_labels, stats, _, hq_bins = compute_clusters_and_stats(
-                    X[cluster_mask], node_names[cluster_mask],
-                    dataset, clustering=clustering, k=k, tsne=args.tsne,
-                    amber=(args.labels is not None and "amber" in args.labels),
-                    unresolved=True, cuda=args.cuda, 
-                )
-        logger.info(f">>> Pre train stats: {str(stats)}")
-
-
-    model = VGAE(X.shape, hidden_dim1=hidden_gnn, hidden_dim2=output_dim_gnn, dropout=0.1,
-             l2_reg=1e-5, embeddings=X, freeze_embeddings=True, lr=lr_gnn)
-    X_train = np.arange(len(X))[:,None].astype(np.int64)
-    A_train = tf.sparse.to_dense(adj)
-    labels = dataset.adj_matrix.toarray()
-    pos_weight = (adj.shape[0] * adj.shape[0] - tf.sparse.reduce_sum(adj)) / tf.sparse.reduce_sum(adj)
-
-    norm = adj.shape[0] * adj.shape[0] / ((adj.shape[0] * adj.shape[0] - tf.sparse.reduce_sum(adj)) * 2)
-
-    pbar_epoch = tqdm(range(epochs), disable=args.quiet, position=0)
-    decay = 0.5**(2./10000)
-    scores = []
-    best_hq = 0
-    batch_size = args.batchsize
-    if batch_size == 0:
-        batch_size = adj.shape[0]
-    train_idx = list(range(adj.shape[0]))
-    for e in pbar_epoch:
-        np.random.shuffle(train_idx)
-        n_batches = len(train_idx)//batch_size
-        pbar_vaebatch = tqdm(range(n_batches), disable=(args.quiet or batch_size == len(train_idx) or n_batches < 100), position=1, ascii=' =')
-        loss = 0
-        for b in pbar_vaebatch:
-            batch_idx = train_idx[b*batch_size:(b+1)*batch_size]
-            loss += model.train_step(X_train, A_train, labels, pos_weight, norm, batch_idx)
-        pbar_epoch.set_description(f'{loss:.3f}')
-        model.optimizer.learning_rate = model.optimizer.learning_rate*decay
-        gpu_mem_alloc = tf.config.experimental.get_memory_usage('GPU:0') / 1000000 if args.cuda else 0
-        if (e + 1) % RESULT_EVERY == 0: # and e >= int(epochs/2):
-            _, embs, _, _, _ = model((X_train, A_train), training=False)
-            node_new_features = embs.numpy()
-
-            best_hq, best_embs, best_epoch, scores, cluster_labels = eval_epoch(logger, summary_writer, node_new_features,
-                                                                cluster_mask, e, args, dataset, e, scores,
-                                                                best_hq, best_embs, best_epoch)
-
-            if args.quiet:
-                logger.info(f"--- EPOCH {e:d} ---")
-                logger.info(f"[VGAE {nlayers_gnn}l] L={loss:.3f}  HQ={stats['hq']}  BestHQ={best_hq} Best Epoch={best_epoch} Max GPU MB={gpu_mem_alloc:.1f}")
-                logger.info(str(stats))
-
-
-    _, embs, _, _, _ = model((X_train, A_train), training=False)
-    embs = embs.numpy()
-
-
+from pathlib import Path
+import time
+import os
+import sys
+import math
+import pdb
+import itertools
+from collections import Counter
+import networkx as nx
+import numpy as np
+from tqdm import tqdm
+import datetime
+import operator
+import scipy
+import logging
+# import dgl
+import random
+from sklearn.cluster import KMeans
+#import tensorflow as tf
+
+SEED = 0
+
+def set_seed(seed=0):
+    if "dgl" in sys.modules:
+        import dgl
+        print("setting dgl seed")
+        dgl.random.seed(seed)
+    if "torch" in sys.modules:
+        import torch
+        print("setting torch seed")
+        torch.manual_seed(seed)
+    random.seed(seed)
+    np.random.seed(seed)
+    if "tensorflow" in sys.modules:
+        import tensorflow
+        print("setting tf seed")
+        tensorflow.random.set_seed(seed)
+
+
+
+class Read:
+    def __init__(self, readid, species=None):
+        self.readid = readid
+        self.species = species
+        self.mappings = set()
+
+
+class ReadMapping:
+    def __init__(self, readid, bitflag, contigname, pos, mapq, seq):
+        self.readid = readid
+        self.bitflag = bitflag
+        self.contigname = contigname
+        self.pos = pos
+        self.mapq = mapq
+
+
+def get_cluster_mask(quick, dataset):
+    if quick and dataset.contig_markers is not None:
+        #connected_marker_nodes = filter_disconnected(dataset.adj_matrix, dataset.node_names, dataset.contig_markers)
+        nodes_with_markers = [
+            i
+            for i, n in enumerate(dataset.node_names)
+            if n in dataset.contig_markers and len(dataset.contig_markers[n]) > 0
+        ]
+        print("eval cluster with ", len(nodes_with_markers), "contigds with markers")
+        cluster_mask = [n in nodes_with_markers for n in range(len(dataset.node_names))]
+    else:
+        cluster_mask = [True] * len(dataset.node_names)
+    return cluster_mask
+
+def save_model(args, epoch, th, th_vae):
+    if th_vae is not None:
+        # save encoder and decoder
+        th_vae.encoder.save(os.path.join(args.outdir, args.outname + "_best_encoder"))
+        th_vae.decoder.save(os.path.join(args.outdir, args.outname + "_best_decoder"))
+    if th is not None:
+        th.gnn_model.save(os.path.join(args.outdir, args.outname + "_best_gnn"))
+
+
+def run_clustering(X, node_names, clustering_algo, cuda, k=0, tsne=False):
+    
+    if clustering_algo == "vamb":
+        from graphmb.vamb_clustering import cluster as vamb_cluster
+        starttime = datetime.datetime.now()
+        X = X.astype(np.float32)
+        cluster_to_contig = {
+            i: c for (i, (n, c)) in enumerate(vamb_cluster(X, node_names, cuda=cuda))
+        }
+        clustering_time = datetime.datetime.now()
+        #print("clustering time", clustering_time-starttime)
+        contig_to_bin = {}
+        #for b in cluster_to_contig:
+        #    for contig in cluster_to_contig[b]:
+        #        contig_to_bin[contig] = b
+        for k, v in cluster_to_contig.items():
+            contig_to_bin.update({n: k for n in v})
+        labels = np.array([contig_to_bin[n] for n in node_names])
+        # very slow code:
+        cluster_centroids = None
+        if tsne:
+            cluster_to_embs = {
+                c: np.array([X[i] for i, n in enumerate(node_names) if n in cluster_to_contig[c]])
+                for c in cluster_to_contig
+            }
+            cluster_centroids = np.array([cluster_to_embs[c].mean(0) for c in cluster_to_contig])
+        processing_time = datetime.datetime.now()
+        #print("processing time",  processing_time - clustering_time)
+    elif clustering_algo == "kmeansbatch":
+        kmeans = MiniBatchKMeans(n_clusters=k, random_state=0, batch_size=2048, verbose=0) #, init=seed_matrix)
+        labels = kmeans.fit_predict(X)
+        contig_to_bin = {node_names[i]: labels[i] for i in range(len(node_names))}
+        cluster_to_contig = {i: [] for i in range(k)}
+        for i in range(len(node_names)):
+            cluster_to_contig[labels[i]].append(node_names[i])
+        #cluster_centroids = kmeans.cluster_centers_
+    elif clustering_algo == "kmeansgpu":
+        pass
+    elif clustering_algo == "kmedoids":
+        import kmedoids
+        breakpoint()
+        # TODO do this on gpu if avail
+        D = np.sum((X[:,None]-X[None])**2, axis=-1)
+        # TODO find best k
+        km = kmedoids.KMedoids(20, method='fasterpam')
+        cluster_labels = km.fit_predict(D).astype(np.int64)
+    elif clustering_algo == "kmeans":
+        clf = KMeans(k, random_state=1234)
+        labels = clf.fit_predict(X)
+        contig_to_bin = {node_names[i]: labels[i] for i in range(len(node_names))}
+        cluster_to_contig = {i: [] for i in range(k)}
+        for i in range(len(node_names)):
+            cluster_to_contig[labels[i]].append(node_names[i])
+        cluster_centroids = None
+    return cluster_to_contig, contig_to_bin, labels, cluster_centroids
+
+def filter_disconnected(adj, node_names, markers):
+    # get idx of nodes that are connected or have at least one marker
+    graph = nx.convert_matrix.from_scipy_sparse_matrix(adj, edge_attribute="weight")
+    # breakpoint()
+    nodes_to_remove = set()
+    for n1 in graph.nodes:
+        if len(list(graph.neighbors(n1))) == 0 or (
+            node_names[n1] not in markers or len(markers[node_names[n1]]) == 0
+        ):
+            nodes_to_remove.add(n1)
+
+    graph.remove_nodes_from(list(nodes_to_remove))
+    assert len(graph.nodes()) == (len(node_names)-len(nodes_to_remove))
+    print(f"{len(nodes_to_remove)} nodes without edges nor markers, keeping {len(graph.nodes())} nodes")
+    return set(graph.nodes())
+
+def run_model_vgae(dataset, args, logger, nrun):
+    node_names = np.array(dataset.node_names)
+    RESULT_EVERY = args.evalepochs
+    hidden_gnn = args.hidden_gnn
+    hidden_vae = args.hidden_vae
+    output_dim_gnn = args.embsize_gnn
+    output_dim_vae = args.embsize_vae
+    epochs = args.epoch
+    lr_vae = args.lr_vae
+    lr_gnn = args.lr_gnn
+    nlayers_gnn = args.layers_gnn
+    clustering = args.clusteringalgo
+    k = args.kclusters
+    use_edge_weights = True
+    cluster_markers_only = args.quick
+    decay = 0.5 ** (2.0 / epochs)
+    concat_features = args.concat_features
+
+    current_time = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
+    train_log_dir = os.path.join(args.outdir, 'logs/' + args.outname + current_time + '/train')
+    summary_writer = tf.summary.create_file_writer(train_log_dir)
+    print("logging to tensorboard")
+    tb_handler = TensorboardLogger(summary_writer, runname=args.outname + current_time)
+    logger.addHandler(tb_handler)
+    #tf.summary.trace_on(graph=True)
+
+    logger.info("******* Running model: VGAE **********")
+    logger.info("***** using edge weights: {} ******".format(use_edge_weights))
+    logger.info("***** concat features: {} *****".format(concat_features))
+    logger.info("***** cluster markers only: {} *****".format(cluster_markers_only))
+    logger.info("***** threshold adj matrix: {} *****".format(args.binarize))
+    logger.info("***** self edges only: {} *****".format(args.noedges))
+    logger.info("***** Using raw kmer+abund features: {}".format(args.rawfeatures))
+    tf.config.experimental_run_functions_eagerly(True)
+
+
+    X, adj, cluster_mask, neg_pair_idx, pos_pair_idx = prepare_data_for_gnn(
+            dataset, use_edge_weights, cluster_markers_only, use_raw=True,
+            binarize=args.binarize, remove_edges=args.noedges)
+    logger.info("***** SCG neg pairs: {}".format(neg_pair_idx.shape))
+    logger.info("***** input features dimension: {}".format(X[cluster_mask].shape))
+    # pre train clustering
+    if not args.skip_preclustering:
+        cluster_labels, stats, _, hq_bins = compute_clusters_and_stats(
+                    X[cluster_mask], node_names[cluster_mask],
+                    dataset, clustering=clustering, k=k, tsne=args.tsne,
+                    amber=(args.labels is not None and "amber" in args.labels),
+                    unresolved=True, cuda=args.cuda, 
+                )
+        logger.info(f">>> Pre train stats: {str(stats)}")
+
+
+    model = VGAE(X.shape, hidden_dim1=hidden_gnn, hidden_dim2=output_dim_gnn, dropout=0.1,
+             l2_reg=1e-5, embeddings=X, freeze_embeddings=True, lr=lr_gnn)
+    X_train = np.arange(len(X))[:,None].astype(np.int64)
+    A_train = tf.sparse.to_dense(adj)
+    labels = dataset.adj_matrix.toarray()
+    pos_weight = (adj.shape[0] * adj.shape[0] - tf.sparse.reduce_sum(adj)) / tf.sparse.reduce_sum(adj)
+
+    norm = adj.shape[0] * adj.shape[0] / ((adj.shape[0] * adj.shape[0] - tf.sparse.reduce_sum(adj)) * 2)
+
+    pbar_epoch = tqdm(range(epochs), disable=args.quiet, position=0)
+    decay = 0.5**(2./10000)
+    scores = []
+    best_hq = 0
+    batch_size = args.batchsize
+    if batch_size == 0:
+        batch_size = adj.shape[0]
+    train_idx = list(range(adj.shape[0]))
+    for e in pbar_epoch:
+        np.random.shuffle(train_idx)
+        n_batches = len(train_idx)//batch_size
+        pbar_vaebatch = tqdm(range(n_batches), disable=(args.quiet or batch_size == len(train_idx) or n_batches < 100), position=1, ascii=' =')
+        loss = 0
+        for b in pbar_vaebatch:
+            batch_idx = train_idx[b*batch_size:(b+1)*batch_size]
+            loss += model.train_step(X_train, A_train, labels, pos_weight, norm, batch_idx)
+        pbar_epoch.set_description(f'{loss:.3f}')
+        model.optimizer.learning_rate = model.optimizer.learning_rate*decay
+        gpu_mem_alloc = tf.config.experimental.get_memory_usage('GPU:0') / 1000000 if args.cuda else 0
+        if (e + 1) % RESULT_EVERY == 0: # and e >= int(epochs/2):
+            _, embs, _, _, _ = model((X_train, A_train), training=False)
+            node_new_features = embs.numpy()
+
+            best_hq, best_embs, best_epoch, scores, cluster_labels = eval_epoch(logger, summary_writer, node_new_features,
+                                                                cluster_mask, e, args, dataset, e, scores,
+                                                                best_hq, best_embs, best_epoch)
+
+            if args.quiet:
+                logger.info(f"--- EPOCH {e:d} ---")
+                logger.info(f"[VGAE {nlayers_gnn}l] L={loss:.3f}  HQ={stats['hq']}  BestHQ={best_hq} Best Epoch={best_epoch} Max GPU MB={gpu_mem_alloc:.1f}")
+                logger.info(str(stats))
+
+
+    _, embs, _, _, _ = model((X_train, A_train), training=False)
+    embs = embs.numpy()
+
+
```

### Comparing `graphmb-0.2.4/src/graphmb/vamb_clustering.py` & `graphmb-0.2.5/src/graphmb/vamb_clustering.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,477 +1,477 @@
-__doc__ = """Iterative medoid clustering.
-
-Usage:
->>> clusters = list(ClusterIterator(matrix))
-
-Implements one core function, cluster, along with the helper
-functions write_clusters and read_clusters.
-"""
-
-import random as _random
-import numpy as _np
-import torch as _torch
-from collections import defaultdict as _defaultdict, deque as _deque
-from math import ceil as _ceil
-
-_DEFAULT_RADIUS = 0.06
-# Distance within which to search for medoid point
-_MEDOID_RADIUS = 0.05
-
-_DELTA_X = 0.005
-_XMAX = 0.3
-
-# This is the PDF of normal with µ=0, s=0.01 from -0.075 to 0.075 with intervals
-# of DELTA_X, for a total of 31 values. We multiply by _DELTA_X so the density
-# of one point sums to approximately one
-_NORMALPDF = _DELTA_X * _torch.Tensor(
-      [2.43432053e-11, 9.13472041e-10, 2.66955661e-08, 6.07588285e-07,
-       1.07697600e-05, 1.48671951e-04, 1.59837411e-03, 1.33830226e-02,
-       8.72682695e-02, 4.43184841e-01, 1.75283005e+00, 5.39909665e+00,
-       1.29517596e+01, 2.41970725e+01, 3.52065327e+01, 3.98942280e+01,
-       3.52065327e+01, 2.41970725e+01, 1.29517596e+01, 5.39909665e+00,
-       1.75283005e+00, 4.43184841e-01, 8.72682695e-02, 1.33830226e-02,
-       1.59837411e-03, 1.48671951e-04, 1.07697600e-05, 6.07588285e-07,
-       2.66955661e-08, 9.13472041e-10, 2.43432053e-11])
-
-class Cluster:
-    __slots__ = ['medoid', 'seed', 'members', 'pvr', 'radius', 'isdefault', 'successes', 'attempts']
-
-    def __init__(self, medoid, seed, members, pvr, radius, isdefault, successes, attempts):
-        self.medoid = medoid
-        self.seed = seed
-        self.members = members
-        self.pvr = pvr
-        self.radius = radius
-        self.isdefault = isdefault
-        self.successes = successes
-        self.attempts = attempts
-
-    def __repr__(self):
-        return '<Cluster of medoid {}, {} members>'.format(self.medoid, len(self.members))
-
-    def as_tuple(self, labels=None):
-        if labels is None:
-            return (self.medoid, {i for i in self.members})
-        else:
-            return (labels[self.medoid], {labels[i] for i in self.members})
-
-    def dump(self):
-        return '{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}'.format(self.medoid, self.seed, self.pvr, self.radius,
-        self.isdefault, self.successes, self.attempts, ','.join([str(i) for i in self.members]))
-
-    def __str__(self):
-        radius = "{:.3f}".format(self.radius)
-        if self.isdefault:
-            radius += " (fallback)"
-
-        return """Cluster of medoid {}
-  N members: {}
-  seed:      {}
-  radius:    {}
-  successes: {} / {}
-  pvr:       {:.1f}
-  """.format(self.medoid, len(self.members), self.seed, radius, self.successes, self.attempts, self.pvr)
-
-class ClusterGenerator:
-    """Iterative medoid cluster generator. Iterate this object to get clusters.
-
-    Inputs:
-        matrix: A (obs x features) Numpy matrix of data type numpy.float32
-        maxsteps: Stop searching for optimal medoid after N futile attempts [25]
-        windowsize: Length of window to count successes [200]
-        minsuccesses: Minimum acceptable number of successes [15]
-        destroy: Save memory by destroying matrix while clustering [False]
-        normalized: Matrix is already preprocessed [False]
-        cuda: Accelerate clustering with GPU [False]
-    """
-
-    __slots__ = ['MAXSTEPS', 'MINSUCCESSES', 'CUDA', 'RNG', 'matrix', 'indices',
-                 'seed', 'nclusters', 'peak_valley_ratio', 'attempts', 'successes',
-                 'histogram', 'kept_mask']
-
-    def __repr__(self):
-        return "ClusterGenerator({} points, {} clusters)".format(len(self.matrix), self.nclusters)
-
-    def __str__(self):
-        return """ClusterGenerator({} points, {} clusters)
-  CUDA:         {}
-  MAXSTEPS:     {}
-  MINSUCCESSES: {}
-  pvr:          {}
-  successes:    {}/{}
-""".format(len(self.matrix), self.nclusters, self.CUDA, self.MAXSTEPS, self.MINSUCCESSES,
-    self.peak_valley_ratio, self.successes, len(self.attempts))
-
-    def _check_params(self, matrix, maxsteps, windowsize, minsuccesses):
-        """Checks matrix, and maxsteps."""
-
-        if matrix.dtype != _np.float32:
-            raise(ValueError("Matrix must be of dtype float32"))
-
-        if maxsteps < 1:
-            raise ValueError('maxsteps must be a positive integer, not {}'.format(maxsteps))
-
-        if windowsize < 1:
-            raise ValueError('windowsize must be at least 1, not {}'.format(windowsize))
-
-        if minsuccesses < 1 or minsuccesses > windowsize:
-            raise ValueError('minsuccesses must be between 1 and windowsize, not {}'.format(minsuccesses))
-
-        if len(matrix) < 1:
-            raise ValueError('Matrix must have at least 1 observation.')
-
-    def _init_histogram_kept_mask(self, N):
-        "N is number of contigs"
-        if _torch.__version__ >= '1.2':
-            # https://github.com/pytorch/pytorch/issues/20208 fixed in PyTorch 1.2
-            cuda_hist_dtype = _torch.float
-            # Masking using uint8 tensors deprecated in PyTorch 1.2
-            kept_mask_dtype = _torch.bool
-        else:
-            cuda_hist_dtype = _torch.long
-            kept_mask_dtype = _torch.uint8
-
-        kept_mask = _torch.ones(N, dtype=kept_mask_dtype)
-
-        if self.CUDA:
-            histogram = _torch.empty(_ceil(_XMAX/_DELTA_X), dtype=cuda_hist_dtype).cuda()
-            kept_mask = kept_mask.cuda()
-        else:
-            histogram = _torch.empty(_ceil(_XMAX/_DELTA_X))
-
-        return histogram, kept_mask
-
-    def __init__(self, matrix, maxsteps=25, windowsize=200, minsuccesses=20, destroy=False,
-                normalized=False, cuda=False):
-        self._check_params(matrix, maxsteps, windowsize, minsuccesses)
-        if not destroy:
-            matrix = matrix.copy()
-
-        # Shuffle matrix in unison to prevent seed sampling bias. Indices keeps
-        # track of which points are which.
-        _np.random.RandomState(0).shuffle(matrix)
-        indices = _np.random.RandomState(0).permutation(len(matrix))
-        indices = _torch.from_numpy(indices)
-        matrix = _torch.from_numpy(matrix)
-
-        if not normalized:
-            _normalize(matrix, inplace=True)
-
-        # Move to GPU
-        if cuda:
-            matrix = matrix.cuda()
-
-        self.MAXSTEPS = maxsteps
-        self.MINSUCCESSES = minsuccesses
-        self.CUDA = cuda
-        self.RNG = _random.Random(0)
-
-        self.matrix = matrix
-        # This refers to the indices of the original matrix. As we remove points, these
-        # indices do not correspond to merely range(len(matrix)) anymore.
-        self.indices = indices
-        self.seed = -1
-        self.nclusters = 0
-        self.peak_valley_ratio = 0.1
-        self.attempts = _deque(maxlen=windowsize)
-        self.successes = 0
-
-        histogram, kept_mask = self._init_histogram_kept_mask(len(indices))
-        self.histogram = histogram
-        self.kept_mask = kept_mask
-
-    # It's an iterator itself
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        # Stop criterion. For CUDA, inplace masking the array is too slow, so the matrix is
-        # unchanged. On CPU, we continually modify the matrix by removing rows.
-        if self.CUDA:
-            if not _torch.any(self.kept_mask).item():
-                raise StopIteration
-        elif len(self.matrix) == 0:
-            raise StopIteration
-
-        cluster, medoid, points = self._findcluster()
-        self.nclusters += 1
-
-        for point in points:
-            self.kept_mask[point] = 0
-
-        # Remove all points that's been clustered away. Is slow it itself, but speeds up
-        # distance calculation by having fewer points. Worth it on CPU, not on GPU
-        if not self.CUDA:
-            self.matrix = self.matrix[self.kept_mask]
-            #_vambtools.torch_inplace_maskarray(self.matrix, self.kept_mask)
-            self.indices = self.indices[self.kept_mask] # no need to inplace mask small array
-            self.kept_mask.resize_(len(self.matrix))
-            self.kept_mask[:] = 1
-
-        return cluster
-
-    def _findcluster(self):
-        """Finds a cluster to output."""
-        threshold = None
-
-        # Keep looping until we find a cluster
-        while threshold is None:
-            # If on GPU, we need to take next seed which has not already been clusted out.
-            # if not, clustered points have been removed, so we can just take next seed
-            if self.CUDA:
-                self.seed = (self.seed + 1) % len(self.matrix)
-                while self.kept_mask[self.seed] == False:
-                    self.seed = (self.seed + 1) % len(self.matrix)
-            else:
-                self.seed = (self.seed + 1) % len(self.matrix)
-
-            medoid, distances = _wander_medoid(self.matrix, self.kept_mask, self.seed, self.MAXSTEPS, self.RNG, self.CUDA)
-
-            # We need to make a histogram of only the unclustered distances - when run on GPU
-            # these have not been removed and we must use the kept_mask
-            if self.CUDA:
-                _torch.histc(distances[self.kept_mask], len(self.histogram), 0, _XMAX, out=self.histogram)
-            else:
-                _torch.histc(distances, len(self.histogram), 0, _XMAX, out=self.histogram)
-            self.histogram[0] -= 1 # Remove distance to self
-
-            threshold, success = _find_threshold(self.histogram, self.peak_valley_ratio, self.CUDA)
-
-            # If success is not None, either threshold detection failed or succeded.
-            if success is not None:
-                # Keep accurately track of successes if we exceed maxlen
-                if len(self.attempts) == self.attempts.maxlen:
-                    self.successes -= self.attempts.popleft()
-
-                # Add the current success to count
-                self.successes += success
-                self.attempts.append(success)
-
-                # If less than minsuccesses of the last maxlen attempts were successful,
-                # we relax the clustering criteria and reset counting successes.
-                if len(self.attempts) == self.attempts.maxlen and self.successes < self.MINSUCCESSES:
-                    self.peak_valley_ratio += 0.1
-                    self.attempts.clear()
-                    self.successes = 0
-
-        # These are the points of the final cluster AFTER establishing the threshold used
-        points = _smaller_indices(distances, self.kept_mask, threshold, self.CUDA)
-        isdefault = success is None and threshold == _DEFAULT_RADIUS and self.peak_valley_ratio > 0.55
-
-        cluster = Cluster(self.indices[medoid].item(), self.seed, self.indices[points].numpy(),
-                        self.peak_valley_ratio,
-                          threshold, isdefault, self.successes, len(self.attempts))
-        return cluster, medoid, points
-
-def _calc_densities(histogram, cuda, pdf=_NORMALPDF):
-    """Given an array of histogram, smoothes the histogram."""
-    pdf_len = len(pdf)
-
-    if cuda:
-        histogram = histogram.cpu()
-
-    densities = _torch.zeros(len(histogram) + pdf_len - 1)
-    for i in range(len(densities) - pdf_len + 1):
-        densities[i:i+pdf_len] += pdf * histogram[i]
-
-    densities = densities[15:-15]
-
-    return densities
-
-def _find_threshold(histogram, peak_valley_ratio, cuda):
-    """Find a threshold distance, where where is a dip in point density
-    that separates an initial peak in densities from the larger bulk around 0.5.
-    Returns (threshold, success), where succes is False if no threshold could
-    be found, True if a good threshold could be found, and None if the point is
-    alone, or the threshold has been used.
-    """
-    peak_density = 0
-    peak_over = False
-    minimum_x = None
-    density_at_minimum = None
-    threshold = None
-    success = False
-    delta_x = _XMAX / len(histogram)
-
-    # If the point is a loner, immediately return a threshold in where only
-    # that point is contained.
-    if histogram[:10].sum().item() == 0:
-        return 0.025, None
-
-    densities = _calc_densities(histogram, cuda)
-
-    # Else we analyze the point densities to find the valley
-    x = 0
-    for density in densities:
-        # Define the first "peak" in point density. That's simply the max until
-        # the peak is defined as being over.
-        if not peak_over and density > peak_density:
-            # Do not accept first peak to be after x = 0.1
-            if x > 0.1:
-                break
-            peak_density = density
-
-        # Peak is over when density drops below 60% of peak density
-        if not peak_over and density < 0.6 * peak_density:
-            peak_over = True
-            density_at_minimum = density
-
-        # If another peak is detected, we stop
-        if peak_over and density > 1.5 * density_at_minimum:
-            break
-
-        # Now find the minimum after the peak
-        if peak_over and density < density_at_minimum:
-            minimum_x, density_at_minimum = x, density
-
-            # If this minimum is below ratio * peak, it's accepted as threshold
-            if density < peak_valley_ratio * peak_density:
-                threshold = minimum_x
-                success = True
-
-        x += delta_x
-
-    # Don't allow a threshold too high - this is relaxed with p_v_ratio
-    if threshold is not None and threshold > 0.2 + peak_valley_ratio:
-        threshold = None
-        success = False
-
-    # If ratio has been set to 0.6, we do not accept returning no threshold.
-    if threshold is None and peak_valley_ratio > 0.55:
-        threshold = _DEFAULT_RADIUS
-        success = None
-
-    return threshold, success
-
-def _smaller_indices(tensor, kept_mask, threshold, cuda):
-    """Get all indices where the tensor is smaller than the threshold.
-    Uses Numpy because Torch is slow - See https://github.com/pytorch/pytorch/pull/15190"""
-
-    # If it's on GPU, we remove the already clustered points at this step.
-    if cuda:
-        return _torch.nonzero((tensor <= threshold) & kept_mask).flatten().cpu()
-    else:
-        arr = tensor.numpy()
-        indices = (arr <= threshold).nonzero()[0]
-        torch_indices = _torch.from_numpy(indices)
-        return torch_indices
-
-def _normalize(matrix, inplace=False):
-    """Preprocess the matrix to make distance calculations faster.
-    The distance functions in this module assumes input has been normalized
-    and will not work otherwise.
-    """
-    if isinstance(matrix, _np.ndarray):
-        matrix = _torch.from_numpy(matrix)
-
-    if not inplace:
-        matrix = matrix.clone()
-
-    # If any rows are kept all zeros, the distance function will return 0.5 to all points
-    # inclusive itself, which can break the code in this module
-    zeromask = matrix.sum(dim=1) == 0
-    matrix[zeromask] = 1/matrix.shape[1]
-    matrix /= (matrix.norm(dim=1).reshape(-1, 1) * (2 ** 0.5))
-    return matrix
-
-
-def _calc_distances(matrix, index):
-    "Return vector of cosine distances from rows of normalized matrix to given row."
-    dists = 0.5 - matrix.matmul(matrix[index])
-    dists[index] = 0.0 # avoid float rounding errors
-    return dists
-
-def _sample_medoid(matrix, kept_mask, medoid, threshold, cuda):
-    """Returns:
-    - A vector of indices to points within threshold
-    - A vector of distances to all points
-    - The mean distance from medoid to the other points in the first vector
-    """
-
-    distances = _calc_distances(matrix, medoid)
-    cluster = _smaller_indices(distances, kept_mask, threshold, cuda)
-
-    if len(cluster) == 1:
-        average_distance = 0.0
-    else:
-        average_distance = distances[cluster].sum().item() / (len(cluster) - 1)
-
-    return cluster, distances, average_distance
-
-
-def _wander_medoid(matrix, kept_mask, medoid, max_attempts, rng, cuda):
-    """Keeps sampling new points within the cluster until it has sampled
-    max_attempts without getting a new set of cluster with lower average
-    distance"""
-
-    futile_attempts = 0
-    tried = {medoid} # keep track of already-tried medoids
-    cluster, distances, average_distance = _sample_medoid(matrix, kept_mask, medoid, _MEDOID_RADIUS, cuda)
-
-    while len(cluster) - len(tried) > 0 and futile_attempts < max_attempts:
-        sampled_medoid = rng.choice(cluster).item()
-
-         # Prevent sampling same medoid multiple times.
-        while sampled_medoid in tried:
-            sampled_medoid = rng.choice(cluster).item()
-
-        tried.add(sampled_medoid)
-
-        sampling = _sample_medoid(matrix, kept_mask, sampled_medoid, _MEDOID_RADIUS, cuda)
-        sample_cluster, sample_distances, sample_avg = sampling
-
-        # If the mean distance of inner points of the sample is lower,
-        # we move the medoid and reset the futile_attempts count
-        if sample_avg < average_distance:
-            medoid = sampled_medoid
-            cluster = sample_cluster
-            average_distance = sample_avg
-            futile_attempts = 0
-            tried = {medoid}
-            distances = sample_distances
-
-        else:
-            futile_attempts += 1
-
-    return medoid, distances
-
-def cluster(matrix, labels=None, maxsteps=25, windowsize=200, minsuccesses=20, destroy=False,
-            normalized=False, cuda=False):
-    """Create iterable of (medoid, {point1, point2 ...}) tuples for each cluster.
-
-    Inputs:
-        matrix: A (obs x features) Numpy matrix of data type numpy.float32
-        labels: None or list of labels of points [None = range(len(matrix))]
-        maxsteps: Stop searching for optimal medoid after N futile attempts [25]
-        windowsize: Length of window to count successes [200]
-        minsuccesses: Minimum acceptable number of successes [15]
-        destroy: Save memory by destroying matrix while clustering [False]
-        normalized: Matrix is already preprocessed [False]
-        cuda: Accelerate clustering with GPU [False]
-
-    Output: Generator of (medoid, {point1, point2 ...}) tuples for each cluster.
-    """
-    if labels is not None and len(matrix) != len(labels):
-        raise ValueError("Got {} labels for {} points".format(len(labels), len(matrix)))
-
-    it = ClusterGenerator(matrix, maxsteps, windowsize, minsuccesses, destroy, normalized, cuda)
-    for cluster in it:
-        yield cluster.as_tuple(labels)
-
-def pairs(clustergenerator, labels):
-    """Create an iterable of (N, {label1, label2 ...}) for each
-    cluster in a ClusterGenerator, where N is "1", "2", "3", etc.
-    Useful to pass to e.g. vambtools.writer_clusters.
-
-    Inputs:
-        clustergenerator: A ClusterGenerator object
-        labels: List or array of cluster labels
-    Output:
-        Generator yielding ("1", {label1, label2 ... }) for each cluster
-    """
-    maxindex = clustergenerator.indices.max()
-    if len(labels) < maxindex:
-        raise ValueError("Cluster generator contains point no {}, "
-                         "but was given only {} labels".format(maxindex, len(labels)))
-
+__doc__ = """Iterative medoid clustering.
+
+Usage:
+>>> clusters = list(ClusterIterator(matrix))
+
+Implements one core function, cluster, along with the helper
+functions write_clusters and read_clusters.
+"""
+
+import random as _random
+import numpy as _np
+import torch as _torch
+from collections import defaultdict as _defaultdict, deque as _deque
+from math import ceil as _ceil
+
+_DEFAULT_RADIUS = 0.06
+# Distance within which to search for medoid point
+_MEDOID_RADIUS = 0.05
+
+_DELTA_X = 0.005
+_XMAX = 0.3
+
+# This is the PDF of normal with µ=0, s=0.01 from -0.075 to 0.075 with intervals
+# of DELTA_X, for a total of 31 values. We multiply by _DELTA_X so the density
+# of one point sums to approximately one
+_NORMALPDF = _DELTA_X * _torch.Tensor(
+      [2.43432053e-11, 9.13472041e-10, 2.66955661e-08, 6.07588285e-07,
+       1.07697600e-05, 1.48671951e-04, 1.59837411e-03, 1.33830226e-02,
+       8.72682695e-02, 4.43184841e-01, 1.75283005e+00, 5.39909665e+00,
+       1.29517596e+01, 2.41970725e+01, 3.52065327e+01, 3.98942280e+01,
+       3.52065327e+01, 2.41970725e+01, 1.29517596e+01, 5.39909665e+00,
+       1.75283005e+00, 4.43184841e-01, 8.72682695e-02, 1.33830226e-02,
+       1.59837411e-03, 1.48671951e-04, 1.07697600e-05, 6.07588285e-07,
+       2.66955661e-08, 9.13472041e-10, 2.43432053e-11])
+
+class Cluster:
+    __slots__ = ['medoid', 'seed', 'members', 'pvr', 'radius', 'isdefault', 'successes', 'attempts']
+
+    def __init__(self, medoid, seed, members, pvr, radius, isdefault, successes, attempts):
+        self.medoid = medoid
+        self.seed = seed
+        self.members = members
+        self.pvr = pvr
+        self.radius = radius
+        self.isdefault = isdefault
+        self.successes = successes
+        self.attempts = attempts
+
+    def __repr__(self):
+        return '<Cluster of medoid {}, {} members>'.format(self.medoid, len(self.members))
+
+    def as_tuple(self, labels=None):
+        if labels is None:
+            return (self.medoid, {i for i in self.members})
+        else:
+            return (labels[self.medoid], {labels[i] for i in self.members})
+
+    def dump(self):
+        return '{}\t{}\t{}\t{}\t{}\t{}\t{}\t{}'.format(self.medoid, self.seed, self.pvr, self.radius,
+        self.isdefault, self.successes, self.attempts, ','.join([str(i) for i in self.members]))
+
+    def __str__(self):
+        radius = "{:.3f}".format(self.radius)
+        if self.isdefault:
+            radius += " (fallback)"
+
+        return """Cluster of medoid {}
+  N members: {}
+  seed:      {}
+  radius:    {}
+  successes: {} / {}
+  pvr:       {:.1f}
+  """.format(self.medoid, len(self.members), self.seed, radius, self.successes, self.attempts, self.pvr)
+
+class ClusterGenerator:
+    """Iterative medoid cluster generator. Iterate this object to get clusters.
+
+    Inputs:
+        matrix: A (obs x features) Numpy matrix of data type numpy.float32
+        maxsteps: Stop searching for optimal medoid after N futile attempts [25]
+        windowsize: Length of window to count successes [200]
+        minsuccesses: Minimum acceptable number of successes [15]
+        destroy: Save memory by destroying matrix while clustering [False]
+        normalized: Matrix is already preprocessed [False]
+        cuda: Accelerate clustering with GPU [False]
+    """
+
+    __slots__ = ['MAXSTEPS', 'MINSUCCESSES', 'CUDA', 'RNG', 'matrix', 'indices',
+                 'seed', 'nclusters', 'peak_valley_ratio', 'attempts', 'successes',
+                 'histogram', 'kept_mask']
+
+    def __repr__(self):
+        return "ClusterGenerator({} points, {} clusters)".format(len(self.matrix), self.nclusters)
+
+    def __str__(self):
+        return """ClusterGenerator({} points, {} clusters)
+  CUDA:         {}
+  MAXSTEPS:     {}
+  MINSUCCESSES: {}
+  pvr:          {}
+  successes:    {}/{}
+""".format(len(self.matrix), self.nclusters, self.CUDA, self.MAXSTEPS, self.MINSUCCESSES,
+    self.peak_valley_ratio, self.successes, len(self.attempts))
+
+    def _check_params(self, matrix, maxsteps, windowsize, minsuccesses):
+        """Checks matrix, and maxsteps."""
+
+        if matrix.dtype != _np.float32:
+            raise(ValueError("Matrix must be of dtype float32"))
+
+        if maxsteps < 1:
+            raise ValueError('maxsteps must be a positive integer, not {}'.format(maxsteps))
+
+        if windowsize < 1:
+            raise ValueError('windowsize must be at least 1, not {}'.format(windowsize))
+
+        if minsuccesses < 1 or minsuccesses > windowsize:
+            raise ValueError('minsuccesses must be between 1 and windowsize, not {}'.format(minsuccesses))
+
+        if len(matrix) < 1:
+            raise ValueError('Matrix must have at least 1 observation.')
+
+    def _init_histogram_kept_mask(self, N):
+        "N is number of contigs"
+        if _torch.__version__ >= '1.2':
+            # https://github.com/pytorch/pytorch/issues/20208 fixed in PyTorch 1.2
+            cuda_hist_dtype = _torch.float
+            # Masking using uint8 tensors deprecated in PyTorch 1.2
+            kept_mask_dtype = _torch.bool
+        else:
+            cuda_hist_dtype = _torch.long
+            kept_mask_dtype = _torch.uint8
+
+        kept_mask = _torch.ones(N, dtype=kept_mask_dtype)
+
+        if self.CUDA:
+            histogram = _torch.empty(_ceil(_XMAX/_DELTA_X), dtype=cuda_hist_dtype).cuda()
+            kept_mask = kept_mask.cuda()
+        else:
+            histogram = _torch.empty(_ceil(_XMAX/_DELTA_X))
+
+        return histogram, kept_mask
+
+    def __init__(self, matrix, maxsteps=25, windowsize=200, minsuccesses=20, destroy=False,
+                normalized=False, cuda=False):
+        self._check_params(matrix, maxsteps, windowsize, minsuccesses)
+        if not destroy:
+            matrix = matrix.copy()
+
+        # Shuffle matrix in unison to prevent seed sampling bias. Indices keeps
+        # track of which points are which.
+        _np.random.RandomState(0).shuffle(matrix)
+        indices = _np.random.RandomState(0).permutation(len(matrix))
+        indices = _torch.from_numpy(indices)
+        matrix = _torch.from_numpy(matrix)
+
+        if not normalized:
+            _normalize(matrix, inplace=True)
+
+        # Move to GPU
+        if cuda:
+            matrix = matrix.cuda()
+
+        self.MAXSTEPS = maxsteps
+        self.MINSUCCESSES = minsuccesses
+        self.CUDA = cuda
+        self.RNG = _random.Random(0)
+
+        self.matrix = matrix
+        # This refers to the indices of the original matrix. As we remove points, these
+        # indices do not correspond to merely range(len(matrix)) anymore.
+        self.indices = indices
+        self.seed = -1
+        self.nclusters = 0
+        self.peak_valley_ratio = 0.1
+        self.attempts = _deque(maxlen=windowsize)
+        self.successes = 0
+
+        histogram, kept_mask = self._init_histogram_kept_mask(len(indices))
+        self.histogram = histogram
+        self.kept_mask = kept_mask
+
+    # It's an iterator itself
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        # Stop criterion. For CUDA, inplace masking the array is too slow, so the matrix is
+        # unchanged. On CPU, we continually modify the matrix by removing rows.
+        if self.CUDA:
+            if not _torch.any(self.kept_mask).item():
+                raise StopIteration
+        elif len(self.matrix) == 0:
+            raise StopIteration
+
+        cluster, medoid, points = self._findcluster()
+        self.nclusters += 1
+
+        for point in points:
+            self.kept_mask[point] = 0
+
+        # Remove all points that's been clustered away. Is slow it itself, but speeds up
+        # distance calculation by having fewer points. Worth it on CPU, not on GPU
+        if not self.CUDA:
+            self.matrix = self.matrix[self.kept_mask]
+            #_vambtools.torch_inplace_maskarray(self.matrix, self.kept_mask)
+            self.indices = self.indices[self.kept_mask] # no need to inplace mask small array
+            self.kept_mask.resize_(len(self.matrix))
+            self.kept_mask[:] = 1
+
+        return cluster
+
+    def _findcluster(self):
+        """Finds a cluster to output."""
+        threshold = None
+
+        # Keep looping until we find a cluster
+        while threshold is None:
+            # If on GPU, we need to take next seed which has not already been clusted out.
+            # if not, clustered points have been removed, so we can just take next seed
+            if self.CUDA:
+                self.seed = (self.seed + 1) % len(self.matrix)
+                while self.kept_mask[self.seed] == False:
+                    self.seed = (self.seed + 1) % len(self.matrix)
+            else:
+                self.seed = (self.seed + 1) % len(self.matrix)
+
+            medoid, distances = _wander_medoid(self.matrix, self.kept_mask, self.seed, self.MAXSTEPS, self.RNG, self.CUDA)
+
+            # We need to make a histogram of only the unclustered distances - when run on GPU
+            # these have not been removed and we must use the kept_mask
+            if self.CUDA:
+                _torch.histc(distances[self.kept_mask], len(self.histogram), 0, _XMAX, out=self.histogram)
+            else:
+                _torch.histc(distances, len(self.histogram), 0, _XMAX, out=self.histogram)
+            self.histogram[0] -= 1 # Remove distance to self
+
+            threshold, success = _find_threshold(self.histogram, self.peak_valley_ratio, self.CUDA)
+
+            # If success is not None, either threshold detection failed or succeded.
+            if success is not None:
+                # Keep accurately track of successes if we exceed maxlen
+                if len(self.attempts) == self.attempts.maxlen:
+                    self.successes -= self.attempts.popleft()
+
+                # Add the current success to count
+                self.successes += success
+                self.attempts.append(success)
+
+                # If less than minsuccesses of the last maxlen attempts were successful,
+                # we relax the clustering criteria and reset counting successes.
+                if len(self.attempts) == self.attempts.maxlen and self.successes < self.MINSUCCESSES:
+                    self.peak_valley_ratio += 0.1
+                    self.attempts.clear()
+                    self.successes = 0
+
+        # These are the points of the final cluster AFTER establishing the threshold used
+        points = _smaller_indices(distances, self.kept_mask, threshold, self.CUDA)
+        isdefault = success is None and threshold == _DEFAULT_RADIUS and self.peak_valley_ratio > 0.55
+
+        cluster = Cluster(self.indices[medoid].item(), self.seed, self.indices[points].numpy(),
+                        self.peak_valley_ratio,
+                          threshold, isdefault, self.successes, len(self.attempts))
+        return cluster, medoid, points
+
+def _calc_densities(histogram, cuda, pdf=_NORMALPDF):
+    """Given an array of histogram, smoothes the histogram."""
+    pdf_len = len(pdf)
+
+    if cuda:
+        histogram = histogram.cpu()
+
+    densities = _torch.zeros(len(histogram) + pdf_len - 1)
+    for i in range(len(densities) - pdf_len + 1):
+        densities[i:i+pdf_len] += pdf * histogram[i]
+
+    densities = densities[15:-15]
+
+    return densities
+
+def _find_threshold(histogram, peak_valley_ratio, cuda):
+    """Find a threshold distance, where where is a dip in point density
+    that separates an initial peak in densities from the larger bulk around 0.5.
+    Returns (threshold, success), where succes is False if no threshold could
+    be found, True if a good threshold could be found, and None if the point is
+    alone, or the threshold has been used.
+    """
+    peak_density = 0
+    peak_over = False
+    minimum_x = None
+    density_at_minimum = None
+    threshold = None
+    success = False
+    delta_x = _XMAX / len(histogram)
+
+    # If the point is a loner, immediately return a threshold in where only
+    # that point is contained.
+    if histogram[:10].sum().item() == 0:
+        return 0.025, None
+
+    densities = _calc_densities(histogram, cuda)
+
+    # Else we analyze the point densities to find the valley
+    x = 0
+    for density in densities:
+        # Define the first "peak" in point density. That's simply the max until
+        # the peak is defined as being over.
+        if not peak_over and density > peak_density:
+            # Do not accept first peak to be after x = 0.1
+            if x > 0.1:
+                break
+            peak_density = density
+
+        # Peak is over when density drops below 60% of peak density
+        if not peak_over and density < 0.6 * peak_density:
+            peak_over = True
+            density_at_minimum = density
+
+        # If another peak is detected, we stop
+        if peak_over and density > 1.5 * density_at_minimum:
+            break
+
+        # Now find the minimum after the peak
+        if peak_over and density < density_at_minimum:
+            minimum_x, density_at_minimum = x, density
+
+            # If this minimum is below ratio * peak, it's accepted as threshold
+            if density < peak_valley_ratio * peak_density:
+                threshold = minimum_x
+                success = True
+
+        x += delta_x
+
+    # Don't allow a threshold too high - this is relaxed with p_v_ratio
+    if threshold is not None and threshold > 0.2 + peak_valley_ratio:
+        threshold = None
+        success = False
+
+    # If ratio has been set to 0.6, we do not accept returning no threshold.
+    if threshold is None and peak_valley_ratio > 0.55:
+        threshold = _DEFAULT_RADIUS
+        success = None
+
+    return threshold, success
+
+def _smaller_indices(tensor, kept_mask, threshold, cuda):
+    """Get all indices where the tensor is smaller than the threshold.
+    Uses Numpy because Torch is slow - See https://github.com/pytorch/pytorch/pull/15190"""
+
+    # If it's on GPU, we remove the already clustered points at this step.
+    if cuda:
+        return _torch.nonzero((tensor <= threshold) & kept_mask).flatten().cpu()
+    else:
+        arr = tensor.numpy()
+        indices = (arr <= threshold).nonzero()[0]
+        torch_indices = _torch.from_numpy(indices)
+        return torch_indices
+
+def _normalize(matrix, inplace=False):
+    """Preprocess the matrix to make distance calculations faster.
+    The distance functions in this module assumes input has been normalized
+    and will not work otherwise.
+    """
+    if isinstance(matrix, _np.ndarray):
+        matrix = _torch.from_numpy(matrix)
+
+    if not inplace:
+        matrix = matrix.clone()
+
+    # If any rows are kept all zeros, the distance function will return 0.5 to all points
+    # inclusive itself, which can break the code in this module
+    zeromask = matrix.sum(dim=1) == 0
+    matrix[zeromask] = 1/matrix.shape[1]
+    matrix /= (matrix.norm(dim=1).reshape(-1, 1) * (2 ** 0.5))
+    return matrix
+
+
+def _calc_distances(matrix, index):
+    "Return vector of cosine distances from rows of normalized matrix to given row."
+    dists = 0.5 - matrix.matmul(matrix[index])
+    dists[index] = 0.0 # avoid float rounding errors
+    return dists
+
+def _sample_medoid(matrix, kept_mask, medoid, threshold, cuda):
+    """Returns:
+    - A vector of indices to points within threshold
+    - A vector of distances to all points
+    - The mean distance from medoid to the other points in the first vector
+    """
+
+    distances = _calc_distances(matrix, medoid)
+    cluster = _smaller_indices(distances, kept_mask, threshold, cuda)
+
+    if len(cluster) == 1:
+        average_distance = 0.0
+    else:
+        average_distance = distances[cluster].sum().item() / (len(cluster) - 1)
+
+    return cluster, distances, average_distance
+
+
+def _wander_medoid(matrix, kept_mask, medoid, max_attempts, rng, cuda):
+    """Keeps sampling new points within the cluster until it has sampled
+    max_attempts without getting a new set of cluster with lower average
+    distance"""
+
+    futile_attempts = 0
+    tried = {medoid} # keep track of already-tried medoids
+    cluster, distances, average_distance = _sample_medoid(matrix, kept_mask, medoid, _MEDOID_RADIUS, cuda)
+
+    while len(cluster) - len(tried) > 0 and futile_attempts < max_attempts:
+        sampled_medoid = rng.choice(cluster).item()
+
+         # Prevent sampling same medoid multiple times.
+        while sampled_medoid in tried:
+            sampled_medoid = rng.choice(cluster).item()
+
+        tried.add(sampled_medoid)
+
+        sampling = _sample_medoid(matrix, kept_mask, sampled_medoid, _MEDOID_RADIUS, cuda)
+        sample_cluster, sample_distances, sample_avg = sampling
+
+        # If the mean distance of inner points of the sample is lower,
+        # we move the medoid and reset the futile_attempts count
+        if sample_avg < average_distance:
+            medoid = sampled_medoid
+            cluster = sample_cluster
+            average_distance = sample_avg
+            futile_attempts = 0
+            tried = {medoid}
+            distances = sample_distances
+
+        else:
+            futile_attempts += 1
+
+    return medoid, distances
+
+def cluster(matrix, labels=None, maxsteps=25, windowsize=200, minsuccesses=20, destroy=False,
+            normalized=False, cuda=False):
+    """Create iterable of (medoid, {point1, point2 ...}) tuples for each cluster.
+
+    Inputs:
+        matrix: A (obs x features) Numpy matrix of data type numpy.float32
+        labels: None or list of labels of points [None = range(len(matrix))]
+        maxsteps: Stop searching for optimal medoid after N futile attempts [25]
+        windowsize: Length of window to count successes [200]
+        minsuccesses: Minimum acceptable number of successes [15]
+        destroy: Save memory by destroying matrix while clustering [False]
+        normalized: Matrix is already preprocessed [False]
+        cuda: Accelerate clustering with GPU [False]
+
+    Output: Generator of (medoid, {point1, point2 ...}) tuples for each cluster.
+    """
+    if labels is not None and len(matrix) != len(labels):
+        raise ValueError("Got {} labels for {} points".format(len(labels), len(matrix)))
+
+    it = ClusterGenerator(matrix, maxsteps, windowsize, minsuccesses, destroy, normalized, cuda)
+    for cluster in it:
+        yield cluster.as_tuple(labels)
+
+def pairs(clustergenerator, labels):
+    """Create an iterable of (N, {label1, label2 ...}) for each
+    cluster in a ClusterGenerator, where N is "1", "2", "3", etc.
+    Useful to pass to e.g. vambtools.writer_clusters.
+
+    Inputs:
+        clustergenerator: A ClusterGenerator object
+        labels: List or array of cluster labels
+    Output:
+        Generator yielding ("1", {label1, label2 ... }) for each cluster
+    """
+    maxindex = clustergenerator.indices.max()
+    if len(labels) < maxindex:
+        raise ValueError("Cluster generator contains point no {}, "
+                         "but was given only {} labels".format(maxindex, len(labels)))
+
     return ((str(i+1), c.as_tuple(labels)[1]) for (i, c) in enumerate(clustergenerator))
```

### Comparing `graphmb-0.2.4/src/graphmb.egg-info/SOURCES.txt` & `graphmb-0.2.5/src/graphmb.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,8 +22,10 @@
 src/graphmb/version.py
 src/graphmb/visualize.py
 src/graphmb.egg-info/PKG-INFO
 src/graphmb.egg-info/SOURCES.txt
 src/graphmb.egg-info/dependency_links.txt
 src/graphmb.egg-info/entry_points.txt
 src/graphmb.egg-info/requires.txt
-src/graphmb.egg-info/top_level.txt
+src/graphmb.egg-info/top_level.txt
+src/graphmb/data/Bacteria.ms
+src/graphmb/data/kernel.npz
```

