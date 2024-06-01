# Comparing `tmp/Geode_Hybrid-2.4.4-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Hybrid-2.4.4rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1558173 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      170 b- defN 24-Jun-01 01:59 geode_hybrid/__init__.py
--rw-rw-rw-  2.0 fat      234 b- defN 24-Jun-01 01:59 geode_hybrid/brep.py
--rw-rw-rw-  2.0 fat  3858432 b- defN 24-Jun-01 01:59 geode_hybrid/bin/Geode-Hybrid_brep.dll
--rw-rw-rw-  2.0 fat   126464 b- defN 24-Jun-01 01:59 geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2264 b- defN 24-Jun-01 01:59 Geode_Hybrid-2.4.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Jun-01 01:59 Geode_Hybrid-2.4.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Jun-01 01:59 Geode_Hybrid-2.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      688 b- defN 24-Jun-01 01:59 Geode_Hybrid-2.4.4.dist-info/RECORD
-8 files, 3988365 bytes uncompressed, 1556971 bytes compressed:  61.0%
+Zip file size: 1558203 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      170 b- defN 24-May-30 08:45 geode_hybrid/__init__.py
+-rw-rw-rw-  2.0 fat      234 b- defN 24-May-30 08:45 geode_hybrid/brep.py
+-rw-rw-rw-  2.0 fat  3858432 b- defN 24-May-30 08:45 geode_hybrid/bin/Geode-Hybrid_brep.dll
+-rw-rw-rw-  2.0 fat   126464 b- defN 24-May-30 08:45 geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2279 b- defN 24-May-30 08:45 Geode_Hybrid-2.4.4rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-30 08:45 Geode_Hybrid-2.4.4rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-May-30 08:45 Geode_Hybrid-2.4.4rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      700 b- defN 24-May-30 08:45 Geode_Hybrid-2.4.4rc1.dist-info/RECORD
+8 files, 3988392 bytes uncompressed, 1556977 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: geode_hybrid/bin/Geode-Hybrid_brep.dll
 Comment: 
 
 Filename: geode_hybrid/bin/geode_hybrid_py_brep.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Hybrid-2.4.4.dist-info/METADATA
+Filename: Geode_Hybrid-2.4.4rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Hybrid-2.4.4.dist-info/WHEEL
+Filename: Geode_Hybrid-2.4.4rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Hybrid-2.4.4.dist-info/top_level.txt
+Filename: Geode_Hybrid-2.4.4rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Hybrid-2.4.4.dist-info/RECORD
+Filename: Geode_Hybrid-2.4.4rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_hybrid/bin/Geode-Hybrid_brep.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001802c3884
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat Jun  1 01:59:33 2024
+Time/Date		Thu May 30 08:45:44 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000002c5e00
 SizeOfInitializedData	00000000000ea800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000002c3884
@@ -66,23 +66,23 @@
  vma:            Hint    Time      Forward  DLL       First
                  Table   Stamp     Chain    Name      Thunk
  0037f92c	0037feb8 00000000 00000000 00381086 002c71e0
 
 	DLL Name: Geode-Numerics_frame_field.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	380f0a	    4  ??0FrameFieldSmoother@geode@@QEAA@AEAVFrameField@1@@Z
-	380f42	   25  ?extract_elements@FrameFieldParameterization@geode@@QEBA?AUExtractedElements@12@XZ
+	380f42	   24  ?extract_elements@FrameFieldParameterization@geode@@QEBA?AUExtractedElements@12@XZ
 	380ee2	    9  ??1FrameFieldSmoother@geode@@QEAA@XZ
-	380eaa	   29  ?smooth_frame_field@FrameFieldSmoother@geode@@QEAAXXZ
+	380eaa	   28  ?smooth_frame_field@FrameFieldSmoother@geode@@QEAAXXZ
 	380e80	    2  ??0FrameField@geode@@QEAA@AEAVBRep@1@@Z
 	380e60	    7  ??1FrameField@geode@@QEAA@XZ
-	380f98	   23  ?compute_parameterization@FrameFieldParameterization@geode@@QEAAXXZ
+	380f98	   22  ?compute_parameterization@FrameFieldParameterization@geode@@QEAAXXZ
 	380fde	    8  ??1FrameFieldParameterization@geode@@QEAA@XZ
 	38100e	    3  ??0FrameFieldParameterization@geode@@QEAA@AEBVFrameField@1@N@Z
-	381050	   27  ?initialize@NumericsFrameFieldLibrary@geode@@SAXXZ
+	381050	   26  ?initialize@NumericsFrameFieldLibrary@geode@@SAXXZ
 
  0037f940	0037ff10 00000000 00000000 003810d4 002c7238
 
 	DLL Name: Geode-Simplex_brep.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	3810a6	    4  ?initialize@SimplexBRepLibrary@geode@@SAXXZ
 
@@ -63186,42 +63186,42 @@
 	  2560: 00 00 00 00 5c 76 38 00 00 00 00 00 60 78 38 00
 	  2570: 00 00 00 00 6a 76 38 00 00 00 00 00 00 00 00 00
 	  2580: 00 00 00 00 46 77 38 00 00 00 00 00 00 00 00 00
 	  2590: 00 00 00 00 07 00 3f 3f 31 46 72 61 6d 65 46 69
 	  25a0: 65 6c 64 40 67 65 6f 64 65 40 40 51 45 41 41 40
 	  25b0: 58 5a 00 00 02 00 3f 3f 30 46 72 61 6d 65 46 69
 	  25c0: 65 6c 64 40 67 65 6f 64 65 40 40 51 45 41 41 40
-	  25d0: 41 45 41 56 42 52 65 70 40 31 40 40 5a 00 1d 00
+	  25d0: 41 45 41 56 42 52 65 70 40 31 40 40 5a 00 1c 00
 	  25e0: 3f 73 6d 6f 6f 74 68 5f 66 72 61 6d 65 5f 66 69
 	  25f0: 65 6c 64 40 46 72 61 6d 65 46 69 65 6c 64 53 6d
 	  2600: 6f 6f 74 68 65 72 40 67 65 6f 64 65 40 40 51 45
 	  2610: 41 41 58 58 5a 00 09 00 3f 3f 31 46 72 61 6d 65
 	  2620: 46 69 65 6c 64 53 6d 6f 6f 74 68 65 72 40 67 65
 	  2630: 6f 64 65 40 40 51 45 41 41 40 58 5a 00 00 04 00
 	  2640: 3f 3f 30 46 72 61 6d 65 46 69 65 6c 64 53 6d 6f
 	  2650: 6f 74 68 65 72 40 67 65 6f 64 65 40 40 51 45 41
 	  2660: 41 40 41 45 41 56 46 72 61 6d 65 46 69 65 6c 64
-	  2670: 40 31 40 40 5a 00 19 00 3f 65 78 74 72 61 63 74
+	  2670: 40 31 40 40 5a 00 18 00 3f 65 78 74 72 61 63 74
 	  2680: 5f 65 6c 65 6d 65 6e 74 73 40 46 72 61 6d 65 46
 	  2690: 69 65 6c 64 50 61 72 61 6d 65 74 65 72 69 7a 61
 	  26a0: 74 69 6f 6e 40 67 65 6f 64 65 40 40 51 45 42 41
 	  26b0: 3f 41 55 45 78 74 72 61 63 74 65 64 45 6c 65 6d
-	  26c0: 65 6e 74 73 40 31 32 40 58 5a 00 00 17 00 3f 63
+	  26c0: 65 6e 74 73 40 31 32 40 58 5a 00 00 16 00 3f 63
 	  26d0: 6f 6d 70 75 74 65 5f 70 61 72 61 6d 65 74 65 72
 	  26e0: 69 7a 61 74 69 6f 6e 40 46 72 61 6d 65 46 69 65
 	  26f0: 6c 64 50 61 72 61 6d 65 74 65 72 69 7a 61 74 69
 	  2700: 6f 6e 40 67 65 6f 64 65 40 40 51 45 41 41 58 58
 	  2710: 5a 00 08 00 3f 3f 31 46 72 61 6d 65 46 69 65 6c
 	  2720: 64 50 61 72 61 6d 65 74 65 72 69 7a 61 74 69 6f
 	  2730: 6e 40 67 65 6f 64 65 40 40 51 45 41 41 40 58 5a
 	  2740: 00 00 03 00 3f 3f 30 46 72 61 6d 65 46 69 65 6c
 	  2750: 64 50 61 72 61 6d 65 74 65 72 69 7a 61 74 69 6f
 	  2760: 6e 40 67 65 6f 64 65 40 40 51 45 41 41 40 41 45
 	  2770: 42 56 46 72 61 6d 65 46 69 65 6c 64 40 31 40 4e
-	  2780: 40 5a 00 00 1b 00 3f 69 6e 69 74 69 61 6c 69 7a
+	  2780: 40 5a 00 00 1a 00 3f 69 6e 69 74 69 61 6c 69 7a
 	  2790: 65 40 4e 75 6d 65 72 69 63 73 46 72 61 6d 65 46
 	  27a0: 69 65 6c 64 4c 69 62 72 61 72 79 40 67 65 6f 64
 	  27b0: 65 40 40 53 41 58 58 5a 00 00 47 65 6f 64 65 2d
 	  27c0: 4e 75 6d 65 72 69 63 73 5f 66 72 61 6d 65 5f 66
 	  27d0: 69 65 6c 64 2e 64 6c 6c 00 00 04 00 3f 69 6e 69
 	  27e0: 74 69 61 6c 69 7a 65 40 53 69 6d 70 6c 65 78 42
 	  27f0: 52 65 70 4c 69 62 72 61 72 79 40 67 65 6f 64 65
@@ -1039667,15 +1039667,15 @@
    18036399a:	(bad)
    18036399b:	(bad)
    18036399c:	(bad)
    18036399d:	(bad)
    18036399e:	(bad)
    18036399f:	incl   (%rax)
    1803639a1:	add    %al,(%rax)
-   1803639a3:	add    %al,0x665a80(%rbp)
+   1803639a3:	add    %bh,0x66583c(%rax)
    1803639a9:	add    %al,(%rax)
    1803639ab:	add    %cl,-0x78000000(%rip)        # 0x1083639b1
    1803639b1:	add    (%rax),%eax
    1803639b3:	add    %ch,0x4eac0036(%rsp,%rbx,2)
    1803639ba:	ss add %al,(%rax)
    1803639bd:	add    %al,(%rax)
    1803639bf:	add    %bh,(%rax)
@@ -1086217,15 +1086217,17 @@
    180380e9c:	rex.B
    180380e9d:	rex.RB
    180380e9e:	push   %r14
    180380ea0:	rex.X push %rdx
    180380ea2:	gs jo  0x180380ee5
    180380ea5:	xor    %eax,0x40(%rax)
    180380ea8:	pop    %rdx
-   180380ea9:	add    %bl,0x6d733f00(%rip)        # 0x1edab4daf
+   180380ea9:	add    %bl,(%rax,%rax,1)
+   180380eac:	(bad)
+   180380ead:	jae    0x180380f1c
    180380eaf:	outsl  %ds:(%rsi),(%dx)
    180380eb0:	outsl  %ds:(%rsi),(%dx)
    180380eb1:	je     0x180380f1b
    180380eb3:	pop    %rdi
    180380eb4:	data16 jb 0x180380f18
    180380eb7:	insl   (%dx),%es:(%rdi)
    180380eb8:	gs pop %rdi
@@ -1086283,15 +1086285,15 @@
    180380f2e:	rex.B
    180380f2f:	rex.RB
    180380f30:	push   %r14
    180380f32:	rex.RX jb 0x180380f96
    180380f35:	insl   (%dx),%es:(%rdi)
    180380f36:	rex.RX imul $0x40314064,%gs:0x6c(%rbp),%r12d
    180380f3f:	rex pop %rdx
-   180380f41:	add    %bl,(%rcx)
+   180380f41:	add    %bl,(%rax)
    180380f43:	add    %bh,(%rdi)
    180380f45:	gs js  0x180380fbc
    180380f48:	jb     0x180380fab
    180380f4a:	movsxd 0x65(%rdi,%rbx,2),%esi
    180380f4e:	insb   (%dx),%es:(%rdi)
    180380f4f:	gs insl (%dx),%es:(%rdi)
    180380f51:	outsb  %gs:(%rsi),(%dx)
@@ -1086416,15 +1086418,15 @@
    18038103c:	rex.X push %rsi
    18038103e:	rex.RX jb 0x1803810a2
    180381041:	insl   (%dx),%es:(%rdi)
    180381042:	rex.RX imul $0x40314064,%gs:0x6c(%rbp),%r12d
    18038104b:	rex.WRX
    18038104c:	rex pop %rdx
    18038104e:	add    %al,(%rax)
-   180381050:	sbb    (%rax),%eax
+   180381050:	sbb    (%rax),%al
    180381052:	(bad)
    180381053:	imul   $0x6c616974,0x69(%rsi),%ebp
    18038105a:	imul   $0x6d754e40,0x65(%rdx),%edi
    180381061:	gs jb  0x1803810cd
    180381064:	movsxd 0x46(%rbx),%esi
    180381067:	jb     0x1803810ca
    180381069:	insl   (%dx),%es:(%rdi)
```

## Comparing `Geode_Hybrid-2.4.4.dist-info/METADATA` & `Geode_Hybrid-2.4.4rc1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: Geode-Hybrid
-Version: 2.4.4
+Version: 2.4.4rc1
 Summary: Hybrid remeshing Geode-solutions OpenGeode module
 Home-page: https://github.com/Geode-solutions/Geode-Hybrid
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: geode-background ==7.*,>=7.11.0
-Requires-Dist: geode-common ==31.*,>=31.2.1
-Requires-Dist: geode-numerics ==4.*,>=4.4.0
-Requires-Dist: geode-simplex ==6.*,>=6.8.2
-Requires-Dist: opengeode-core ==14.*,>=14.21.3
+Requires-Dist: geode-background ==7.*,>=7.11.0rc1
+Requires-Dist: geode-common ==31.*,>=31.2.0rc1
+Requires-Dist: geode-numerics ==4.*,>=4.3.4rc1
+Requires-Dist: geode-simplex ==6.*,>=6.8.2rc1
+Requires-Dist: opengeode-core ==14.*,>=14.21.1
 Requires-Dist: opengeode-inspector ==5.*,>=5.1.4
 
 <h1 align="center">Geode-ModuleTemplate_private<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Template for creating your own OpenGeode private module</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CI/badge.svg" alt="Build Status">
```

### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.4.4 Summary: Hybrid
+Metadata-Version: 2.1 Name: Geode-Hybrid Version: 2.4.4rc1 Summary: Hybrid
 remeshing Geode-solutions OpenGeode module Home-page: https://github.com/Geode-
 solutions/Geode-Hybrid Author: Geode-solutions Author-email: contact@geode-
 solutions.com License: Proprietary Platform: UNKNOWN Description-Content-Type:
-text/markdown Requires-Dist: geode-background ==7.*,>=7.11.0 Requires-Dist:
-geode-common ==31.*,>=31.2.1 Requires-Dist: geode-numerics ==4.*,>=4.4.0
-Requires-Dist: geode-simplex ==6.*,>=6.8.2 Requires-Dist: opengeode-core
-==14.*,>=14.21.3 Requires-Dist: opengeode-inspector ==5.*,>=5.1.4
+text/markdown Requires-Dist: geode-background ==7.*,>=7.11.0rc1 Requires-Dist:
+geode-common ==31.*,>=31.2.0rc1 Requires-Dist: geode-numerics ==4.*,>=4.3.4rc1
+Requires-Dist: geode-simplex ==6.*,>=6.8.2rc1 Requires-Dist: opengeode-core
+==14.*,>=14.21.1 Requires-Dist: opengeode-inspector ==5.*,>=5.1.4
          ************ GGeeooddee--MMoodduulleeTTeemmppllaattee__pprriivvaatteebbyy GGeeooddee--ssoolluuttiioonnss ************
        ******** TTeemmppllaattee ffoorr ccrreeaattiinngg yyoouurr oowwnn OOppeennGGeeooddee pprriivvaattee mmoodduullee ********
             [Build Status][Deploy Status][Coverage Status][Version]
               [Windows support][Ubuntu support][Red Hat support]
  [Language][License][Semantic-release]_[_S_l_a_c_k_ _i_n_v_i_t_e_]Copyright (c) 2019 - 2024,
                                 Geode-solutions
```

