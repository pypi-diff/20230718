# Comparing `tmp/ec_ecology_toolbox-0.0.6.tar.gz` & `tmp/ec_ecology_toolbox-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec_ecology_toolbox-0.0.6.tar", last modified: Sat Jun  3 03:14:09 2023, max compression
+gzip compressed data, was "ec_ecology_toolbox-0.0.8.tar", last modified: Tue Jul 18 05:04:25 2023, max compression
```

## Comparing `ec_ecology_toolbox-0.0.6.tar` & `ec_ecology_toolbox-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:09.662514 ec_ecology_toolbox-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-03 03:13:53.000000 ec_ecology_toolbox-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-03 03:14:09.662514 ec_ecology_toolbox-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-03 03:13:53.000000 ec_ecology_toolbox-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:09.662514 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-03 03:14:09.000000 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-03 03:14:09.000000 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 03:14:09.000000 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 03:14:09.000000 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-03 03:14:09.000000 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 03:14:09.000000 ec_ecology_toolbox-0.0.6/ec_ecology_toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-03 03:13:53.000000 ec_ecology_toolbox-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-03 03:14:09.662514 ec_ecology_toolbox-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-03 03:13:53.000000 ec_ecology_toolbox-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:09.662514 ec_ecology_toolbox-0.0.6/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-03 03:13:53.000000 ec_ecology_toolbox-0.0.6/source/wrapper.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 03:14:09.662514 ec_ecology_toolbox-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-03 03:13:53.000000 ec_ecology_toolbox-0.0.6/tests/test_toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:04:25.392547 ec_ecology_toolbox-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-18 05:04:10.000000 ec_ecology_toolbox-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-18 05:04:25.392547 ec_ecology_toolbox-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-18 05:04:10.000000 ec_ecology_toolbox-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:04:25.392547 ec_ecology_toolbox-0.0.8/ec_ecology_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-18 05:04:25.000000 ec_ecology_toolbox-0.0.8/ec_ecology_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-18 05:04:25.000000 ec_ecology_toolbox-0.0.8/ec_ecology_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 05:04:25.000000 ec_ecology_toolbox-0.0.8/ec_ecology_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 05:04:25.000000 ec_ecology_toolbox-0.0.8/ec_ecology_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 05:04:25.000000 ec_ecology_toolbox-0.0.8/ec_ecology_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 05:04:25.000000 ec_ecology_toolbox-0.0.8/ec_ecology_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-18 05:04:10.000000 ec_ecology_toolbox-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-18 05:04:25.392547 ec_ecology_toolbox-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-18 05:04:10.000000 ec_ecology_toolbox-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:04:25.392547 ec_ecology_toolbox-0.0.8/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-07-18 05:04:10.000000 ec_ecology_toolbox-0.0.8/source/wrapper.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:04:25.392547 ec_ecology_toolbox-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-07-18 05:04:10.000000 ec_ecology_toolbox-0.0.8/tests/test_toolbox.py
```

### Comparing `ec_ecology_toolbox-0.0.6/LICENSE` & `ec_ecology_toolbox-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ec_ecology_toolbox-0.0.6/README.md` & `ec_ecology_toolbox-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ec_ecology_toolbox-0.0.6/setup.py` & `ec_ecology_toolbox-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
-__version__ = "0.0.6"
+__version__ = "0.0.8"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
```

### Comparing `ec_ecology_toolbox-0.0.6/source/wrapper.cc` & `ec_ecology_toolbox-0.0.8/source/wrapper.cc`

 * *Files 19% similar despite different names*

```diff
@@ -27,56 +27,80 @@
               (optional) The epsilon value to use (if you want epsilon-lexicase selection probabilities; default value is 0, which is equivalent to standard lexicase selection).  
 
             Returns
             -------
             List of floats
               The probabilities of each individual in pop being selected by lexicase selection.            
             )mydelimiter",
-          py::arg("pop"), py::arg("epsilon") = 0.0, py::arg("binary") = false);
-
-    m.def("LexicaseFitnessIndividual", &LexicaseFitnessIndividual<emp::vector<double>>, 
+          py::arg("pop"), py::arg("epsilon") = 0.0);//, py::arg("binary") = false);
+    
+    m.def("UnoptimizedLexicaseFitness", &UnoptimizedLexicaseFitness<emp::vector<double>>, 
             R"mydelimiter(
-            Returns the probability that a single individual is selected by lexicase selection.
+            Return a vector containing the probability that each member of the population will be selected by lexicase selection or epsilon lexicase selection.
+            
+            For example, LexicaseFitness([[1, 2, 2], [2, 1, 2], [0, 0, 0]]) will return [.5, .5, 0], because the first two score vectors each have a 50% chance
+            of being chosen and the third has no chance of being chosen.
 
             Note: calculating these probabilities is an NP-Hard problem (Dolson, 2023). This function is optimized, but if you try to use it with too large of input
-            it might take a very a long time. This version is faster than LexicaseFitness if you just need the probability for a single individual, but is still worst-case O(N!)
+            it might take a very a long time.
 
             Parameters
             ----------
             pop: list of lists of floats 
-              The scores of a population on each test case/fitness criterion.
-            i: int
-              The index of the individual in pop to calculate selection probability for
+              The scores of each member of the population population on each test case/fitness criterion.
             epsilon: float
               (optional) The epsilon value to use (if you want epsilon-lexicase selection probabilities; default value is 0, which is equivalent to standard lexicase selection).  
-            
+
             Returns
             -------
-            float
-              The probability of individual i being selected by lexicase selection.
-            )mydelimiter", 
-          py::arg("pop"), py::arg("i"), py::arg("epsilon") = 0.0);
+            List of floats
+              The probabilities of each individual in pop being selected by lexicase selection.            
+            )mydelimiter",
+          py::arg("pop"), py::arg("epsilon") = 0.0);//, py::arg("binary") = false);
 
-        m.def("LexicaseFitnessIndividualBinary", &SolveBinary<emp::vector<double>>, 
+    m.def("LexicaseFitnessIndividual", &LexicaseFitnessIndividual<emp::vector<double>>, 
             R"mydelimiter(
-            Returns the probability that a single individual is selected by lexicase selection in the case where all scores are either 0 or 1.
+            Returns the probability that a single individual is selected by lexicase selection.
+
+            Note: calculating these probabilities is an NP-Hard problem (Dolson, 2023). This function is optimized, but if you try to use it with too large of input
+            it might take a very a long time. This version is faster than LexicaseFitness if you just need the probability for a single individual, but is still worst-case O(N!)
 
             Parameters
             ----------
             pop: list of lists of floats 
               The scores of a population on each test case/fitness criterion.
             i: int
               The index of the individual in pop to calculate selection probability for
+            epsilon: float
+              (optional) The epsilon value to use (if you want epsilon-lexicase selection probabilities; default value is 0, which is equivalent to standard lexicase selection).  
             
             Returns
             -------
             float
               The probability of individual i being selected by lexicase selection.
             )mydelimiter", 
-          py::arg("pop"), py::arg("i"));
+          py::arg("pop"), py::arg("i"), py::arg("epsilon") = 0.0);
+
+        // m.def("LexicaseFitnessIndividualBinary", &SolveBinary<emp::vector<double>>, 
+        //     R"mydelimiter(
+        //     Returns the probability that a single individual is selected by lexicase selection in the case where all scores are either 0 or 1.
+
+        //     Parameters
+        //     ----------
+        //     pop: list of lists of floats 
+        //       The scores of a population on each test case/fitness criterion.
+        //     i: int
+        //       The index of the individual in pop to calculate selection probability for
+            
+        //     Returns
+        //     -------
+        //     float
+        //       The probability of individual i being selected by lexicase selection.
+        //     )mydelimiter", 
+        //   py::arg("pop"), py::arg("i"));
 
     m.def("SharingFitness", &SharingFitness<emp::vector<double>>, 
             R"mydelimiter(
             Return a vector containing the probability that each member of the population will be selected under tournament selection with fitness sharing.
 
             The numbers in the pop parameter are assumed to be scores on a set of test cases/fitness criteria/tasks.
             Similarity will be calculated as the euclidean distance between these scores.
```

### Comparing `ec_ecology_toolbox-0.0.6/tests/test_toolbox.py` & `ec_ecology_toolbox-0.0.8/tests/test_toolbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,39 +26,39 @@
                         #   (6, 20, 30),
                         #   (7, 30, 30),
                         #   (8, 40, 40)
                           ])
 def test_benchmark_lex_prob(benchmark, seed, n, m):
     random.seed(seed)
     benchmark(eco.LexicaseFitness,
-              [[random.randint(0, 1) for i in range(n)] for j in range(m)], 0, True)
-
-@pytest.mark.parametrize("seed, n, m",
-                         [(1, 10, 10),
-                          (2, 10, 20),
-                          (3, 10, 30),
-                          (4, 20, 10),
-                          (5, 20, 20),
-                          (6, 3, 20),                          
-                          (7, 20, 3),                          
-                          (8, 8, 20),                          
-                          (9, 20, 8),                          
-                        #   (6, 20, 30),
-                        #   (7, 30, 30),
-                        #   (8, 40, 40)
-                          ])
-def test_benchmark_binary_lex_prob(benchmark, seed, n, m):
-    random.seed(seed)
-    benchmark(eco.LexicaseFitnessIndividualBinary,
               [[random.randint(0, 1) for i in range(n)] for j in range(m)], 0)
 
+# @pytest.mark.parametrize("seed, n, m",
+#                          [(1, 10, 10),
+#                           (2, 10, 20),
+#                           (3, 10, 30),
+#                           (4, 20, 10),
+#                           (5, 20, 20),
+#                           (6, 3, 20),                          
+#                           (7, 20, 3),                          
+#                           (8, 8, 20),                          
+#                           (9, 20, 8),                          
+#                         #   (6, 20, 30),
+#                         #   (7, 30, 30),
+#                         #   (8, 40, 40)
+#                           ])
+# def test_benchmark_binary_lex_prob(benchmark, seed, n, m):
+#     random.seed(seed)
+#     benchmark(eco.LexicaseFitnessIndividualBinary,
+#               [[random.randint(0, 1) for i in range(n)] for j in range(m)], 0)
+
 
 def test_lex_prob_individual():
     assert eco.LexicaseFitnessIndividual([[1, 2, 3]], 0, 1) == 1
-    assert eco.LexicaseFitnessIndividual([[1, 2, 3], [2, 1, 4]], 1, 1) == .5
+    assert eco.LexicaseFitnessIndividual([[1, 2, 3], [2, 1, 4]], 1, 1.1) == .5
     assert eco.LexicaseFitnessIndividual([[1, 2, 3], [2, 1, 4]], 0) == pytest.approx(.3333333333)
     assert eco.LexicaseFitnessIndividual([[1, 2, 3], [2, 1, 4]], 1) == pytest.approx(.6666666667)
 
 
 def test_sharing_prob():
     result = eco.SharingFitness([[1, 2, 3], [1, 2, 3], [3, 2, 1]])
     assert result[2] == pytest.approx(5/9)
```

