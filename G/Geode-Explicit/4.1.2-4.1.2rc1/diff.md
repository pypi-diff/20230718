# Comparing `tmp/Geode_Explicit-4.1.2-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-4.1.2rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 2269147 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 23-Jul-18 00:28 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 23-Jul-18 00:28 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 23-Jul-18 00:28 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  2316800 b- defN 23-Jul-18 00:28 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    33280 b- defN 23-Jul-18 00:28 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  2073600 b- defN 23-Jul-18 00:28 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   153600 b- defN 23-Jul-18 00:28 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   141824 b- defN 23-Jul-18 00:28 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2380 b- defN 23-Jul-18 00:28 Geode_Explicit-4.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-18 00:28 Geode_Explicit-4.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-18 00:28 Geode_Explicit-4.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1118 b- defN 23-Jul-18 00:28 Geode_Explicit-4.1.2.dist-info/RECORD
-12 files, 4723431 bytes uncompressed, 2267247 bytes compressed:  52.0%
+Zip file size: 2269174 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      194 b- defN 23-Jul-17 13:15 geode_explicit/__init__.py
+-rw-rw-rw-  2.0 fat      271 b- defN 23-Jul-17 13:15 geode_explicit/brep.py
+-rw-rw-rw-  2.0 fat      249 b- defN 23-Jul-17 13:15 geode_explicit/section.py
+-rw-rw-rw-  2.0 fat  2316800 b- defN 23-Jul-17 13:15 geode_explicit/bin/Geode-Explicit_brep.dll
+-rw-rw-rw-  2.0 fat    33280 b- defN 23-Jul-17 13:15 geode_explicit/bin/Geode-Explicit_common.dll
+-rw-rw-rw-  2.0 fat  2073600 b- defN 23-Jul-17 13:15 geode_explicit/bin/Geode-Explicit_section.dll
+-rw-rw-rw-  2.0 fat   153600 b- defN 23-Jul-17 13:15 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   141824 b- defN 23-Jul-17 13:15 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2383 b- defN 23-Jul-17 13:15 Geode_Explicit-4.1.2rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-17 13:15 Geode_Explicit-4.1.2rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-17 13:15 Geode_Explicit-4.1.2rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1130 b- defN 23-Jul-17 13:15 Geode_Explicit-4.1.2rc1.dist-info/RECORD
+12 files, 4723446 bytes uncompressed, 2267250 bytes compressed:  52.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
 Comment: 
 
 Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Explicit-4.1.2.dist-info/METADATA
+Filename: Geode_Explicit-4.1.2rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-4.1.2.dist-info/WHEEL
+Filename: Geode_Explicit-4.1.2rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-4.1.2.dist-info/top_level.txt
+Filename: Geode_Explicit-4.1.2rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-4.1.2.dist-info/RECORD
+Filename: Geode_Explicit-4.1.2rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/bin/Geode-Explicit_brep.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001801942cc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Jul 18 00:28:32 2023
+Time/Date		Mon Jul 17 13:15:45 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000197400
 SizeOfInitializedData	000000000009e200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000001942cc
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		0023d000
 SizeOfHeaders		00000400
-CheckSum		002398c6
+CheckSum		00235d67
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -686320,15 +686320,15 @@
    180200df8:	(bad)
    180200dfd:	insb   (%dx),%es:(%rdi)
    180200dfe:	insb   (%dx),%es:(%rdi)
    180200dff:	outsl  %ds:(%rsi),(%dx)
    180200e00:	movsxd 0x74(%rcx),%esp
    180200e03:	imul   $0x0,0x6e(%rdi),%ebp
    180200e0a:	add    %al,(%rax)
-   180200e0c:	mov    $0xdc,%al
+   180200e0c:	add    %edi,(%rdi)
    180200e0e:	mov    $0x64,%ch
    180200e10:	add    %al,(%rax)
    180200e12:	add    %al,(%rax)
    180200e14:	or     $0x60000000,%eax
    180200e19:	add    (%rax),%eax
    180200e1b:	add    %bl,-0x67ffdfd2(%rax)
    180200e21:	(bad)
```

## geode_explicit/bin/Geode-Explicit_common.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800040e0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Jul 18 00:28:08 2023
+Time/Date		Mon Jul 17 13:15:26 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000004000
 SizeOfInitializedData	0000000000003e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000040e0
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		0000d000
 SizeOfHeaders		00000400
-CheckSum		0000e97f
+CheckSum		0000ae2a
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -6720,17 +6720,19 @@
    18000552a:	(bad)
    18000552b:	(bad)
    18000552c:	(bad)
    18000552d:	(bad)
    18000552e:	(bad)
    18000552f:	incl   (%rax)
    180005531:	add    %al,(%rax)
-   180005533:	add    %bl,0x64b5dc(%rax)
-   180005539:	add    %al,(%rax)
-   18000553b:	add    %cl,0x7c000000(%rip)        # 0x1fc005541
+   180005533:	add    %ch,%dh
+   180005535:	ds mov $0x64,%ch
+   180005538:	add    %al,(%rax)
+   18000553a:	add    %al,(%rax)
+   18000553c:	or     $0x7c000000,%eax
    180005541:	add    (%rax),%al
    180005543:	add    %ah,0x5b(%rax)
    180005546:	add    %al,(%rax)
    180005548:	(bad)
    180005549:	rex.WRXB add %r8b,(%r8)
    18000554c:	add    %al,(%rax)
    18000554e:	add    %al,(%rax)
```

## geode_explicit/bin/Geode-Explicit_section.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180166e40
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Jul 18 00:28:17 2023
+Time/Date		Mon Jul 17 13:15:30 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000168a00
 SizeOfInitializedData	0000000000091600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000166e40
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00201000
 SizeOfHeaders		00000400
-CheckSum		001fe314
+CheckSum		001fa7b5
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -623960,20 +623960,21 @@
    1801d0f38:	(bad)
    1801d0f3d:	insb   (%dx),%es:(%rdi)
    1801d0f3e:	insb   (%dx),%es:(%rdi)
    1801d0f3f:	outsl  %ds:(%rsi),(%dx)
    1801d0f40:	movsxd 0x74(%rcx),%esp
    1801d0f43:	imul   $0x0,0x6e(%rdi),%ebp
    1801d0f4a:	add    %al,(%rax)
-   1801d0f4c:	movabs 0xd0000000064b5dc,%eax
-   1801d0f55:	add    %al,(%rax)
-   1801d0f57:	add    %ah,0x3(%rax)
-   1801d0f5a:	add    %al,(%rax)
-   1801d0f5c:	push   $0x68001d26
-   1801d0f61:	adc    $0x1d,%al
+   1801d0f4c:	repnz ds mov $0x64,%ch
+   1801d0f50:	add    %al,(%rax)
+   1801d0f52:	add    %al,(%rax)
+   1801d0f54:	or     $0x60000000,%eax
+   1801d0f59:	add    (%rax),%eax
+   1801d0f5b:	add    %ch,0x26(%rax)
+   1801d0f5e:	sbb    $0x1d146800,%eax
 	...
    1801d0f6f:	add    %bh,(%rax)
    1801d0f71:	add    %eax,(%rax)
 	...
    1801d0fc7:	add    %cl,(%rax)
    1801d0fc9:	lea    (%rsi),%ebx
    1801d0fcb:	addb   $0x0,(%rcx)
```

## Comparing `Geode_Explicit-4.1.2.dist-info/METADATA` & `Geode_Explicit-4.1.2rc1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geode-Explicit
-Version: 4.1.2
+Version: 4.1.2rc1
 Summary: Geode-solutions OpenGeode module for building explicit models
 Home-page: https://github.com/Geode-solutions/Geode-Explicit
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.1.2 Summary: Geode-
+Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.1.2rc1 Summary: Geode-
 solutions OpenGeode module for building explicit models Home-page: https://
 github.com/Geode-solutions/Geode-Explicit Author: Geode-solutions Author-email:
 contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
 Content-Type: text/markdown Requires-Dist: geode-background (==7.*,>=7.3.1)
 Requires-Dist: geode-common (==26.*,>=26.1.3) Requires-Dist: geode-conversion
 (==5.*,>=5.0.9) Requires-Dist: opengeode-core (==14.*,>=14.4.3) Requires-Dist:
 opengeode-geosciences (==7.*,>=7.1.3) Requires-Dist: opengeode-geosciencesio
```

## Comparing `Geode_Explicit-4.1.2.dist-info/RECORD` & `Geode_Explicit-4.1.2rc1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 geode_explicit/__init__.py,sha256=-1Ma-Q_qKho5-HJywdEjGH_v91Dp0h8zchFCzKp7ADk,194
 geode_explicit/brep.py,sha256=5gXUGyujJVK7W7i2Zoqb5_9Mb5jPPZLiYZX9piVVUGY,271
 geode_explicit/section.py,sha256=diHY0-G0OXfICdOX3HSTnwrdrW3WOsct7GAT4rECQb4,249
-geode_explicit/bin/Geode-Explicit_brep.dll,sha256=F6imELIHvWbcYIHF1qTezqXBViodWiDLFq8CiByRTPI,2316800
-geode_explicit/bin/Geode-Explicit_common.dll,sha256=dkFPmpnEXNkxRtD9xL0emrgC99SF4GMhyNINaE8kp6U,33280
-geode_explicit/bin/Geode-Explicit_section.dll,sha256=CflQuinobeSHN8RLIwNInXNTdHdMBCFmH2fCcc_iioA,2073600
-geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=3G3Ow3qIwghasn8Peb4T0UH8hYNAQEX6ih501SbIRC4,153600
-geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=2wxCiCKPkzwHHC4J5XANLh9aiY_nn8ZesOncXYLVCjk,141824
-Geode_Explicit-4.1.2.dist-info/METADATA,sha256=hzm0jDeyvqkEFPQt78YgJNn2zP0cFUcV7B8rYXesnt4,2380
-Geode_Explicit-4.1.2.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-Geode_Explicit-4.1.2.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
-Geode_Explicit-4.1.2.dist-info/RECORD,,
+geode_explicit/bin/Geode-Explicit_brep.dll,sha256=AOogB7gIXOjvEFmUeUXtq4EzNFHNNpymX-_4goU9EAE,2316800
+geode_explicit/bin/Geode-Explicit_common.dll,sha256=Z-7euka8fCXDl5NstKXY3ku8psi3j-harAbz7yQhP78,33280
+geode_explicit/bin/Geode-Explicit_section.dll,sha256=oC5YlamVhjz5fqFBUbekgjBmdKZyc6l6BN8Do_4WRIU,2073600
+geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=iYIQERHwB1OATZTR7ksaydJkBY1sJpGCaEklGsBi0aA,153600
+geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=ZhGyYpySoIHY8WC3FLTH9ctztFHmcWDac_ItjD_iQl0,141824
+Geode_Explicit-4.1.2rc1.dist-info/METADATA,sha256=bipJPDGZGgR6OqeyxlWfMOVX4ADQh8_zFWHtd5uqshA,2383
+Geode_Explicit-4.1.2rc1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+Geode_Explicit-4.1.2rc1.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
+Geode_Explicit-4.1.2rc1.dist-info/RECORD,,
```

