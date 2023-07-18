# Comparing `tmp/grassmanntn-1.2.1.tar.gz` & `tmp/grassmanntn-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassmanntn-1.2.1.tar", last modified: Wed Jul 12 07:39:46 2023, max compression
+gzip compressed data, was "grassmanntn-1.2.2.tar", last modified: Tue Jul 18 06:26:14 2023, max compression
```

## Comparing `grassmanntn-1.2.1.tar` & `grassmanntn-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-12 07:39:46.319229 grassmanntn-1.2.1/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.2.1/LICENSE.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-12 07:39:46.319229 grassmanntn-1.2.1/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.2.1/README.md
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-12 07:39:46.319229 grassmanntn-1.2.1/grassmanntn/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109008 2023-07-12 07:37:50.000000 grassmanntn-1.2.1/grassmanntn/__init__.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     6961 2023-07-04 06:49:49.000000 grassmanntn-1.2.1/grassmanntn/example.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132605 2023-07-06 08:59:36.000000 grassmanntn-1.2.1/grassmanntn/gauge2d.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.2.1/grassmanntn/param.py
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-12 07:39:46.319229 grassmanntn-1.2.1/grassmanntn.egg-info/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-12 07:39:46.000000 grassmanntn-1.2.1/grassmanntn.egg-info/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-12 07:39:46.000000 grassmanntn-1.2.1/grassmanntn.egg-info/SOURCES.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-12 07:39:46.000000 grassmanntn-1.2.1/grassmanntn.egg-info/dependency_links.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-12 07:39:46.000000 grassmanntn-1.2.1/grassmanntn.egg-info/requires.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-12 07:39:46.000000 grassmanntn-1.2.1/grassmanntn.egg-info/top_level.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-12 07:39:46.319229 grassmanntn-1.2.1/setup.cfg
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-12 07:39:27.000000 grassmanntn-1.2.1/setup.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-18 06:26:14.153402 grassmanntn-1.2.2/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.2.2/LICENSE.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-18 06:26:14.153402 grassmanntn-1.2.2/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      553 2023-06-26 04:06:04.000000 grassmanntn-1.2.2/README.md
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-18 06:26:14.153402 grassmanntn-1.2.2/grassmanntn/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109098 2023-07-13 04:03:14.000000 grassmanntn-1.2.2/grassmanntn/__init__.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     7455 2023-07-13 04:02:04.000000 grassmanntn-1.2.2/grassmanntn/example.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   134349 2023-07-13 03:54:48.000000 grassmanntn-1.2.2/grassmanntn/gauge2d.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.2.2/grassmanntn/param.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-07-18 06:26:14.153402 grassmanntn-1.2.2/grassmanntn.egg-info/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1325 2023-07-18 06:26:14.000000 grassmanntn-1.2.2/grassmanntn.egg-info/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      305 2023-07-18 06:26:14.000000 grassmanntn-1.2.2/grassmanntn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-07-18 06:26:14.000000 grassmanntn-1.2.2/grassmanntn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-07-18 06:26:14.000000 grassmanntn-1.2.2/grassmanntn.egg-info/requires.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-07-18 06:26:14.000000 grassmanntn-1.2.2/grassmanntn.egg-info/top_level.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-07-18 06:26:14.153402 grassmanntn-1.2.2/setup.cfg
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1895 2023-07-18 06:26:07.000000 grassmanntn-1.2.2/setup.py
```

### Comparing `grassmanntn-1.2.1/LICENSE.txt` & `grassmanntn-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.2.1/PKG-INFO` & `grassmanntn-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.2.1
+Version: 1.2.2
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_121.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_122.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.2.1/README.md` & `grassmanntn-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.2.1/grassmanntn/__init__.py` & `grassmanntn-1.2.2/grassmanntn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,14 +321,15 @@
         print(indent+"     density:",self.nnz,"/",self.size,"~",self.nnz/self.size*100,"%")
         print(indent+"  statistics:",self.statistics)
         print(indent+"      format:",self.format)
         print(indent+"     encoder:",self.encoder)
         print(indent+"      memory:",memory_display(sys.getsizeof(self.data)+sys.getsizeof(self)))
         print(indent+"        norm:",self.norm)
         print(indent+"     entries:")
+        print(indent+" [coords]  [values]")
         iterator = np.nditer(self, flags=['multi_index'])
         for element in iterator:
             coords = iterator.multi_index
             if(np.abs(element.item())>numer_display_cutoff):
                 print(indent+"\t",coords,clean_format(element.item()))
         print()
 
@@ -630,14 +631,15 @@
         print(indent+"     density:",self.nnz,"/",self.size,"~",self.nnz/self.size*100,"%")
         print(indent+"  statistics:",self.statistics)
         print(indent+"      format:",self.format)
         print(indent+"     encoder:",self.encoder)
         print(indent+"      memory:",memory_display(sys.getsizeof(self.data)+sys.getsizeof(self)))
         print(indent+"        norm:",self.norm)
         print(indent+"     entries:")
+        print(indent+" [coords]  [values]")
 
         C = self.coords
         V = self.value
         for elem in range(self.nnz):
             if(np.abs(V[elem])>numer_display_cutoff):
                 print(indent+"\t",C[elem],clean_format(V[elem]))
         print()
```

### Comparing `grassmanntn-1.2.1/grassmanntn/example.py` & `grassmanntn-1.2.2/grassmanntn/example.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,44 +67,47 @@
 parse.add_argument('--cgsteps', default=5,   type=int)
 parse.add_argument('--Dcutz',   default=32,  type=int)
 parse.add_argument('--Dcutxy',  default=32,  type=int)
 parse.add_argument('--boundary_conditions', default="anti-periodic")
 parse.add_argument('--clear_screen', default=False, action='store_true')
 parse.add_argument('--cls', default=False, action='store_true')
 parse.add_argument('--show_progress', default=False, action='store_true')
+parse.add_argument('--sp', default=False, action='store_true')
+parse.add_argument('--trg', default=False, action='store_true')
+parse.add_argument('--TRG', default=False, action='store_true')
 
 args = parse.parse_args()
 
 
 #:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::#
 #:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::#
 #:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::#
 
 if args.clear_screen or args.cls:
     os.system('clear')
 
-if args.show_progress:
-    gtn.progress_bar_enabled = True
-else:
-    gtn.progress_bar_enabled = True #False
+gtn.progress_bar_enabled = args.show_progress or args.sp
+
+doTRG = args.trg or args.TRG
+
     
 β = args.beta             # inverse coupling
 m = args.mass             # mass
 μ = args.mu               # chemical potential
 q = args.charge           # charge
 a = args.spacing          # lattice spacing
 Nf = args.Nf              # fermion species
 Nphi = args.K             # Z_K group
 Zcut  = args.Dcutz        # Zcut for flavors
 XYcut = args.Dcutxy       # XYcut for TRG
 cgsteps = args.cgsteps    # the number of 2dtrgs
 bc = args.boundary_conditions
 
 print(
-    " _parameters: β="+str(β)
+    " parameters: β="+str(β)
     +", m="+str(m)
     +", κ="+str(gtn.clean_format(1.0/(2*m+4)))
     +", μ="+str(μ)
     +", q="+str(q)
     +", a="+str(a)
     +", Nf="+str(Nf)
     +", Z_"+str(Nphi)
@@ -114,15 +117,15 @@
     )
 
 t0 = time.time()
 T, err = gauge.tensor_preparation(Nphi=Nphi, beta=β, Nf=Nf, spacing=a, mass=m, charge=q, mu=μ, mute=True)
 logNorm = 0
 vol = 1
 
-print(" _initial_tensor:",(T.shape[0],T.shape[1]),"   ",'{:.3g}'.format(err),"   ",gtn.time_display(time.time()-t0))
+print(" initial_tensor:",(T.shape[0],T.shape[1]),"   ",'{:.3g}'.format(err),"   ",gtn.time_display(time.time()-t0))
 
 #:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::#
 #                      Flavor Coarse-graining Procedure                       #
 #:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::#
 
 Log2Nf = int(np.log2(Nf))
 intermediate_dcut=Zcut
@@ -130,40 +133,50 @@
     
     t0 = time.time()
     T, Tnorm, err = gauge.hotrg3dz(T,T,Zcut,intermediate_dcut=intermediate_dcut,iternum=i
                                         ,error_test=True
                                         )
     logNorm = 2*logNorm + np.log(Tnorm)
 
-    print(" _flavor_cg:",(T.shape[0],T.shape[1]),"   ",'{:.3g}'.format(err),"   ",gtn.time_display(time.time()-t0))
+    print(" flavor_cg:",(T.shape[0],T.shape[1]),"   ",'{:.3g}'.format(err),"   ",gtn.time_display(time.time()-t0))
 
 T = gauge.zcap(T)
 
 #:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::#
 #                         2D Coarse-graining Procedure                        #
 #:::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::::#
 
 F = gauge.logZ(T,boundary_conditions=bc)+logNorm
 
 cgxfirst = T.shape[0] > T.shape[1]
 
-print(" trg:",vol,β,m,μ,q,a,Nf,Nphi,"   ",np.real(F),"   ",np.imag(F),"   ",(T.shape[0],T.shape[1]))
+process = ''
+
+print("   _ini:",vol,β,m,μ,q,a,Nf,Nphi,"   ",np.real(F),"   ",np.imag(F),"   ",(T.shape[0],T.shape[1]))
 for i in range(cgsteps):
     t0 = time.time()
     direction=""
-    if cgxfirst :
-        if i%2==0 :
-            T, Tnorm, err = gauge.atrg2dx(T,T,XYcut,iternum=i,error_test=True)
-        else:
-            T, Tnorm, err = gauge.atrg2dy(T,T,XYcut,iternum=i,error_test=True)
+    if doTRG:
+        T, Tnorm, err = gauge.trg(T,XYcut,iternum=i,error_test=True)
+        process = '   _trg'
     else:
-        if i%2==0 :
-            T, Tnorm, err = gauge.atrg2dy(T,T,XYcut,iternum=i,error_test=True)
+        if cgxfirst :
+            if i%2==0 :
+                T, Tnorm, err = gauge.atrg2dx(T,T,XYcut,iternum=i,error_test=True)
+                process = ' _atrgx'
+            else:
+                T, Tnorm, err = gauge.atrg2dy(T,T,XYcut,iternum=i,error_test=True)
+                process = ' _atrgy'
         else:
-            T, Tnorm, err = gauge.atrg2dx(T,T,XYcut,iternum=i,error_test=True)
+            if i%2==0 :
+                T, Tnorm, err = gauge.atrg2dy(T,T,XYcut,iternum=i,error_test=True)
+                process = ' _atrgy'
+            else:
+                T, Tnorm, err = gauge.atrg2dx(T,T,XYcut,iternum=i,error_test=True)
+                process = ' _atrgx'
 
     vol = 2**(i+1)
     logNorm = 2*logNorm + np.log(Tnorm)
     F = (gauge.logZ(T,bc)+logNorm)/vol
 
     #print(gtn.clean_format(F))
-    print(" trg:",vol,β,m,μ,q,a,Nf,Nphi,"   ",np.real(F),"   ",np.imag(F),"   ",(T.shape[0],T.shape[1]),"   ",'{:.3g}'.format(err),"   ",gtn.time_display(time.time()-t0))
+    print(process+":",vol,β,m,μ,q,a,Nf,Nphi,"   ",np.real(F),"   ",np.imag(F),"   ",(T.shape[0],T.shape[1]),"   ",'{:.3g}'.format(err),"   ",gtn.time_display(time.time()-t0))
```

### Comparing `grassmanntn-1.2.1/grassmanntn/gauge2d.py` & `grassmanntn-1.2.2/grassmanntn/gauge2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1453,36 +1453,48 @@
 
     return np.log(Z)
 
 ####################################################
 ##                       TRG                      ##
 ####################################################
 
-def trg(T,dcut=16):
+def trg(T,dcut=64,iternum=None,error_test=False):
+
+    process_name = "trg"
+    if iternum != None:
+        process_name = process_name+"["+str(iternum)+"]"
+    process_length = 10
+    process_color = "purple"
+    step = 1
+    s00 = time.time()
+    gtn.progress_space() # << Don't remove this. This is for the gtn.show_progress!
 
     # mandatory properties of T:
     #    - shape = (nx,ny,nx,ny)
     #    - statistics = (1,1,-1,-1)
 
     if [T.shape[0],T.shape[1]] != [T.shape[2],T.shape[3]] :
         error("Error[trg]: The shape must be of the form (m,n,m,n)!")
 
-    if make_list(T.statistics) != [1,1,-1,-1] :
+    if gtn.make_list(T.statistics) != [1,1,-1,-1] :
         error("Error[trg]: The statistics must be (1,1,-1,-1)!")
 
     #===============================================================================#
     #   Step 1: Rearrange the tensor legs in two ways                               #
     #===============================================================================#
     
+    step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
     T1 = gtn.einsum('ijkl->jkli',T)
     T2 = gtn.einsum('ijkl->klij',T)
 
+    step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
     U1,S1,V1 = T1.svd('ab|cd',dcut)
     U2,S2,V2 = T2.svd('ab|cd',dcut)
 
+    step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
     #
     #                             j                                     j
     #                             ↑                                     ↑
     #        j                    ↑                                     ↑
     #        ↑              k → →(U1)                                 (V2)→ → i
     #        ↑                      ↘                                 ↗
     #  k → →(T)→ → i    =             ↘              =              ↗
@@ -1493,18 +1505,20 @@
     #                                     l                     l
     #
 
     #===============================================================================#
     #   Step 2: Multiply sqrt(S) into U and V                                       #
     #===============================================================================#
     
+    step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
     sqrtS = gtn.sqrt(S1)
     U1 = gtn.einsum('abx,xc->abc',U1,sqrtS)
     V1 = gtn.einsum('ax,xbc->abc',sqrtS,V1)
 
+    step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
     sqrtS = gtn.sqrt(S2)
     U2 = gtn.einsum('abx,xc->abc',U2,sqrtS)
     V2 = gtn.einsum('ax,xbc->abc',sqrtS,V2)
     
     #===============================================================================#
     #   Step 3: Renormalization                                                     #
     #===============================================================================#
@@ -1521,36 +1535,47 @@
     #            ↑           ↑
     #          (V2)→ → x → →(U1)
     #          ↗               ↘
     #        ↗                   ↘
     #      l                       i
     #
     
+    step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
     VV = gtn.einsum('kwz,lxw->lxzk',V1,V2);
+    step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
     UU = gtn.einsum('yxi,zyj->jzxi',U1,U2);
-    T2 = gtn.einsum('lxzk,jzxi->ijkl',VV,UU,debug_mode=True);
+    step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
+    T2 = gtn.einsum('lxzk,jzxi->ijkl',VV,UU);
+    step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
 
-    tr1 = gtn.einsum('ijkl,klij',T,T);
-    tr2 = gtn.einsum('ijij',T2);
-    err = np.abs(tr1-tr2)
-    print("Error:",err)
+    if error_test :
+        Z1 = gtn.einsum('ijkl,klij',T,T);
+        Z2 = gtn.einsum('ijij',T2);
+        err = np.abs(1-Z2/Z1)
+    #print("Error:",err)
+    
+    gtn.clear_progress()
+    gtn.tab_up()
     
     Tnorm = T2.norm
     T2 = gtn.dense(T2)
     T2.data = T2.data/Tnorm
     if type(T) == gtn.sparse :
         T2 = gtn.sparse(T2)
     
-    return T2, Tnorm
+    if error_test :
+        return T2, Tnorm, err
+    else:
+        return T2, Tnorm
 
 ####################################################
 ##                     2D ATRG                    ##
 ####################################################
 
-def atrg2dy(T1,T2,dcut=16,intermediate_dcut=None,iternum=None,error_test=False,alignment="y"):
+def atrg2dy(T1,T2,dcut=64,intermediate_dcut=None,iternum=None,error_test=False,alignment="y"):
     
     T1ori = T1.copy()
     T2ori = T2.copy()
     
     process_name = "atrg2d"+alignment
     if iternum != None:
         process_name = process_name+"["+str(iternum)+"]"
@@ -1652,15 +1677,15 @@
     T.data = T.data/Tnorm
 
     if error_test :
         return T, Tnorm, error
     else :
         return T, Tnorm
 
-def atrg2dx(T1,T2,dcut=16,intermediate_dcut=None,iternum=None,error_test=False):
+def atrg2dx(T1,T2,dcut=64,intermediate_dcut=None,iternum=None,error_test=False):
     T1 = gtn.einsum('ijkl->jikl',T1)
     T1 = gtn.einsum('jikl->jilk',T1)
     T2 = gtn.einsum('ijkl->jikl',T2)
     T2 = gtn.einsum('jikl->jilk',T2)
     if error_test :
         T, Tnorm, err = atrg2dy(T1,T2,dcut,intermediate_dcut,iternum,True,alignment="x")
     else:
@@ -1672,15 +1697,15 @@
     else :
         return T, Tnorm
 
 ####################################################
 ##                     3D ATRG                    ##
 ####################################################
 
-def hotrg3dz(T1,T2,dcut=16,intermediate_dcut=None,iternum=None,error_test=False,svd_only=False,print_svd=False):
+def hotrg3dz(T1,T2,dcut=64,intermediate_dcut=None,iternum=None,error_test=False,svd_only=False,print_svd=False):
     dt_string = datetime.now().strftime("%y%m%d.%H%M%S.%f")
 
     if print_svd :
         if(not os.path.exists("data/")):
             os.mkdir("data/")
         directory = "data/hotrg3dz_svd"+dt_string+".txt"
         fsvd = open(directory, "a")
```

### Comparing `grassmanntn-1.2.1/grassmanntn/param.py` & `grassmanntn-1.2.2/grassmanntn/param.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.2.1/grassmanntn.egg-info/PKG-INFO` & `grassmanntn-1.2.2/grassmanntn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.2.1
+Version: 1.2.2
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_121.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_122.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.2.1/setup.py` & `grassmanntn-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'grassmanntn',         # How you named your package folder (MyLib)
   packages = ['grassmanntn'],   # Chose the same as "name"
-  version = '1.2.1',      # Start with a small number and increase it with every change you make
+  version = '1.2.2',      # Start with a small number and increase it with every change you make
   license='Apache',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a Python library for Grassmann tensor network computation',   # Give a short description about your library
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Atis Yosprakob',                   # Type in your name
   author_email = 'yosprakob2@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ayosprakob/grassmanntn',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_121.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_122.tar.gz',    # I explain this later on
   keywords = ['physics', 'lattice', 'gauge theory', 'tensor network', 'grassmann'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'sparse',
           'opt_einsum',
       ],
   classifiers=[
```

