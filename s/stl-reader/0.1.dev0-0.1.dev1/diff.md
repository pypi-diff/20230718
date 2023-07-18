# Comparing `tmp/stl-reader-0.1.dev0.tar.gz` & `tmp/stl-reader-0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stl-reader-0.1.dev0.tar", last modified: Tue Jul 18 20:16:21 2023, max compression
+gzip compressed data, was "stl-reader-0.1.dev1.tar", last modified: Tue Jul 18 21:03:04 2023, max compression
```

## Comparing `stl-reader-0.1.dev0.tar` & `stl-reader-0.1.dev1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-18 20:16:21.366658 stl-reader-0.1.dev0/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1088 2023-07-18 18:04:45.000000 stl-reader-0.1.dev0/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     5847 2023-07-18 20:16:21.366658 stl-reader-0.1.dev0/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     5196 2023-07-18 20:15:43.000000 stl-reader-0.1.dev0/README.rst
--rw-rw-r--   0 alex      (1000) alex      (1000)     1352 2023-07-18 19:45:35.000000 stl-reader-0.1.dev0/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-18 20:16:21.366658 stl-reader-0.1.dev0/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     2219 2023-07-18 17:56:30.000000 stl-reader-0.1.dev0/setup.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-18 20:16:21.366658 stl-reader-0.1.dev0/stl_reader/
--rw-rw-r--   0 alex      (1000) alex      (1000)       63 2023-07-18 19:31:31.000000 stl-reader-0.1.dev0/stl_reader/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)   438109 2023-07-18 19:41:45.000000 stl-reader-0.1.dev0/stl_reader/_stlfile_wrapper.c
--rw-rw-r--   0 alex      (1000) alex      (1000)      217 2023-07-18 16:21:38.000000 stl-reader-0.1.dev0/stl_reader/_version.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2178 2023-07-18 17:41:31.000000 stl-reader-0.1.dev0/stl_reader/hash96.h
--rw-rw-r--   0 alex      (1000) alex      (1000)     3771 2023-07-18 19:39:05.000000 stl-reader-0.1.dev0/stl_reader/reader.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5083 2023-07-18 17:40:33.000000 stl-reader-0.1.dev0/stl_reader/stlfile.c
--rw-rw-r--   0 alex      (1000) alex      (1000)     1360 2023-07-18 18:08:01.000000 stl-reader-0.1.dev0/stl_reader/stlfile.h
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-18 20:16:21.366658 stl-reader-0.1.dev0/stl_reader.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     5847 2023-07-18 20:16:21.000000 stl-reader-0.1.dev0/stl_reader.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      391 2023-07-18 20:16:21.000000 stl-reader-0.1.dev0/stl_reader.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-18 20:16:21.000000 stl-reader-0.1.dev0/stl_reader.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       13 2023-07-18 20:16:21.000000 stl-reader-0.1.dev0/stl_reader.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       11 2023-07-18 20:16:21.000000 stl-reader-0.1.dev0/stl_reader.egg-info/top_level.txt
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-18 20:16:21.366658 stl-reader-0.1.dev0/tests/
--rw-rw-r--   0 alex      (1000) alex      (1000)      861 2023-07-18 19:39:05.000000 stl-reader-0.1.dev0/tests/test_reader.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-18 21:03:04.234921 stl-reader-0.1.dev1/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1088 2023-07-18 18:04:45.000000 stl-reader-0.1.dev1/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)       85 2023-07-18 20:59:21.000000 stl-reader-0.1.dev1/MANIFEST.in
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5847 2023-07-18 21:03:04.234921 stl-reader-0.1.dev1/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5196 2023-07-18 20:15:43.000000 stl-reader-0.1.dev1/README.rst
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1352 2023-07-18 19:45:35.000000 stl-reader-0.1.dev1/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-18 21:03:04.234921 stl-reader-0.1.dev1/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2319 2023-07-18 20:56:02.000000 stl-reader-0.1.dev1/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-18 21:03:04.234921 stl-reader-0.1.dev1/stl_reader/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       63 2023-07-18 19:31:31.000000 stl-reader-0.1.dev1/stl_reader/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2646 2023-07-18 18:09:24.000000 stl-reader-0.1.dev1/stl_reader/_stlfile_wrapper.pyx
+-rw-rw-r--   0 alex      (1000) alex      (1000)      217 2023-07-18 21:02:44.000000 stl-reader-0.1.dev1/stl_reader/_version.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2178 2023-07-18 17:41:31.000000 stl-reader-0.1.dev1/stl_reader/hash96.h
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3771 2023-07-18 19:39:05.000000 stl-reader-0.1.dev1/stl_reader/reader.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5252 2023-07-18 20:31:44.000000 stl-reader-0.1.dev1/stl_reader/stlfile.c
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1360 2023-07-18 18:08:01.000000 stl-reader-0.1.dev1/stl_reader/stlfile.h
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-18 21:03:04.234921 stl-reader-0.1.dev1/stl_reader.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5847 2023-07-18 21:03:04.000000 stl-reader-0.1.dev1/stl_reader.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      405 2023-07-18 21:03:04.000000 stl-reader-0.1.dev1/stl_reader.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-18 21:03:04.000000 stl-reader-0.1.dev1/stl_reader.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       13 2023-07-18 21:03:04.000000 stl-reader-0.1.dev1/stl_reader.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       11 2023-07-18 21:03:04.000000 stl-reader-0.1.dev1/stl_reader.egg-info/top_level.txt
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-18 21:03:04.234921 stl-reader-0.1.dev1/tests/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      861 2023-07-18 19:39:05.000000 stl-reader-0.1.dev1/tests/test_reader.py
```

### Comparing `stl-reader-0.1.dev0/LICENSE` & `stl-reader-0.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `stl-reader-0.1.dev0/PKG-INFO` & `stl-reader-0.1.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stl-reader
-Version: 0.1.dev0
+Version: 0.1.dev1
 Summary: Read in STL files
 Home-page: https://github.com/pyvista/pymeshfix
 Author: PyVista Developers
 Author-email: info@pyvista.org
 License: MIT
 Keywords: read stl
 Classifier: Development Status :: 4 - Beta
```

### Comparing `stl-reader-0.1.dev0/README.rst` & `stl-reader-0.1.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `stl-reader-0.1.dev0/pyproject.toml` & `stl-reader-0.1.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stl-reader-0.1.dev0/setup.py` & `stl-reader-0.1.dev1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,10 +70,13 @@
                 language="c",
                 extra_compile_args=extra_compile_args,
                 define_macros=macros,
                 include_dirs=[np.get_include()],
             )
         ]
     ),
+    package_data={
+        "stl_reader": ["*.pyx"],  # include all .pyx files in the package
+    },
     keywords="read stl",
     install_requires=["numpy>1.11.0"],
 )
```

### Comparing `stl-reader-0.1.dev0/stl_reader/hash96.h` & `stl-reader-0.1.dev1/stl_reader/hash96.h`

 * *Files identical despite different names*

### Comparing `stl-reader-0.1.dev0/stl_reader/reader.py` & `stl-reader-0.1.dev1/stl_reader/reader.py`

 * *Files identical despite different names*

### Comparing `stl-reader-0.1.dev0/stl_reader/stlfile.c` & `stl-reader-0.1.dev1/stl_reader/stlfile.c`

 * *Files 17% similar despite different names*

```diff
@@ -22,183 +22,177 @@
 THE SOFTWARE.
 
 Also modified by Alex Kaszynski 2023 to check is the file is ASCII and the
 elimination of stderr.
 
 */
 
+#include <stdint.h>
 #include <stdio.h>
 #include <stdlib.h>
-#include <stdint.h>
 #include <string.h>
-#include "stlfile.h"
+
 #include "hash96.h"
+#include "stlfile.h"
 
 #define STL_INVALID 0
 #define STL_ASCII 1
 #define STL_BINARY 2
 
 typedef int STL_STATUS;
 
-static uint32_t
-get16(uint8_t *buf)
-{
-	return (uint32_t)buf[0] + ((uint32_t)buf[1]<<8);
+static uint32_t get16(uint8_t *buf) {
+  return (uint32_t)buf[0] + ((uint32_t)buf[1] << 8);
 }
 
-static uint32_t
-get32(uint8_t *buf)
-{
-	return (uint32_t)buf[0] + ((uint32_t)buf[1]<<8) + ((uint32_t)buf[2]<<16) + ((uint32_t)buf[3]<<24);
+static uint32_t get32(uint8_t *buf) {
+  return (uint32_t)buf[0] + ((uint32_t)buf[1] << 8) + ((uint32_t)buf[2] << 16) +
+         ((uint32_t)buf[3] << 24);
 }
 
-static vertex_t
-vertex(uint32_t *verts, vertex_t nverts, vertex_t *vht, vertex_t vhtcap, uint32_t *vert)
-{
-	vertex_t *vip, vi;
-	vertex_t hash;
-	vertex_t i;
-
-	hash = final96(vert[0], vert[1], vert[2]);
-	for(i = 0; i < vhtcap; i++){
-		vip = vht + ((hash + i) & (vhtcap - 1));
-		vi = *vip;
-		if(vi == 0){
-			*vip = nverts+1;
-			return nverts;
-		}
-		vi--;
-		if(cmp96(vert, verts + 3*vi) == 0)
-			return vi;
-
-	}
-	return ~(vertex_t)0;
+static vertex_t vertex(uint32_t *verts, vertex_t nverts, vertex_t *vht,
+                       vertex_t vhtcap, uint32_t *vert) {
+  vertex_t *vip, vi;
+  vertex_t hash;
+  vertex_t i;
+
+  hash = final96(vert[0], vert[1], vert[2]);
+  for (i = 0; i < vhtcap; i++) {
+    vip = vht + ((hash + i) & (vhtcap - 1));
+    vi = *vip;
+    if (vi == 0) {
+      *vip = nverts + 1;
+      return nverts;
+    }
+    vi--;
+    if (cmp96(vert, verts + 3 * vi) == 0)
+      return vi;
+  }
+  return ~(vertex_t)0;
 }
 
-
-STL_STATUS check_stl_format(FILE *fp)
-{
-    if(fp == NULL){
-        printf("\n\tUnable to open the file");
-        return STL_INVALID;
+STL_STATUS check_stl_format(FILE *fp) {
+  if (fp == NULL) {
+    printf("\n\tUnable to open the file");
+    return STL_INVALID;
+  }
+
+  fseek(fp, 0, SEEK_END);
+  size_t fileSize = ftell(fp);
+  rewind(fp);
+
+  if (fileSize < 15) {
+    printf("\n\tThe STL file is not long enough (%zu bytes).\n", fileSize);
+    return STL_INVALID;
+  }
+
+  char sixBytes[7];
+  fread(sixBytes, 1, 6, fp);
+  sixBytes[6] = '\0';
+
+  if (strcmp(sixBytes, "solid ") == 0) {
+    char line[100];
+    fgets(line, 100, fp);
+    if (strncmp(line, "facet ", 6) == 0) {
+      return STL_ASCII;
     }
-
-    fseek(fp, 0, SEEK_END);
-    size_t fileSize = ftell(fp);
     rewind(fp);
+  }
 
-    if (fileSize < 15) {
-        printf("\n\tThe STL file is not long enough (%zu bytes).\n", fileSize);
-        return STL_INVALID;
-    }
-
-    char sixBytes[7];
-    fread(sixBytes, 1, 6, fp);
-    sixBytes[6] = '\0';
-
-    if(strcmp(sixBytes, "solid ") == 0){
-        char line[100];
-        fgets(line, 100, fp);
-        if(strncmp(line, "facet ", 6) == 0){
-            return STL_ASCII;
-        }
-        rewind(fp);
-    }
+  if (fileSize < 84) {
+    printf("\n\tThe STL file is not long enough (%zu bytes).\n", fileSize);
+    return STL_INVALID;
+  }
+
+  fseek(fp, 80, SEEK_SET);
+  uint32_t nTriangles;
+  fread(&nTriangles, sizeof(nTriangles), 1, fp);
+  if (fileSize != (84 + (nTriangles * 50))) {
+    return STL_INVALID;
+  }
 
-    if (fileSize < 84) {
-        printf("\n\tThe STL file is not long enough (%zu bytes).\n", fileSize);
-        return STL_INVALID;
-    }
-
-    fseek(fp, 80, SEEK_SET);
-    uint32_t nTriangles;
-    fread(&nTriangles, sizeof(nTriangles), 1, fp);
-    if (fileSize != (84 + (nTriangles * 50))){
-        return STL_INVALID;
-    }
-
-    fseek(fp, 0, SEEK_SET);
-    return STL_BINARY;
+  fseek(fp, 0, SEEK_SET);
+  return STL_BINARY;
 }
 
-
-int
-loadstl(FILE *fp, char *comment, float **vertp, vertex_t *nvertp, vertex_t **trip, uint16_t **attrp, triangle_t *ntrip)
-{
-	uint8_t buf[128];
-	triangle_t i, ti;
-	vertex_t *tris;
-	triangle_t ntris;
-	vertex_t *vht, vi, nverts, vhtcap;
-	uint32_t *verts;
-	uint16_t *attrs;
-
-    STL_STATUS format_status = check_stl_format(fp);
-    if(format_status == STL_INVALID) {
-        fprintf(stderr, "loadstl: Invalid or unrecognized STL file format\n");
-        return -2;
-    }
-
-	// the comment and triangle count
-	if(fread(buf, 84, 1, fp) != 1){
-		fprintf(stderr, "loadstl: short read at header\n");
-		return -1;
-	}
-
-	if(comment != NULL)
-		memcpy(comment, buf, 80);
-
-	ntris = get32(buf+80);
-
-	tris = malloc(ntris * 3*sizeof tris[0]);
-	attrs = malloc(ntris * sizeof attrs[0]);
-	verts = malloc(3*ntris * 3*sizeof verts[0]);
-
-	vhtcap = nextpow2(4*ntris);
-	vht = malloc(vhtcap * sizeof vht[0]);
-	memset(vht, 0, vhtcap * sizeof vht[0]);
-
-	/* fprintf(stderr, "loadstl: number of triangles: %u, vhtcap %d\n", ntris, vhtcap); */
-
-	nverts = 0;
-	for(i = 0; i < ntris; i++){
-		if(fread(buf, 50, 1, fp) != 1){
-			fprintf(stderr, "loadstl: short read at triangle %d/%d\n", i, ntris);
-			goto exit_fail;
-		}
-		// there's a normal vector at buf[0..11] which we are ignoring
-		for(ti = 0; ti < 3; ti++){
-			uint32_t vert[3];
-			vert[0] = get32(buf+12 + 4*3*ti);
-			vert[1] = get32(buf+12 + 4*3*ti+4);
-			vert[2] = get32(buf+12 + 4*3*ti+8);
-			vi = vertex(verts, nverts, vht, vhtcap, vert);
-			if(vi == ~(uint32_t)0){
-				fprintf(stderr, "loadstl: vertex hash full at triangle %d/%d\n", i, ntris);
-				goto exit_fail;
-			}
-			if(vi == nverts){
-				copy96(verts + 3*nverts, vert);
-				nverts++;
-			} else {
-			}
-			tris[3*i+ti] = vi;
-		}
-		attrs[i] = get16(buf + 48);
-	}
-
-	free(vht);
-	verts = realloc(verts, nverts * 3*sizeof verts[0]);
-	*vertp = (float *)verts;
-	*nvertp = nverts;
-	*trip = tris;
-	*attrp = attrs;
-	*ntrip = ntris;
-	return 0;
+int loadstl(FILE *fp, char *comment, float **vertp, vertex_t *nvertp,
+            vertex_t **trip, uint16_t **attrp, triangle_t *ntrip) {
+  uint8_t buf[128];
+  triangle_t i, ti;
+  vertex_t *tris;
+  triangle_t ntris;
+  vertex_t *vht, vi, nverts, vhtcap;
+  uint32_t *verts;
+  uint16_t *attrs;
+
+  STL_STATUS format_status = check_stl_format(fp);
+  if (format_status == STL_INVALID) {
+    fprintf(stderr, "loadstl: Invalid or unrecognized STL file format\n");
+    return -2;
+  }
+
+  // the comment and triangle count
+  if (fread(buf, 84, 1, fp) != 1) {
+    fprintf(stderr, "loadstl: short read at header\n");
+    return -1;
+  }
+
+  if (comment != NULL)
+    memcpy(comment, buf, 80);
+
+  ntris = get32(buf + 80);
+
+  tris = malloc(ntris * 3 * sizeof tris[0]);
+  attrs = malloc(ntris * sizeof attrs[0]);
+  verts = malloc(3 * ntris * 3 * sizeof verts[0]);
+
+  vhtcap = nextpow2(4 * ntris);
+  vht = malloc(vhtcap * sizeof vht[0]);
+  memset(vht, 0, vhtcap * sizeof vht[0]);
+
+  /* fprintf(stderr, "loadstl: number of triangles: %u, vhtcap %d\n", ntris,
+   * vhtcap); */
+
+  nverts = 0;
+  for (i = 0; i < ntris; i++) {
+    if (fread(buf, 50, 1, fp) != 1) {
+      fprintf(stderr, "loadstl: short read at triangle %d/%d\n", i, ntris);
+      goto exit_fail;
+    }
+    // there's a normal vector at buf[0..11] which we are ignoring
+    for (ti = 0; ti < 3; ti++) {
+      uint32_t vert[3];
+      vert[0] = get32(buf + 12 + 4 * 3 * ti);
+      vert[1] = get32(buf + 12 + 4 * 3 * ti + 4);
+      vert[2] = get32(buf + 12 + 4 * 3 * ti + 8);
+      vi = vertex(verts, nverts, vht, vhtcap, vert);
+      if (vi == ~(uint32_t)0) {
+        fprintf(stderr, "loadstl: vertex hash full at triangle %d/%d\n", i,
+                ntris);
+        goto exit_fail;
+      }
+      if (vi == nverts) {
+        copy96(verts + 3 * nverts, vert);
+        nverts++;
+      } else {
+      }
+      tris[3 * i + ti] = vi;
+    }
+    attrs[i] = get16(buf + 48);
+  }
+
+  free(vht);
+  verts = realloc(verts, nverts * 3 * sizeof verts[0]);
+  *vertp = (float *)verts;
+  *nvertp = nverts;
+  *trip = tris;
+  *attrp = attrs;
+  *ntrip = ntris;
+  return 0;
 
 exit_fail:
-	free(vht);
-	free(verts);
-	free(tris);
-	free(attrs);
-	return -1;
+  free(vht);
+  free(verts);
+  free(tris);
+  free(attrs);
+  return -1;
 }
```

### Comparing `stl-reader-0.1.dev0/stl_reader/stlfile.h` & `stl-reader-0.1.dev1/stl_reader/stlfile.h`

 * *Files identical despite different names*

### Comparing `stl-reader-0.1.dev0/stl_reader.egg-info/PKG-INFO` & `stl-reader-0.1.dev1/stl_reader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stl-reader
-Version: 0.1.dev0
+Version: 0.1.dev1
 Summary: Read in STL files
 Home-page: https://github.com/pyvista/pymeshfix
 Author: PyVista Developers
 Author-email: info@pyvista.org
 License: MIT
 Keywords: read stl
 Classifier: Development Status :: 4 - Beta
```

### Comparing `stl-reader-0.1.dev0/tests/test_reader.py` & `stl-reader-0.1.dev1/tests/test_reader.py`

 * *Files identical despite different names*

