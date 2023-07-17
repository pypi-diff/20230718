# Comparing `tmp/hsmm_mvpy-0.1.0b7.tar.gz` & `tmp/hsmm_mvpy-0.1.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsmm_mvpy-0.1.0b7.tar", last modified: Mon Jun 19 17:13:47 2023, max compression
+gzip compressed data, was "hsmm_mvpy-0.1.0b8.tar", last modified: Mon Jul 17 22:22:34 2023, max compression
```

## Comparing `hsmm_mvpy-0.1.0b7.tar` & `hsmm_mvpy-0.1.0b8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 17:13:47.768928 hsmm_mvpy-0.1.0b7/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b7/LICENSE.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 17:13:47.768928 hsmm_mvpy-0.1.0b7/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22740 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b7/README.md
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      830 2023-06-19 17:09:10.000000 hsmm_mvpy-0.1.0b7/pyproject.toml
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-06-19 17:13:47.768928 hsmm_mvpy-0.1.0b7/setup.cfg
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 17:13:47.768928 hsmm_mvpy-0.1.0b7/src/
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 17:13:47.768928 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      194 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/__init__.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    57320 2023-06-19 17:06:18.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/models.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     5735 2023-06-19 15:40:39.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/resample.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    11082 2023-06-19 17:02:09.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/simulations.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    41436 2023-06-19 16:49:13.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/utils.py
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22869 2023-06-19 16:59:30.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/visu.py
-drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-06-19 17:13:47.768928 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    25106 2023-06-19 17:13:47.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/PKG-INFO
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      369 2023-06-19 17:13:47.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/SOURCES.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-06-19 17:13:47.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/dependency_links.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       71 2023-06-19 17:13:47.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/requires.txt
--rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-06-19 17:13:47.000000 hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/top_level.txt
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-07-17 22:22:34.121746 hsmm_mvpy-0.1.0b8/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     1558 2022-08-29 11:38:13.000000 hsmm_mvpy-0.1.0b8/LICENSE.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    24957 2023-07-17 22:22:34.121746 hsmm_mvpy-0.1.0b8/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    22591 2023-07-17 22:09:09.000000 hsmm_mvpy-0.1.0b8/README.md
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      848 2023-07-17 22:21:32.000000 hsmm_mvpy-0.1.0b8/pyproject.toml
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       38 2023-07-17 22:22:34.121746 hsmm_mvpy-0.1.0b8/setup.cfg
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-07-17 22:22:34.121746 hsmm_mvpy-0.1.0b8/src/
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-07-17 22:22:34.121746 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      229 2023-07-12 12:31:26.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/__init__.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     7130 2023-07-17 21:14:25.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/clusters.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    60568 2023-07-17 21:23:44.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/models.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)     6659 2023-07-17 21:55:30.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/resample.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    14197 2023-07-17 21:23:49.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/simulations.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    41218 2023-07-17 20:48:35.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/utils.py
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    26816 2023-07-16 16:24:07.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/visu.py
+drwxrwxr-x   0 gweindel  (1000) gweindel  (1000)        0 2023-07-17 22:22:34.121746 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)    24957 2023-07-17 22:22:34.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/PKG-INFO
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)      395 2023-07-17 22:22:34.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)        1 2023-07-17 22:22:34.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       86 2023-07-17 22:22:34.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/requires.txt
+-rw-rw-r--   0 gweindel  (1000) gweindel  (1000)       10 2023-07-17 22:22:34.000000 hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/top_level.txt
```

### Comparing `hsmm_mvpy-0.1.0b7/LICENSE.md` & `hsmm_mvpy-0.1.0b8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hsmm_mvpy-0.1.0b7/PKG-INFO` & `hsmm_mvpy-0.1.0b8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm_mvpy
-Version: 0.1.0b7
+Version: 0.1.0b8
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
         
@@ -53,23 +53,22 @@
 - Describing experimental effects based on a particular stage duration
 - Estimating the effect of trial-wise manipuations on the identified stages (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
 - Time-lock EEG signal to the onset of a given stage and perform classical ERPs or time-frequency analysis based on the onset of a new stage
 - And many more (e.g. evidence accumulation models on decision stage, classification based on the number of transition events in the signal,...)
 
 
 # Documentation
-**Important note** The current tutorials are based on the latest (unstable) version not yet default in _pip_, installing through github is therefore recommended or specify the beta version when installing through _pip_: ```pip install hsmm-mvpy==0.1.0b1```
 
 The package is available through *pip*. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
     $ conda create -n hmp 
     $ conda activate hmp
     $ conda install pip #if not already installed
-    $ pip install hsmm-mvpy==0.1.0b1
+    $ pip install hsmm-mvpy
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
     import hsmm_mvpy as hmp
 ```
 
@@ -123,56 +122,56 @@
 
 ## Importing HMP
 import hsmm_mvpy as hmp
 from hsmm_mvpy import simulations
 ```
 
 
+
 ### Simulating data
 
 In the following code block we simulate 50 trials from four known sources, this is not code you would need for your own analysis except if you'd want to simulate and test properties of HMP models. All four sources are defined by a location, an activation amplitude and a distribution in time (here a gamma with shape and scale parameters) for the onsets of the stages on each trial. The simulation functions are based on this [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
 
 _If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once (alternatively you can just download the corresponding simulation file and place it in the same folder from where you are running this notebook)_
 
 
 
+
 ```python
 cpus = 5 # For multiprocessing, usually a good idea to use multiple CPUs as long as you have enough RAM
 
 n_trials = 50 #Number of trials to simulate
 
 ##### Here we define the sources of the brain activity (event) for each trial
-# Because the last source determines the response, we will get four events during the trials, and therefore five stages
 n_sources = 5
 frequency = 10.#Frequency of the event defining its duration, half-sine of 10Hz = 50ms
 amplitude = .5e-6 #Amplitude of the event in nAm, defining signal to noise ratio
 shape = 2 #shape of the gamma distribution
 means = np.array([60, 150, 200, 100, 80])/shape #Mean duration of the stages in ms
-names = simulations.available_sources()[:n_sources]#Which source to activate at each stage (see atlas when calling simulations.available_sources())
+names = simulations.available_sources()[:n_sources+1]#Which source to activate at each stage (see atlas when calling simulations.available_sources())
 
 sources = []
 for source in zip(names, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
     sources.append([source[0], frequency, amplitude, gamma(shape, scale=source[1])])
 
 # Function used to generate the data
-file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True) #location indicates the middle of the event after the stage start time in ms
+file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True)
 #Recovering sampling frequency of the simulated dataset
 sfreq = simulations.simulation_sfreq()
 #load electrode position, specific to the simulations
 positions = simulations.simulation_positions()
 ```
 
     Simulating ./dataset_README_raw.fif
+    [done]
     ./dataset_README_raw.fif simulated
 
 
-
 ### Creating the event structure and plotting the raw data
 
-
 To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 1 signal the onset of the stimulus and 6 the moment of the response. Hence a trial is defined as the times occuring between the triggers 1 and 6.
 
 
 ```python
 #Recovering the events to epoch the data (in the number of trials defined above)
 generating_events = np.load(file[1])
 resp_trigger = int(np.max(np.unique(generating_events[:,2])))#Resp trigger is the last source in each trial
@@ -182,96 +181,108 @@
 events = generating_events[(generating_events[:,2] == 1) | (generating_events[:,2] == resp_trigger)]#only retain stimulus and response triggers
 
 #Visualising the raw simulated EEG data
 import mne
 raw = mne.io.read_raw_fif(file[0], preload=False, verbose=False)
 raw.pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events, block=True);
 ```
-![png](README_files/README_7_1.png)
 
+    NOTE: pick_types() is a legacy function. New code should use inst.pick(...).
+    Using qt as 2D backend.
+    Channels marked as bad:
+    none
+
+
+![png](README_files/README_7_1.png)
 
 ### Recovering number of stages as well as actual by-trial variation
 
 To see how well HMP does at recovering by-trial stages below, here we get the ground truth from our simulation. Unfortunately, with an actual dataset you don’t have access to this, of course. 
 
+
 ```python
 %matplotlib inline
 number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
 #Recover the actual time of the simulated events
 random_source_times = np.reshape(np.ediff1d(generating_events[:,0],to_begin=0)[generating_events[:,2] > 1], \
            (n_trials, number_of_sources))
 ```
 
 ## Demo for a single participant in a single condition based on the simulated data
 
-First we read the EEG data as we would for a single participant:
+First we read the EEG data as we would for a single participant
 
 
 ```python
 # Reading the data
 eeg_data = hmp.utils.read_mne_data(file[0], event_id=event_id, resp_id=resp_id, sfreq=sfreq, 
             events_provided=events, verbose=False)
 
 ```
 
     Processing participant ./dataset_README_raw.fif's continuous eeg
-    Reading 0 ... 143915  =      0.000 ...   239.613 secs...
+    Reading 0 ... 161924  =      0.000 ...   269.597 secs...
     50 trials were retained for participant ./dataset_README_raw.fif
 
 
+
 HMP uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
 
 
+
+
 ```python
 #example of usage of xarray
 print(eeg_data)
-eeg_data.sel(electrodes=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
-    .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='electrodes');
+eeg_data.sel(channels=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
+    .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='channels');
 ```
 
     <xarray.Dataset>
-    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 783)
+    Dimensions:      (participant: 1, epochs: 50, channels: 59, samples: 667)
     Coordinates:
       * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
-      * electrodes   (electrodes) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
-      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 776 777 778 779 780 781 782
+      * channels     (channels) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
+      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 660 661 662 663 664 665 666
+        event_name   (epochs) object 'stimulus' 'stimulus' ... 'stimulus' 'stimulus'
+        rt           (epochs) float64 0.5628 0.9956 0.5478 ... 0.7043 0.7659 0.8591
       * participant  (participant) <U2 'S0'
     Data variables:
-        data         (participant, epochs, electrodes, samples) float64 -3.747e-0...
-        event_name   (participant, epochs) object 'stimulus' ... 'stimulus'
-        rt           (participant, epochs) float64 0.5444 0.641 ... 0.8991 1.304
+        data         (participant, epochs, channels, samples) float64 -1.603e-06 ...
     Attributes:
         sfreq:    600.614990234375
         offset:   0
 
 
 
     
 ![png](README_files/README_12_1.png)
     
 
 
-
 Next we transform the data as in Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) including standardization of individual variances (not in this case as we have only one simulated participant), z-scoring and spatial principal components analysis (PCA). 
 
 Note that if the number of components to retain is not specified, the scree plot of the PCA is displayed and a prompt ask how many PCs should be retained (in this case we specify it as building the README does not allow for prompts)
 
 
 ```python
 hmp_data = hmp.utils.transform_data(eeg_data, apply_standard=False, n_comp=4)
 ```
 
 # HMP model
 
 Once the data is in the expected format, we can initialize an HMP object; note that no estimation is performed yet.
 
+
+
 ```python
 init = hmp.models.hmp(hmp_data, eeg_data, event_width=50, cpus=cpus)#Initialization of the model
 ```
 
+
 We are looking for stages in the data (**Hidden Markov**) and assume that transitions between stages are signaled by a template in the data (**pattern analysis**). By default we use the same template as Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet'.apa.org/doi/10.1037/rev0000030)), a 10 Hz half-sine, resulting in a 50ms duration bump-like shape:
 
 
 
 ```python
 plt.plot(init.template,'x');
 ```
@@ -285,27 +296,27 @@
 This pattern is assumed to be present across several electrodes (**multivariate**). In order to find it, we apply a cross-correlation between that shape and the (normalized) EEG data:
 
 
 
 ```python
 epoch = 0 #illustrating the first trial
 hmp_data.unstack().sel(component=[0,1,2], epochs=epoch).squeeze().plot.line(hue='component');
-plt.vlines(random_source_times[epoch,:-1].cumsum()-1, -3, 3, 'k')#overlaying the simulated stage transition times
+plt.vlines(random_source_times[epoch,:-1].cumsum()-1, -3, 3, 'k');#overlaying the simulated stage transition times
 ```
 
 
     
-![png](README_files/README_20_1.png)
+![png](README_files/README_20_0.png)
     
 
 
-
 The by-trial onset of this transition pattern event is assumed to be captured by a probability distribution (**semi-Markov**), e.g. in this application a gamma with a shape of 2:
 
 
+
 ```python
 T = 350
 plt.plot(np.linspace(0,T,1001),gamma.pdf(np.linspace(0,T,1001), 2, scale=50)) 
 plt.xlabel('t');
 ```
 
 
@@ -318,36 +329,41 @@
 
 # Estimating an HMP model
 
 We can directly fit an HMP model without giving any info on the number of stages (see tutorial 2 for a detailed explanation of the following cell)
 
 
 
+
+
 ```python
 estimates = init.fit(step=20, verbose=True)
 ```
 
 
+      0%|          | 0/418 [00:00<?, ?it/s]
 
-    Transition event 1 found around sample 37
-    Transition event 2 found around sample 137
-    Transition event 3 found around sample 277
-    Transition event 4 found around sample 348
+
+    Transition event 1 found around sample 42
+    Transition event 2 found around sample 154
+    Transition event 3 found around sample 285
+    Transition event 4 found around sample 369
     Estimating 4 events model
     Parameters estimated for 4 events model
 
 
 ### Visualizing results of the fit
 
 In the previous cell we initiated an HMP model looking for default 50ms bumps – the transition events – in the EEG signal. The method discovered four events, and therefore five gamma-distributed stages with a fixed shape of 2 and an estimated scale. We can now inspect the results of the fit.
 
 We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
 
 
 
+
 ```python
 hmp.visu.plot_topo_timecourse(eeg_data, estimates, #Data and estimations 
                                positions, init,#position of the electrodes and initialized model
                                magnify=1, sensors=False, time_step=1000/init.sfreq,#Display control parameters
                                times_to_display = np.mean(init.ends - init.starts))#plot reaction times
 ```
 
@@ -358,17 +374,19 @@
 
 
 This shows us the electrode activity on the scalp as well as the average time of occurence of the events based on the stage distributions.
 
 As we are estimating the event onsets on a by-trial basis we can look at the by-trial variation in stage duration.
 
 
+
 ```python
-event_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('event')#computing predicted event times
-ax = hmp.visu.plot_latencies_average(event_times_estimates, init.event_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
+event_times_estimates = init.compute_times(init, estimates, mean=False,fill_value=0, add_rt=True).dropna('event')#computing predicted event times
+ax = hmp.visu.plot_latencies_average(event_times_estimates, 1, errs='ci', \
+                                     times_to_display = np.mean(init.ends - init.starts))
 ax.set_ylabel('your label here');
 ```
 
 
     
 ![png](README_files/README_28_0.png)
     
@@ -382,15 +400,15 @@
 hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)), survival=True)
 ```
 
 
 
 
-    <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
+    <Axes: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
 ![png](README_files/README_30_1.png)
     
@@ -401,39 +419,42 @@
 ![png](README_files/README_30_2.png)
     
 
 
 As HMP estimated stage onset per trial we can also look at the predicted stage onsets for a given trial.
 
 
+
 ```python
 hmp.visu.plot_distribution(estimates.eventprobs.sel(trial_x_participant=('S0', 0)), 
                             xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 ```
 
 
 
 
-    <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
+    <Axes: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
 ![png](README_files/README_32_1.png)
     
 
 
+
 This then shows the likeliest stage onset location in time for the first trial!
 
 ## Comparing with ground truth
 
 As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HMP. Perhaps to state the obvious, this code is specific to the case where you simulate data.
 
 
+
 ```python
 colors = sns.color_palette(None, number_of_sources)
 plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.prod(axis=1), color=colors,s=50)
 plt.plot([np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],
          [np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],'--');
 plt.title('Actual vs estimated stage durations')
 plt.xlabel('Simulated stage duration')
@@ -459,19 +480,21 @@
 
 
     
 ![png](README_files/README_36_0.png)
     
 
 
+
 We see that the HMP recovered the exact average location of the bumps defined in the simulated data.
 
 We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HMP model
 
 
+
 ```python
 fig, ax= plt.subplots(number_of_sources,1, figsize=(5,3.5*number_of_sources), dpi=300)
 ax[0].set_title('Comparing true vs estimated single trial stage durations')
 i = 0
 
 for event in init.compute_times(init, estimates, duration=True, mean=False, add_rt=True).T:
     sns.regplot(x=random_source_times[:,i].T, y=event, ax=ax[i], color=colors[i])
@@ -483,14 +506,15 @@
 
 
     
 ![png](README_files/README_38_0.png)
     
 
 
+
 We see that every stage gets nicely recovered even on a by-trial basis!
 
 # Beyond summary statistics for EEG analysis
 
 Now the purpose, apart from determining the number and time course of important EEG events in the reaction time, is also to use the by-trial information.
 
 We illustrate this by first plotting the traditional event-related potentials (i.e. taking the average of given electrodes across the different time points) with cherry-picked electrodes.
@@ -502,15 +526,15 @@
 import pandas as pd
 
 data = eeg_data.stack({'trial_x_participant':['participant','epochs']}).data.dropna('trial_x_participant', how="all")
 fig, ax = plt.subplots(1,1, figsize=(20,5), sharey=True)
 
 for electrode in zip(['EEG 016','EEG 025','EEG 020'],#Cherry-picked electrodes
                      ['darkgreen','darkred','darkblue']):
-    df = pd.DataFrame(data.sel(electrodes=electrode[0]).squeeze().T).melt(var_name='Time')
+    df = pd.DataFrame(data.sel(channels=electrode[0]).squeeze().T).melt(var_name='Time')
     sns.lineplot(x='Time', y='value',data=df, color=electrode[1])
 
 plt.vlines(np.cumsum(random_source_times.mean(axis=0)), -3e-6, 3e-6)
 plt.ylabel('Volt')
 plt.xlim(0,500)
 plt.ylim(-3e-6,3e-6);
 
@@ -523,14 +547,16 @@
 
 
 Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is similar to traditional ERPs that have a very clear signal in the beginning of a trial (as events are more in phase) and summed and blurred further away from the stimulus (as events are off phase).
 
 Now things can get better if we first parse, by-trial, the signal into the different stages based on the HMP estimates:
 
 
+
+
 ```python
 BRP_times = init.compute_times(init, estimates.dropna('event'), fill_value=0, add_rt=True)
 
 fig, ax = plt.subplots(1,number_of_sources, figsize=(20,5), sharey=True, sharex=True)
 ax[0].set_ylabel('Volt')
 for stage in range(number_of_sources):
     BRP = hmp.utils.event_times(data, BRP_times,'EEG 016',stage=stage)
@@ -548,18 +574,20 @@
 
     
 ![png](README_files/README_42_0.png)
     
 
 
 
+
 In this case we clearly see at each stage the half-sine (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sine). Note that the end of the stages tend to be noisier because fewer trials are defining the average signal.
 
 
 ### Follow-up
 
 For examples on how to use the package when the number of transition events/stages is unkown, or to compare stage durations across conditions see the tutorial notebooks:
 - Load EEG data (tutorial 1)
 - Estimating a given number of events (tutorial 2)
 - Test for the number of events that best explains the data (tutorial 3)
 - Testing differences across conditions (tutorial 4)
+- Plotting Event Related Potentials with an HMP decomposition (tutorial 5)
```

### Comparing `hsmm_mvpy-0.1.0b7/README.md` & `hsmm_mvpy-0.1.0b8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,22 @@
 - Describing experimental effects based on a particular stage duration
 - Estimating the effect of trial-wise manipuations on the identified stages (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
 - Time-lock EEG signal to the onset of a given stage and perform classical ERPs or time-frequency analysis based on the onset of a new stage
 - And many more (e.g. evidence accumulation models on decision stage, classification based on the number of transition events in the signal,...)
 
 
 # Documentation
-**Important note** The current tutorials are based on the latest (unstable) version not yet default in _pip_, installing through github is therefore recommended or specify the beta version when installing through _pip_: ```pip install hsmm-mvpy==0.1.0b1```
 
 The package is available through *pip*. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
     $ conda create -n hmp 
     $ conda activate hmp
     $ conda install pip #if not already installed
-    $ pip install hsmm-mvpy==0.1.0b1
+    $ pip install hsmm-mvpy
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
     import hsmm_mvpy as hmp
 ```
 
@@ -80,56 +79,56 @@
 
 ## Importing HMP
 import hsmm_mvpy as hmp
 from hsmm_mvpy import simulations
 ```
 
 
+
 ### Simulating data
 
 In the following code block we simulate 50 trials from four known sources, this is not code you would need for your own analysis except if you'd want to simulate and test properties of HMP models. All four sources are defined by a location, an activation amplitude and a distribution in time (here a gamma with shape and scale parameters) for the onsets of the stages on each trial. The simulation functions are based on this [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
 
 _If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once (alternatively you can just download the corresponding simulation file and place it in the same folder from where you are running this notebook)_
 
 
 
+
 ```python
 cpus = 5 # For multiprocessing, usually a good idea to use multiple CPUs as long as you have enough RAM
 
 n_trials = 50 #Number of trials to simulate
 
 ##### Here we define the sources of the brain activity (event) for each trial
-# Because the last source determines the response, we will get four events during the trials, and therefore five stages
 n_sources = 5
 frequency = 10.#Frequency of the event defining its duration, half-sine of 10Hz = 50ms
 amplitude = .5e-6 #Amplitude of the event in nAm, defining signal to noise ratio
 shape = 2 #shape of the gamma distribution
 means = np.array([60, 150, 200, 100, 80])/shape #Mean duration of the stages in ms
-names = simulations.available_sources()[:n_sources]#Which source to activate at each stage (see atlas when calling simulations.available_sources())
+names = simulations.available_sources()[:n_sources+1]#Which source to activate at each stage (see atlas when calling simulations.available_sources())
 
 sources = []
 for source in zip(names, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
     sources.append([source[0], frequency, amplitude, gamma(shape, scale=source[1])])
 
 # Function used to generate the data
-file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True) #location indicates the middle of the event after the stage start time in ms
+file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True)
 #Recovering sampling frequency of the simulated dataset
 sfreq = simulations.simulation_sfreq()
 #load electrode position, specific to the simulations
 positions = simulations.simulation_positions()
 ```
 
     Simulating ./dataset_README_raw.fif
+    [done]
     ./dataset_README_raw.fif simulated
 
 
-
 ### Creating the event structure and plotting the raw data
 
-
 To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 1 signal the onset of the stimulus and 6 the moment of the response. Hence a trial is defined as the times occuring between the triggers 1 and 6.
 
 
 ```python
 #Recovering the events to epoch the data (in the number of trials defined above)
 generating_events = np.load(file[1])
 resp_trigger = int(np.max(np.unique(generating_events[:,2])))#Resp trigger is the last source in each trial
@@ -139,96 +138,108 @@
 events = generating_events[(generating_events[:,2] == 1) | (generating_events[:,2] == resp_trigger)]#only retain stimulus and response triggers
 
 #Visualising the raw simulated EEG data
 import mne
 raw = mne.io.read_raw_fif(file[0], preload=False, verbose=False)
 raw.pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events, block=True);
 ```
-![png](README_files/README_7_1.png)
 
+    NOTE: pick_types() is a legacy function. New code should use inst.pick(...).
+    Using qt as 2D backend.
+    Channels marked as bad:
+    none
+
+
+![png](README_files/README_7_1.png)
 
 ### Recovering number of stages as well as actual by-trial variation
 
 To see how well HMP does at recovering by-trial stages below, here we get the ground truth from our simulation. Unfortunately, with an actual dataset you don’t have access to this, of course. 
 
+
 ```python
 %matplotlib inline
 number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
 #Recover the actual time of the simulated events
 random_source_times = np.reshape(np.ediff1d(generating_events[:,0],to_begin=0)[generating_events[:,2] > 1], \
            (n_trials, number_of_sources))
 ```
 
 ## Demo for a single participant in a single condition based on the simulated data
 
-First we read the EEG data as we would for a single participant:
+First we read the EEG data as we would for a single participant
 
 
 ```python
 # Reading the data
 eeg_data = hmp.utils.read_mne_data(file[0], event_id=event_id, resp_id=resp_id, sfreq=sfreq, 
             events_provided=events, verbose=False)
 
 ```
 
     Processing participant ./dataset_README_raw.fif's continuous eeg
-    Reading 0 ... 143915  =      0.000 ...   239.613 secs...
+    Reading 0 ... 161924  =      0.000 ...   269.597 secs...
     50 trials were retained for participant ./dataset_README_raw.fif
 
 
+
 HMP uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
 
 
+
+
 ```python
 #example of usage of xarray
 print(eeg_data)
-eeg_data.sel(electrodes=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
-    .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='electrodes');
+eeg_data.sel(channels=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
+    .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='channels');
 ```
 
     <xarray.Dataset>
-    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 783)
+    Dimensions:      (participant: 1, epochs: 50, channels: 59, samples: 667)
     Coordinates:
       * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
-      * electrodes   (electrodes) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
-      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 776 777 778 779 780 781 782
+      * channels     (channels) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
+      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 660 661 662 663 664 665 666
+        event_name   (epochs) object 'stimulus' 'stimulus' ... 'stimulus' 'stimulus'
+        rt           (epochs) float64 0.5628 0.9956 0.5478 ... 0.7043 0.7659 0.8591
       * participant  (participant) <U2 'S0'
     Data variables:
-        data         (participant, epochs, electrodes, samples) float64 -3.747e-0...
-        event_name   (participant, epochs) object 'stimulus' ... 'stimulus'
-        rt           (participant, epochs) float64 0.5444 0.641 ... 0.8991 1.304
+        data         (participant, epochs, channels, samples) float64 -1.603e-06 ...
     Attributes:
         sfreq:    600.614990234375
         offset:   0
 
 
 
     
 ![png](README_files/README_12_1.png)
     
 
 
-
 Next we transform the data as in Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) including standardization of individual variances (not in this case as we have only one simulated participant), z-scoring and spatial principal components analysis (PCA). 
 
 Note that if the number of components to retain is not specified, the scree plot of the PCA is displayed and a prompt ask how many PCs should be retained (in this case we specify it as building the README does not allow for prompts)
 
 
 ```python
 hmp_data = hmp.utils.transform_data(eeg_data, apply_standard=False, n_comp=4)
 ```
 
 # HMP model
 
 Once the data is in the expected format, we can initialize an HMP object; note that no estimation is performed yet.
 
+
+
 ```python
 init = hmp.models.hmp(hmp_data, eeg_data, event_width=50, cpus=cpus)#Initialization of the model
 ```
 
+
 We are looking for stages in the data (**Hidden Markov**) and assume that transitions between stages are signaled by a template in the data (**pattern analysis**). By default we use the same template as Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet'.apa.org/doi/10.1037/rev0000030)), a 10 Hz half-sine, resulting in a 50ms duration bump-like shape:
 
 
 
 ```python
 plt.plot(init.template,'x');
 ```
@@ -242,27 +253,27 @@
 This pattern is assumed to be present across several electrodes (**multivariate**). In order to find it, we apply a cross-correlation between that shape and the (normalized) EEG data:
 
 
 
 ```python
 epoch = 0 #illustrating the first trial
 hmp_data.unstack().sel(component=[0,1,2], epochs=epoch).squeeze().plot.line(hue='component');
-plt.vlines(random_source_times[epoch,:-1].cumsum()-1, -3, 3, 'k')#overlaying the simulated stage transition times
+plt.vlines(random_source_times[epoch,:-1].cumsum()-1, -3, 3, 'k');#overlaying the simulated stage transition times
 ```
 
 
     
-![png](README_files/README_20_1.png)
+![png](README_files/README_20_0.png)
     
 
 
-
 The by-trial onset of this transition pattern event is assumed to be captured by a probability distribution (**semi-Markov**), e.g. in this application a gamma with a shape of 2:
 
 
+
 ```python
 T = 350
 plt.plot(np.linspace(0,T,1001),gamma.pdf(np.linspace(0,T,1001), 2, scale=50)) 
 plt.xlabel('t');
 ```
 
 
@@ -275,36 +286,41 @@
 
 # Estimating an HMP model
 
 We can directly fit an HMP model without giving any info on the number of stages (see tutorial 2 for a detailed explanation of the following cell)
 
 
 
+
+
 ```python
 estimates = init.fit(step=20, verbose=True)
 ```
 
 
+      0%|          | 0/418 [00:00<?, ?it/s]
 
-    Transition event 1 found around sample 37
-    Transition event 2 found around sample 137
-    Transition event 3 found around sample 277
-    Transition event 4 found around sample 348
+
+    Transition event 1 found around sample 42
+    Transition event 2 found around sample 154
+    Transition event 3 found around sample 285
+    Transition event 4 found around sample 369
     Estimating 4 events model
     Parameters estimated for 4 events model
 
 
 ### Visualizing results of the fit
 
 In the previous cell we initiated an HMP model looking for default 50ms bumps – the transition events – in the EEG signal. The method discovered four events, and therefore five gamma-distributed stages with a fixed shape of 2 and an estimated scale. We can now inspect the results of the fit.
 
 We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
 
 
 
+
 ```python
 hmp.visu.plot_topo_timecourse(eeg_data, estimates, #Data and estimations 
                                positions, init,#position of the electrodes and initialized model
                                magnify=1, sensors=False, time_step=1000/init.sfreq,#Display control parameters
                                times_to_display = np.mean(init.ends - init.starts))#plot reaction times
 ```
 
@@ -315,17 +331,19 @@
 
 
 This shows us the electrode activity on the scalp as well as the average time of occurence of the events based on the stage distributions.
 
 As we are estimating the event onsets on a by-trial basis we can look at the by-trial variation in stage duration.
 
 
+
 ```python
-event_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('event')#computing predicted event times
-ax = hmp.visu.plot_latencies_average(event_times_estimates, init.event_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
+event_times_estimates = init.compute_times(init, estimates, mean=False,fill_value=0, add_rt=True).dropna('event')#computing predicted event times
+ax = hmp.visu.plot_latencies_average(event_times_estimates, 1, errs='ci', \
+                                     times_to_display = np.mean(init.ends - init.starts))
 ax.set_ylabel('your label here');
 ```
 
 
     
 ![png](README_files/README_28_0.png)
     
@@ -339,15 +357,15 @@
 hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)), survival=True)
 ```
 
 
 
 
-    <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
+    <Axes: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
 ![png](README_files/README_30_1.png)
     
@@ -358,39 +376,42 @@
 ![png](README_files/README_30_2.png)
     
 
 
 As HMP estimated stage onset per trial we can also look at the predicted stage onsets for a given trial.
 
 
+
 ```python
 hmp.visu.plot_distribution(estimates.eventprobs.sel(trial_x_participant=('S0', 0)), 
                             xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 ```
 
 
 
 
-    <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
+    <Axes: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
 ![png](README_files/README_32_1.png)
     
 
 
+
 This then shows the likeliest stage onset location in time for the first trial!
 
 ## Comparing with ground truth
 
 As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HMP. Perhaps to state the obvious, this code is specific to the case where you simulate data.
 
 
+
 ```python
 colors = sns.color_palette(None, number_of_sources)
 plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.prod(axis=1), color=colors,s=50)
 plt.plot([np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],
          [np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],'--');
 plt.title('Actual vs estimated stage durations')
 plt.xlabel('Simulated stage duration')
@@ -416,19 +437,21 @@
 
 
     
 ![png](README_files/README_36_0.png)
     
 
 
+
 We see that the HMP recovered the exact average location of the bumps defined in the simulated data.
 
 We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HMP model
 
 
+
 ```python
 fig, ax= plt.subplots(number_of_sources,1, figsize=(5,3.5*number_of_sources), dpi=300)
 ax[0].set_title('Comparing true vs estimated single trial stage durations')
 i = 0
 
 for event in init.compute_times(init, estimates, duration=True, mean=False, add_rt=True).T:
     sns.regplot(x=random_source_times[:,i].T, y=event, ax=ax[i], color=colors[i])
@@ -440,14 +463,15 @@
 
 
     
 ![png](README_files/README_38_0.png)
     
 
 
+
 We see that every stage gets nicely recovered even on a by-trial basis!
 
 # Beyond summary statistics for EEG analysis
 
 Now the purpose, apart from determining the number and time course of important EEG events in the reaction time, is also to use the by-trial information.
 
 We illustrate this by first plotting the traditional event-related potentials (i.e. taking the average of given electrodes across the different time points) with cherry-picked electrodes.
@@ -459,15 +483,15 @@
 import pandas as pd
 
 data = eeg_data.stack({'trial_x_participant':['participant','epochs']}).data.dropna('trial_x_participant', how="all")
 fig, ax = plt.subplots(1,1, figsize=(20,5), sharey=True)
 
 for electrode in zip(['EEG 016','EEG 025','EEG 020'],#Cherry-picked electrodes
                      ['darkgreen','darkred','darkblue']):
-    df = pd.DataFrame(data.sel(electrodes=electrode[0]).squeeze().T).melt(var_name='Time')
+    df = pd.DataFrame(data.sel(channels=electrode[0]).squeeze().T).melt(var_name='Time')
     sns.lineplot(x='Time', y='value',data=df, color=electrode[1])
 
 plt.vlines(np.cumsum(random_source_times.mean(axis=0)), -3e-6, 3e-6)
 plt.ylabel('Volt')
 plt.xlim(0,500)
 plt.ylim(-3e-6,3e-6);
 
@@ -480,14 +504,16 @@
 
 
 Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is similar to traditional ERPs that have a very clear signal in the beginning of a trial (as events are more in phase) and summed and blurred further away from the stimulus (as events are off phase).
 
 Now things can get better if we first parse, by-trial, the signal into the different stages based on the HMP estimates:
 
 
+
+
 ```python
 BRP_times = init.compute_times(init, estimates.dropna('event'), fill_value=0, add_rt=True)
 
 fig, ax = plt.subplots(1,number_of_sources, figsize=(20,5), sharey=True, sharex=True)
 ax[0].set_ylabel('Volt')
 for stage in range(number_of_sources):
     BRP = hmp.utils.event_times(data, BRP_times,'EEG 016',stage=stage)
@@ -505,18 +531,20 @@
 
     
 ![png](README_files/README_42_0.png)
     
 
 
 
+
 In this case we clearly see at each stage the half-sine (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sine). Note that the end of the stages tend to be noisier because fewer trials are defining the average signal.
 
 
 ### Follow-up
 
 For examples on how to use the package when the number of transition events/stages is unkown, or to compare stage durations across conditions see the tutorial notebooks:
 - Load EEG data (tutorial 1)
 - Estimating a given number of events (tutorial 2)
 - Test for the number of events that best explains the data (tutorial 3)
 - Testing differences across conditions (tutorial 4)
+- Plotting Event Related Potentials with an HMP decomposition (tutorial 5)
```

### Comparing `hsmm_mvpy-0.1.0b7/pyproject.toml` & `hsmm_mvpy-0.1.0b8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "hsmm_mvpy"
-version = "0.1.0-beta7"
+version = "0.1.0-beta8"
 authors = [
   { name="Gabriel Weindel", email="gabriel.weindel@gmail.com" },
   { name="Leendert van Maanen", email="e@mail.com" },
   { name="Jelmer Borst", email="e@mail.com" },
 ]
 description = "Package for fitting Hidden Semi-Markov Models to electro-encephalographic data"
 readme = "README.md"
@@ -22,12 +22,13 @@
 dependencies=["mne >=1.0.0",
 "numpy",
 "xarray",
 "scikit-learn",
 "statsmodels",
 "seaborn",
 "scipy",
-"netcdf4"]
+"netcdf4",
+"more_itertools"]
 
 [project.urls]
 "Homepage" = "https://github.com/GWeindel/hmp"
 "Bug Tracker" = "https://github.com/GWeindel/hmp/issues"
```

### Comparing `hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/models.py` & `hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,35 @@
 
 '''
 
 import numpy as np
 import xarray as xr
 import multiprocessing as mp
 import itertools
-import math
-import time#Just for speed testing
+from pandas import MultiIndex
 from warnings import warn, filterwarnings, resetwarnings
 from scipy.stats import gamma as sp_gamma
 import matplotlib.pyplot as plt
-from tqdm.auto import tqdm
-default_colors =  ['cornflowerblue','indianred','orange','darkblue','darkgreen','gold', 'brown']
+from matplotlib.colors import LinearSegmentedColormap
+from hsmm_mvpy import utils
+from itertools import cycle
+
 
+try:
+    __IPYTHON__
+    from tqdm.notebook import tqdm
+except NameError:
+    import tqdm.tqdm
+
+default_colors =  ['cornflowerblue','indianred','orange','darkblue','darkgreen','gold', 'brown']
 
+                   
 class hmp:
     
-    def __init__(self, data, eeg_data=None, sfreq=None, offset=0, cpus=1, event_width=50, shape=2, estimate_magnitudes=True, estimate_parameters=True, template=None, location=None, distribution='gamma'):
+    def __init__(self, data, eeg_data=None, sfreq=None, offset=0, cpus=1, event_width=50, shape=2, estimate_magnitudes=True, estimate_parameters=True, template=None, location=None, distribution='gamma', em_method="mean"):
         '''
         HMP calculates the probability of data summing over all ways of 
         placing the n events to break the trial into n + 1 stages.
 
         Parameters
         ----------
         data : ndarray
@@ -29,54 +38,54 @@
         sfreq : int
             Sampling frequency of the signal (initially 100)
         event_width : int
             width of events in milliseconds, originally 5 samples
         location : float
             Minimum stage duration in milliseconds. 
         '''
-        if distribution == 'gamma':
-            from scipy.stats import gamma as sp_dist
-        elif distribution == 'lognormal':
-            from scipy.stats import lognorm as sp_dist
-        elif distribution == 'wald':
-            from scipy.stats import invgauss as sp_dist
-        elif distribution == 'weibull':
-            from scipy.stats import weibull_min as sp_dist
-        else:
-            raise ValueError(f'Unknown Distribution {distribution}')
+        match distribution:
+            case 'gamma':
+                from scipy.stats import gamma as sp_dist
+            case 'lognormal':
+                from scipy.stats import lognorm as sp_dist
+            case 'wald':
+                from scipy.stats import invgauss as sp_dist
+            case 'weibull':
+                from scipy.stats import weibull_min as sp_dist
+            case _:
+                raise ValueError(f'Unknown Distribution {distribution}')
         self.cdf = sp_dist.cdf
             
         if sfreq is None:
             sfreq = eeg_data.sfreq
         if offset is None:
             offset = eeg_data.offset
         self.sfreq = sfreq
         self.steps = 1000/self.sfreq
         self.shape = float(shape)
         self.event_width = event_width
         self.event_width_samples = int(np.round(self.event_width / self.steps))
         if location is None:
-            self.location = int(np.round(self.event_width_samples/2))
-        else: self.location =  int(np.round(location / self.steps))
-        durations = data.unstack().sel(component=0).swap_dims({'epochs':'trials'})\
+            self.location = self.event_width / self.steps/2
+        else: self.location =  location / self.steps
+        durations = data.unstack().sel(component=0).rename({'epochs':'trials'})\
             .stack(trial_x_participant=['participant','trials']).dropna(dim="trial_x_participant",\
             how="all").groupby('trial_x_participant').count(dim="samples").cumsum().squeeze()
         if durations.trial_x_participant.count() > 1:
             dur_dropped_na = durations.dropna("trial_x_participant")
             starts = np.roll(dur_dropped_na.data, 1)
             starts[0] = 0
             ends = dur_dropped_na.data-1 -offset
         else: 
             dur_dropped_na = durations
             starts = np.array([0])
             ends = np.array([dur_dropped_na.data-1 -offset])
         self.starts = starts
         self.ends = ends
         self.durations =  self.ends-self.starts+1
-        self.max_events = self.compute_max_events()
         if durations.trial_x_participant.count() > 1:
             self.named_durations =  durations.dropna("trial_x_participant") - durations.dropna("trial_x_participant").shift(trial_x_participant=1, fill_value=0)
             self.coords = durations.reset_index('trial_x_participant').coords
         else: 
             self.named_durations = durations
             self.coords = durations.coords
         self.mean_d = self.durations.mean()
@@ -85,14 +94,21 @@
         self.cpus = cpus
         self.n_samples, self.n_dims = np.shape(data.data.T)
         if template is None:
             self.template = self.event_shape()
         else: self.template = template
         self.events = self.cross_correlation(data.data.T)#adds event morphology
         self.max_d = self.durations.max()
+        self.em_method = em_method
+        if self.em_method == "mean":
+            self.data_matrix = np.zeros((self.max_d, self.n_trials, self.n_dims), dtype=np.float64)
+            for trial in range(self.n_trials):
+                self.data_matrix[:self.durations[trial],trial,:] = \
+                    self.events[self.starts[trial]:self.ends[trial]+1,:]
+                #Reorganize samples crosscorrelated with template on trial basis
         self.estimate_magnitudes = estimate_magnitudes
         self.estimate_parameters = estimate_parameters
         if self.max_d > 500:#FFT conv from scipy faster in this case
             from scipy.signal import fftconvolve
             self.convolution = fftconvolve
         else:
             self.convolution = np.convolve
@@ -114,30 +130,31 @@
         
         Parameters
         ----------
         data : ndarray
             2D ndarray with n_samples * components
         Returns
         -------
-        bumbs : ndarray
+        events : ndarray
             a 2D ndarray with samples * PC components where cell values have
             been correlated with event morphology
         '''
         from scipy.signal import fftconvolve
         events = np.zeros(data.shape)
         for trial in range(self.n_trials):#avoids confusion of gains between trials
             for dim in np.arange(self.n_dims):
                 events[self.starts[trial]:self.ends[trial]+1,dim] = \
                     fftconvolve(data[self.starts[trial]:self.ends[trial]+1, dim], \
                         self.template, mode='full')\
                         [len(self.template)-1:self.durations[trial]+len(self.template)+1]
         return events
 
-    def fit_single(self, n_events=None, magnitudes=None, parameters=None, threshold=1, verbose=True,
-            starting_points=1, parameters_to_fix=None, magnitudes_to_fix=None, method='random', multiple_n_events=None):
+    def fit_single(self, n_events=None, magnitudes=None, parameters=None, parameters_to_fix=None, 
+                   magnitudes_to_fix=None, tolerance=1e-4, max_iteration=1e3, maximization=True, min_iteration = 1,
+                   starting_points=1, method='random', return_max=True, verbose=True, cpus=None):
         '''
         Fit HMP for a single n_events model
         
         Parameters
         ----------
         n_events : int
             how many events are estimated
@@ -146,22 +163,23 @@
         parameters : list
             list of initial conditions for Gamma distribution scale parameter. If parameters are estimated, the list provided is used as starting point,
             if parameters are fixed, parameters estimated will be the same as the one provided. When providing a list, stage need to be in the same order
             _n_th gamma parameter is  used for the _n_th stage
         threshold : float
             threshold for the HMP algorithm, 0 skips HMP
         '''
-        import pandas as pd 
-        if n_events is None:
-            raise ValueError('The fit_single() function needs to be provided with a number of expected transition events. Look at function fit() if you want to fit a model without assuming a particular number of events.')
+        assert n_events is not None, 'The fit_single() function needs to be provided with a number of expected transition events'
+        assert self.location*(n_events) < min(self.durations), f'{n_events} events do not fit given the minimum duration of {min(self.durations)} and a location of {self.location}'
         if verbose:
             if parameters is None:
                 print(f'Estimating {n_events} events model with {starting_points} starting point(s)')
             else:
                 print(f'Estimating {n_events} events model')
+        if cpus is None:
+            cpus = self.cpus
         if n_events is None and parameters is not None:
             n_events = len(parameters)-1
         if self.estimate_magnitudes == False:#Don't need to manually fix mags if not estimated
             magnitudes_to_fix = np.arange(n_events)
         if self.estimate_parameters == False:#Don't need to manually fix pars if not estimated
             parameters_to_fix = np.arange(n_events+1)            
         #Formatting parameters
@@ -171,195 +189,237 @@
             magnitudes = magnitudes.dropna(dim='event').values  
         if isinstance(magnitudes, np.ndarray):
             magnitudes = magnitudes.copy()
         if isinstance(parameters, np.ndarray):
             parameters = parameters.copy()          
         if parameters_to_fix is None: parameters_to_fix=[]
         if magnitudes_to_fix is None: magnitudes_to_fix=[]
+        
+        if parameters is not None:
+            if len(np.shape(parameters)) == 3:
+                starting_points = np.shape(parameters)[0]
+        if magnitudes is not None:
+            if len(np.shape(magnitudes)) == 3:
+                starting_points = np.shape(magnitudes)[0]
+        
         if starting_points > 0:#Initialize with equally spaced option
             if parameters is None:
                 parameters = np.tile([self.shape, ((np.mean(self.durations))/(n_events+1)-self.location)/self.shape], (n_events+1,1))
+                parameters[0,1] = np.mean(self.durations)/(n_events+1)/self.shape #first stage has no location
             initial_p = parameters
             
             if magnitudes is None:
                 magnitudes = np.zeros((n_events,self.n_dims), dtype=np.float64)
             initial_m = magnitudes
-        
-        if starting_points > 1:
-            filterwarnings("ignore", category=RuntimeWarning)#Error in the generation of random see GH issue #38
-            parameters = [initial_p]
-            magnitudes = [initial_m]
-            if method == 'random':
-                for sp in np.arange(starting_points):
-                    proposal_p = self.gen_random_stages(n_events, self.mean_d)
-                    proposal_m = np.zeros((n_events,self.n_dims), dtype=np.float64)#Mags are NOT random but always 0
-                    proposal_p[parameters_to_fix] = initial_p[parameters_to_fix]
-                    proposal_m[magnitudes_to_fix] = initial_m[magnitudes_to_fix]
-                    parameters.append(proposal_p)
-                    magnitudes.append(proposal_m)
-            elif method == 'grid':
-                parameters = self._grid_search(n_events+1, iter_limit=starting_points, method='grid')
-                magnitudes = np.zeros((len(parameters), n_events, self.n_dims), dtype=np.float64)
-            else:
-                raise ValueError('Unknown starting point method requested, use "random" or "grid"')
-            with mp.Pool(processes=self.cpus) as pool:
-                estimates = pool.starmap(self.EM, 
-                    zip(itertools.repeat(n_events), magnitudes, parameters, itertools.repeat(1),\
-                    itertools.repeat(magnitudes_to_fix),itertools.repeat(parameters_to_fix),))   
+        if starting_points > 1 or len(np.shape(magnitudes)) == 3 or len(np.shape(parameters)) == 3:
+            filterwarnings('ignore', 'Convergence failed, estimation hitted the maximum ', )#will be the case but for a subset only hence ignore
+            if len(np.shape(initial_m)) == 2:
+                parameters = [initial_p]
+                magnitudes = [initial_m]
+                if method == 'random':
+                    for _ in np.arange(starting_points):
+                        proposal_p = self.gen_random_stages(n_events, self.mean_d)
+                        proposal_p[parameters_to_fix] = initial_p[parameters_to_fix]
+                        parameters.append(proposal_p)
+                    magnitudes = self.gen_mags(n_events, starting_points, method='random', verbose=False)
+                    magnitudes[:,magnitudes_to_fix,:] = np.tile(initial_m[magnitudes_to_fix], (len(magnitudes), 1, 1))
+
+                elif method == 'grid':
+                    parameters = self._grid_search(n_events+1, iter_limit=starting_points, method='grid')
+                    magnitudes = np.zeros((len(parameters), n_events, self.n_dims), dtype=np.float64)#Grid search is not yet done for mags
+                else:
+                    raise ValueError('Unknown starting point method requested, use "random" or "grid"')
+            elif len(np.shape(initial_m)) == 3:
+                magnitudes = initial_m
+                if len(np.shape(initial_p)) == 3:
+                    parameters = initial_p
+                else:
+                    parameters = np.tile(parameters, (len(magnitudes),1,1))
+            if cpus>1: 
+                with mp.Pool(processes=cpus) as pool:
+
+                    estimates = pool.starmap(self.EM, 
+                        zip(itertools.repeat(n_events), magnitudes, parameters, itertools.repeat(maximization),
+                        itertools.repeat(magnitudes_to_fix),itertools.repeat(parameters_to_fix), itertools.repeat(max_iteration), itertools.repeat(tolerance), itertools.repeat(min_iteration)))   
+            else:#avoids problems if called in an already parallel function
+                estimates = []
+                for pars, mags in zip(parameters, magnitudes):
+                    estimates.append(self.EM(n_events, mags, pars, maximization,\
+                    magnitudes_to_fix, parameters_to_fix, max_iteration, tolerance, min_iteration))
+                resetwarnings()
             lkhs_sp = [x[0] for x in estimates]
             mags_sp = [x[1] for x in estimates]
             pars_sp = [x[2] for x in estimates]
             eventprobs_sp = [x[3] for x in estimates]
-            max_lkhs = np.where(lkhs_sp == np.max(lkhs_sp))[0][0]
-            lkh = lkhs_sp[max_lkhs]
-            mags = mags_sp[max_lkhs]
-            pars = pars_sp[max_lkhs]
-            eventprobs = eventprobs_sp[max_lkhs]
-            resetwarnings()
+            traces_sp = [x[4] for x in estimates]
+            if return_max:
+                max_lkhs = np.argmax(lkhs_sp)
+                lkh = lkhs_sp[max_lkhs]
+                mags = mags_sp[max_lkhs]
+                pars = pars_sp[max_lkhs]
+                eventprobs = eventprobs_sp[max_lkhs]
+                traces = traces_sp[max_lkhs]
+            else:
+                lkh = lkhs_sp
+                mags = mags_sp
+                pars = pars_sp
+                eventprobs = eventprobs_sp
+                traces = np.zeros((len(lkh),  max([len(x) for x in traces_sp])))*np.nan
+                for i, _i in enumerate(traces_sp):
+                    traces[i, :len(_i)] = _i
             
         elif starting_points==1:#informed starting point
-            lkh, mags, pars, eventprobs = self.EM(n_events, initial_m, initial_p,\
-                                        threshold, magnitudes_to_fix, parameters_to_fix)
+            lkh, mags, pars, eventprobs, traces = self.EM(n_events, initial_m, initial_p,\
+                                        maximization, magnitudes_to_fix, parameters_to_fix, \
+                                         max_iteration, tolerance, min_iteration)
 
         else:#uninitialized    
             if np.any(parameters)== None:
                 parameters = np.tile([self.shape, (self.mean_d)/self.shape], (n_events+1,1))
             if np.any(magnitudes)== None:
                 magnitudes = np.zeros((n_events, self.n_dims), dtype=np.float64)
-            lkh, mags, pars, eventprobs = self.EM(n_events, magnitudes, parameters,\
-                                        threshold, magnitudes_to_fix, parameters_to_fix)
-        if multiple_n_events is not None and len(pars) != multiple_n_events+1:#align all dimensions
-            pars = np.concatenate((pars, np.tile(np.nan, (multiple_n_events+1-len(pars),2))))
-            mags = np.concatenate((mags, np.tile(np.nan, 
-                (multiple_n_events-len(mags), np.shape(mags)[1]))),axis=0)
-            eventprobs = np.concatenate((eventprobs, np.tile(np.nan, (np.shape(eventprobs)[0],\
-                    np.shape(eventprobs)[1], multiple_n_events-np.shape(eventprobs)[2]))),axis=2)
-            n_events = multiple_n_events
-        
-        xrlikelihoods = xr.DataArray(lkh , name="likelihoods")
-        xrparams = xr.DataArray(pars, dims=("stage",'parameter'), name="parameters", 
-                        coords = [range(len(pars)), ['shape','scale']])
-        xrmags = xr.DataArray(mags, dims=("event","component"), name="magnitudes",
-                    coords = [range(len(mags)), range(np.shape(mags)[1])])
-        part, trial = self.coords['participant'].values, self.coords['trials'].values
-        if n_events>0:
-            n_samples, n_participant_x_trials,_ = np.shape(eventprobs)
-        else:
-            n_samples, n_participant_x_trials = np.shape(eventprobs)
-        if n_participant_x_trials >1 and n_events >0:
-            xreventprobs = xr.Dataset({'eventprobs': (('event', 'trial_x_participant','samples'), 
-                                         eventprobs.T)},
-                         {'event':np.arange(n_events),
-                          'samples':np.arange(n_samples),
-                        'trial_x_participant':  pd.MultiIndex.from_arrays([part,trial],
-                                names=('participant','trials'))})
-            xreventprobs = xreventprobs.transpose('trial_x_participant','samples','event')
-        elif n_events == 0:
-            xreventprobs = xr.Dataset({'eventprobs': (('trial_x_participant','samples'), 
-                                         eventprobs.T)},
-                         {'samples':np.arange(n_samples),
-                        'trial_x_participant':  pd.MultiIndex.from_arrays([part,trial],
-                                names=('participant','trials'))})
-            xreventprobs = xreventprobs.transpose('trial_x_participant','samples')
+            lkh, mags, pars, eventprobs, traces = self.EM(n_events, magnitudes, parameters, maximization, magnitudes_to_fix, parameters_to_fix,\
+                                        max_iteration, tolerance, min_iteration)
+        if len(np.shape(eventprobs)) == 3:
+            n_event_xr = n_event_xreventprobs = len(mags)
+            n_stage = n_event_xr+1
+        elif len(np.shape(eventprobs)) == 2:#0 event case
+            eventprobs = np.transpose(eventprobs[np.newaxis], axes=(1,2,0))
+            mags = np.transpose(mags[np.newaxis], axes=(1,0))
+            n_event_xr = 0
+            n_event_xreventprobs = 1
+            n_stage = 1
+        if len(np.shape(eventprobs)) == 3:
+            xrlikelihoods = xr.DataArray(lkh , name="likelihoods")
+            xrtraces = xr.DataArray(traces, dims=("em_iteration"), name="traces", coords={'em_iteration':range(len(traces))})
+            xrparams = xr.DataArray(pars, dims=("stage",'parameter'), name="parameters", 
+                            coords = [range(n_stage), ['shape','scale']])
+            xrmags = xr.DataArray(mags, dims=("event","component"), name="magnitudes",
+                        coords={'event':range(n_event_xr),
+                                "component":range(self.n_dims)})
+            part, trial = self.coords['participant'].values, self.coords['trials'].values
 
-        elif n_participant_x_trials == 1: 
             xreventprobs = xr.Dataset({'eventprobs': (('event', 'trial_x_participant','samples'), 
-                                         eventprobs.T)},
-                         {'event':np.arange(n_events),
-                          'samples':np.arange(n_samples)})
+                                             eventprobs.T)},
+                             {'event':range(n_event_xreventprobs),
+                              'samples':range(np.shape(eventprobs)[0]),
+                            'trial_x_participant':  MultiIndex.from_arrays([part,trial],
+                                    names=('participant','trials'))})
             xreventprobs = xreventprobs.transpose('trial_x_participant','samples','event')
-        estimated = xr.merge((xrlikelihoods, xrparams, xrmags, xreventprobs))
+        else: 
+            n_event_xr = len(mags[0])
+            # if traces[-1] - traces[-2] < 0:
+            #     warn(f'Last iteration of the estimation procedure lead to a decrease in log-likelihood, convergence ', RuntimeWarning)
+            xrlikelihoods = xr.DataArray(lkh , dims=("iteration"), name="likelihoods", coords={'iteration':range(len(lkh))})
+            xrtraces = xr.DataArray(traces, dims=("iteration","em_iteration"), name="traces", coords={'iteration':range(len(lkh)), 'em_iteration':range(len(traces[0]))})
+            xrparams = xr.DataArray(pars, dims=("iteration","stage",'parameter'), name="parameters", 
+                            coords = {'iteration': range(len(lkh)), 'parameter':['shape','scale']})
+            xrmags = xr.DataArray(mags, dims=("iteration","event","component"), name="magnitudes",
+                        coords={'iteration':range(len(lkh)), 'event':range(n_event_xr),
+                                "component":range(self.n_dims)})
+            part, trial = self.coords['participant'].values, self.coords['trials'].values
+
+            xreventprobs = xr.Dataset({'eventprobs': (('iteration','event', \
+                                    'trial_x_participant','samples'), [x.T for x in eventprobs])},
+                             {'iteration':range(len(lkh)),
+                              'event':np.arange(n_event_xr),
+                              'samples':np.arange(np.shape(eventprobs)[1]),
+                              'trial_x_participant':  MultiIndex.from_arrays([part,trial],
+                                    names=('participant','trials'))})
+            xreventprobs = xreventprobs.transpose('iteration','trial_x_participant','samples','event')
+        estimated = xr.merge((xrlikelihoods, xrparams, xrmags, xreventprobs, xrtraces))
 
         if verbose:
             print(f"Parameters estimated for {n_events} events model")
         return estimated
     
-    def EM(self, n_events, magnitudes, parameters,  threshold, magnitudes_to_fix=None, parameters_to_fix=None, max_iteration = 1e3):
+    def EM(self, n_events, magnitudes, parameters,  maximization=True, magnitudes_to_fix=None, parameters_to_fix=None, max_iteration=1e3, tolerance=1e-4, min_iteration=1):  
         '''
         Expectation maximization function underlying fit
         ''' 
+        if not isinstance(maximization, bool):#Backward compatibility with previous versions
+            warn('Deprecated use of the threshold function, use maximization and tolerance arguments. Setting tolerance at 1 for compatibility')
+            maximization = {1:True, 0:False}[maximization]
+            if maximization:#Backward compatibility, equivalent to previous threshold = 1
+                tolerance = 1
         null_stages = np.where(parameters[:,1]<0)[0]
         wrong_shape = np.where(parameters[:,0]!=self.shape)[0]
         if len(null_stages)>0:
             raise ValueError(f'Wrong scale parameter input, provided scale parameter(s) {null_stages} should be positive but have value {parameters[null_stages,:].prod(axis=1)}')
         if len(wrong_shape)>0:
             raise ValueError(f'Wrong shape parameter input, provided parameter(s) {wrong_shape} shape is {parameters[wrong_shape,0]} but expected  expected {self.shape}')
         initial_parameters =  np.copy(parameters)
         initial_magnitudes = np.copy(magnitudes)
         
         lkh, eventprobs = self.estim_probs(magnitudes, parameters, n_events)
-        means = np.zeros((self.max_d, self.n_trials, self.n_dims), dtype=np.float64)
-        for trial in range(self.n_trials):
-            means[:self.durations[trial],trial,:] = self.events[self.starts[trial]:self.ends[trial]+1,:]
-            #Reorganize samples crosscorrelated with template on trial basis
-        if threshold == 0 or n_events==0:
+        traces = []
+        i = 0
+        if not maximization or n_events==0:
             lkh_prev = lkh
             magnitudes_prev = initial_magnitudes
             parameters_prev = initial_parameters
             eventprobs_prev = eventprobs
         else:
-            for event in range(n_events):
-                for comp in range(self.n_dims):
-                    magnitudes[event,comp] = np.mean(np.sum( \
-                        eventprobs[:,:,event]*means[:,:,comp], axis=0))
-            parameters = self.scale_parameters(eventprobs, n_events)
-            null_stages = np.where(parameters[:,1]<0)[0]
-            if len(null_stages) == 0: 
-                lkh_prev = -np.inf
+            lkh_prev = -np.inf
+            while i < max_iteration :#Expectation-Maximization algorithm
+                if i > min_iteration and tolerance > lkh - lkh_prev:
+                    break
+                    #As long as new run gives better likelihood, go on  
+                lkh_prev = lkh.copy()
                 magnitudes_prev = magnitudes.copy()
                 parameters_prev = parameters.copy()
                 eventprobs_prev = eventprobs.copy()
-            else:#Corner case in simulations
-                lkh_prev = lkh
-                magnitudes_prev = initial_magnitudes
-                parameters_prev = initial_parameters
-                eventprobs_prev = eventprobs
-        i = 0
-        while lkh - lkh_prev > threshold and i < max_iteration:#Expectation-Maximization algorithm
-            #As long as new run gives better likelihood, go on  
-            lkh_prev = lkh.copy()
-            magnitudes_prev = magnitudes.copy()
-            parameters_prev = parameters.copy()
-            eventprobs_prev = eventprobs.copy()
-            #Magnitudes from Expectation
-            for event in range(n_events):
-                for comp in range(self.n_dims):
-                    magnitudes[event,comp] = np.mean(np.sum( \
-                        eventprobs[:,:,event]*means[:,:,comp], axis=0))
-                    # Scale cross-correlation with likelihood of the transition
-                    # sum by-trial these scaled activation for each transition events
-                    # average across trials
-
-            magnitudes[magnitudes_to_fix,:] = initial_magnitudes[magnitudes_to_fix,:].copy()
-            #Parameters from Expectation
-            parameters = self.scale_parameters(eventprobs, n_events)
-            parameters[parameters_to_fix, :] = initial_parameters[parameters_to_fix,:].copy()
-            lkh, eventprobs = self.estim_probs(magnitudes, parameters, n_events)
-            i += 1
-        null_probs = np.where(eventprobs_prev<-1e-10)[0]
-        if len(null_probs)>0:
-            warn('Negative probabilities found after estimation, this likely refers to several events overlapping events. In case of simulated data ensure that events are enoughly separated (i.e. location parameter). In the case of real data this error is not expected, please report to the maintainers')
+                #Magnitudes from Expectation
+                if self.em_method == "max": 
+                    event_times = np.zeros((n_events+1, self.n_trials))
+                    event_times[-1,:] = self.mean_d
+                for event in range(n_events):
+                    if self.em_method == "max":
+                        #Take time point at maximum p() for each trial
+                        #Average channel activity at those points
+                        event_values = np.zeros((self.n_trials, self.n_dims))
+                        for trial in range(self.n_trials):
+                            event_times[event,trial]  = np.argmax(eventprobs[:, trial, event])
+                            event_values[trial] = self.events[self.starts[trial] + int(event_times[event,trial])]
+                        magnitudes[event] = np.mean(event_values, axis=0)
+                    elif self.em_method == "mean":
+                        for comp in range(self.n_dims):
+                            magnitudes[event,comp] = np.mean(np.sum( \
+                                eventprobs[:,:,event]*self.data_matrix[:,:,comp], axis=0))
+                        # Scale cross-correlation with likelihood of the transition
+                        # sum by-trial these scaled activation for each transition events
+                        # average across trials
+                magnitudes[magnitudes_to_fix,:] = initial_magnitudes[magnitudes_to_fix,:].copy()
+                if self.em_method == "max":
+                    parameters = self.scale_parameters(eventprobs=None, n_events=n_events, averagepos=np.mean(event_times,axis=1))#Parameters from Expectation
+                elif self.em_method == "mean":
+                    parameters = self.scale_parameters(eventprobs, n_events)#Parameters from Expectation
+                parameters[parameters_to_fix, :] = initial_parameters[parameters_to_fix,:].copy()
+                lkh, eventprobs = self.estim_probs(magnitudes, parameters, n_events)
+                traces.append(lkh)
+                i += 1
         if i == max_iteration:
             warn(f'Convergence failed, estimation hitted the maximum number of iteration ({int(max_iteration)})', RuntimeWarning)
-        return lkh_prev, magnitudes_prev, parameters_prev, eventprobs_prev
+        return lkh_prev, magnitudes_prev, parameters_prev, eventprobs_prev, np.array(traces)
 
+    
     def estim_probs(self, magnitudes, parameters, n_events, lkh_only=False):
         '''
         
         Returns
         -------
         likelihood : float
             Summed log probabilities
         eventprobs : ndarray
             Probabilities with shape max_samples*n_trials*n_events
         '''
         n_stages = n_events+1
         gains = np.zeros((self.n_samples, n_events), dtype=np.float64)
         for i in range(self.n_dims):
-            # computes the gains, i.e. how much the congruence between the pattern shape
+            # computes the gains, i.e. congruence between the pattern shape
             # and the data given the magnitudes of the sensors
             gains = gains + self.events[:,i][np.newaxis].T * magnitudes[:,i]
         gains = np.exp(gains)
         probs = np.zeros([self.max_d,self.n_trials,n_events], dtype=np.float64) # prob per trial
         probs_b = np.zeros([self.max_d,self.n_trials,n_events], dtype=np.float64)# Sample and state reversed
         for trial in np.arange(self.n_trials):
             # Following assigns gain per trial to variable probs 
@@ -367,20 +427,17 @@
                 gains[self.starts[trial]:self.ends[trial]+1,:] 
             # Same but samples and events are reversed, this allows to compute
             # fwd and bwd in the same way in the following steps
             probs_b[:self.durations[trial],trial,:] = \
                 gains[self.starts[trial]:self.ends[trial]+1,:][::-1,::-1]
 
         pmf = np.zeros([self.max_d, n_stages], dtype=np.float64) # Gamma pmf for each stage parameters
+        locations = np.concatenate([[0], np.repeat(self.location, n_events)])#all stages except first stage have a location (mainly to avoid overlap in cross-correlated signal)
         for stage in range(n_stages):
-            if n_stages-1 > stage > 0:
-                location = self.location
-            else:
-                location = 0
-            pmf[:,stage] = self.distribution_pmf(parameters[stage,0], parameters[stage,1], location)
+            pmf[:,stage] = self.distribution_pmf(parameters[stage,0], parameters[stage,1], locations[stage])
         pmf_b = pmf[:,::-1] # Stage reversed gamma pmf, same order as prob_b
 
         if n_events > 0:
             forward = np.zeros((self.max_d, self.n_trials, n_events), dtype=np.float64)
             backward = np.zeros((self.max_d, self.n_trials, n_events), dtype=np.float64)
             # Computing forward and backward helper variable
             #  when stage = 0:
@@ -398,19 +455,43 @@
                     backward[:,trial,event] = self.convolution(add_b[:,trial], pmf_b[:, event])[:self.max_d]
                 forward[:,:,event] = forward[:,:,event]*probs[:,:,event]
             #re-arranging backward to the expected variable
             backward = backward[:,:,::-1]#undoes stage inversion
             for trial in np.arange(self.n_trials):#Undoes sample inversion
                 backward[:self.durations[trial],trial,:] = \
                     backward[:self.durations[trial],trial,:][::-1]
+            
             eventprobs = forward * backward
-            eventprobs[eventprobs < 1e-10] = 0 #floating point precision error
-            likelihood = np.sum(np.log(eventprobs[:,:,0].sum(axis=0)))#sum over max_samples to avoid 0s in log
-            eventprobs = eventprobs / eventprobs.sum(axis=0)
+            eventprobs = np.clip(eventprobs, 0, None) #floating point precision error
+            
+            #eventprobs can be so low as to be 0, avoid dividing by 0
+            #this only happens when magnitudes are 0 and gammas are randomly determined
+            if (eventprobs.sum(axis=0) == 0).any() or (eventprobs[:,:,0].sum(axis=0) == 0).any(): 
+
+                #set likelihood
+                eventsums = eventprobs[:,:,0].sum(axis=0)
+                eventsums[eventsums != 0] = np.log(eventsums[eventsums != 0])
+                eventsums[eventsums == 0] = -np.inf
+                likelihood = np.sum(eventsums)
+
+                #set eventprobs, check if any are 0   
+                eventsums = eventprobs.sum(axis=0)
+                if (eventsums == 0).any():
+                    for i in range(eventprobs.shape[0]):
+                        eventprobs[i,:,:][eventsums == 0] = 0
+                        eventprobs[i,:,:][eventsums != 0] = eventprobs[i,:,:][eventsums != 0] / eventsums[eventsums != 0]
+                else:
+                    eventprobs = eventprobs / eventprobs.sum(axis=0)
+
+            else:
+
+                likelihood = np.sum(np.log(eventprobs[:,:,0].sum(axis=0)))#sum over max_samples to avoid 0s in log
+                eventprobs = eventprobs / eventprobs.sum(axis=0)
             #conversion to probabilities, divide each trial and state by the sum of the likelihood of the n points in a trial
+            
         else:
             forward = np.zeros((self.max_d, self.n_trials), dtype=np.float64)
             backward = np.zeros((self.max_d, self.n_trials), dtype=np.float64)
             forward[:,:] = np.tile(pmf[:,0][np.newaxis].T,\
                 (1,self.n_trials))
             backward[:,:] = np.tile(pmf_b[:,0][np.newaxis].T,\
                         (1,self.n_trials))
@@ -439,20 +520,20 @@
         Returns
         -------
         p : ndarray
             probabilty mass function for a gamma with given parameters
         '''
         if scale == 0:
             warn('Convergence failed: one stage has been found to be null')
-        p = self.cdf(np.arange(self.max_d), shape, scale=scale, loc=location)
-        #Location is in fact +1 as np.arange starts from 0
+        p = self.cdf(np.arange(1, self.max_d+1), shape, scale=scale, loc=location)
+        #Location is at least = to 1 given that range starts at 0, desirable as these are durations
         p = np.diff(p, prepend=0)#going to pmf
         return p
     
-    def scale_parameters(self, eventprobs, n_events):
+    def scale_parameters(self, eventprobs=None, n_events=None, averagepos=None):
         '''
         Used for the re-estimation in the EM procdure. The likeliest location of 
         the event is computed from eventprobs. The scale parameters are then taken as the average 
         distance between the events corrected for (eventual) location
         Parameters
         ----------
         eventprobs : ndarray
@@ -464,77 +545,27 @@
         shape : float
             shape parameter for the gamma, defaults to 2  
         Returns
         -------
         params : ndarray
             shape and scale for the gamma distributions
         '''
-        averagepos = np.concatenate([np.arange(1,self.max_d+1)@eventprobs.mean(axis=1),
-                                     [self.mean_d]])#Durations
+        if eventprobs is not None:
+            averagepos = np.concatenate([np.arange(1,self.max_d+1)@eventprobs.mean(axis=1),
+                                         [self.mean_d]])#Durations
         params = np.zeros((n_events+1,2), dtype=np.float64)
         params[:,0] = self.shape
         params[:,1] = np.diff(averagepos, prepend=0)
-        # params[[0.-1],1] += self.location
-        params[0,1] -= .5#Event following starts half-sample before position
-        params[-1,1] += .5# Last event terminates half-sample earlier
+        params[:-1,1] += .5
+        params[-1,1] -= 1
         params[:,1] = params[:,1]/params[:,0]
         return params
-    
-    def __multi_cpu_dispatch(self, list_n_events, list_mags, list_pars, threshold=1, verbose=False):
-        if self.cpus > 1:
-            if len(list_n_events) == 1:
-                list_n_events = itertools.repeat(list_n_events)
-            with mp.Pool(processes=self.cpus) as pool:
-                event_loo_results = pool.starmap(self.fit_single, 
-                    zip(list_n_events, list_mags, list_pars,
-                        itertools.repeat(threshold),itertools.repeat(verbose)))
-        else:
-            event_loo_results = []
-            for event_tmp, flat_tmp in zip(list_mags, list_pars):
-                n_event = len(event_loo_results)+1
-                event_loo_results.append(self.fit_single(n_event, event_tmp, flat_tmp, 0, False))
-        return event_loo_results
-        
-    def loo_loglikelihood(self, estimates):
-        event_loo_results = [estimates.copy()]
-        n_events = event_loo_results[0].dropna('event').event.max().values
-        list_values_n_events = [n_events]
-        print(event_loo_results[0].parameters.values)  
-        i = 0
-        while n_events  > 0:
-            print(f'Estimating all solutions for {n_events} number of events')
-            temp_best = event_loo_results[i]#previous event solution
-            temp_best = temp_best.dropna('event')
-            temp_best = temp_best.dropna('stage')
-            n_events_list = np.arange(n_events+1)#all events from previous solution
-            flats = temp_best.parameters.values
-            print(flats)
-            events_temp, flats_temp = [], []
-            for event in np.arange(n_events+1):#creating all possible solutions
-                events_temp.append(temp_best.magnitudes.sel(event = np.array(list(set(n_events_list) - set([event])))).values)
-                flat = event + 1 #one more flat than events
-                temp = flats[:,1].copy()
-                temp[flat-1] += temp[flat]
-                temp = np.delete(temp, flat)
-                flats_temp.append(np.reshape(np.concatenate([np.repeat(self.shape, len(temp)), temp]), (2, len(temp))).T)
-
-            event_loo_likelihood_temp = self.__multi_cpu_dispatch(np.repeat(n_events,n_events+1), events_temp, 
-                     flats_temp, 0, False)
-            print([[x.likelihoods.values, x.parameters.values[:,1],'---------------------------------------\n'] for x in event_loo_likelihood_temp])
-            print('---------------------------------------\n')
-            models = xr.concat(event_loo_likelihood_temp, dim="iteration")
-            event_loo_results.append(models.sel(iteration=[np.where(models.likelihoods == models.likelihoods.max())[0][0]]).squeeze('iteration'))
-            n_events = event_loo_results[-1].dropna('event').event.max().values
-            list_values_n_events.append(n_events)
-            i += 1
-        lkh = [x.likelihoods for x in event_loo_results]
-        return lkh
 
 
-    def backward_estimation(self,max_events=None, min_events=0, max_fit=None, max_starting_points=1, method="random", threshold=1):
+    def backward_estimation(self,max_events=None, min_events=0, max_fit=None, max_starting_points=1, method="random", tolerance=1e-4, maximization=True, max_iteration=1e3):
         '''
         First read or estimate max_event solution then estimate max_event - 1 solution by 
         iteratively removing one of the event and pick the one with the highest 
         likelihood
         
         Parameters
         ----------
@@ -544,62 +575,64 @@
         max_starting_points: int
             how many random starting points iteration to try for the model estimating the maximal number of events
         
         '''
         if max_events is None and max_fit is None:
             max_events = self.compute_max_events()
         if not max_fit:
-            if max_starting_points >0:
+            if max_starting_points > 0:
                 print(f'Estimating all solutions for maximal number of events ({max_events}) with 1 pre-defined starting point and {max_starting_points-1} {method} starting points')
             event_loo_results = [self.fit_single(max_events, starting_points=max_starting_points, method=method, verbose=False)]
         else:
             event_loo_results = [max_fit]
         max_events = event_loo_results[0].event.max().values+1
         i = 0
         for n_events in np.arange(max_events-1,min_events,-1):
             print(f'Estimating all solutions for {n_events} number of events')
             temp_best = event_loo_results[i]#previous event solution
             temp_best = temp_best.dropna('event')
             temp_best = temp_best.dropna('stage')
             n_events_list = np.arange(n_events+1)#all events from previous solution
             flats = temp_best.parameters.values
-            events_temp,flats_temp = [],[]
+            events_temp,pars_temp = [],[]
             for event in np.arange(n_events+1):#creating all possible solutions
                 events_temp.append(temp_best.magnitudes.sel(event = np.array(list(set(n_events_list) - set([event])))).values)
                 flat = event + 1 #one more flat than events
                 temp = np.copy(flats[:,1])
                 temp[flat-1] = temp[flat-1] + temp[flat]
                 temp = np.delete(temp, flat)
-                flats_temp.append(np.reshape(np.concatenate([np.repeat(self.shape, len(temp)), temp]), (2, len(temp))).T)
-            if self.cpus > 1:
-                with mp.Pool(processes=self.cpus) as pool:
-                    event_loo_likelihood_temp = pool.starmap(self.fit_single, 
-                        zip(itertools.repeat(n_events), events_temp, flats_temp,
-                            itertools.repeat(threshold),itertools.repeat(False),itertools.repeat(1),\
-                            itertools.repeat([]),itertools.repeat([]),\
-                            itertools.repeat('random'),itertools.repeat(max_events)))
-            else:
-                raise ValueError('For loop not yet written use cpus >1')
+                pars_temp.append(np.reshape(np.concatenate([np.repeat(self.shape, len(temp)), temp]), (2, len(temp))).T)
+            inputs = zip(itertools.repeat(n_events), events_temp, pars_temp,\
+                        itertools.repeat([]), itertools.repeat([]),\
+                        itertools.repeat(tolerance), itertools.repeat(max_iteration), \
+                        itertools.repeat(maximization), itertools.repeat(1),\
+                        itertools.repeat(1),itertools.repeat('random'), itertools.repeat(True),\
+                        itertools.repeat(False),itertools.repeat(1))
+            with mp.Pool(processes=self.cpus) as pool:
+                event_loo_likelihood_temp = pool.starmap(self.fit_single, inputs)
+
             models = xr.concat(event_loo_likelihood_temp, dim="iteration")
             event_loo_results.append(models.sel(iteration=[np.where(models.likelihoods == models.likelihoods.max())[0][0]]).squeeze('iteration'))
             i+=1
         bests = xr.concat(event_loo_results, dim="n_events")
         bests = bests.assign_coords({"n_events": np.arange(max_events,min_events,-1)})
         #bests = bests.squeeze('iteration')
         return bests
 
     def compute_max_events(self):
         '''
         Compute the maximum possible number of events given event width and mean or minimum reaction time
         '''
-        return int(np.min(self.durations)//(self.event_width_samples))
+        return int(np.rint(np.min(self.durations)//(self.location)))-1
 
     def event_times(self, eventprobs, mean=True):
         '''
         Compute event onset times based on event probabilities
+        This function is mainly kept for compatibility with previous matlab applications
+
         Parameters
         ----------
         a : float
             shape parameter
         b : float
             scale parameter
         max_length : int
@@ -641,16 +674,19 @@
 
         Returns
         -------
         times : xr.DataArray
             Transition event onset or stage duration with trial_x_participant*event dimensions
         '''
 
-        eventprobs = estimates.eventprobs
-        times = xr.dot(eventprobs, eventprobs.samples, dims='samples')#Most likely event location
+        eventprobs = estimates.eventprobs.fillna(0).copy()
+        if init.em_method == "max":
+            times = times = eventprobs.argmax('samples')#Most likely event location
+        else:
+            times = xr.dot(eventprobs, eventprobs.samples, dims='samples')
         n = len(times[0,:].values[np.isfinite(times[0,:].values)])
         if duration:
             fill_value=0
         if fill_value != None:            
             added = xr.DataArray(np.repeat(fill_value,len(times.trial_x_participant))[np.newaxis,:],
                                  coords={'event':[0], 
                                          'trial_x_participant':times.trial_x_participant})
@@ -668,29 +704,58 @@
                 times = times.diff(dim='stage')
         if mean:
             times = times.mean('trial_x_participant')
         return times
    
     @staticmethod
     def compute_topologies(channels, estimated, event_width_samples, extra_dim=False, mean=True):
-        shifted_times = estimated.eventprobs.shift(samples=event_width_samples//2+1, fill_value=0).copy()#Shifts to compute channel topology at the peak of the event
-        if extra_dim:
-            data =  xr.dot(channels.rename({'epochs':'trials'}).\
-                      stack(trial_x_participant=['participant','trials']).data.fillna(0).drop_duplicates('trial_x_participant'), \
-                      shifted_times.fillna(0), dims=['samples']).\
-                      transpose(extra_dim,'trial_x_participant','event','channels')
+        shift = event_width_samples//2+1#Shifts to compute channel topology at the peak of the event
+        channels = channels.rename({'epochs':'trials'}).\
+                          stack(trial_x_participant=['participant','trials']).data.fillna(0).drop_duplicates('trial_x_participant')
+        estimated = estimated.eventprobs.fillna(0).copy()
+        n_events = estimated.event.count().values
+        n_trials = estimated.trial_x_participant.count().values
+        n_channels = channels.channels.count().values
+        if not extra_dim:
+            event_values = np.zeros((n_trials, n_events, n_channels))*np.nan
+            for event in range(n_events):
+                #Take time point at maximum p() for each trial
+                #Average channel activity at those points            
+                for t, trial in enumerate(estimated.trial_x_participant):
+                    time = estimated.sel(trial_x_participant=trial, event=event).argmax('samples')
+                    event_values[t, event, :] = channels.sel(trial_x_participant=trial, samples=time+shift).values
+            event_values = xr.DataArray(event_values, 
+                        dims = ["trial_x_participant","event","channels"],
+                        coords={"trial_x_participant":estimated.trial_x_participant,
+                                "event": estimated.event,
+                                "channels":channels.channels
+                        })
         else:
-            data = xr.dot(channels.rename({'epochs':'trials'}).\
-                      stack(trial_x_participant=['participant','trials']).data.fillna(0).drop_duplicates('trial_x_participant'), \
-                      shifted_times.fillna(0), dims=['samples']).\
-                      transpose('trial_x_participant','event','channels')
+            n_dim = estimated[extra_dim].count().values
+            event_values = np.zeros((n_dim, n_trials, n_events, n_channels))*np.nan
+            for x in range(n_dim):
+                for event in range(n_events):
+                    #Take time point at maximum p() for each trial
+                    #Average channel activity at those points     
+                    for t, trial in enumerate(estimated[x].trial_x_participant):
+                        time = estimated[x].sel(trial_x_participant=trial, event=event).argmax('samples')
+                        event_values[x, t, event, :] = channels.sel(trial_x_participant=trial, samples=time+shift).values
+            event_values = xr.DataArray(event_values, 
+                    dims = [extra_dim, "trial_x_participant","event","channels"],
+                    coords={extra_dim:estimated[extra_dim],
+                            "trial_x_participant":estimated.trial_x_participant,
+                            "event": estimated.event,
+                            "channels":channels.channels
+                    })
         if mean:
-            data = data.mean('trial_x_participant')
-        return data
-    
+            return event_values.mean('trial_x_participant')
+        else:
+            return event_values
+
+
     def gen_random_stages(self, n_events, mean_d):
         '''
         Returns random stage duration between 0 and mean RT by iteratively drawind sample from a 
         uniform distribution between the last stage duration (equal to 0 for first iteration) and 1.
         Last stage is equal to 1-previous stage duration.
         The stages are then scaled to the mean RT
         Parameters
@@ -700,17 +765,55 @@
         mean_d : float
             scale parameter
         Returns
         -------
         random_stages : ndarray
             random partition between 0 and mean_d
         '''
-        random_stages = np.array([[self.shape,x*mean_d/self.shape] for x in np.random.beta(2, 2, n_events+1)])
+        mean_d = int(mean_d) - n_events * self.location #remove minimum stage duration
+        rnd_durations = np.zeros(n_events + 1)
+        while any(rnd_durations < 2): #make sure they are at least 2 samples
+            rnd_events = np.random.default_rng().integers(low = 0, high = mean_d, size = n_events) #n_events between 0 and mean_d
+            rnd_events = np.sort(rnd_events)
+            rnd_durations = np.hstack((rnd_events, mean_d)) - np.hstack((0, rnd_events))  #associated durations
+        random_stages = np.array([[self.shape, x / self.shape] for x in rnd_durations])
         return random_stages
     
+    def gen_mags(self, n_events, n_samples=None, lower_bound=-1, upper_bound=1, method=None, size=3, decimate=False, verbose=True):
+        '''
+        Return magnitudes sampled on a grid with n points between lower_bound and upper_bound for the n_events. All combinations are tested
+        '''
+        from itertools import product    
+        if n_samples == 1:
+            grid = np.zeros((n_events, 1, self.n_dims))
+        else: 
+            grid = np.array([x for x in product(np.linspace(lower_bound,upper_bound,size), repeat=self.n_dims)])
+
+        if verbose:
+            print(f'Number of potential magnitudes: {len(grid)}') 
+
+        if n_samples is None or n_samples > len(grid):
+            n_samples = len(grid)
+        if decimate:
+            n_samples = int(np.rint(len(grid) / decimate))
+            
+        if method is None and len(grid) != n_samples:
+            grid = grid[::len(grid)//n_samples]
+            n_samples = len(grid)
+            if verbose:
+                print(f'Because of decimation {len(grid)} will be estimated.')
+        gen_mags = np.zeros((n_events, n_samples, self.n_dims))
+        for event in range(n_events):
+            if method is None:
+                gen_mags[event,:,:] = grid
+            elif method == "random":
+                gen_mags[event,:,:] = grid[np.random.choice(range(len(grid)), size=n_samples, replace=False)]
+        gen_mags = np.transpose(gen_mags, axes=(1,0,2))
+        return gen_mags
+    
     def _grid_search(self, n_stages, n_points=None, verbose=True, start_time=0, end_time=None, iter_limit=np.inf, step=1, offset=None, method='slide'):
         '''
         This function decomposes the mean RT into a grid with points. Ideal case is to have a grid with one sample = one search point but the number
         of possibilities badly scales with the length of the RT and the number of stages. Therefore the iter_limit is used to select an optimal number
         of points in the grid with a given spacing. After having defined the grid, the function then generates all possible combination of 
         event placements within this grid. It is faster than using random points (both should converge) but depending on the mean RT and the number 
         of events to look for, the number of combination can be really large. 
@@ -736,15 +839,15 @@
         if end_time is None:
             end_time = int(self.mean_d)
         duration = end_time-start_time
         if n_points is None:
             n_points = duration//step
             duration = step*n_points
         check_n_posibilities = binomcoeff(n_points-1, n_stages-1)
-        if binomcoeff(n_points-1, n_stages-1) > iter_limit:
+        if check_n_posibilities > iter_limit:
             while binomcoeff(n_points-1, n_stages-1) > iter_limit:
                 n_points = n_points-1
             step = duration//n_points#same if no points removed in the previous step
             end_time = start_time+step*(n_points-1)#Rounding up to step size
             duration = end_time-start_time
         end_time = start_time+step*(n_points)#Rounding up to step size  
         grid = np.array([x for x in np.linspace(start_time+step, end_time-step, (duration//step))-start_time])#all possible durations
@@ -757,209 +860,254 @@
                 new_comb.append(np.array(list(mit.distinct_permutations(c))))
             comb = np.vstack(new_comb)
             parameters = np.zeros((len(comb),n_stages,2), dtype=np.float64)
             for idx, y in enumerate(comb):
                 parameters[idx, :, :] = [[self.shape, x/self.shape] for x in y]
             if verbose:
                 if check_n_posibilities > iter_limit:
-                    print(f'Initial number of possibilities is {check_n_posibilities}. Given a number of max iteration = {iter_limit}: fitting {len(parameters)} models based on all possibilities from grid search with a spacing of {int(step)} samples and {n_points} points and durations of {grid}')
+                    print(f'Initial number of possibilities is {check_n_posibilities}.') 
+                    print(f'Given the number of max iterations = {iter_limit}: fitting {len(comb)} models based on all \n possibilities from grid search with a spacing of {int(step)} samples and {n_points} points  \n and durations of {grid}.')
                 else:
-                    print(f'Fitting {len(parameters)} models using grid search')
+                    print(f'Fitting {len(comb)} models using grid search')
             if method == 'grid':
                 return parameters
             else:
                 return parameters[np.argsort(parameters[:,0,1]),:,:]
         else:
             raise ValueError(f'No combination found given length of the data {self.mean_d}, number of events {n_stages} and a max iteration of {iter_limit}')
     
-    def sliding_event(self, n_events=None, colors=default_colors, figsize=(12,3), verbose=True, method=None, plot_deriv=False, magnitudes=None, step=1):
+    def sliding_event_mags(self, epoch_data, step=5, decimate_grid = False, cpu=1, plot=False, tolerance=1e-4, min_iteration=10,alpha=.05):
+
+        grid = np.squeeze(self.gen_mags(1, decimate = decimate_grid,size=3)) #get magn grid
+        n_iter = len(grid)
+
+        #calculate estimates, returns lkhs, mags, times
+        inputs = zip(itertools.repeat((12,3)), itertools.repeat(False), itertools.repeat('search'), 
+                    grid, itertools.repeat(step), itertools.repeat(False), itertools.repeat(None),
+                    itertools.repeat(False),itertools.repeat(1), itertools.repeat(tolerance),itertools.repeat(min_iteration))
+        with mp.Pool(processes=cpu) as pool:
+            estimates = list(tqdm(pool.imap(self.sliding_event_star, inputs), total=len(grid)))
+        #topo prep
+        stacked_eeg_data = epoch_data.stack(trial_x_participant=('participant','epochs')).dropna('trial_x_participant',how='all').data.to_numpy() 
+        n_electrodes, _, n_trials = stacked_eeg_data.shape
+        shift = int(self.event_width_samples/2)
+
+        #collect results
+        max_run_len = max([len(x[0]) for x in estimates])
+        lkhs = np.zeros((n_iter * max_run_len))*np.nan
+        times = np.zeros((n_iter * max_run_len))*np.nan
+        mags = np.zeros((n_iter * max_run_len, self.n_dims))*np.nan
+        channels = np.zeros((n_iter * max_run_len, epoch_data.dims['channels']))*np.nan
+
+        for i, est in enumerate(estimates):
+            idx = i * max_run_len
+            lkhs[idx:(idx + len(est[0]))] = est[0]
+            mags[idx:(idx + len(est[0])), :] = est[1].squeeze()
+            times[idx:(idx + len(est[0]))] = np.mean(est[2],axis=1)  #these should NOT be shifted, later used to calc pars
+            
+            #get topos per estimation per trial, then average
+            topos = np.zeros((n_electrodes, n_trials, len(est[0])))
+            for j, times_per_event in enumerate(est[2]):
+                for trial in range(n_trials):
+                    topos[:,trial,j] = stacked_eeg_data[:, times_per_event[trial] + shift,trial]
+                
+            channels[idx:(idx+len(est[0])), :] = np.nanmean(topos,axis=1).T
+
+        mags = mags[~np.isnan(lkhs),:]
+        channels = channels[~np.isnan(lkhs),:]
+        times = times[~np.isnan(lkhs)]
+        lkhs = lkhs[~np.isnan(lkhs)]
+
+        if plot:
+            _, ax = plt.subplots(1,1,figsize=(20,3))
+            ax.plot(times, lkhs, '.', alpha=alpha)
+        
+        return lkhs, mags, channels, times
+
+    def sliding_event_star(self, args): #for tqdm usage
+        return self.sliding_event(*args)
+        
+    def sliding_event(self, figsize=(12,3), verbose=True, method=None, magnitudes=None, step=1, show=True, ax=None, fix_mags=False, fix_pars=False, cpus=None, tolerance=1e-4, min_iteration=1):
         '''
         This method outputs the likelihood and estimated parameters of a 1 event model with each sample, from 0 to the mean 
         epoch duration. The parameters and likelihoods that are returned are 
         Take the highest likelihood, place a event by excluding event width space around it, follow with the next one
         '''
-        
-        from itertools import cycle
-        
-        mean_d = int(self.mean_d)
-        init_n_events = n_events
-        # if n_events == None:
-        #     n_events = self.max_events
+             
         parameters = self._grid_search(2, verbose=verbose, step=step)#Looking for all possibilities with one event
-        if magnitudes is None:
+        if method is None or magnitudes is None:
             magnitudes = np.zeros((len(parameters),1, self.n_dims), dtype=np.float64)
+            maximization = True
+            if fix_mags:
+                mags_to_fix = [0]
+            else:        
+                mags_to_fix = []
+            ls = '-'
         else:
-            magnitudes = np.tile(magnitudes, (len(parameters),1, self.n_dims))
-            method = 'single_event'
-        lkhs_init, mags_init, pars_init, _ = \
-            self.estimate_single_event(magnitudes, parameters, [0,1], [], 1)
+            magnitudes = np.tile(magnitudes, (len(parameters),1,1))
+            if fix_mags:
+                maximization = False
+                mags_to_fix = [0]
+                ls = '-'
+            else:
+                maximization = True
+                mags_to_fix = []
+                ls = '.'
+        if fix_pars:
+            pars_to_fix = [0,1]
+        else: 
+            pars_to_fix = []
+            ls = 'o'
+        lkhs_init, mags_init, pars_init, times_init = self.estimate_single_event(magnitudes, parameters, pars_to_fix, mags_to_fix, maximization, cpus, tolerance=tolerance,min_iteration=min_iteration)
+        
         if verbose:
-            _, ax = plt.subplots(figsize=figsize, dpi=300)
-            ax.plot(pars_init[:,0,1]*self.shape, lkhs_init, '-', color='k')
-        if method == 'derivative':
-            deriv = np.gradient(lkhs_init)
-            event_idx = np.where(np.diff(np.sign(deriv)) < 0)[0]
-            n_events = len(event_idx)
-            cycol = cycle(colors)
-            colors = [next(cycol) for x in range(n_events)]
-            pars = np.zeros((len(event_idx)+1, 2), dtype=np.float64)
-            pars[:len(event_idx), :] = pars_init[:, 0, :][event_idx, :]
-            pars[len(event_idx),:] = np.array([self.shape, mean_d/self.shape])#last stage defined as rt
-            mags = mags_init[:, :, :][event_idx]
-            lkhs = lkhs_init[event_idx]
-            if verbose:
-                for event in range(len(event_idx)):
-                    ax.plot(np.array(pars)[event,1]*self.shape, lkhs[event], 'o', color=colors[event], label='Likelihood of Transition event %s'%(event+1))
-                plt.ylabel('Log-likelihood')
-                plt.xlabel('Sample number')
-                plt.legend()
-                plt.show()
-                if plot_deriv:
-                    _, ax = plt.subplots(figsize=figsize, dpi=300)
-                    plt.plot(pars_init[:,0,1]*self.shape, np.gradient(lkhs_init), '-', color='k')
-                    plt.hlines(0, 0, mean_d)
-                    plt.show()
-            
-        elif method == 'estimation':
-            if n_events is None:
-                n_events = self.compute_max_events()
-            lkhs_sp, mags_sp, pars_sp, eventprobs_sp = \
-                self.estimate_single_event(np.zeros((len(parameters),1,self.n_dims), dtype=np.float64), \
-                parameters, [], [], 1)
-            lkhs_sp_sorting = lkhs_sp.copy()
-            mags_sp_sorting = mags_sp.copy()
-            pars_sp_sorting = pars_sp.copy()
-            group_color = np.empty(len(lkhs_sp),dtype=str)
-            max_lkhs = []
-            for event in range(n_events):
-                if not np.isnan(lkhs_sp_sorting).all():#Avoids problem if n_events > actual events
-                    max_lkh = np.where(lkhs_sp_sorting == np.nanmax(lkhs_sp_sorting))[0][0]
-                    max_lkhs.append(max_lkh)
-                    gamma_max = pars_sp[max_lkh,0,1] 
-                    neighbors = np.where(abs(pars_sp[:,0,1]-gamma_max) <= (self.event_width_samples/2)/self.shape)[0]
-                    group = np.concatenate([[max_lkh], neighbors])
-                    if verbose:
-                        ax.plot(np.array(pars_sp)[group,0,1]*self.shape, lkhs_sp_sorting[group], 'o', color=colors[event])
-                    lkhs_sp_sorting[group] = np.nan
-                    pars_sp_sorting[group, :, :] = np.nan
-
-            if np.isnan(lkhs_sp_sorting).all() and init_n_events != None and verbose:
-                print(f'The number of requested events exceeds the number of convergence points found in the parameter space, events {event} to {n_events} were not found') 
-
-            if not np.isnan(lkhs_sp_sorting).all() and verbose:#plot remaining points if all where not handled before
-                ax.plot(pars_sp_sorting[:,0,1]*self.shape, lkhs_sp_sorting, 'o', color='gray', label='Not attributed')
-                ax.legend()
-            if verbose: 
-                ax.set_xlabel('sample #')
-                ax.set_ylabel('Loglikelihood')
-                plt.show()
-            pars = np.tile(np.nan, (n_events+1, 2))
-            pars[:len(max_lkhs), :] = pars_sp[max_lkhs, 0, :]
-            order = np.argsort(pars[:len(max_lkhs),1])#sorted index based on first stage duration
-            pars[:len(max_lkhs), :] = pars[order, :]
-            mags = mags_sp[max_lkhs][order]
-            max_lkhs = np.array(max_lkhs)[order]
-            pars[len(max_lkhs),:] = np.array([self.shape, mean_d/self.shape])#last stage defined as rt
-            lkhs = np.repeat(np.nan, n_events)
-            lkhs[:len(max_lkhs)] = lkhs_sp[max_lkhs]
-        elif method is None:
+            if ax is None:
+                 _, ax = plt.subplots(figsize=figsize, dpi=100)
+            ax.plot(pars_init[:,0,1]*self.shape, lkhs_init, ls)
+        plt.ylabel('Log-likelihood')
+        plt.xlabel('Sample number')
+        if show:
+            plt.show()        
+        if method is None:
             #pars, mags, lkhs = pars_init, mags_init, lkhs_init
-            plt.ylabel('Log-likelihood')
-            plt.xlabel('Sample number')
-            plt.show()
+            return ax
         else:
-            return pars, mags[:, 0, :], lkhs
-
-    def estimate_single_event(self, magnitudes, parameters, parameters_to_fix, magnitudes_to_fix, threshold):
-        if self.cpus >1:
+            return lkhs_init, mags_init, times_init
+        
+    def estimate_single_event(self, magnitudes, parameters, parameters_to_fix, magnitudes_to_fix, maximization, cpus, max_iteration=1e2, tolerance=1e-4,min_iteration=1):
+        filterwarnings('ignore', 'Convergence failed, estimation hitted the maximum ', )#will be the case but for a subset only hence ignore
+        if cpus is None:
+            cpus = self.cpus
+        if cpus > 1:
             if np.shape(magnitudes) == 2:
                 magnitudes = np.tile(magnitudes, (len(parameters), 1, 1))
             with mp.Pool(processes=self.cpus) as pool:
                 estimates = pool.starmap(self.EM, 
                     zip(itertools.repeat(1), magnitudes, parameters, 
-                        itertools.repeat(threshold), itertools.repeat(magnitudes_to_fix), 
-                        itertools.repeat(parameters_to_fix)))
+                        itertools.repeat(maximization), itertools.repeat(magnitudes_to_fix), 
+                        itertools.repeat(parameters_to_fix), itertools.repeat(max_iteration),
+                        itertools.repeat(tolerance), itertools.repeat(min_iteration)))
         else:
             estimates = []
             for pars, mags in zip(parameters, magnitudes):
-                estimates.append(self.EM(1, mags, pars, threshold, magnitudes_to_fix, parameters_to_fix))
+                estimates.append(self.EM(1, mags, pars, maximization, magnitudes_to_fix, parameters_to_fix, max_iteration, tolerance, min_iteration=min_iteration))
         lkhs_sp = np.array([x[0] for x in estimates])
         mags_sp = np.array([x[1] for x in estimates])
         pars_sp = np.array([x[2] for x in estimates])
-        eventprobs_sp = np.array([x[3] for x in estimates])
-        return lkhs_sp, mags_sp, pars_sp, eventprobs_sp
+
+        #take max prob times from eventprobs, to reduce memory usage
+        times_sp = np.array([np.argmax(np.squeeze(x[3]),axis=0) for x in estimates])
+
+        resetwarnings()
+        return lkhs_sp, mags_sp, pars_sp, times_sp
     
-    def fit(self, step=1, verbose=True, figsize=(12,3), end=None, threshold=1, trace=False):
+    def fit(self, step=1, verbose=True, end=None, trace=False, fix_iter=False, max_iterations=1e3, tolerance=1e-3, grid_points=1, cpus=None, diagnostic=False, min_iteration=1, decimate=None):
         '''
+        Cumulative fit method.
+        step = size of steps across samples
+        end = max explored duration
+        threshold = 
         '''
+        if cpus is None:
+            cpus = self.cpus
         if end is None:
             end = self.mean_d
-        n_points = int(end//step)
-        if threshold is None:
-            means = np.array([np.mean(self.events[np.random.choice(range(len(self.events)), self.n_trials),:], axis=0) for x in range(1000)])
-            threshold = np.abs(np.max(np.percentile(means, [0.01, 99.99], axis=0)))
-        end = step*(n_points)#Rounding up to step size  
-        lkh = -np.inf
-        pars = np.zeros((n_points-1,2))
-        pars[:,0] = self.shape
-        pars[0,1] = 0.5#initialize with one event
-        mags = np.zeros((n_points-1, self.n_dims))
-        pbar = tqdm(total = end)
+        if verbose and decimate is not None:#Just for printing the info
+             self.gen_mags(1, decimate=decimate, verbose=True)
+        max_event_n = self.compute_max_events()
+        n_points = int(np.rint(end)//step)
+        if diagnostic:
+            cycol = cycle(default_colors)
+        pbar = tqdm(total = int(np.rint(end)))#progress bar
         n_events, j, time = 0,1,0
-        last_stage = end
         if trace:
             all_pars, all_mags, all_mags_prop, all_pars_prop, all_diffs = [],[],[],[],[]
-        pars_accepted, mags_accepted = pars.copy(), mags.copy()
-        pars_prop = pars_accepted[:n_events+2].copy()#cumulative
-        pars_prop[n_events,1] = step*j/self.shape
-        last_stage = end/self.shape - np.sum(pars_prop[:n_events+1,1])
-        pars_prop[n_events+1,1] = last_stage
-        while last_stage*self.shape > self.location+step:
-            prev_n_events, prev_lkh, prev_time = n_events, lkh, time
-            mags_prop = mags[:n_events+1].copy()#cumulative
-            lkh, mags[:n_events+1], pars[:n_events+2], _ = \
-                self.EM(n_events+1, mags_prop, pars_prop.copy(), 1, [], [])
-            signif = True# np.all(np.any(np.abs(mags[:n_events+1]) > threshold, axis=1))
-            if n_events > 0:
-                diffs = np.all(np.any(np.abs(np.diff(mags[:n_events+1], axis=0)) > threshold, axis=1))
+        #Init pars
+        pars = np.zeros((int(end),2))
+        pars[:,0] = self.shape #parameters during estimation, shape x scale
+        pars_prop = pars[:n_events+2].copy()
+        pars_prop[0,1] = 1/self.shape#initialize scale
+        pars_prop[n_events+1,1] = last_stage = (end-1)/self.shape 
+        pars_accepted = pars.copy()
+        #Init mags
+        mags = np.zeros((int(end), self.n_dims)) #mags during estimation
+        mags_accepted = mags.copy()
+        i = 0
+        while last_stage*self.shape > self.location and n_events+1 < max_event_n:
+            prev_time = time
+            if fix_iter:
+                to_fix = [range(n_events)]
+            else:
+                to_fix = []
+            #Generate a grid of magnitudes as proposition 
+            if decimate is None:
+                mags_props = self.gen_mags(n_events+1, n_samples=grid_points, verbose=False)
             else:
-                diffs = True
-            if signif and diffs:
+                mags_props = self.gen_mags(n_events+1, decimate=decimate, verbose=False)
+            #replave eventual event already found
+            mags_props[:,:n_events,:] = np.tile(mags_accepted[:n_events,:], (len(mags_props), 1, 1))
+            #estimate all grid_points models while fixing previous found events
+            solutions = self.fit_single(n_events+1, mags_props, pars_prop, to_fix, to_fix,\
+                            return_max=False, verbose=False, cpus=cpus, min_iteration=min_iteration, tolerance=tolerance)
+            if diagnostic:#Diagnostic plot
+                plt.plot(solutions.traces.T, alpha=.3, c='k')
+            #Exclude non-converged models (negative EM LL curve)
+            solutions = utils.filter_non_converged(solutions)
+            if len(solutions.iteration) > 0:#Success
+
+                ##Average among the converged solutions and store as future starting points
+                # mags[:n_events+1], pars[:n_events+2] = solutions.magnitudes.mean('iteration').values, solutions.parameters.mean('iteration').values
+                # #OR take the nearest converged solution
+                nearest_solution = solutions.sel(iteration=solutions.parameters.sel(parameter="scale", \
+                    stage=n_events).argmin('iteration').values)
+                if diagnostic:#Diagnostic plot
+                    color = next(cycol)
+                    plt.plot(solutions.traces.T, c=color)
+                    plt.plot(nearest_solution.traces.T, c='k', label=f'Iteration {i}')
+                mags[:n_events+1], pars[:n_events+2] = nearest_solution.magnitudes.values,\
+                    nearest_solution.parameters.values
+                pars[n_events+1,1] -= 1
+                recalibrated = self.fit_single(n_events+1, mags[:n_events+1], pars[:n_events+2], [], [],\
+                            return_max=False, verbose=False, cpus=cpus, min_iteration=min_iteration, tolerance=tolerance)
                 n_events += 1
-                pars_accepted = pars[:n_events+2].copy()
-                mags_accepted = mags[:n_events+2].copy()
-                mags_accepted[n_events] =  np.zeros(self.n_dims)
+                pars_accepted[:n_events+1] = recalibrated.parameters.values#pars[:n_events+1].copy()###
+                mags_accepted[:n_events] = recalibrated.magnitudes.values#mags[:n_events].copy()###
                 j = 0
                 if verbose:
-                    print(f'Transition event {n_events} found around sample {int(np.round(np.sum(pars_accepted[:n_events,:].prod(axis=1))))}')#: Transition event samples = {np.round(pars[:n_events].prod(axis=1).cumsum())+self.location*np.arange(n_events)}')
-            if trace:
-                all_mags_prop.append(mags_prop.copy())
-                all_pars_prop.append(pars_prop.copy())
-                all_mags.append(mags_accepted[:n_events].copy())
-                all_pars.append(pars_accepted[:n_events+1].copy())
-                all_diffs.append(np.abs(np.diff(mags[:n_events+1], axis=0)))
+                    print(f'Transition event {n_events} found around sample {int(np.round(np.sum(pars_accepted[:n_events,:].prod(axis=1))))}')
+                if trace:#keep trace of algo
+                    all_mags_prop.append(mags[:n_events].copy())
+                    all_pars_prop.append(pars[:n_events+1].copy())
+                    all_mags.append(mags_accepted[:n_events].copy())
+                    all_pars.append(pars_accepted[:n_events+1].copy())
+                    all_diffs.append(np.abs(np.diff(mags[:n_events+1], axis=0)))
+
             j += 1
-            pars_prop = pars_accepted[:n_events+2].copy()
+            #New parameter proposition
+            pars_prop = pars[:n_events+2].copy()
             pars_prop[n_events,1] = step*j/self.shape
             last_stage = end/self.shape - np.sum(pars_prop[:n_events+1,1])
             pars_prop[n_events+1,1] = last_stage
-            time = np.sum(pars_prop[:n_events,1])*self.shape + \
-                self.location*n_events + step*j/self.shape
-            try:
-                pbar.update(int(np.round(time-prev_time+1)))
-            except:
-                pbar.update(1)
-        # pbar.update(int(np.round(end-prev_time)+self.location+step))
+            time = np.sum(pars_prop[:n_events+1,1])*self.shape 
+            pbar.update(int(np.round(time-prev_time)))
+            i += 1
+        pbar.update(int(np.round(np.rint(end))-np.rint(time)))
+        if diagnostic:
+            plt.ylabel('Log-likelihood')
+            plt.xlabel('EM iteration')
+            plt.legend()
+            plt.show()
         mags = mags_accepted[:n_events, :]
         pars = pars_accepted[:n_events+1, :]
+        # pars[-1,1] += 1#corrects for the absence of a following one
         if n_events > 1: 
             fit = self.fit_single(n_events, parameters=pars, magnitudes=mags, verbose=verbose)
         else:
             warn('Failed to find more than two stages, returning 2 stage model with default starting values')
-            fit = self.fit_single(n_events)
+            fit = self.fit_single(n_events, verbose=verbose)
         if trace:
             all_pars_aligned = np.tile(np.nan, (len(all_pars)+1, np.max([len(x) for x in all_pars]), 2))
             all_pars_prop_aligned = np.tile(np.nan, (len(all_pars_prop)+1, np.max([len(x) for x in all_pars_prop]), 2))
             all_mags_aligned = np.tile(np.nan, (len(all_mags)+1, np.max([len(x) for x in all_mags]), self.n_dims))
             all_mags_prop_aligned = np.tile(np.nan, (len(all_mags_prop)+1, np.max([len(x) for x in all_mags_prop]), self.n_dims))
             all_diffs_aligned = np.tile(np.nan, (len(all_diffs)+1, np.max([len(x) for x in all_diffs]), self.n_dims))
             for iteration, _i in enumerate(zip(all_pars, all_mags, all_mags_prop, all_pars_prop, all_diffs)):
@@ -978,106 +1126,7 @@
                                          all_mags_prop_aligned),
                                 'difference_magnitudes':(('iteration','diffs', 'component'), 
                                          all_diffs_aligned)})
             return fit, traces
         else:
             return fit
     
-    def _bwd_fit(self, step=1, verbose=True, figsize=(12,3), end=None, threshold=None, bwd=True):
-        '''
-        '''
-        if threshold is None:
-            threshold = .05*self.n_dims
-        if end is None:
-            end = int(self.mean_d)
-        n_points = int(end//step)
-        lkh = np.repeat(-np.inf, n_points*3)
-        pars, mags = np.zeros((n_points-1,2)),np.zeros((n_points-1, self.n_dims))
-        new_pars, new_mags = pars.copy(), mags.copy()
-        pbar = tqdm(total = n_points-1)
-        n_events, i,j = 0,1,0
-        event_width = self.event_width_samples / self.shape
-        all_diffs = []
-        while pars[-n_events:].prod(axis=1).sum() < self.mean_d:
-            if bwd:
-                index = range(-n_events-2,0)
-            else:
-                index = range(0,n_events+2)[::-1]
-            if j == 0:
-                print(np.round(pars[index[1:]].prod(axis=1).sum()))
-                next_pars = self._grid_search(2, verbose=False, start_time=(np.round(pars[index[:n_events]].prod(axis=1).sum())), step=step, end_time=end)#next steps in parameter space
-                if bwd:
-                    next_pars = next_pars[:,::-1,:]
-                    
-                next_mags = np.zeros(self.n_dims)#reinitialisze mags
-            if j < len(next_pars):
-                pars_prop = np.concatenate([pars[index[2:]], next_pars[j]])
-                mags_prop = np.concatenate([mags[index[2:]], [next_mags]])
-                print(mags_prop)
-                print(pars_prop)
-                # next_pars[j, 1, 1] = end/self.shape-np.sum(pars_prop[:n_events+1, 1])
-                lkh[i], new_mags[index[1:],:], new_pars[index,:], _ = \
-                    self.EM(n_events+1, mags_prop.copy(), pars_prop.copy(), 1, [], [])
-                print(new_mags[index[1:],:])
-                print(new_pars[index,:])
-
-                diffs = np.sum(np.diff(new_mags[index[1:]],axis=0, prepend=0)**2,axis=1)
-                all_diffs.append(diffs[-1])
-                print(diffs)
-                # print(f'Times = {np.round(pars[:n_events].prod(axis=1).cumsum())}')
-                if (diffs > threshold).all() and np.all(new_mags[index[1:]][-1]>0):#valid iteration
-                    j = 0
-                    n_events += 1
-                    pars[index], mags[index] = new_pars[index], new_mags[index]
-                    if verbose:
-                        print(f'Transition event {n_events} found around time {np.round(np.sum(pars[index[1:]].prod(axis=1)))} (step {i})')
-                    print(f'New pars : {pars[index[0]]}')
-                    print(int((pars[-n_events,1] - np.sum(pars_prop[index[1:],1]))*self.shape))
-                    pbar.update(int((np.sum(pars[-n_events:,1]) - np.sum(pars_prop[-n_events:,1]))*self.shape))
-                else:
-                    pbar.update(1)
-                    j += 1
-                i += 1
-            else:
-                break
-        all_diffs = np.array(all_diffs)
-        plt.hist(all_diffs, bins=40)
-        plt.xlim(0, threshold+threshold/2)
-        plt.show()
-        plt.plot(all_diffs)
-        plt.show()
-        mags = mags[index[2:], :]
-        pars = pars[index[1:], :]
-        pars[-1, :] = np.concatenate([[self.shape], [self.mean_d/self.shape-np.sum(pars[:-1, 1])]])
-        # if pars[-1, 1] <= 0:
-        #     print(True)
-        #     pars[-1, 1] = .5
-        if verbose:
-            _, ax = plt.subplots(figsize=figsize, dpi=300)
-            ax.plot(lkh, '-', color='k')
-            ax.set_ylabel('Log-likelihood')
-            ax.set_xlabel('Sample number')
-            plt.show()
-        print(mags)
-        print(pars)
-        fit = self.fit_single(len(pars)-1, parameters=pars, magnitudes=mags)
-        return fit, lkh    
-    
-    def event_gain_plot(self, lkh, pars, mags, colors=default_colors, figsize=(12,3)):
-        
-        from itertools import cycle
-        n_events = len(mags)
-        _, ax = plt.subplots(figsize=figsize, dpi=300)
-        cycol = cycle(colors)
-        colors = [next(cycol) for x in range(n_events)]
-        parameters = self._grid_search(2, verbose=True)
-        for event in range(n_events):
-            event_lkh = np.zeros(len(parameters))
-            iteration = 0
-            print(mags[event,:])
-            for pars_event in parameters:
-                event_lkh[iteration], _, _, _ = \
-                    self.EM(1,  np.array([mags[event,:]]), pars_event,1, [0], [0,1])
-                iteration += 1
-            ax.plot(parameters[:,0,1], event_lkh, color=colors[event])
-        plt.show()
-
```

### Comparing `hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/resample.py` & `hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/resample.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 import multiprocessing as mp
 import warnings
 from warnings import warn, filterwarnings
 from hsmm_mvpy.models import hmp
 from hsmm_mvpy.utils import transform_data, stack_data, save_eventprobs
 from hsmm_mvpy.visu import plot_topo_timecourse
 
+try:
+    __IPYTHON__
+    from tqdm.notebook import tqdm
+except NameError:
+    import tqdm.tqdm
+
 def _gen_idx(data, dim, iterations=1):
     orig_index = data[dim].values
     indexes = np.array([np.random.choice(orig_index, size=len(orig_index), replace=True) for x in range(iterations)])
     sort_idx = orig_index.argsort()
     corresponding_indexes = sort_idx[np.searchsorted(orig_index,indexes[0],sorter = sort_idx)]
     return  indexes[0]#corresponding_indexes,
 
@@ -25,23 +31,30 @@
             raise ValueError('Cannot stack more than two dimensions')
         else: dim = dim[0]
     named_index = []
     for iteration in range(n_iterations):
         named_index.append(_gen_idx(data, dim))
     return named_index, data, dim, original_dim_order_data
 
-def _bootstrapped_run(data, dim, indexes, order, init, positions, sfreq, n_iter, threshold, summarize=True, verbose=True, plots=True, cpus=1,
+def _bootstrapped_run(data, dim, indexes, order, init, positions, sfreq, n_iter, tolerance, decimate, summarize, verbose, plots=True, cpus=1,
                       trace=False, path='./'):
     resampled_data = data.loc[{dim:list(indexes)}].unstack().transpose(*order)
+    if '_x_' in dim:
+        dim = dim.split('_x_')
+    if isinstance(dim, list):
+        resampled_data = resampled_data.assign_coords({dim[0]: np.arange(len(resampled_data[dim[0]]))})#Removes indices to avoid duplicates
+        resampled_data = resampled_data.assign_coords({dim[1]: np.arange(len(resampled_data[dim[1]]))})
+    else:
+        resampled_data = resampled_data.assign_coords({dim: np.arange(len(resampled_data[dim]))})
     if 'channels' in resampled_data.dims:
         hmp_data_boot = transform_data(resampled_data, n_comp=init.n_dims)
     else:
         hmp_data_boot = resampled_data
-    init_boot = hmp(hmp_data_boot, sfreq=sfreq, event_width=init.event_width, cpus=init.cpus)
-    estimates_boot = init_boot.fit(verbose=verbose, threshold=threshold)
+    init_boot = hmp(hmp_data_boot, sfreq=sfreq, event_width=init.event_width, cpus=1)
+    estimates_boot = init_boot.fit(verbose=verbose, tolerance=tolerance, decimate=decimate)
     if trace:
         save_eventprobs(estimates_boot.eventprobs, path+str(n_iter)+'.nc')
     if summarize:
         times = init_boot.compute_times(init_boot, estimates_boot, mean=True)
         channels = init_boot.compute_topologies(resampled_data, estimates_boot, 
                                                 init_boot.event_width_samples, mean=True)
         boot_results = xr.combine_by_coords([estimates_boot.magnitudes.to_dataset(name='magnitudes'),
@@ -50,32 +63,35 @@
                                          channels.to_dataset(name='channels_activity')])
     else:
         boot_results = xr.combine_by_coords([estimates_boot.magnitudes.to_dataset(name='magnitudes'),
                                          estimates_boot.parameters.to_dataset(name='parameters'), 
                                          estimates_boot.eventprobs.to_dataset(name='eventprobs')])
     return boot_results
 
-def bootstrapping(data, dim, n_iterations, init, positions, sfreq, threshold, summarize=True, verbose=True,
+def bootstrapping(data, dim, n_iterations, init, positions, sfreq, tolerance=1e-4,
+                  decimate=None, summarize=True, verbose=False,
                   plots=True, cpus=1, trace=False, path='./'):
-    import multiprocessing
     import itertools
     if 'channels' in data.dims:
         data_type = 'raw'
     else:
         data_type = 'transformed'
     if verbose:
         print(f'Bootstrapping {data_type} on {n_iterations} iterations')
     data_views, data, dim, order = _gen_dataset(data, dim, n_iterations)
-    with multiprocessing.Pool(processes=cpus) as pool:
-        boot = pool.starmap(_bootstrapped_run, 
-            zip(itertools.repeat(data), itertools.repeat(dim), data_views, itertools.repeat(order), 
+    
+    #calculate estimates, returns lkhs, mags, times
+    inputs = zip(itertools.repeat(data), itertools.repeat(dim), data_views, itertools.repeat(order), 
                 itertools.repeat(init), 
                 itertools.repeat(positions), itertools.repeat(init.sfreq), np.arange(n_iterations),
-                itertools.repeat(threshold), itertools.repeat(summarize), itertools.repeat(verbose),
-                itertools.repeat(plots),itertools.repeat(cpus), itertools.repeat(trace), itertools.repeat(path)))
+                itertools.repeat(tolerance), itertools.repeat(decimate), itertools.repeat(summarize), itertools.repeat(verbose),
+                itertools.repeat(plots),itertools.repeat(cpus), itertools.repeat(trace), itertools.repeat(path))
+    with mp.Pool(processes=cpus) as pool:
+            boot = list(tqdm(pool.imap(_boot_star, inputs), total=n_iterations))
+        
     boot = xr.concat(boot, dim='iteration')
     # if plots:
     #     plot_topo_timecourse(boot.channels, boot.event_times, positions, init_boot, title='iteration = '+str(n_iter), skip_electodes_computation=True)
     return boot
 
 def percent_event_occurence(iterations,  model_to_compare=None, count=False):
     from scipy.spatial import distance_matrix
@@ -85,23 +101,27 @@
         model_to_compare = iterations.sel(iteration=max_n_bump_model_index)
     else:
         max_mags = model_to_compare.magnitudes
     all_diffs = []
     all_n = np.zeros(len(iterations.iteration))
     for iteration in iterations.iteration:
         n_events_iter = int(np.sum(np.isfinite(iterations.sel(iteration=iteration).magnitudes.values[:,0])))
-        # if iteration != max_n_bump_model_index:
-        diffs = distance_matrix(iterations.sel(iteration=iteration).magnitudes.squeeze(),
-                    max_mags)
-        index_event = diffs.argmin(axis=1)
-        index_event[n_events_iter:] = 9999
-        all_diffs.append(index_event)
+        if iteration != max_n_bump_model_index:
+            diffs = distance_matrix(iterations.sel(iteration=iteration).magnitudes.squeeze(),
+                        max_mags)
+            index_event = diffs.argmin(axis=1)
+            index_event[n_events_iter:] = 9999
+
+            all_diffs.append(index_event)
         all_n[iteration] = n_events_iter
     labels, counts = np.unique(all_diffs, return_counts=True)
     n_event_labels, n_event_count = np.unique(all_n, return_counts=True)
-    if count:
+    n_events_per_iter = [int(np.sum(np.isfinite(iterations.sel(iteration=i).magnitudes.values[:,0]))) for i in iterations.iteration]
+    if np.any(np.diff(n_events_per_iter) != 0):
         labels, counts = labels[:-1], counts[:-1]
-    else:
-        labels, counts = labels[:-1], counts[:-1]/iterations.iteration.max().values
+    if not count:
+        labels, counts = labels, counts/iterations.iteration.max().values
         n_event_count = n_event_count/iterations.iteration.max().values
     return model_to_compare, labels, counts, n_event_count, n_event_labels
 
+def _boot_star(args): #for tqdm usage
+    return _bootstrapped_run(*args)
```

### Comparing `hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/simulations.py` & `hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/simulations.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,45 +30,53 @@
     data_path = sample.data_path()
     subjects_dir = op.join(data_path, 'subjects')
     evoked_fname = op.join(data_path, 'MEG', 'sample', 'sample_audvis-ave.fif')
     info = mne.io.read_info(evoked_fname, verbose=False)
     return info['sfreq']
 
 def simulation_positions():
-    from mne import channels
     data_path = sample.data_path()
     subjects_dir = op.join(data_path, 'subjects')
     subject = 'sample'
     evoked_fname = op.join(data_path, 'MEG', subject, 'sample_audvis-ave.fif')
     info = mne.io.read_info(evoked_fname, verbose=False)
-    positions = np.delete(channels.layout._find_topomap_coords(info, 'eeg'),52,axis=0)#inferring channel location using MNE    
+    positions = np.delete(mne.channels.layout._find_topomap_coords(info, 'eeg'),52,axis=0)#inferring channel location using MNE    
     return positions
 
-def bump_shape(bump_width, bump_width_samples, steps):
+def simulation_info():
+    data_path = sample.data_path()
+    subjects_dir = op.join(data_path, 'subjects')
+    subject = 'sample'
+    evoked_fname = op.join(data_path, 'MEG', subject, 'sample_audvis-ave.fif')
+    info = mne.io.read_info(evoked_fname, verbose=False)
+    
+    return info
+
+def event_shape(event_width, event_width_samples, steps):
     '''
-    Computes the template of a half-sine (bump) with given frequency f and sampling frequency
+    Computes the template of a half-sine (event) with given frequency f and sampling frequency
     '''
-    bump_idx = np.arange(bump_width_samples)*steps+steps/2
-    bump_frequency = 1000/(bump_width*2)#gives bump frequency given that bumps are defined as half-sines
-    template = np.sin(2*np.pi*bump_idx/1000*bump_frequency)#bump morph based on a half sine with given bump width and sampling frequency
+    event_idx = np.arange(event_width_samples)*steps+steps/2
+    event_frequency = 1000/(event_width*2)#gives event frequency given that events are defined as half-sines
+    template = np.sin(2*np.pi*event_idx/1000*event_frequency)#event morph based on a half sine with given event width and sampling frequency
     template = template/np.sum(template**2)#Weight normalized
     return template
 
 
 def simulate(sources, n_trials, n_jobs, file, data_type='eeg', n_subj=1, path='./', overwrite=False, verbose=False, noise=True, times=None, location=1, seed=None): 
     '''
     Simulates n_trials of EEG and/or MEG using MNE's tools based on the specified sources
     
     Parameters
     ----------
     sources : list
         2D or 3D list with dimensions (n_subjects *) sources * source_parameters
         Source parameters should contain :
         - the name of the source (see the output of available_source())
-        - the duration of the bump (in frequency, usually 10Hz)
+        - the duration of the event (in frequency, usually 10Hz)
         - the amplitude or strength of the signal from the source, expressed in volt (e.g. 1e-8 V)
         - the duration of the preceding stage as a scipy.stats distribution (e.g. scipy.stats.gamma(a, scale))
     n_trials: int
         Number of trials
     n_jobs: int
         Number of jobs to use with MNE's function (multithreading)
     file: str
@@ -89,15 +97,15 @@
         Deterministic simulation of event transitions times. Format is n_sources X n_trials
     location: float
         value in ms to add after a simulated event and before another one
     
     Returns
     -------
     generating_events: ndarray
-        Times of the simulated bumps used to test for accurate recovery compared to estimation
+        Times of the simulated events used to test for accurate recovery compared to estimation
     files: list
         list of file names (file + number of subject)
     '''
     if seed is not None:
         random_state = np.random.RandomState(seed)
     else:
         random_state = None
@@ -181,16 +189,16 @@
             for source in sources_subj:
                 selected_label = mne.read_labels_from_annot(
                     subject, regexp=source[0], subjects_dir=subjects_dir, verbose=verbose)[0]
                 label = mne.label.select_sources(subject, selected_label, subjects_dir=subjects_dir, location=0, grow_outside=False, random_state=random_state)
                 #last two parameters ensure sources that are different enough
                 # Define the time course of the activity for each source of the region to
                 # activate
-                bump_duration = int(((1/source[1])/2)*info['sfreq'])
-                source_time_series = bump_shape(((1000/source[1])/2),bump_duration,1000/info['sfreq'])*source[2]
+                event_duration = int(((1/source[1])/2)*info['sfreq'])
+                source_time_series = event_shape(((1000/source[1])/2),event_duration,1000/info['sfreq'])*source[2]
 
                 #adding source event
                 events = events.copy()
                 if times is None:
                     rand_i = np.round(source[-1].rvs(size=n_trials, random_state=random_state)/(tstep*1000),decimals=0)
                 else:
                     rand_i = times[:,trigger-2]
@@ -230,7 +238,61 @@
             files.append(files_subj)
             print(f'{subj_file} simulated')
     if n_subj == 1:
         return files[0]
     else:
         return files
     
+
+def demo(cpus, n_events, seed=667):#12
+    
+    ## Imports and code specific to the simulation (see tutorial 3 and 4 for real data)
+    from scipy.stats import gamma
+    import matplotlib.pyplot as plt 
+    from hsmm_mvpy.utils import read_mne_data
+    
+    random_gen =  np.random.default_rng(seed=seed)
+
+    ## Parameters for the simulations
+    frequency, amplitude = 10., .3e-6 #Frequency of the transition event and its amplitude in Volt
+    shape = 2#shape of the gamma distribution
+
+    #Storing electrode position, specific to the simulations
+    positions = simulation_info()#Electrode position
+    sfreq = simulation_sfreq()#sampling freqency of the simulated data
+    resample_freq = sfreq/np.round(sfreq / 100).astype(int)#Resampling at 100Hz to make processing faster and less demanding
+    all_source_names = available_sources()#all brain sources you can play with
+    n_trials = 50 #Number of trials to simulate
+    
+    # Randomly specify the transition events
+    name_sources = random_gen.choice(all_source_names,n_events+1, replace=False)#randomly pick source without replacement
+
+    times = random_gen.uniform(25,300,n_events+1)/shape#randomly pick average times in millisecond between the events
+
+    sources = []
+    for source in range(len(name_sources)):
+        sources.append([name_sources[source], frequency, amplitude, \
+                          gamma(shape, scale=times[source])])
+
+    file = 'dataset_tutorial2' #Name of the file to save
+
+    #Simulating and recover information on electrode location and true time onset of the simulated events
+    files = simulate(sources, n_trials, cpus,file, overwrite=True, location=25, seed=seed)
+    generating_events = np.load(files[1])
+    number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
+    random_source_times = np.reshape(np.diff(generating_events[:,0], prepend=0),(n_trials,number_of_sources+1))[:,1:]/(sfreq/resample_freq)#By-trial generated event times
+
+    #Reading the necessary info to read the EEG data
+    resp_trigger = int(np.max(np.unique(generating_events[:,2])))#Resp trigger is the last source in each trial
+    event_id = {'stimulus':1}
+    resp_id = {'response':resp_trigger}
+    events = generating_events[(generating_events[:,2] == 1) | (generating_events[:,2] == resp_trigger)]#only retain stimulus and response triggers
+
+    # Reading the data
+    eeg_dat = read_mne_data(files[0], event_id, resp_id, sfreq=resample_freq, events_provided=events, verbose=False)
+    
+    all_other_chans = range(len(positions.ch_names[:-61]))#non-eeg
+    chan_list = list(np.arange(len(positions.ch_names)))
+    chan_list = [e for e in chan_list if e not in all_other_chans]
+    chan_list.pop(52)#Bad elec
+    positions = mne.pick_info(positions, sel=chan_list)
+    return eeg_dat, random_source_times, positions
```

### Comparing `hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/utils.py` & `hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -151,19 +151,23 @@
                 events_stim = np.array([list(x) for x in events if x[2] in event_id.values()])#only stim
             else:
                 if len(np.shape(events_provided)) == 2:
                     events_provided = events_provided[np.newaxis]
                 events = events_provided[y]
 
             data.load_data()
-            data.filter(high_pass, low_pass, fir_design='firwin', verbose=verbose)
 
             if sfreq < data.info['sfreq']:#Downsampling
                 print(f'Downsampling to {sfreq} Hz')
-                data, events = data.resample(sfreq, events=events)
+                decim = np.round( data.info['sfreq'] / sfreq).astype(int)
+                obtained_sfreq = data.info['sfreq'] / decim
+                low_pass = obtained_sfreq / 3.1
+            else: decim = 1
+            data.filter(high_pass, low_pass, fir_design='firwin', verbose=verbose)
+
             combined =  {**event_id, **resp_id}#event_id | resp_id 
             stim = list(event_id.keys())
             
             if verbose:
                 print(f'Creating epochs based on following event ID :{np.unique(events[:,2])}')
 
             offset_after_resp_samples = int(offset_after_resp*sfreq)
@@ -171,15 +175,15 @@
                 metadata_i, meta_events, event_id = mne.epochs.make_metadata(
                     events=events, event_id=combined, tmin=tmin, tmax=tmax,
                     sfreq=data.info["sfreq"], row_events=stim, keep_first=["response"])
                 metadata_i = metadata_i[["event_name","response"]]#only keep event_names and rts
             else:
                 metadata_i = metadata[y]
             epochs = mne.Epochs(data, meta_events, event_id, tmin, tmax, proj=False,
-                    baseline=baseline, preload=True, picks=pick_channels,
+                    baseline=baseline, preload=True, picks=pick_channels, decim=decim,
                     verbose=verbose, detrend=1, on_missing = 'warn', event_repeated='drop',
                     metadata=metadata_i, reject_by_annotation=True, reject=reject_threshold)
             epochs.metadata.rename({'response':'rt'}, axis=1, inplace=True)
             metadata_i = epochs.metadata
         else:
             if '.fif' in participant:
                 epochs = mne.read_epochs(participant, preload=True, verbose=verbose)
@@ -474,41 +478,39 @@
     Returns
     -------
     data : xarray.Dataset
         xarray dataset [samples * channels]
     '''    
     if isinstance(data, (xr.DataArray,xr.Dataset)) and 'component' not in data.dims:
         data = data.rename_dims({'channels':'component'})
-        print(data.participant)
     if "participant" not in data.dims:
         data = data.expand_dims("participant")
     data = data.stack(all_samples=['participant','epochs',"samples"]).dropna(dim="all_samples")
-    return data #xr.Dataset({'data':data, 'durations':durations})
-    #return data, durations
+    return data
 
-def transform_data(data, subjects_variable="participant", apply_standard=True,  apply_zscore=True, method='pca', n_comp=None, return_weights=False):
+def transform_data(data, participants_variable="participant", apply_standard=True,  apply_zscore='participant', method='pca', n_comp=None, return_weights=False):
     '''
     Adapts EEG epoched data (in xarray format) to the expected data format for hmps. 
     First this code can apply standardization of individual variances (if apply_standard=True).
     Second, a spatial PCA on the average variance-covariance matrix is performed (if method='pca', more methods in development)
     Third,stacks the data going from format [participant * epochs * samples * channels] to [samples * channels]
-    Last, performs z-scoring on each epoch and for each principal component (PC)
-    
-    
+    Last, performs z-scoring on each epoch and for each principal component (PC), or for each participant and PC,
+    or across all data for each PC.
+        
     Parameters
     ----------
     data : xarray
         unstacked xarray data from transform_data() or anyother source yielding an xarray with dimensions 
         [participant * epochs * samples * channels] 
-    subjects_variable : str
-        name of the dimension for subjects ID
+    participants_variable : str
+        name of the dimension for participants ID
     apply_standard : bool 
         Whether to apply standardization
-    apply_zscore : bool 
-        Whether to apply z-scoring
+    apply_zscore : str 
+        Whether to apply z-scoring and on what data, either None, 'all', 'participant', 'trial', for zscoring across all data, by participant, or by trial, respectively. If set to true, evaluates to 'trial' for backward compatibility.
     method : str
         Method to apply, for now limited to 'pca'
     n_comp : int
         How many components to select from the PC space, if None plots the scree plot and a prompt requires user
         to specify how many PCs should be retained
 
     Returns
@@ -520,18 +522,26 @@
     pca.explained_variance_ : ndarray
         explained variance for each component
     means : xarray.DataArray
         means of the channels before PCA/zscore
     '''
     if isinstance(data, xr.DataArray):
         raise ValueError('Expected a xarray Dataset with data and event as DataArrays, check the data format')
+    if not apply_zscore in ['all', 'participant', 'trial'] and not isinstance(apply_zscore,bool):
+        raise ValueError('apply_zscore should be either a boolean or one of [\'all\', \'participant\', \'trial\']')
+    sfreq = data.sfreq
+    if apply_zscore == True:
+        apply_zscore = 'trial' #defaults to trial
     if apply_standard:
-        mean_std = data.groupby(subjects_variable).std(dim=...).data.mean()
-        data = data.assign(mean_std=mean_std.data)
-        data = data.groupby(subjects_variable).map(standardize)
+        if 'participant' not in data.dims or len(data.participant) == 1:
+            warn('Requested standardization of between participant variance yet no participant dimension is found in the data or only one participant is present. No standardization is done, set apply_standard to False to avoid this warning.')
+        else:
+            mean_std = data.groupby(participants_variable).std(dim=...).data.mean()
+            data = data.assign(mean_std=mean_std.data)
+            data = data.groupby(participants_variable).map(standardize)
     if method == 'pca':
         from sklearn.decomposition import PCA
         var_cov_matrices = []
         if isinstance(data, xr.Dataset):
             data = data.data
         for i,trial_dat in data.stack(trial=("participant", "epochs")).drop_duplicates('trial').groupby('trial'):
             var_cov_matrices.append(vcov_mat(trial_dat)) #Would be nice not to have a for loop but groupby.map seem to fal
@@ -565,114 +575,123 @@
         pca_data = xr.DataArray(pca_data, dims=("channels","component"), coords=coords)
         means = data.groupby('channels').mean(...)
         data = data @ pca_data
 
     elif method is None:
         data = data.rename({'channels':'component'})
         data['component'] = np.arange(len(data.component ))
-    if apply_zscore:
-        data = data.stack(trial=[subjects_variable,'epochs','component']).groupby('trial').map(zscore).unstack()
+    
+    # zscore either across all data, by participant (preferred), or by trial
+    match apply_zscore:
+        case 'all':
+            data = data.stack(comp=['component']).groupby('comp').map(zscore).unstack()
+        case 'participant':
+            data = data.stack(participant_comp=[participants_variable,'component']).groupby('participant_comp').map(zscore).unstack()
+        case 'trial':
+            data = data.stack(trial=[participants_variable,'epochs','component']).groupby('trial').map(zscore).unstack()
+    data.attrs['components'] = pca_data
+    data.attrs['sfreq'] = sfreq
     if stack_data:
         data = stack_data(data)
     if return_weights:
         return data, pca_data, pca.explained_variance_, means
     else:
         return data
     
 
-def LOOCV(data, subject, n_events, initial_fit, sfreq, event_width=50):
+def LOOCV(data, participant, n_events, initial_fit, sfreq, event_width=50):
     '''
     Performs Leave-one-out cross validation, removes one participant from data, estimate n_events HMP parameters, 
     compute the likelihood of the data from the left out participant with the estimated parameters. The model is fit
     using initial fit as starting points for magnitudes and parameters
     
     
     Parameters
     ----------
     data : xarray.Dataset
         xarray data from transform_data() 
-    subject : str
-        name of the subject to remove
+    participant : str
+        name of the participant to remove
     n_events : int 
         How many events in the model
     initial_fit : xarray.Dataset
         Fit of the model with the same number of events and all participants
     sfreq : float
         Sampling frequency of the data
     event_width : float
         length of the events in milliseconds
     
     Returns
     -------
     likelihood : float
         likelihood computed for the left-out participant
-    subject : str
-        name of the subject to remove
+    participant : str
+        name of the participant to remove
     '''
     # wc 
     from hsmm_mvpy.models import hmp
     #Looping over possible number of events
-    subjects_idx = data.participant.values
+    participants_idx = data.participant.values
     likelihoods_loo = []
-    #Extracting data without left out subject
-    stacked_loo = stack_data(data.sel(participant= subjects_idx[subjects_idx!=subject],drop=False))
+    #Extracting data without left out participant
+    stacked_loo = stack_data(data.sel(participant= participants_idx[participants_idx!=participant],drop=False))
     #Fitting the HMP using previous estimated parameters as initial parameters
     model_loo = hmp(stacked_loo, sfreq=sfreq, event_width=event_width)
     fit = model_loo.fit_single(n_events, initial_fit.magnitudes.dropna('event').values, initial_fit.parameters, 1, verbose=False)
-    #Evaluating likelihood for left out subject
-    #Extracting data of left out subject
-    stacked_left_out = stack_data(data.sel(participant=subject, drop=False))
+    #Evaluating likelihood for left out participant
+    #Extracting data of left out participant
+    stacked_left_out = stack_data(data.sel(participant=participant, drop=False))
     model_left_out = hmp(stacked_left_out, sfreq=sfreq, event_width=event_width)
     likelihood = model_left_out.estim_probs(fit.magnitudes.dropna('event').values, fit.parameters, n_events,True)
-    return likelihood, subject
+    return likelihood, participant
 
-def loocv_estimation(data, subject, sfreq, event_width):
+def loocv_estimation(data, participant, sfreq, event_width):
     '''
     Performs Leave-one-out cross validation, removes one participant from data, estimate n_events HMP parameters, 
     compute the likelihood of the data from the left out participant with the estimated parameters. The model is fit
     using initial fit as starting points for magnitudes and parameters
     
     
     Parameters
     ----------
     data : xarray
         xarray data from transform_data() 
-    subject : str
-        name of the subject to remove
+    participant : str
+        name of the participant to remove
     sfreq : float
         Sampling frequency of the data
     event_width : float
         length of the events in milliseconds
     
     Returns
     -------
     likelihood : float
         likelihood computed for the left-out participant
-    subject : str
-        name of the subject to remove
+    participant : str
+        name of the participant to remove
     '''    
-    print(f'Leaving out participant #{subject}')
+    print(f'Leaving out participant #{participant}')
     from hsmm_mvpy.models import hmp
     #Looping over possible number of events
-    subjects_idx = data.participant.values
+    participants_idx = data.participant.values
     likelihoods_loo = []
-    #Extracting data without left out subject
-    stacked_loo = stack_data(data.sel(participant= subjects_idx[subjects_idx!=subject],drop=False))
+    #Extracting data without left out participant
+    stacked_loo = stack_data(data.sel(participant= participants_idx[participants_idx!=participant],drop=False))
     #Fitting the HMP using previous estimated parameters as initial parameters
     model_loo = hmp(stacked_loo, sfreq=sfreq, event_width=event_width, cpus=1)
     parameters, magnitudes, likelihoods = model_loo.sliding_event(verbose=False)
     estimates = model_loo.iterative_fit(likelihoods=likelihoods, parameters=parameters, magnitudes=magnitudes)
-    #Evaluating likelihood for left out subject
-    #Extracting data of left out subject
-    stacked_left_out = stack_data(data.sel(participant=subject, drop=False))
+    #Evaluating likelihood for left out participant
+    #Extracting data of left out participant
+    stacked_left_out = stack_data(data.sel(participant=participant, drop=False))
     model_left_out = hmp(stacked_left_out, sfreq=sfreq, event_width=event_width, cpus=1)
     n_events = int(estimates.dropna('n_events',how='all').n_events.max())
     for n_event in range(1,n_events+1):
         likelihoods_loo.append( model_left_out.calc_EEG_50h(estimates.sel(n_events=n_event).magnitudes.dropna('event').values, estimates.sel(n_events=n_event).parameters.dropna('stage').values, n_event, True))
-    return likelihoods_loo, subject
+    return likelihoods_loo, participant
 
 def loocv(stacked_data,sfreq, max_event, cpus=1, event_width=50):
     '''
     Performs Leave-one-out cross validation, removes one participant from data, estimate n_events HMP parameters, 
     compute the likelihood of the data from the left out participant with the estimated parameters. The model is fit
     using initial fit as starting points for magnitudes and parameters
     
@@ -860,54 +879,27 @@
         except:
             brp_data[i, :1] = trial_elec
             
         i += 1
 
     return brp_data    
     
-def condition_selection(hmp_data, eeg_data, condition_string, variable='event'):
-    unstacked = hmp_data.unstack().where(eeg_data[variable].str.contains(condition_string),drop=True)
+def condition_selection(hmp_data, epoch_data, condition_string, variable='event'):
+    unstacked = hmp_data.unstack().where(epoch_data[variable].str.contains(condition_string),drop=True)
     stacked = stack_data(unstacked)
     return stacked
 
 def load_data(path):
     return xr.load_dataset(path)
 
     
-def participant_selection(hmp_data, eeg_data, participant):
+def participant_selection(hmp_data, participant):
     unstacked = hmp_data.unstack().sel(participant = participant)
     stacked = stack_data(unstacked)
     return stacked
 
-def bootstrapping(init, hmp_data, general_run, positions, eeg_data, iterations, threshold=1, verbose=True, plots=True, cpus=1):
-    warn('This method is inaccurate and will be removed in future version, see the bootstraping function in the resample module instead', DeprecationWarning, stacklevel=2)
-    from hsmm_mvpy.models import hmp
-    from hsmm_mvpy.visu import plot_topo_timecourse
-    try:
-        import xskillscore as xs#Todo remove from dependency list
-    except:
-        raise ValueError('xskillscore should be installed to run this (deprecated) function')
-    fitted_mags = general_run.magnitudes.values[np.unique(np.where(np.isfinite(general_run.magnitudes))[0]),:]#remove NAs
-    mags_boot_mat = []#np.tile(np.nan, (iterations, init.compute_max_events(), init.n_dims))
-    pars_boot_mat = []#np.tile(np.nan, (iterations, init.compute_max_events()+1, 2))
-
-    for i in range(iterations):
-        bootstapped = xs.resample_iterations(hmp_data.unstack(), iterations=1, dim='epochs')
-        hmp_data_boot = stack_data(bootstapped.squeeze())
-        init_boot = hmp(hmp_data_boot, sfreq=eeg_data.sfreq, event_width=init.event_width, cpus=init.cpus)
-        estimates_boot = init_boot.fit(verbose=verbose, threshold=threshold)
-        mags_boot_mat.append(estimates_boot.magnitudes)
-        pars_boot_mat.append(estimates_boot.parameters)
-        if plots:
-            plot_topo_timecourse(eeg_data, estimates_boot, positions, init_boot)
-
-    all_pars_aligned = np.tile(np.nan, (iterations, np.max([len(x) for x in pars_boot_mat]), 2))
-    all_mags_aligned = np.tile(np.nan, (iterations, np.max([len(x) for x in mags_boot_mat]), init.n_dims))
-    for iteration, _i in enumerate(zip(pars_boot_mat, mags_boot_mat)):
-        all_pars_aligned[iteration, :len(_i[0]), :] = _i[0]
-        all_mags_aligned[iteration, :len(_i[1]), :] = _i[1]
-
-    booted = xr.Dataset({'parameters': (('iteration', 'stage','parameter'), 
-                                 all_pars_aligned),
-                        'magnitudes': (('iteration', 'event','component'), 
-                                 all_mags_aligned)})
-    return booted
+def filter_non_converged(estimates):
+    for iteration in estimates.iteration.values:
+        if np.diff(estimates.sel(iteration=iteration).traces.dropna('em_iteration')[-2:]) < -1e-10:
+            estimates = estimates.drop_sel({'iteration':iteration})
+    estimates["iteration"] = range(len(estimates.iteration))
+    return estimates
```

### Comparing `hsmm_mvpy-0.1.0b7/src/hsmm_mvpy/visu.py` & `hsmm_mvpy-0.1.0b8/src/hsmm_mvpy/visu.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import xarray as xr
 from itertools import cycle
 default_colors =  ['cornflowerblue','indianred','orange','darkblue','darkgreen','gold']
 
+
 def plot_topo_timecourse(channels, estimated, channel_position, init, time_step=1, ydim=None,
                 figsize=None, dpi=100, magnify=1, times_to_display=None, cmap='Spectral_r',
-                ylabels=[], max_time = None, vmin=None, vmax=None, title=False, ax=None, 
-                sensors=False, skip_channels_computation=False):
+                ylabels=[], xlabel = None, max_time = None, vmin=None, vmax=None, title=False, ax=None, 
+                sensors=False, skip_channels_computation=False, contours=6, event_lines='tab:orange',
+                colorbar=True, topo_size_scaling=False):
     '''
     Plotting the event topologies at the average time of the end of the previous stage.
     
     Parameters
     ----------
     channels : ndarray | xr.Dataarray 
         a 2D or 3D matrix of channel activity with channels and event as dimension (+ eventually a varying dimension) OR
@@ -37,104 +39,178 @@
     magnify : float
         How much should the events be enlarged, useful to zoom on topologies, providing any other value than 1 will 
         however change the displayed size of the event
     times_to_display : ndarray
         Times to display (e.g. Reaction time or any other relevant time) in the time unit of the fitted data
     cmap : str
         Colormap of matplotlib
+    xlabel : str
+        label of x-axis, default = None, which give "Time (samples)" or "Time" in case time_step != 1
     ylabels : dict
         dictonary with {label_name : label_values}
     max_time : float
         limit of the x (time) axe
     vmin : float
-        Colormap limits to use (see https://mne.tools/dev/generated/mne.viz.plot_topomap.html)
+        Colormap limits to use (see https://mne.tools/dev/generated/mne.viz.plot_topomap.html). If not explicitly
+        set, uses min across all topos while keeping colormap symmetric.
     vmax : float
-        Colormap limits to use (see https://mne.tools/dev/generated/mne.viz.plot_topomap.html)
+        Colormap limits to use (see https://mne.tools/dev/generated/mne.viz.plot_topomap.html). If not explicitly
+        set, uses max across all topos while keeping colormap symmetric.
     title : str
         title of the plot
     ax : matplotlib.pyplot.ax
         Matplotlib object on which to draw the plot, can be useful if you want to control specific aspects of the plots
         outside of this function
     sensors : bool
         Whether to plot the sensors on the topologies
+    contours : int / array_like
+        The number of contour lines to draw (see https://mne.tools/dev/generated/mne.viz.plot_topomap.html)
+    event_lines : bool / color
+        Whether to plot lines and shading to indicate the moment of the event. If True uses tab:orange, if
+        set as color, uses the color
+    colorbar : bool
+        Whether a colorbar is plotted.
+    topo_size_scaling : bool
+        Whether to scale the size of the topologies with the event size. If True, size of topologies depends
+        on total plotted time interval, if False it is only dependent on magnify.
         
     Returns
     -------
     ax : matplotlib.pyplot.ax
         if ax was specified otherwise returns the plot
     '''
-    
-    from mne.viz import plot_topomap
+
+    from mne.viz import plot_brain_colorbar, plot_topomap
+    from mne.io.meas_info import Info
     from mpl_toolkits.axes_grid1.inset_locator import inset_axes
+    from mpl_toolkits.axes_grid1 import make_axes_locatable
+
     return_ax = True
     if times_to_display is None:
-        times_to_display = init.mean_d*time_step
+        times_to_display = init.mean_d
+    if xlabel is None:
+        if time_step == 1:
+            xlabel = 'Time (in samples)'
+        else:
+            xlabel = 'Time'
+    if event_lines == True:
+        event_color='tab:orange'
+    else:
+        event_color=event_lines
+
+    
     if isinstance(estimated, (xr.DataArray, xr.Dataset)) and 'event' in estimated:
         if ydim is None and 'n_events' in estimated.dims:
             if estimated.n_events.count() > 1:
                 ydim = 'n_events'
         if ydim is not None and not skip_channels_computation:
             channels = init.compute_topologies(channels, estimated, init.event_width_samples, ydim).data
         elif not skip_channels_computation:
             channels = init.compute_topologies(channels, estimated, init.event_width_samples).data
-        channels[channels == 0] = np.nan
         times = init.compute_times(init, estimated, mean=True).data
+        channels[times == 0] = np.nan#removes the empty topologies, e.g. in the case of mutliple varying number of events
+
     else:#assumes times already computed
         times = estimated
     if len(np.shape(channels)) == 2:
         channels = channels[np.newaxis]
     n_iter = np.shape(channels)[0]
     if ax is None:
         if figsize == None:
-            figsize = (12, 1*n_iter)
-        fig, ax = plt.subplots(1, 1, figsize=figsize, dpi=dpi)
+            if n_iter == 1:
+                figsize = (12, .7 * np.max([magnify,1.8])) #make sure they don't get too flat
+            else:
+                figsize = (12, n_iter*.7) #make sure they don't get too flat
+
+        _, ax = plt.subplots(1, 1, figsize=figsize, dpi=dpi)
         return_ax = False
-    event_size = init.event_width_samples*time_step*magnify
-    yoffset =.25*magnify
+    event_size = init.event_width_samples * time_step
+    if topo_size_scaling: #does topo width scale with time interval of plot?
+        topo_size = event_size * magnify
+    else:
+        timescale = (max_time if max_time else (np.max(times_to_display) * time_step * 1.05)) + time_step
+        topo_size = .08 * timescale * magnify #8% of time scale
     axes = []
     if n_iter == 1:
         times = [times]
     times = np.array(times, dtype=object)
+    #fix vmin/vmax across topos, while keeping symmetric
+    if vmax == None: #vmax = absolute max, unless no positive values
+        vmax = np.nanmax(np.abs(channels[:])) if np.nanmax(channels[:]) >= 0 else 0
+    if vmin == None: #vmin = absolute max, unless no negative values
+        vmin = -np.nanmax(np.abs(channels[:])) if np.nanmin(channels[:]) < 0 else 0
+ 
     for iteration in np.arange(n_iter):
         times_iteration = times[iteration]*time_step
+
         channels_ = channels[iteration,:,:]
         n_event = int(sum(np.isfinite(channels_[:,0])))
         channels_ = channels_[:n_event,:]
         for event in np.arange(n_event):
-            axes.append(ax.inset_axes([times_iteration[event],iteration-yoffset,
-                                (event_size),yoffset*2], transform=ax.transData))
+
+            rowheight = 1/n_iter 
+            ylow = iteration * rowheight
+            axes.append(ax.inset_axes([times_iteration[event] + event_size/2 - topo_size / 2, ylow+.1*rowheight,
+                                topo_size, rowheight*.8], transform=ax.get_xaxis_transform())) 
             plot_topomap(channels_[event,:], channel_position, axes=axes[-1], show=False,
-                         cmap=cmap, vlim=(vmin, vmax), sensors=sensors)
+                         cmap=cmap, vlim=(vmin, vmax), sensors=sensors, contours=contours)
+
+            if event_lines:
+                #bottom of row + 5% if n_iter > 1
+                ylow = iteration * rowheight if n_iter == 1 else iteration * rowheight + .05 * rowheight
+                #top of row - 5% if n_iter > 1
+                yhigh = (iteration + 1) * rowheight if n_iter == 1 else (iteration + 1) * rowheight - .05 * rowheight
+
+                ax.vlines(times_iteration[event],ylow,yhigh, linestyles='dotted',color=event_color,alpha=.5,transform=ax.get_xaxis_transform())
+                ax.vlines(times_iteration[event]+event_size,ylow, yhigh, linestyles='dotted',color=event_color,alpha=.5, transform=ax.get_xaxis_transform())
+                ax.fill_between(np.array([times_iteration[event],times_iteration[event]+event_size]), ylow, yhigh, alpha=0.15,color=event_color, transform=ax.get_xaxis_transform(),edgecolor=None)
+
+    if colorbar:
+        cheight = "100%" if n_iter == 1 else f"{200/n_iter}%" 
+        axins = inset_axes(ax, width="0.5%", height=cheight, loc="lower left", bbox_to_anchor=(1.025, 0, 2, 1), bbox_transform=ax.transAxes, borderpad=0)
+        if isinstance(channel_position, Info):
+            lab = 'Voltage' if channel_position['chs'][0]['unit'] == 107 else channel_position['chs'][0]['unit']._name
+        else:
+            lab = 'Voltage'
+        plot_brain_colorbar(axins, dict(kind='value', lims = [vmin,0,vmax]),colormap=cmap, label = lab, bgcolor='.5', transparent=None)
     if isinstance(ylabels, dict):
-        ax.set_yticks(np.arange(len(list(ylabels.values())[0])),
+        ax.set_yticks(np.arange(len(list(ylabels.values())[0]))+.5,
                       [str(x) for x in list(ylabels.values())[0]])
         ax.set_ylabel(str(list(ylabels.keys())[0]))
     else:
         ax.set_yticks([])
         ax.spines['left'].set_visible(False)
     __display_times(ax, times_to_display, 0, time_step, max_time, times, n_iter)
     if not return_ax:
         ax.spines['top'].set_visible(False)
         ax.spines['right'].set_visible(False)
-        ax.set_ylim(0-yoffset, n_iter-1+yoffset)
-        if time_step == 1:
-            ax.set_xlabel('Time (in samples)')
-        else:
-            ax.set_xlabel('Time')
+        ax.set_ylim(0, n_iter) #-1
+        ax.set_xlabel(xlabel)
         if title:
             ax.set_title(title)
         if np.any(max_time) == None and np.any(times_to_display) == None:
             ax.set_xlim(0, np.nanmax(times)+np.nanmax(times)/10)
+    if plt.get_backend()[0:2] == 'Qt': #fixes issue with yscaling
+        plt.tight_layout()
     if return_ax:
-        ax.set_ylim(0-yoffset, n_iter-1+yoffset)
+        ax.set_ylim(0, n_iter) #-1
         return ax
     else:
         plt.show()    
 
 
+
+def plot_components_sensor(hmp_data, positions):
+    from mne.viz import plot_topomap
+    fig, ax = plt.subplots(1,len(hmp_data.attrs['components'].component))
+    for comp in hmp_data.attrs['components'].component:
+        plot_topomap(hmp_data.attrs['components'].values[:,comp], positions, axes=ax[comp], show=False, cmap='Spectral_r')
+    plt.show()
+
+
 def plot_loocv(loocv_estimates, pvals=True, test='t-test', figsize=(16,5), indiv=True, ax=None, mean=False):
     '''
     Plotting the LOOCV results
     
     Parameters
     ----------
     loocv_estimates : ndarray or xarra.DataArray
@@ -207,15 +283,15 @@
     ax[1].set_xlabel('')
     if return_ax:
         return ax
     else:
         plt.tight_layout()
         plt.show()
 
-def plot_latencies_average(times, event_width, time_step=1, labels=[], colors=default_colors,
+def plot_latencies_average(times, time_step=1, labels=[], colors=default_colors,
     figsize=None, errs='ci', max_time=None, times_to_display=None):
     '''
     REDUNDANT WITH plot_latencies() WILL BE DEPRECATED
     Plots the average of stage latencies with choosen errors bars
 
     Parameters
     ----------
@@ -237,48 +313,53 @@
         Whether to display 95% confidence interval ('ci') or standard deviation (std)
     times_to_display : ndarray
         Times to display (e.g. Reaction time or any other relevant time) in the time unit of the fitted data
     max_time : float
         limit of the x (time) axe
     '''
     from seaborn.algorithms import bootstrap #might be too much to ask for seaborn install?
-    j = 0
-    
+   
     if len(np.shape(times)) == 2:
         times = [times]
 
     if figsize == None:
         figsize = (8, 1*len(times)+2)
     f, axs = plt.subplots(1,1, figsize=figsize,dpi=100)
-    for time in times:
-        time = time*time_step
+    for j, time in enumerate(times):
+        time = time.data*time_step
         cycol = cycle(colors)
-        n_stages = len(time[-1][np.isfinite(time[-1])])
+        n_stages = len(time[-1][np.isfinite(time[-1])]) - 1
         colors = [next(cycol) for x in np.arange(n_stages)]
+
+        duration = time[:,1:] - time[:,:-1]
+
+        avg_time = np.mean(time, axis=0)
+        avg_duration = np.mean(duration, axis=0)
+
         for stage in np.arange(n_stages-1,-1,-1):
             colors.append(next(cycol))
-            plt.barh(j+.02*stage, np.mean(time[:,stage]), color='w', edgecolor=colors[stage])
+            plt.barh(j, avg_duration[stage],left=avg_time[stage], color='w', edgecolor=colors[stage])
             if errs == 'ci':
-                errorbars = np.transpose([np.nanpercentile(bootstrap(time[:,stage]), q=[2.5,97.5])])
-                errorbars = np.abs(errorbars-np.mean(time[:,stage].values))
+                errorbars = np.transpose([np.nanpercentile(bootstrap(duration[:,stage]), q=[2.5,97.5])])
+                errorbars = np.abs(errorbars-avg_duration[stage])
             elif errs == 'std':
-                errorbars = np.std(time[:,stage])
+                errorbars = np.std(duration[:,stage])
             else:
                 print('Unknown errorbar type')
                 errorbars = np.repeat(0,2)
-            plt.errorbar(np.mean(time[:,stage]), j+.02*stage, xerr=errorbars, 
+            plt.errorbar(avg_time[stage+1], j, xerr=errorbars, 
                      color=colors[stage], fmt='none', capsize=10)
-        j += 1
+
     plt.yticks(np.arange(len(labels)),labels)
-    plt.ylim(0-1,j)
+    plt.ylim(0-1,j+1)
     __display_times(axs, times_to_display, np.arange(np.shape(times)[0]), time_step, max_time, times)
     if time_step == 1:
-        plt.xlabel('(Cumulative) Stages durations from stimulus onset (samples)')
+        plt.xlabel('Cumulative stage durations from stimulus onset (samples)')
     else:
-        plt.xlabel('(Cumulative) Stages durations from stimulus onset')
+        plt.xlabel('Cumulative stage durations from stimulus onset (ms)')
     plt.tight_layout()
     # Hide the right and top spines
     axs.spines.right.set_visible(False)
     axs.spines.top.set_visible(False)
     # Only show ticks on the left and bottom spines
     axs.yaxis.set_ticks_position('left')
     axs.xaxis.set_ticks_position('bottom')
@@ -320,20 +401,16 @@
         axs.set_xlim(xlims[0], xlims[1])
     return axs
 
 def __display_times(ax, times_to_display, yoffset, time_step, max_time, times, ymax=1):
     n_iter = len(times)
     times = np.asarray(times,dtype=object)
     if isinstance(times_to_display, (np.ndarray, np.generic)):
-        if isinstance(times_to_display, np.ndarray):
-            ax.vlines(times_to_display*time_step, yoffset-1.1, yoffset+ymax+1.1, ls='--')
-            ax.set_xlim(-1*time_step, max(times_to_display)*time_step+((max(times_to_display)*time_step)/15))
-        else:
-            ax.vlines(times_to_display*time_step, yoffset-1.1, yoffset+ymax+1.1, ls='--')
-            ax.set_xlim(-1*time_step, times_to_display*time_step+(times_to_display*time_step)/15)
+        ax.vlines(times_to_display*time_step, yoffset-1.1, yoffset+ymax+1.1, ls='--')
+        ax.set_xlim(-1*time_step, np.max(times_to_display)*time_step * 1.05)
     if max_time:
         ax.set_xlim(-1*time_step, max_time)
     return ax
 
 def plot_latencies_gamma(gammas, event_width=0, time_step=1, labels=[''], colors=default_colors, 
                          figsize=False, times_to_display=None, max_time=None, kind='bar', legend=False):
     '''
@@ -396,16 +473,16 @@
     axs.spines.top.set_visible(False)
     # Only show ticks on the left and bottom spines
     axs.yaxis.set_ticks_position('left')
     if legend:
         axs.legend()
     return axs
 
-def plot_latencies(times, event_width, time_step=1, labels=[], colors=default_colors,
-    figsize=False, errs='ci',  max_time=None, times_to_display=None, kind='bar', legend=False):
+def plot_latencies(times, time_step=1, labels=[], colors=default_colors,
+    figsize=False, errs='ci', kind='bar', legend=False):
     '''
     Plots the average of stage latencies with choosen errors bars
 
     Parameters
     ----------
     times : ndarray
         2D or 3D numpy array, Either trials * events or conditions * trials * events
@@ -425,25 +502,24 @@
         Whether to display 95% confidence interval ('ci') or standard deviation (std)
     times_to_display : ndarray
         Times to display (e.g. Reaction time or any other relevant time) in the time unit of the fitted data
     max_time : float
         limit of the x (time) axe
     '''
     from seaborn.algorithms import bootstrap #might be too much to ask for seaborn install?
-    j = 0
-    
+       
     if len(np.shape(times)) == 2:
         times = [times]
 
     if not figsize:
         figsize = (8, 1*len(times)+2)
     f, axs = plt.subplots(1,1, figsize=figsize, dpi=100)
     cycol = cycle(colors)
     colors = [next(cycol) for x in np.arange(len(times))]
-    for time in times:
+    for j, time in enumerate(times):
         time = time*time_step
         time = np.diff(time, axis=1, prepend=0)
         n_stages = len(time[-1])
         if errs == 'ci':
             errorbars = np.nanpercentile(bootstrap(time, axis=0), q=[2.5,97.5], axis=0)
             errorbars = np.abs(errorbars-np.mean(time, axis=0))
         elif errs == 'std':
@@ -454,21 +530,21 @@
         if kind == 'bar':
             plt.bar(np.arange(n_stages)+1, np.mean(time, axis=0), color='w', edgecolor=colors[j])
             plt.errorbar(np.arange(n_stages)+1, np.mean(time, axis=0), yerr=errorbars, 
                      color=colors[j], fmt='none', capsize=10)
         elif kind == 'point':
             plt.errorbar(np.arange(n_stages)+1, np.mean(time, axis=0), 
                 yerr=errorbars, color=colors[j], fmt='o-', capsize=10, label=labels[j])
-        j += 1
 
     plt.xlim(1-.5, n_stages+.5)
     if time_step == 1:
         plt.ylabel('Stage durations (samples)')
     else:
-        plt.ylabel('Stage durations')
+        plt.ylabel('Stage durations (ms)')
+    plt.xlabel('Stage')
     plt.tight_layout()
     # Hide the right and top spines
     axs.spines.right.set_visible(False)
     axs.spines.top.set_visible(False)
     # Only show ticks on the left and bottom spines
     axs.yaxis.set_ticks_position('left')
     axs.xaxis.set_ticks_position('bottom')
@@ -484,15 +560,15 @@
         except:
             iterations = iterations.expand_dims({'iteration':[0]}, axis=1)
             iterations['iteration'] = [0]
     for iteration in iterations.iteration[:-1]:
         selected = init.fit_single(iterations.sel(iteration=iteration)[dims[0]].dropna(dim='event').event[-1].values+1,\
             magnitudes = iterations.sel(iteration=iteration)[dims[0]].dropna(dim='event'),\
             parameters = iterations.sel(iteration=iteration)[dims[1]].dropna(dim='stage'),\
-            threshold=0, verbose=False)
+            maximization=False, verbose=False)
         #Visualizing
         plot_topo_timecourse(eeg_data, selected, positions,  init, magnify=1, sensors=False,ax=ax)
     
 
 def plot_bootstrap_results(bootstrapped, info, init, model_to_compare=None, epoch_data=None):
     from hsmm_mvpy.resample import percent_event_occurence
     maxboot_model, labels, counts, event_number, label_event_num = percent_event_occurence(bootstrapped, model_to_compare)
```

### Comparing `hsmm_mvpy-0.1.0b7/src/hsmm_mvpy.egg-info/PKG-INFO` & `hsmm_mvpy-0.1.0b8/src/hsmm_mvpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsmm-mvpy
-Version: 0.1.0b7
+Version: 0.1.0b8
 Summary: Package for fitting Hidden Semi-Markov Models to electro-encephalographic data
 Author-email: Gabriel Weindel <gabriel.weindel@gmail.com>, Leendert van Maanen <e@mail.com>, Jelmer Borst <e@mail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Gabriel Weindel, Leendert van Maanen, Jelmer Borst
         All rights reserved.
         
@@ -53,23 +53,22 @@
 - Describing experimental effects based on a particular stage duration
 - Estimating the effect of trial-wise manipuations on the identified stages (e.g. the by-trial variation of stimulus strength or the effect of time-on-task)
 - Time-lock EEG signal to the onset of a given stage and perform classical ERPs or time-frequency analysis based on the onset of a new stage
 - And many more (e.g. evidence accumulation models on decision stage, classification based on the number of transition events in the signal,...)
 
 
 # Documentation
-**Important note** The current tutorials are based on the latest (unstable) version not yet default in _pip_, installing through github is therefore recommended or specify the beta version when installing through _pip_: ```pip install hsmm-mvpy==0.1.0b1```
 
 The package is available through *pip*. 
 A recommended way of using the package is to use a conda environment (see [anaconda](https://www.anaconda.com/products/distribution>) for how to install conda):
 
     $ conda create -n hmp 
     $ conda activate hmp
     $ conda install pip #if not already installed
-    $ pip install hsmm-mvpy==0.1.0b1
+    $ pip install hsmm-mvpy
 
 Then import hsmm-mvpy in your favorite python IDE through:
 
 ```python
     import hsmm_mvpy as hmp
 ```
 
@@ -123,56 +122,56 @@
 
 ## Importing HMP
 import hsmm_mvpy as hmp
 from hsmm_mvpy import simulations
 ```
 
 
+
 ### Simulating data
 
 In the following code block we simulate 50 trials from four known sources, this is not code you would need for your own analysis except if you'd want to simulate and test properties of HMP models. All four sources are defined by a location, an activation amplitude and a distribution in time (here a gamma with shape and scale parameters) for the onsets of the stages on each trial. The simulation functions are based on this [MNE tutorial ](https://mne.tools/stable/auto_examples/simulation/simulated_raw_data_using_subject_anatomy.html).
 
 _If you're running this for the first time a 1.65 G file will be downloaded in order to perform the simulation but this will be done only once (alternatively you can just download the corresponding simulation file and place it in the same folder from where you are running this notebook)_
 
 
 
+
 ```python
 cpus = 5 # For multiprocessing, usually a good idea to use multiple CPUs as long as you have enough RAM
 
 n_trials = 50 #Number of trials to simulate
 
 ##### Here we define the sources of the brain activity (event) for each trial
-# Because the last source determines the response, we will get four events during the trials, and therefore five stages
 n_sources = 5
 frequency = 10.#Frequency of the event defining its duration, half-sine of 10Hz = 50ms
 amplitude = .5e-6 #Amplitude of the event in nAm, defining signal to noise ratio
 shape = 2 #shape of the gamma distribution
 means = np.array([60, 150, 200, 100, 80])/shape #Mean duration of the stages in ms
-names = simulations.available_sources()[:n_sources]#Which source to activate at each stage (see atlas when calling simulations.available_sources())
+names = simulations.available_sources()[:n_sources+1]#Which source to activate at each stage (see atlas when calling simulations.available_sources())
 
 sources = []
 for source in zip(names, means):#One source = one frequency, one amplitude and a given by-trial variability distribution
     sources.append([source[0], frequency, amplitude, gamma(shape, scale=source[1])])
 
 # Function used to generate the data
-file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True) #location indicates the middle of the event after the stage start time in ms
+file = simulations.simulate(sources, n_trials, cpus, 'dataset_README', location=25, overwrite=True)
 #Recovering sampling frequency of the simulated dataset
 sfreq = simulations.simulation_sfreq()
 #load electrode position, specific to the simulations
 positions = simulations.simulation_positions()
 ```
 
     Simulating ./dataset_README_raw.fif
+    [done]
     ./dataset_README_raw.fif simulated
 
 
-
 ### Creating the event structure and plotting the raw data
 
-
 To recover the data we need to create the event structure based on the triggers sent during simulation. This is the same as analyzing real EEG data and recovering events in the stimulus channel. In our case 1 signal the onset of the stimulus and 6 the moment of the response. Hence a trial is defined as the times occuring between the triggers 1 and 6.
 
 
 ```python
 #Recovering the events to epoch the data (in the number of trials defined above)
 generating_events = np.load(file[1])
 resp_trigger = int(np.max(np.unique(generating_events[:,2])))#Resp trigger is the last source in each trial
@@ -182,96 +181,108 @@
 events = generating_events[(generating_events[:,2] == 1) | (generating_events[:,2] == resp_trigger)]#only retain stimulus and response triggers
 
 #Visualising the raw simulated EEG data
 import mne
 raw = mne.io.read_raw_fif(file[0], preload=False, verbose=False)
 raw.pick_types(eeg=True).plot(scalings=dict(eeg=1e-5), events=events, block=True);
 ```
-![png](README_files/README_7_1.png)
 
+    NOTE: pick_types() is a legacy function. New code should use inst.pick(...).
+    Using qt as 2D backend.
+    Channels marked as bad:
+    none
+
+
+![png](README_files/README_7_1.png)
 
 ### Recovering number of stages as well as actual by-trial variation
 
 To see how well HMP does at recovering by-trial stages below, here we get the ground truth from our simulation. Unfortunately, with an actual dataset you don’t have access to this, of course. 
 
+
 ```python
 %matplotlib inline
 number_of_sources = len(np.unique(generating_events[:,2])[1:])#one trigger = one source
 #Recover the actual time of the simulated events
 random_source_times = np.reshape(np.ediff1d(generating_events[:,0],to_begin=0)[generating_events[:,2] > 1], \
            (n_trials, number_of_sources))
 ```
 
 ## Demo for a single participant in a single condition based on the simulated data
 
-First we read the EEG data as we would for a single participant:
+First we read the EEG data as we would for a single participant
 
 
 ```python
 # Reading the data
 eeg_data = hmp.utils.read_mne_data(file[0], event_id=event_id, resp_id=resp_id, sfreq=sfreq, 
             events_provided=events, verbose=False)
 
 ```
 
     Processing participant ./dataset_README_raw.fif's continuous eeg
-    Reading 0 ... 143915  =      0.000 ...   239.613 secs...
+    Reading 0 ... 161924  =      0.000 ...   269.597 secs...
     50 trials were retained for participant ./dataset_README_raw.fif
 
 
+
 HMP uses [xarray](https://docs.xarray.dev/en/stable/) named dimension matrices, allowing to directly manipulate the data using the name of the dimensions:
 
 
+
+
 ```python
 #example of usage of xarray
 print(eeg_data)
-eeg_data.sel(electrodes=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
-    .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='electrodes');
+eeg_data.sel(channels=['EEG 001','EEG 002','EEG 003'], samples=range(400))\
+    .data.groupby('samples').mean(['participant','epochs']).plot.line(hue='channels');
 ```
 
     <xarray.Dataset>
-    Dimensions:      (participant: 1, epochs: 50, electrodes: 59, samples: 783)
+    Dimensions:      (participant: 1, epochs: 50, channels: 59, samples: 667)
     Coordinates:
       * epochs       (epochs) int64 0 1 2 3 4 5 6 7 8 ... 41 42 43 44 45 46 47 48 49
-      * electrodes   (electrodes) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
-      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 776 777 778 779 780 781 782
+      * channels     (channels) <U7 'EEG 001' 'EEG 002' ... 'EEG 059' 'EEG 060'
+      * samples      (samples) int64 0 1 2 3 4 5 6 7 ... 660 661 662 663 664 665 666
+        event_name   (epochs) object 'stimulus' 'stimulus' ... 'stimulus' 'stimulus'
+        rt           (epochs) float64 0.5628 0.9956 0.5478 ... 0.7043 0.7659 0.8591
       * participant  (participant) <U2 'S0'
     Data variables:
-        data         (participant, epochs, electrodes, samples) float64 -3.747e-0...
-        event_name   (participant, epochs) object 'stimulus' ... 'stimulus'
-        rt           (participant, epochs) float64 0.5444 0.641 ... 0.8991 1.304
+        data         (participant, epochs, channels, samples) float64 -1.603e-06 ...
     Attributes:
         sfreq:    600.614990234375
         offset:   0
 
 
 
     
 ![png](README_files/README_12_1.png)
     
 
 
-
 Next we transform the data as in Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet.apa.org/doi/10.1037/rev0000030)) including standardization of individual variances (not in this case as we have only one simulated participant), z-scoring and spatial principal components analysis (PCA). 
 
 Note that if the number of components to retain is not specified, the scree plot of the PCA is displayed and a prompt ask how many PCs should be retained (in this case we specify it as building the README does not allow for prompts)
 
 
 ```python
 hmp_data = hmp.utils.transform_data(eeg_data, apply_standard=False, n_comp=4)
 ```
 
 # HMP model
 
 Once the data is in the expected format, we can initialize an HMP object; note that no estimation is performed yet.
 
+
+
 ```python
 init = hmp.models.hmp(hmp_data, eeg_data, event_width=50, cpus=cpus)#Initialization of the model
 ```
 
+
 We are looking for stages in the data (**Hidden Markov**) and assume that transitions between stages are signaled by a template in the data (**pattern analysis**). By default we use the same template as Anderson, Zhang, Borst, & Walsh  ([2016](https://psycnet'.apa.org/doi/10.1037/rev0000030)), a 10 Hz half-sine, resulting in a 50ms duration bump-like shape:
 
 
 
 ```python
 plt.plot(init.template,'x');
 ```
@@ -285,27 +296,27 @@
 This pattern is assumed to be present across several electrodes (**multivariate**). In order to find it, we apply a cross-correlation between that shape and the (normalized) EEG data:
 
 
 
 ```python
 epoch = 0 #illustrating the first trial
 hmp_data.unstack().sel(component=[0,1,2], epochs=epoch).squeeze().plot.line(hue='component');
-plt.vlines(random_source_times[epoch,:-1].cumsum()-1, -3, 3, 'k')#overlaying the simulated stage transition times
+plt.vlines(random_source_times[epoch,:-1].cumsum()-1, -3, 3, 'k');#overlaying the simulated stage transition times
 ```
 
 
     
-![png](README_files/README_20_1.png)
+![png](README_files/README_20_0.png)
     
 
 
-
 The by-trial onset of this transition pattern event is assumed to be captured by a probability distribution (**semi-Markov**), e.g. in this application a gamma with a shape of 2:
 
 
+
 ```python
 T = 350
 plt.plot(np.linspace(0,T,1001),gamma.pdf(np.linspace(0,T,1001), 2, scale=50)) 
 plt.xlabel('t');
 ```
 
 
@@ -318,36 +329,41 @@
 
 # Estimating an HMP model
 
 We can directly fit an HMP model without giving any info on the number of stages (see tutorial 2 for a detailed explanation of the following cell)
 
 
 
+
+
 ```python
 estimates = init.fit(step=20, verbose=True)
 ```
 
 
+      0%|          | 0/418 [00:00<?, ?it/s]
 
-    Transition event 1 found around sample 37
-    Transition event 2 found around sample 137
-    Transition event 3 found around sample 277
-    Transition event 4 found around sample 348
+
+    Transition event 1 found around sample 42
+    Transition event 2 found around sample 154
+    Transition event 3 found around sample 285
+    Transition event 4 found around sample 369
     Estimating 4 events model
     Parameters estimated for 4 events model
 
 
 ### Visualizing results of the fit
 
 In the previous cell we initiated an HMP model looking for default 50ms bumps – the transition events – in the EEG signal. The method discovered four events, and therefore five gamma-distributed stages with a fixed shape of 2 and an estimated scale. We can now inspect the results of the fit.
 
 We can directly take a look to the topologies and latencies of the events by calling ```hmp.visu.plot_topo_timecourse```
 
 
 
+
 ```python
 hmp.visu.plot_topo_timecourse(eeg_data, estimates, #Data and estimations 
                                positions, init,#position of the electrodes and initialized model
                                magnify=1, sensors=False, time_step=1000/init.sfreq,#Display control parameters
                                times_to_display = np.mean(init.ends - init.starts))#plot reaction times
 ```
 
@@ -358,17 +374,19 @@
 
 
 This shows us the electrode activity on the scalp as well as the average time of occurence of the events based on the stage distributions.
 
 As we are estimating the event onsets on a by-trial basis we can look at the by-trial variation in stage duration.
 
 
+
 ```python
-event_times_estimates = init.compute_times(init, estimates, mean=False, add_rt=True).dropna('event')#computing predicted event times
-ax = hmp.visu.plot_latencies_average(event_times_estimates, init.event_width_samples, 1, errs='ci', times_to_display = np.mean(init.ends - init.starts))
+event_times_estimates = init.compute_times(init, estimates, mean=False,fill_value=0, add_rt=True).dropna('event')#computing predicted event times
+ax = hmp.visu.plot_latencies_average(event_times_estimates, 1, errs='ci', \
+                                     times_to_display = np.mean(init.ends - init.starts))
 ax.set_ylabel('your label here');
 ```
 
 
     
 ![png](README_files/README_28_0.png)
     
@@ -382,15 +400,15 @@
 hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 hmp.visu.plot_distribution(estimates.eventprobs.mean(dim=['trial_x_participant']), xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)), survival=True)
 ```
 
 
 
 
-    <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
+    <Axes: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
 ![png](README_files/README_30_1.png)
     
@@ -401,39 +419,42 @@
 ![png](README_files/README_30_2.png)
     
 
 
 As HMP estimated stage onset per trial we can also look at the predicted stage onsets for a given trial.
 
 
+
 ```python
 hmp.visu.plot_distribution(estimates.eventprobs.sel(trial_x_participant=('S0', 0)), 
                             xlims=(0,np.percentile(random_source_times.sum(axis=1), q=90)))
 ```
 
 
 
 
-    <AxesSubplot: xlabel='Time (in samples)', ylabel='p(event)'>
+    <Axes: xlabel='Time (in samples)', ylabel='p(event)'>
 
 
 
 
     
 ![png](README_files/README_32_1.png)
     
 
 
+
 This then shows the likeliest stage onset location in time for the first trial!
 
 ## Comparing with ground truth
 
 As we simulated the data we have access to the ground truth of the underlying generative events. We can then compare the average stage durations compared to the one estimated by HMP. Perhaps to state the obvious, this code is specific to the case where you simulate data.
 
 
+
 ```python
 colors = sns.color_palette(None, number_of_sources)
 plt.scatter(np.mean(random_source_times, axis=0), estimates.parameters.prod(axis=1), color=colors,s=50)
 plt.plot([np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],
          [np.min(np.mean(random_source_times,axis=0)),np.max(np.mean(random_source_times,axis=0))],'--');
 plt.title('Actual vs estimated stage durations')
 plt.xlabel('Simulated stage duration')
@@ -459,19 +480,21 @@
 
 
     
 ![png](README_files/README_36_0.png)
     
 
 
+
 We see that the HMP recovered the exact average location of the bumps defined in the simulated data.
 
 We can further test how well the package did by comparing the generated single trial onsets with those estimated from the HMP model
 
 
+
 ```python
 fig, ax= plt.subplots(number_of_sources,1, figsize=(5,3.5*number_of_sources), dpi=300)
 ax[0].set_title('Comparing true vs estimated single trial stage durations')
 i = 0
 
 for event in init.compute_times(init, estimates, duration=True, mean=False, add_rt=True).T:
     sns.regplot(x=random_source_times[:,i].T, y=event, ax=ax[i], color=colors[i])
@@ -483,14 +506,15 @@
 
 
     
 ![png](README_files/README_38_0.png)
     
 
 
+
 We see that every stage gets nicely recovered even on a by-trial basis!
 
 # Beyond summary statistics for EEG analysis
 
 Now the purpose, apart from determining the number and time course of important EEG events in the reaction time, is also to use the by-trial information.
 
 We illustrate this by first plotting the traditional event-related potentials (i.e. taking the average of given electrodes across the different time points) with cherry-picked electrodes.
@@ -502,15 +526,15 @@
 import pandas as pd
 
 data = eeg_data.stack({'trial_x_participant':['participant','epochs']}).data.dropna('trial_x_participant', how="all")
 fig, ax = plt.subplots(1,1, figsize=(20,5), sharey=True)
 
 for electrode in zip(['EEG 016','EEG 025','EEG 020'],#Cherry-picked electrodes
                      ['darkgreen','darkred','darkblue']):
-    df = pd.DataFrame(data.sel(electrodes=electrode[0]).squeeze().T).melt(var_name='Time')
+    df = pd.DataFrame(data.sel(channels=electrode[0]).squeeze().T).melt(var_name='Time')
     sns.lineplot(x='Time', y='value',data=df, color=electrode[1])
 
 plt.vlines(np.cumsum(random_source_times.mean(axis=0)), -3e-6, 3e-6)
 plt.ylabel('Volt')
 plt.xlim(0,500)
 plt.ylim(-3e-6,3e-6);
 
@@ -523,14 +547,16 @@
 
 
 Given how variable and serial each of these stages are, the more you progress in the chain of events the less clear the signal gets. This is similar to traditional ERPs that have a very clear signal in the beginning of a trial (as events are more in phase) and summed and blurred further away from the stimulus (as events are off phase).
 
 Now things can get better if we first parse, by-trial, the signal into the different stages based on the HMP estimates:
 
 
+
+
 ```python
 BRP_times = init.compute_times(init, estimates.dropna('event'), fill_value=0, add_rt=True)
 
 fig, ax = plt.subplots(1,number_of_sources, figsize=(20,5), sharey=True, sharex=True)
 ax[0].set_ylabel('Volt')
 for stage in range(number_of_sources):
     BRP = hmp.utils.event_times(data, BRP_times,'EEG 016',stage=stage)
@@ -548,18 +574,20 @@
 
     
 ![png](README_files/README_42_0.png)
     
 
 
 
+
 In this case we clearly see at each stage the half-sine (of 50ms hence ~ 30 samples for the sampling frequency used) we simulated in the first step and the preceding period of silence (hence the first stage doesn't contain such a half-sine). Note that the end of the stages tend to be noisier because fewer trials are defining the average signal.
 
 
 ### Follow-up
 
 For examples on how to use the package when the number of transition events/stages is unkown, or to compare stage durations across conditions see the tutorial notebooks:
 - Load EEG data (tutorial 1)
 - Estimating a given number of events (tutorial 2)
 - Test for the number of events that best explains the data (tutorial 3)
 - Testing differences across conditions (tutorial 4)
+- Plotting Event Related Potentials with an HMP decomposition (tutorial 5)
```

