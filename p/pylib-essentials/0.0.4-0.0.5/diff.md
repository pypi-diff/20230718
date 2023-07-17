# Comparing `tmp/pylib_essentials-0.0.4.tar.gz` & `tmp/pylib_essentials-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylib_essentials-0.0.4.tar", last modified: Mon Jul 17 21:06:54 2023, max compression
+gzip compressed data, was "pylib_essentials-0.0.5.tar", last modified: Mon Jul 17 22:16:07 2023, max compression
```

## Comparing `pylib_essentials-0.0.4.tar` & `pylib_essentials-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-17 21:06:54.126747 pylib_essentials-0.0.4/
--rw-r--r--   0 feiye    (49086) vims     (50001)      312 2023-07-17 21:06:54.125748 pylib_essentials-0.0.4/PKG-INFO
--rw-r--r--   0 feiye    (49086) vims     (50001)      292 2023-06-12 21:54:20.000000 pylib_essentials-0.0.4/README.md
-drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-17 21:06:53.852746 pylib_essentials-0.0.4/pylib_essentials/
--rw-r--r--   0 feiye    (49086) vims     (50001)        0 2023-06-13 06:47:18.000000 pylib_essentials-0.0.4/pylib_essentials/__init__.py
--rw-r--r--   0 feiye    (49086) vims     (50001)   182932 2023-07-17 20:33:36.000000 pylib_essentials-0.0.4/pylib_essentials/schism_file.py
--rw-r--r--   0 feiye    (49086) vims     (50001)    53637 2023-07-17 18:11:09.000000 pylib_essentials-0.0.4/pylib_essentials/utility_functions.py
-drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-17 21:06:54.095747 pylib_essentials-0.0.4/pylib_essentials.egg-info/
--rw-r--r--   0 feiye    (49086) vims     (50001)      312 2023-07-17 21:06:53.000000 pylib_essentials-0.0.4/pylib_essentials.egg-info/PKG-INFO
--rw-r--r--   0 feiye    (49086) vims     (50001)      316 2023-07-17 21:06:53.000000 pylib_essentials-0.0.4/pylib_essentials.egg-info/SOURCES.txt
--rw-r--r--   0 feiye    (49086) vims     (50001)        1 2023-07-17 21:06:53.000000 pylib_essentials-0.0.4/pylib_essentials.egg-info/dependency_links.txt
--rw-r--r--   0 feiye    (49086) vims     (50001)      163 2023-07-17 21:06:53.000000 pylib_essentials-0.0.4/pylib_essentials.egg-info/requires.txt
--rw-r--r--   0 feiye    (49086) vims     (50001)       17 2023-07-17 21:06:53.000000 pylib_essentials-0.0.4/pylib_essentials.egg-info/top_level.txt
--rw-r--r--   0 feiye    (49086) vims     (50001)       38 2023-07-17 21:06:54.127747 pylib_essentials-0.0.4/setup.cfg
--rw-r--r--   0 feiye    (49086) vims     (50001)      600 2023-07-17 18:04:10.000000 pylib_essentials-0.0.4/setup.py
+drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-17 22:16:07.245876 pylib_essentials-0.0.5/
+-rw-r--r--   0 feiye    (49086) vims     (50001)      265 2023-07-17 22:16:07.230876 pylib_essentials-0.0.5/PKG-INFO
+-rw-r--r--   0 feiye    (49086) vims     (50001)      292 2023-06-12 21:54:20.000000 pylib_essentials-0.0.5/README.md
+drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-17 22:16:07.124875 pylib_essentials-0.0.5/pylib_essentials/
+-rw-r--r--   0 feiye    (49086) vims     (50001)        0 2023-06-13 06:47:18.000000 pylib_essentials-0.0.5/pylib_essentials/__init__.py
+-rw-r--r--   0 feiye    (49086) vims     (50001)   183235 2023-07-17 22:13:40.000000 pylib_essentials-0.0.5/pylib_essentials/schism_file.py
+-rw-r--r--   0 feiye    (49086) vims     (50001)    53637 2023-07-17 18:11:09.000000 pylib_essentials-0.0.5/pylib_essentials/utility_functions.py
+drwxr-xr-x   0 feiye    (49086) vims     (50001)        0 2023-07-17 22:16:07.160875 pylib_essentials-0.0.5/pylib_essentials.egg-info/
+-rw-r--r--   0 feiye    (49086) vims     (50001)      265 2023-07-17 22:16:06.000000 pylib_essentials-0.0.5/pylib_essentials.egg-info/PKG-INFO
+-rw-r--r--   0 feiye    (49086) vims     (50001)      316 2023-07-17 22:16:06.000000 pylib_essentials-0.0.5/pylib_essentials.egg-info/SOURCES.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)        1 2023-07-17 22:16:06.000000 pylib_essentials-0.0.5/pylib_essentials.egg-info/dependency_links.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)      163 2023-07-17 22:16:06.000000 pylib_essentials-0.0.5/pylib_essentials.egg-info/requires.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)       17 2023-07-17 22:16:06.000000 pylib_essentials-0.0.5/pylib_essentials.egg-info/top_level.txt
+-rw-r--r--   0 feiye    (49086) vims     (50001)       38 2023-07-17 22:16:07.246876 pylib_essentials-0.0.5/setup.cfg
+-rw-r--r--   0 feiye    (49086) vims     (50001)      600 2023-07-17 22:14:51.000000 pylib_essentials-0.0.5/setup.py
```

### Comparing `pylib_essentials-0.0.4/pylib_essentials/schism_file.py` & `pylib_essentials-0.0.5/pylib_essentials/schism_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
         '''
         Compute gradient on each element first, then convert to node value
           fmt: interploation method (see details in interp_elem_to_node())
               (0: simple avarage; fmt=1: inverse distance; fmt=2: maximum of surrounding nodal values)
           value=None: gd.dp is used;    value: array of [np,] or [ne]
           outfmt=0: return (dpdx,dpdy,dpdxy); outfmt=1: return (dpdx,dpdy,dpdxy,dpedx,dpedy,dpedxy)
           cpp=1: CPP projection. It project decimal degress (lon/lat) to CPP coordinate (https://www.xmswiki.com/wiki/CPP_Coordinate_System).
-                 If lon_ori and lat_ori are not defined, they will be the center of the grid 
+                 If lon_ori and lat_ori are not defined, they will be the center of the grid
         '''
         if not hasattr(self,'area'): self.compute_area()
         if not hasattr(self,'dpe'): self.compute_ctr()
 
         if cpp==1:
             ox=self.x.copy(); oy=self.y.copy()
             if lon_ori==None or lat_ori==None:
@@ -2493,37 +2493,37 @@
     return S
 
 def read_schism_slab(run,varname,levels,stacks=None,nspool=1,mdt=None,sname=None,fname=None):
     '''
     extract slabs of SCHISM results (works for scribe IO and combined oldIO)
        run:     run directory where (grid.npz or hgrid.gr3,vgrid.in) and outputs are located
        varname: variables to be extracted; accept shortname(s) or fullname(s) (elev, hvel, horizontalVelX, NO3, ICM_NO3, etc. )
-       levels:  schism level indices (1-nvrt: surface-bottom; (>nvrt): kbp level) 
+       levels:  schism level indices (1-nvrt: surface-bottom; (>nvrt): kbp level)
        stacks:  (optional) output stacks to be extract; all avaiable stacks will be extracted if not specified
        nspool:  (optional) sub-sampling frequency within each stack (npsool=1 means all records)
        mdt:     (optional) time window (day) for averaging output
        sname:   (optional) variable name for save
        fname:   (optional) save the results as fname.npz
     '''
     #proc
     bdir=run+'/outputs'; modules,outfmt,dstacks,dvars,dvars_2d =get_schism_output_info(bdir,1)
     if isinstance(varname,str): varname=[varname]
     if sname is None: sname=varname
     if stacks is None: stacks=dstacks
     if outfmt==1: sys.exit('OLDIO not supported yet')
-    
+
     #read output
     S=zdata(); sdict=S.__dict__; sdict['time']=[]; S.levels=array(levels)
     for i in sname: sdict[i]=[]
     for istack in [*unique(stacks).ravel()]:
         if outfmt==0:
            C0=ReadNC('{}/out2d_{}.nc'.format(bdir,istack),1); nvrt=C0.dimensions['nSCHISM_vgrid_layers'].size
            #np=C0.dimensions['nSCHISM_hgrid_node'].size; ne=C0.dimensions['nSCHISM_hgrid_face'].size
            mt=array(C0.variables['time'][:])/86400; nt=len(mt); sdict['time'].extend(mt[::nspool])
-    
+
         for snamei,varnamei in zip(sname,varname):
             svars=get_schism_var_info(varnamei,modules,fmt=outfmt); nvar=len(svars)
             for m,[vari,svar] in enumerate(svars):
                 if svar in dvars_2d:  #2D
                    A=array([array(C0.variables[svar][i]).astype('float32') for i in arange(nt) if i%nspool==0])
                 else:   #3D
                    C=ReadNC('{}/{}_{}.nc'.format(bdir,svar,istack),1); A=[]
@@ -3014,15 +3014,15 @@
               gd=schism_grid(); gd.x=array(cvar['SCHISM_hgrid_node_x']); gd.y=array(cvar['SCHISM_hgrid_node_y']); gd.dp=array(cvar['depth'])
               gd.elnode=array(cvar['SCHISM_hgrid_face_nodes'])-1; gd.np,gd.ne=gd.dp.size,len(gd.elnode); gd.i34=sum(gd.elnode!=-2,axis=1); gd.ns=cvar['SCHISM_hgrid_edge_x'].size
            self.hgrid=gd; self.xm=[gd.x.min(),gd.x.max()]; self.ym=[gd.y.min(),gd.y.max()]; self.vm=[gd.dp.min(),gd.dp.max()]; self.fp3=nonzero(gd.i34==3)[0]; self.fp4=nonzero(gd.i34==4)[0]
            self.kbp, self.nvrt=[vd.kbp, vd.nvrt] if vd!=None else [array(cvar['bottom_index_node']), cdim['nSCHISM_vgrid_layers'].size]; self.kbe=gd.compute_kb(self.kbp)
            while not hasattr(self,'wp'): time.sleep(0.01)
            w=self.wp; w._layer['values']=['surface','bottom',*arange(2,self.nvrt+1)]; print('schismview ready')
            w.vmin.set(self.vm[0]); w.vmax.set(self.vm[1]); w.xmin.set(self.xm[0]); w.xmax.set(self.xm[1]); w.ymin.set(self.ym[0]); w.ymax.set(self.ym[1])
-        self.nvrt=2; self.xm=[0,1]; self.ym=[0,1]; self.vm=[0,1] 
+        self.nvrt=2; self.xm=[0,1]; self.ym=[0,1]; self.vm=[0,1]
         threading.Thread(target=_read_grid).start()
 
         #read available time
         if iout==0: self.stacks=[0]; self.julian=[0]; self.istack=[0]; self.irec=[0]; self.mls=['0']; return
         self.stacks=[]; self.julian=[]; self.istack=[]; self.irec=[]
         ti=array(cvar['time'])/86400; nt=len(ti); t0=ti[0]  #assume all stacks have the same number of records
         if (not hasattr(self,'StartT')) and hasattr(C.variables['time'],'base_date'):
@@ -3216,14 +3216,21 @@
         for i in arange(0,100,3):
             L1['text']=' '*i; L2['text']=' '*i; wd.update(); xs=fms[-1].winfo_width()
             if xs>xm: wd.geometry('{}x210'.format(xs)); wd.update(); break
         return wd,w
 
 # ---------------------experimental functions and classes-------------------------------------
 def read_schism_hgrid_cached(fname, overwrite_cache=False):
+    '''
+    This function manages the caching for schism grid files.
+    It tries to save a cache at the original file location (target of the symlink if any)
+    for later reading.
+    If a cache cannot be saved at the original location, it will be saved
+    at the present location instead.
+    '''
     gd_fname = Path(fname).absolute()  # force pathlib.Path and absolute path
     gd_original_fname = gd_fname.resolve()
 
     gd = None
     if overwrite_cache:
         for cache_name in [f'{gd_original_fname}.pkl', f'{gd_fname}.pkl']:
             Path(cache_name).unlink(missing_ok=True)
@@ -3231,41 +3238,45 @@
     # try to read from cache: original file location first, then present location
     for cache_name in [f'{gd_original_fname}.pkl', f'{gd_fname}.pkl']:
         try:
             with open(cache_name, 'rb') as file:
                 print(f'Try reading from cache: {cache_name}.')
                 gd = pickle.load(file)
         except Exception as e:
-            print(f'{e}\nError reading from original cache: {cache_name}.')
+            print(f'{e}\nWarning: failed to read from original cache: {cache_name}.')
         finally:
             if gd is not None:
                 return gd  # success, return gd based on cache
 
-    # if cache read is not successful, read from file and update cache
+    # if cache read is not successful, read from file
     for filename in [gd_original_fname, gd_fname]:
         try:
             print(f'Try reading from {filename}.')
-            gd = schism_grid(filename)
+            gd = schism_grid(str(filename))
             gd.source_file = filename
         except Exception as e:
-            print(f'{e}\nError reading from original file: {filename}.')
+            print(f'{e}\nWarning: failed to read from original file: {filename}.')
         finally:
             if gd is not None:
                 break
-
     if gd is None:
         raise Exception(f'Error reading {filename}.')
 
     # write to cache
+    iDumpCache = False
     for cache_fname in [f'{gd_original_fname}.pkl', f'{gd_fname}.pkl']:
         try:
             with open(cache_fname, 'wb') as file:
                 pickle.dump(gd, file)
+                iDumpCache = True
         except Exception as e:
-            print(f'{e}\nError writing cache file {cache_fname}.')  
+            print(f'{e}\nWarning: failed to write cache file {cache_fname}.')
+        finally:
+            if iDumpCache:
+                break
 
     if gd.source_file is None:
         gd.source_file = gd_fname
 
     return gd
 
 def read_schism_vgrid_cached(vg_filename, overwrite_cache=False):
@@ -3293,15 +3304,15 @@
 
     # warn if B's time period does not contain A's time
     if B.index[0] > A.index[0] or B.index[-1] < A.index[-1]:
         print('Warning: B\'s time period does not contain A\'s time period')
         print('In the interpolated B, NaN will be filled for the time period that is not covered by B')
         print('and the NaN in the interpolated B will be treated as 0 when summing up')
 
-    # Interpolate B to A's index 
+    # Interpolate B to A's index
     B_interpolated = B.reindex(A.index).interpolate(method='time')
 
     # Find the columns that are in B but not in A
     new_columns = B_interpolated.columns.difference(A.columns)
 
     # append these columns to A
     AB = pd.concat([A, B_interpolated[new_columns]], axis=1)
@@ -3341,19 +3352,19 @@
         seconds = (self.df.index - self.df.index[0]).total_seconds().values
         t = seconds / self.sec_per_time_unit
         return t
 
     @property
     def n_time(self):
         return self.df.shape[0]
-    
+
     @property
     def n_station(self):
         return self.df.shape[1]
-    
+
     @property
     def data(self):
         # original data excluding time
         return self.df.values
 
     def __init__(self, start_time_str="2000-01-01 00:00:00", data_array=None, columns=None, th_unit='seconds'):
         """
@@ -3406,15 +3417,15 @@
         """
         Initialize from a file.
         Note that the *.th file doen't have information about the time units and start time,
         and columns names, so you need to provide them.
         """
         data = np.loadtxt(file_name)
         return cls(data_array=data, th_unit=th_unit, start_time_str=start_time_str, columns=columns)
-    
+
     def __add__(self, other, weights=[1.0, 1.0]):
         """
         Add two TimeHistory objects together
         Interpolate other to self's time stamps;
         other attributes also inherit from self.
         When combining columns with the same name,
         the default weights are 1.0 for both self and other,
@@ -3427,15 +3438,15 @@
 
         A = copy.deepcopy(self)
         B = other
 
         A.df = combine_dataframes(A.df, B.df, weights=weights)
 
         return A
-    
+
     def __eq__(self, other) -> bool:
         """Check if two TimeHistory objects are equal"""
         for att in ['sec_per_time_unit']:
             if getattr(self, att) != getattr(other, att):
                 print(f'{att} is not equal')
                 return False
 
@@ -3443,40 +3454,40 @@
         # return self.df.equals(other.df)
 
         # test if the data are equal within a tolerance
         if np.any(self.df.columns != other.df.columns):
             print('column labels are not equal')
             return False
         return np.allclose(self.df, other.df, rtol=0.001, atol=0.0001)
-    
+
     def writer(self, file_name, np_savetxt_args={'fmt':'%.4f', 'delimiter':' ', 'newline':'\n'}):
         # assemble data array in *.th format and write to file
         np.savetxt(file_name, np.c_[self.time, self.data], **np_savetxt_args)
 
 
 class SourceSinkIn():
     def __init__(self, ele_groups=[[], []]):
         self.ele_groups = ele_groups  # 0: source; 1: sink
-    
+
     @property
     def n_group(self):
         return len(self.ele_groups)
 
     @property
     def np_group(self):
         return [len(x) for x in self.ele_groups]
 
     @property
     def ip_group(self):
         return [np.array(x) for x in self.ele_groups]
-    
+
     @property
     def n_source(self):
         return self.np_group[0]
-    
+
     @property
     def n_sink(self):
         return self.np_group[1]
 
     @classmethod
     def from_file(cls, filename):
         ele_groups = [[], []]
@@ -3488,15 +3499,15 @@
                 # blank line between groups
                 if k == 0:
                     file.readline()
         source_sink_in = cls(ele_groups=ele_groups)
         source_sink_in.print_info()
 
         return source_sink_in
-    
+
     def print_info(self):
         print(f"nsource: {self.n_source}")
         if self.n_source > 0:
             print(f"first and last ele: {self.ele_groups[0][0]}, {self.ele_groups[0][-1]}")
 
         print(f"nsink: {self.n_sink}")
         if self.n_sink > 0:
@@ -3534,46 +3545,46 @@
     In addition, there are no complete time info in the *.th files,
     so the TimeHistory class is also used to bind the time info and
     provide additional functions.
     """
     @property
     def source_eles(self):
         return self.source_sink_in.ele_groups[0]
-    
+
     @property
     def sink_eles(self):
         return self.source_sink_in.ele_groups[1]
-    
+
     @property
     def nsource(self):
         return self.source_sink_in.n_source
-    
+
     @property
     def nsink(self):
         return self.source_sink_in.n_sink
 
     def __init__(self, vsource:TimeHistory, vsink:TimeHistory, msource:list):
         """initialize from TimeHistory objects,
         vsource: TimeHistory object for volume source
         vsink: TimeHistory object for volume sink
         msource: list of TimeHistory objects for mass source
-        
+
         Note that msource is different from SCHISM's native msource.th
-        because saving all tracers in one array is not convenient for 
-        subsequent processing; instead, each tracer is saved in a separate 
+        because saving all tracers in one array is not convenient for
+        subsequent processing; instead, each tracer is saved in a separate
         TimeHistory object in a list
         """
 
         # list of main attributes
         self.vsource = vsource
         self.vsink = vsink
         self.msource = msource
         self.ntracers = None
         self.source_sink_in = None
-                        
+
         # if vsource, vsink, and msources are properly set,
         # then ntracers and source_sink_in will be automatically set
         if vsource is not None:
             self.ntracers = len(msource)
             source_eles = vsource.df.columns.astype(int).values
         else:
             self.ntracers = 0
@@ -3596,15 +3607,15 @@
         else:
             if len(source_eles) != vsource_data.shape[1] + 1:
                 raise ValueError("source_eles and vsource_data must have the same number of elements")
         if vsink_data is None:
             vsink_data = np.zeros([nt, nsinks])
         else:
             if len(sink_eles) != vsink_data.shape[1] + 1:
-                raise ValueError("sink_eles and vsink_data must have the same number of elements")  
+                raise ValueError("sink_eles and vsink_data must have the same number of elements")
 
         # initialize a set of source/sink files from scratch
         nt = len(timedeltas)
         nsources = len(source_eles)
         nsinks = len(sink_eles)
         vsource = None
         vsink = None
@@ -3676,19 +3687,19 @@
         if source_sink_in.n_sink > 0:
             print('reading vsink\n')
             vsink = TimeHistory.from_file(
                 f"{source_dir}/vsink.th",
                 start_time_str=start_time_str,
                 columns=source_sink_in.ele_groups[1]
             )
-        
+
         source_sink = cls(vsource, vsink, msource)
         source_sink.check_consistency()
         return source_sink
-    
+
     def writer(self, output_dir):
         '''
         Write source/sink files to the output_dir.
         '''
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
 
@@ -3699,39 +3710,39 @@
             msource_total = self.msource[0].time
             for i in range(self.ntracers):
                 msource_total = np.c_[msource_total, self.msource[i].df.values]
             np.savetxt(f"{output_dir}/msource.th", msource_total)
 
         if self.vsink is not None:
             self.vsink.writer(f"{output_dir}/vsink.th")
-        
+
     def check_consistency(self):
         # check consistency of source_sink_in and vsource/vsink/msource
         if self.nsource == 0:
             if self.vsource is not None:
                 raise Exception('inconsistent number of sources in source_sink.in and vsource.th')
         else:
             if len(self.msource) != self.ntracers:
                 raise Exception('inconsistent number of sources in source_sink.in and msource.th')
             if self.nsource != self.msource[0].n_station:
                 raise Exception('inconsistent number of sources in source_sink.in and vsource.th')
             if self.nsource != self.vsource.n_station:
                 raise Exception('inconsistent number of sources in source_sink.in and vsource.th')
             if np.min(self.vsource.df.values, axis=None) < 0:
                 raise Exception('vsource must be positive')
-        
+
         if self.nsink == 0:
             if self.vsink is not None:
                 raise Exception('inconsistent number of sinks in source_sink.in and vsink.th')
         else:
             if self.nsink != self.vsink.n_station:
-                raise Exception('inconsistent number of sinks in source_sink.in and vsink.th')  
+                raise Exception('inconsistent number of sinks in source_sink.in and vsink.th')
             if np.max(self.vsink.df.values, axis=None) > 0:
                 raise Exception('vsink must be negative')
-    
+
     def __add__(self, other):
         '''
         Add source/sink other to source/sink self,
         retaining self's time stamps.
         '''
         A = self
         B = other
@@ -3751,15 +3762,15 @@
             vsource = A.vsource
             msource = A.msource
         else:  # both have source
             vsource = A.vsource + B.vsource  # using TimeHistory.__add__
             msource = [None] * A.ntracers
             for i in range(A.ntracers):  # also using TimeHistory.__add__, but with weights
                 msource[i] = A.msource[i].__add__(B.msource[i], weights=[A.vsource, B.vsource])
-        
+
         # most cases are trivial unless both A and B have sink
         if A.nsink == 0 and B.nsink == 0:  # neither has sink
             vsink = None
         elif A.nsink == 0:  # only B has sink
             vsink = B.vsink
         elif B.nsink == 0:  # only A has sink
             vsink = A.vsink
@@ -3820,8 +3831,8 @@
 
         # Check that the values of the resulting dataframe are correct
         common_columns = self.df_A.columns.intersection(self.df_B.columns)
         for col in common_columns:
             self.assertTrue(all(np.isclose(df_combined[col].loc[self.df_B.index], self.df_A[col].loc[self.df_B.index] + self.df_B[col], atol=1e-5)))
 
 if __name__ == "__main__":
-    unittest.main()
+    unittest.main()
```

### Comparing `pylib_essentials-0.0.4/pylib_essentials/utility_functions.py` & `pylib_essentials-0.0.5/pylib_essentials/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pylib_essentials-0.0.4/setup.py` & `pylib_essentials-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='pylib_essentials',
-    version='0.0.4',
+    version='0.0.5',
     description='The essentials of the experimental package of pylibs, which require minimum dependencies',
     license='MIT',
     packages=['pylib_essentials'],
     package_data={},
     install_requires=[
       'setuptools',
       'numpy',
```

