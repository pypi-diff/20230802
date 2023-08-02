# Comparing `tmp/ansys_dpf_gatebin-0.4.0-py3-none-win_amd64.whl.zip` & `tmp/ansys_dpf_gatebin-0.4.1-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3321093 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat  8754688 b- defN 23-Jul-28 07:21 ansys/dpf/gatebin/Ans.Dpf.GrpcClient.dll
--rw-rw-rw-  2.0 fat   859136 b- defN 23-Jul-28 07:14 ansys/dpf/gatebin/DPFClientAPI.dll
--rw-rw-rw-  2.0 fat      165 b- defN 23-Jul-28 08:10 ansys/dpf/gatebin/_version.py
--rw-rw-rw-  2.0 fat     1331 b- defN 23-Jul-28 08:11 ansys_dpf_gatebin-0.4.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1246 b- defN 23-Jul-28 08:11 ansys_dpf_gatebin-0.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      103 b- defN 23-Jul-28 08:11 ansys_dpf_gatebin-0.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-28 08:11 ansys_dpf_gatebin-0.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      714 b- defN 23-Jul-28 08:11 ansys_dpf_gatebin-0.4.0.dist-info/RECORD
-8 files, 9617389 bytes uncompressed, 3319839 bytes compressed:  65.5%
+Zip file size: 3321094 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat  8754688 b- defN 23-Aug-01 10:27 ansys/dpf/gatebin/Ans.Dpf.GrpcClient.dll
+-rw-rw-rw-  2.0 fat   859136 b- defN 23-Aug-01 10:18 ansys/dpf/gatebin/DPFClientAPI.dll
+-rw-rw-rw-  2.0 fat      165 b- defN 23-Aug-01 11:10 ansys/dpf/gatebin/_version.py
+-rw-rw-rw-  2.0 fat     1331 b- defN 23-Aug-01 11:11 ansys_dpf_gatebin-0.4.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1246 b- defN 23-Aug-01 11:11 ansys_dpf_gatebin-0.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      103 b- defN 23-Aug-01 11:11 ansys_dpf_gatebin-0.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Aug-01 11:11 ansys_dpf_gatebin-0.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      714 b- defN 23-Aug-01 11:11 ansys_dpf_gatebin-0.4.1.dist-info/RECORD
+8 files, 9617389 bytes uncompressed, 3319840 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: ansys/dpf/gatebin/DPFClientAPI.dll
 Comment: 
 
 Filename: ansys/dpf/gatebin/_version.py
 Comment: 
 
-Filename: ansys_dpf_gatebin-0.4.0.dist-info/LICENSE
+Filename: ansys_dpf_gatebin-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: ansys_dpf_gatebin-0.4.0.dist-info/METADATA
+Filename: ansys_dpf_gatebin-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: ansys_dpf_gatebin-0.4.0.dist-info/WHEEL
+Filename: ansys_dpf_gatebin-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: ansys_dpf_gatebin-0.4.0.dist-info/top_level.txt
+Filename: ansys_dpf_gatebin-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ansys_dpf_gatebin-0.4.0.dist-info/RECORD
+Filename: ansys_dpf_gatebin-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ansys/dpf/gatebin/Ans.Dpf.GrpcClient.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018037d3e0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Jul 28 07:21:32 2023
+Time/Date		Tue Aug  1 10:27:49 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	20
 SizeOfCode		00000000005aec00
 SizeOfInitializedData	00000000002cd600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000037d3e0
@@ -238506,15 +238506,15 @@
 	reloc   32 offset  eb0 [7f7eb0] DIR64
 	reloc   33 offset    0 [7f7000] ABSOLUTE
 
 There is a debug directory in .rdata at 0x1806ca330
 
 Type                Size     Rva      Offset
   2        CodeView 0000006c 0071bafc 0071aafc
-(format RSDS signature 335009b8015141c1af3e91fceb564fc1 age 1 pdb E:\ANSYSDev\TFSAgent\_work\2\b\BUILD_OUTPUT\aisol\Bin\winx64\Ans.Dpf.GrpcClient.pdb)
+(format RSDS signature 6027d1e3c1b74ee2abfd0ce1bad66788 age 1 pdb E:\ANSYSDev\TFSAgent\_work\2\b\BUILD_OUTPUT\aisol\Bin\winx64\Ans.Dpf.GrpcClient.pdb)
  12         Feature 00000014 0071bb68 0071ab68
  13         CoffGrp 0000034c 0071bb7c 0071ab7c
  14           ILTCG 00000000 00000000 00000000
 
 The .rsrc Resource Directory section:
 000  Type Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 010   Entry: ID: 0x000018, Value: 0x80000018
@@ -2294123,53 +2294123,46 @@
    1806ca325:	add    %al,(%rax)
    1806ca327:	add    %al,(%rax)
    1806ca329:	add    %al,(%rax)
    1806ca32b:	add    %al,(%rcx)
    1806ca32d:	add    %al,(%rax)
    1806ca32f:	add    %al,(%rax)
    1806ca331:	add    %al,(%rax)
-   1806ca333:	add    %bh,-0x3d(%rsp,%rbp,2)
-   1806ca337:	add    %al,%fs:(%rax)
-   1806ca33a:	add    %al,(%rax)
-   1806ca33c:	add    (%rax),%al
-   1806ca33e:	add    %al,(%rax)
-   1806ca340:	insb   (%dx),%es:(%rdi)
-   1806ca341:	add    %al,(%rax)
+   1806ca333:	add    %ah,0x64c8de(%rip)        # 0x180d16c17
+   1806ca339:	add    %al,(%rax)
+   1806ca33b:	add    %al,(%rdx)
+   1806ca33d:	add    %al,(%rax)
+   1806ca33f:	add    %ch,0x0(%rax,%rax,1)
    1806ca343:	add    %bh,%ah
    1806ca345:	mov    $0xaafc0071,%edx
    1806ca34a:	jno    0x1806ca34c
    1806ca34c:	add    %al,(%rax)
    1806ca34e:	add    %al,(%rax)
-   1806ca350:	jl     0x1806ca3be
-   1806ca352:	ret
-   1806ca353:	add    %al,%fs:(%rax)
-   1806ca356:	add    %al,(%rax)
-   1806ca358:	or     $0x0,%al
+   1806ca350:	and    $0x64c8de,%eax
+   1806ca355:	add    %al,(%rax)
+   1806ca357:	add    %cl,(%rax,%rax,1)
    1806ca35a:	add    %al,(%rax)
    1806ca35c:	adc    $0x0,%al
    1806ca35e:	add    %al,(%rax)
    1806ca360:	push   $0x680071bb
    1806ca365:	stos   %eax,%es:(%rdi)
    1806ca366:	jno    0x1806ca368
    1806ca368:	add    %al,(%rax)
    1806ca36a:	add    %al,(%rax)
-   1806ca36c:	jl     0x1806ca3da
-   1806ca36e:	ret
-   1806ca36f:	add    %al,%fs:(%rax)
-   1806ca372:	add    %al,(%rax)
-   1806ca374:	or     $0x4c000000,%eax
+   1806ca36c:	and    $0x64c8de,%eax
+   1806ca371:	add    %al,(%rax)
+   1806ca373:	add    %cl,0x4c000000(%rip)        # 0x1cc6ca379
    1806ca379:	add    (%rax),%eax
    1806ca37b:	add    %bh,0x71(%rbx,%rdi,4)
    1806ca37f:	add    %bh,0x71(%rbx,%rbp,4)
    1806ca383:	add    %al,(%rax)
    1806ca385:	add    %al,(%rax)
-   1806ca387:	add    %bh,-0x3d(%rsp,%rbp,2)
-   1806ca38b:	add    %al,%fs:(%rax)
-   1806ca38e:	add    %al,(%rax)
-   1806ca390:	(bad)
+   1806ca387:	add    %ah,0x64c8de(%rip)        # 0x180d16c6b
+   1806ca38d:	add    %al,(%rax)
+   1806ca38f:	add    %cl,(%rsi)
 	...
    1806ca39d:	add    %al,(%rax)
    1806ca39f:	add    %cl,(%rax)
    1806ca3a1:	add    %eax,(%rax)
 	...
    1806ca3f7:	add    %cl,0x18079ad(%rax)
 	...
@@ -2383699,24 +2383692,28 @@
    18071bae8:	clc
    18071bae9:	stos   %eax,%es:(%rdi)
    18071baea:	jno    0x18071baec
    18071baec:	shrb   $0x0,0x71(%rcx)
 	...
    18071bafb:	add    %dl,0x53(%rdx)
    18071bafe:	rex.R push %rbx
-   18071bb00:	mov    $0x51335009,%eax
-   18071bb05:	add    %eax,%ecx
-   18071bb07:	rex.B scas %es:(%rdi),%eax
-   18071bb09:	ds xchg %eax,%ecx
-   18071bb0b:	cld
-   18071bb0c:	jmp    0x18071bb64
-   18071bb0e:	rex.WRXB rolq $0x0,(%r9)
-   18071bb12:	add    %al,(%rax)
-   18071bb14:	cmp    0x4e(%r9,%rax,2),%r11b
-   18071bb19:	push   %rbx
+   18071bb00:	jrcxz  0x18071bad3
+   18071bb02:	(bad)
+   18071bb03:	(bad)
+   18071bb04:	mov    $0xc1,%bh
+   18071bb06:	loop   0x18071bb56
+   18071bb08:	stos   %eax,%es:(%rdi)
+   18071bb09:	std
+   18071bb0a:	or     $0xe1,%al
+   18071bb0c:	mov    $0x18867d6,%edx
+   18071bb11:	add    %al,(%rax)
+   18071bb13:	add    %al,0x3a(%rbp)
+   18071bb16:	pop    %rsp
+   18071bb17:	rex.B
+   18071bb18:	rex.WRX push %rbx
    18071bb1a:	pop    %rcx
    18071bb1b:	push   %rbx
    18071bb1c:	rex.R
    18071bb1d:	gs jbe 0x18071bb7c
    18071bb20:	push   %rsp
    18071bb21:	rex.RX push %rbx
    18071bb23:	rex.B
```

## ansys/dpf/gatebin/DPFClientAPI.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018007c3c8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Jul 28 07:14:33 2023
+Time/Date		Tue Aug  1 10:18:33 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	20
 SizeOfCode		000000000007c800
 SizeOfInitializedData	0000000000055600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000007c3c8
@@ -20226,15 +20226,15 @@
 	reloc   28 offset  778 [cd778] DIR64
 	reloc   29 offset    0 [cd000] ABSOLUTE
 
 There is a debug directory in .rdata at 0x1800b2cf0
 
 Type                Size     Rva      Offset
   2        CodeView 00000066 000b3a24 000b2624
-(format RSDS signature 949e983fd4b142a7a13b6a6bce780b58 age 1 pdb E:\ANSYSDev\TFSAgent\_work\2\b\BUILD_OUTPUT\aisol\bin\winx64\DPFClientAPI.pdb)
+(format RSDS signature 8dd91f8fb92a462bb31aa5523e6bbff3 age 1 pdb E:\ANSYSDev\TFSAgent\_work\2\b\BUILD_OUTPUT\aisol\bin\winx64\DPFClientAPI.pdb)
  12         Feature 00000014 000b3a8c 000b268c
  13         CoffGrp 00000278 000b3aa0 000b26a0
  14           ILTCG 00000000 00000000 00000000
 
 The .rsrc Resource Directory section:
 000  Type Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 010   Entry: ID: 0x000018, Value: 0x80000018
@@ -243052,49 +243052,53 @@
    1800b2ce6:	add    %al,(%rax)
    1800b2ce8:	add    %al,(%rax)
    1800b2cea:	add    %al,(%rax)
    1800b2cec:	add    %eax,(%rax)
    1800b2cee:	add    %al,(%rax)
    1800b2cf0:	add    %al,(%rax)
    1800b2cf2:	add    %al,(%rax)
-   1800b2cf4:	fldcw  -0x3d(%rdx)
+   1800b2cf4:	stc
+   1800b2cf5:	fcmovne %st(0),%st
    1800b2cf7:	add    %al,%fs:(%rax)
    1800b2cfa:	add    %al,(%rax)
    1800b2cfc:	add    (%rax),%al
    1800b2cfe:	add    %al,(%rax)
    1800b2d00:	data16 add %al,(%rax)
    1800b2d03:	add    %ah,(%rdx,%rdi,1)
    1800b2d06:	or     (%rax),%eax
    1800b2d08:	and    $0x26,%al
    1800b2d0a:	or     (%rax),%eax
    1800b2d0c:	add    %al,(%rax)
    1800b2d0e:	add    %al,(%rax)
-   1800b2d10:	fldcw  -0x3d(%rdx)
+   1800b2d10:	stc
+   1800b2d11:	fcmovne %st(0),%st
    1800b2d13:	add    %al,%fs:(%rax)
    1800b2d16:	add    %al,(%rax)
    1800b2d18:	or     $0x0,%al
    1800b2d1a:	add    %al,(%rax)
    1800b2d1c:	adc    $0x0,%al
    1800b2d1e:	add    %al,(%rax)
    1800b2d20:	mov    %?,(%rdx)
    1800b2d22:	or     (%rax),%eax
    1800b2d24:	mov    %fs,(%rsi)
    1800b2d26:	or     (%rax),%eax
    1800b2d28:	add    %al,(%rax)
    1800b2d2a:	add    %al,(%rax)
-   1800b2d2c:	fldcw  -0x3d(%rdx)
+   1800b2d2c:	stc
+   1800b2d2d:	fcmovne %st(0),%st
    1800b2d2f:	add    %al,%fs:(%rax)
    1800b2d32:	add    %al,(%rax)
    1800b2d34:	or     $0x78000000,%eax
    1800b2d39:	add    (%rax),%al
    1800b2d3b:	add    %ah,-0x5ffff4c6(%rax)
    1800b2d41:	es or  (%rax),%eax
    1800b2d44:	add    %al,(%rax)
    1800b2d46:	add    %al,(%rax)
-   1800b2d48:	fldcw  -0x3d(%rdx)
+   1800b2d48:	stc
+   1800b2d49:	fcmovne %st(0),%st
    1800b2d4b:	add    %al,%fs:(%rax)
    1800b2d4e:	add    %al,(%rax)
    1800b2d50:	(bad)
 	...
    1800b2d5d:	add    %al,(%rax)
    1800b2d5f:	add    %cl,(%rax)
    1800b2d61:	add    %eax,(%rax)
@@ -243925,25 +243929,22 @@
    1800b3a1e:	or     (%rax),%eax
    1800b3a20:	add    %al,(%rax)
    1800b3a22:	add    %al,(%rax)
    1800b3a24:	push   %rdx
    1800b3a25:	push   %rbx
    1800b3a26:	rex.R push %rbx
    1800b3a28:	(bad)
-   1800b3a29:	cwtl
-   1800b3a2a:	sahf
-   1800b3a2b:	xchg   %eax,%esp
-   1800b3a2c:	mov    $0xd4,%cl
-   1800b3a2e:	cmpsl  %es:(%rdi),%ds:(%rsi)
-   1800b3a2f:	rex.X movabs 0x1580b78ce6b6a3b,%eax
-   1800b3a39:	add    %al,(%rax)
-   1800b3a3b:	add    %al,0x3a(%rbp)
-   1800b3a3e:	pop    %rsp
-   1800b3a3f:	rex.B
-   1800b3a40:	rex.WRX push %rbx
+   1800b3a29:	(bad)
+   1800b3a2a:	(bad)  0x462bb92a(%rbp)
+   1800b3a30:	mov    $0x1a,%bl
+   1800b3a32:	movsl  %ds:(%rsi),%es:(%rdi)
+   1800b3a33:	push   %rdx
+   1800b3a34:	ds imul $0x0,0x1f3(%rdi),%edi
+   1800b3a3c:	cmp    0x4e(%r9,%rax,2),%r11b
+   1800b3a41:	push   %rbx
    1800b3a42:	pop    %rcx
    1800b3a43:	push   %rbx
    1800b3a44:	rex.R
    1800b3a45:	gs jbe 0x1800b3aa4
    1800b3a48:	push   %rsp
    1800b3a49:	rex.RX push %rbx
    1800b3a4b:	rex.B
```

## ansys/dpf/gatebin/_version.py

```diff
@@ -1,6 +1,6 @@
 """Version for ansys-dpf-gatebin"""
 # major, minor, patch
-version_info = 0, 4, "0"
+version_info = 0, 4, "1"
 
 # Nice string for the version
 __version__ = ".".join(map(str, version_info))
```

## Comparing `ansys_dpf_gatebin-0.4.0.dist-info/LICENSE` & `ansys_dpf_gatebin-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ansys_dpf_gatebin-0.4.0.dist-info/METADATA` & `ansys_dpf_gatebin-0.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-dpf-gatebin
-Version: 0.4.0
+Version: 0.4.1
 Summary: DPF binaries dependencies for ansys-dpf-gate
 Author: ANSYS
 Author-email: ramdane.lagha@ansys.com
 Maintainer-email: pyansys.maintainers@ansys.com
 License: Ansys Redistribution License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

